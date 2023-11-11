[Github repository](https://github.com/frostime/sy-dark-purple)

This theme is modelled on Jetbrain's Dark Purple theme and contains only css styles.

### Acknowledge

This theme was inspired in part by the following themes, for which we would like to thank you.

- [Light Blue](https://github.com/Morganwan90/Darkblue-siyuan-theme)
- [Tsundoku](https://github.com/Achuan-2/siyuan-themes-tsundoku)
- [Savor](https://github.com/royc01/notion-theme)

### About ref-link style

Current ref-link/wiki-link use the style `[[#<ref name>]]`, you can modify it in code snippet.

- Current stype: `[[# ]]`

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

- Old style `「 」`

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
