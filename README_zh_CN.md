[Github 仓库](https://github.com/frostime/sy-dark-purple)

本主题仿照 Jetbrain 的 Dark Purple 主题制作而成，只包含 css 样式。

## 其他说明

### 致谢

本主题在制作过程中从以下主题汲取了部分灵感，在此表示致谢:

- [Light Blue](https://github.com/Morganwan90/Darkblue-siyuan-theme)
- [Tsundoku](https://github.com/Achuan-2/siyuan-themes-tsundoku)
- [Savor](https://github.com/royc01/notion-theme)

### 引用样式

当前引用的样式为 `[[#引用名]]`。如果对样式不满或者更喜欢之前的版本，可参考下述 css 在代码片段中自定义。

- 当前样式 `[[# ]]`

    ```css
    .protyle-wysiwyg [data-node-id] span[data-type~="block-ref"]::before {
        content: "[[#";
        color: var(--b3-theme-primary);
        display: inline-block;
        text-align: center;
        margin: 0 0 0 0.125em;
        padding: 0;
        position: inherit;
        font-size: 1em;
    }

    .protyle-wysiwyg [data-node-id] span[data-type~="block-ref"]::after {
        content: "]]";
        color: var(--b3-theme-primary);
        display: inline-block;
        text-align: center;
        margin: 0 0.125em 0 0;
        padding: 0;
        position: inherit;
        font-size: 1em;
    }
    ```

- 旧版本 `「 」`

    ```css
    .protyle-wysiwyg [data-node-id] span[data-type~="block-ref"]::before {
        content: "「";
        position: relative;
        color: var(--bracket-color);
        margin-right: 0.1em;
        font-weight: bold;
        font-size: 0.75em;
        top: -0.25em;
    }

    .protyle-wysiwyg [data-node-id] span[data-type~="block-ref"]::after {
        content: "」";
        position: relative;
        color: var(--bracket-color);
        margin-left: 0.1em;
        font-weight: bold;
        font-size: 0.75em;
        bottom: -0.25em;
    }
    ```


