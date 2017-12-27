```sh
注意：在 Atom 1.13 中删除了 Shadow DOM 。下面介绍的 `:host` 选择器将不起作用，不应该再使用。
```

# 升级你的语法主题

文本编辑器的内容现在支持在 shadow DOM 中，这样可以有效的避免某些样式被全局样式表所影响，用来防止意外出现的样式污染。有关 shadow DOM 的更多背景信息，请查看 HTML 5 Rocks 上的 [shadow DOM 101](https://www.html5rocks.com/en/tutorials/webcomponents/shadowdom/) 。

语法主题是专门用于设置文本编辑器内容的样式，因此在启用文本编辑器的 shadow DOM 时，它们会自动直接加载到文本编辑器的 shadow DOM 中。当主题的 `package.json` 包含 `theme:"syntax"` 描述语句时将会自动运行，因此你不需要改变任何内容来适应你目标的上下文。

当主题样式表加载到文本编辑器的 shadow DOM 中时，想要从外部对准编辑器的选择器将不再有意义。以 `.editor` 和 `.editor-color` 类为目标的样式需要定位到 `:host` 伪元素，该伪元素与包含的 `atom-text-editor` 节点相匹配。有关 `:host` 伪元素的更多信息，请参阅 [shadow DOM 201](https://www.html5rocks.com/en/tutorials/webcomponents/shadowdom-201/#toc-style-host) 上的文章。

这里有一个来自 Atom 的 light 语法主题的例子。请注意，从外部对准编辑器的 `atom-text-editor` 选择器已被保留下来，当禁用 shadow DOM 的时候用来允许主题在过渡阶段保持工作状态。
```sh
atom-text-editor, :host { /* :host added */
  background-color: @syntax-background-color;
  color: @syntax-text-color;

  .invisible-character {
    color: @syntax-invisible-character-color;
  }
  /* more nested selectors... */
}
```
