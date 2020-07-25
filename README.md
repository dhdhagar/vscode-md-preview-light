# vscode-md-preview-light

Light-themed stylesheet for markdown preview to use with VSCode's **Dark+** theme.

## Why

In earlier versions of VSCode, setting the Color Theme did not affect the Markdown Preview style. I needed the default white-background-black-font preview while also using a dark theme for the VSCode editor.

## Instructions

In VSCode, edit the **Markdown: Styles** configuration or add the following line to `settings.json`:  

```json
"markdown.styles": [
        "https://cdn.jsdelivr.net/gh/dhdhagar/vscode-md-preview-light/style.min.css"
    ]
```

## Notes

* Maintaining a local style sheet and referencing it with an absolute path did not work
* Referencing `style.css` through <https://raw.githubusercontent.com/dhdhagar/vscode-md-preview-light/master/style.css> did not work either. According to [this discussion](https://github.com/microsoft/vscode/issues/60742), it is because GitHub responds with `X-Frame-Options: deny`
