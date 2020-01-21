# vscode-notes README

This extension adds the `.nt` or `.note` file type. This file type offers syntax highlighting for list-based note items indexed by one of the common list denominators (including `-`, `*`, or even `•`). It is meant to be used by programmers or non-programmers alike and requires no knowledge of any programming language syntax.

## Example

```
Headline:

    Sub-headline:

        - Bullet point: this is a bullet point
        • Bullet point 2: this is also a bullet point
```

## Markdown

The note file type supports limited markdown (specifically, bold and italic) via either the asterisk or underscore notation (`**bold**` or `__bold__` and `*italic*` or `__italic__`). However, to make these work, an additional step is necessary.

Open your VSCode's `settings.json` and add the following:

```
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": ["formatting.italic"],
                "settings": {
                    "fontStyle": "italic"
                }
            },
            {
                "scope": ["formatting.bold"],
                "settings": {
                    "fontStyle": "bold"
                }
            },
        ]
    }
```