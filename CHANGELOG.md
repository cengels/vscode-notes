# Change Log

All notable changes to the "vscode-notes" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [1.0.0] - 2020-07-19

- Fix issue where markdown highlighting (bold and italic) wouldn't function inside a note item
- Fix issue where list punctuation (bullet points) were incorrectly scoped as `support.type.property-name.note` (now: `punctuation.definition.block.sequence.item.note`)
- Add non-dictionary list items (like `• simple list item`)
