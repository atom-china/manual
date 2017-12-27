```sh
注意：在 Atom 1.13 中删除了 Shadow DOM 。下面介绍的 `:host` 选择器将不起作用，不应该再使用。
```

# 升级你的语法主题

文本编辑器的内容是在 shadow DOM 中渲染，shadow DOM 用于保护内容的样式不被全局样式表所污染。有关 shadow DOM 的更多背景信息，请查看 HTML 5 Rocks 上的 [shadow DOM 101](https://www.html5rocks.com/en/tutorials/webcomponents/shadowdom/) 。

语法主题是专门用于设置文本编辑器内容的样式，因此在启用文本编辑器的 shadow DOM 时，它们会自动直接加载到文本编辑器的 shadow DOM 中。当主题的 `package.json` 包含 `theme:"syntax"` 声明语句时将会自动渲染该主题，因此不需要改变任何内容来适应目标的上下文。

当主题样式表加载到文本编辑器的 shadow DOM 中时，想要从外部以编辑器为目标的选择器将不起作用。以 `.editor` 和 `.editor-color` 类为目标的样式需要以 `:host` 伪元素为目标，该伪元素与包含的 `atom-text-editor` 节点相匹配。有关 `:host` 伪元素的更多信息，请参阅 [shadow DOM 201](https://www.html5rocks.com/en/tutorials/webcomponents/shadowdom-201/#toc-style-host) 上的文章。

这里有一个来自 Atom 的 light 语法主题的例子。请注意，从外部以编辑器为目标的 `atom-text-editor` 选择器已被保留下来，当禁用 shadow DOM 的时候用来允许主题在过渡阶段保持工作状态。
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
