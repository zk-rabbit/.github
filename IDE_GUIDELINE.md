# IDE Guideline

## Common

### Using [.editorconfig](https://editorconfig.org/)

To maintain a consistent code style across different IDEs, add an `.editorconfig` file to the root of your project.
The following settings ensure that a newline is automatically inserted at the end of each file and that trailing whitespace is trimmed.
(Note: Removing final newlines is not supported. See the [full list of EditorConfig properties](https://github.com/editorconfig/editorconfig/wiki/EditorConfig-Properties).):

```ini
[*]
trim_trailing_whitespace = true
insert_final_newline = true
```

## VS Code or Cursor

### Configuration

1. Insert Final Newline

   ![vscode_insert_final_newline.png](/vscode_insert_final_newline.png)

2. Trim Final Newlines, Trim Trailing Whitespaces

   ![vscode_trim.png](/vscode_trim.png)

3. Format on Save

   ![vscode_format_on_save.png](/vscode_format_on_save.png)

### Recommended Extensions

- [autopep8](https://open-vsx.org/extension/ms-python/autopep8)
- [code-spell-checker](https://open-vsx.org/extension/streetsidesoftware/code-spell-checker)
- [shellcheck](https://marketplace.visualstudio.com/items?itemName=timonwong.shellcheck)
- [vscode-bazel](https://marketplace.visualstudio.com/items?itemName=BazelBuild.vscode-bazel)
- [vscode-clangd](https://open-vsx.org/extension/llvm-vs-code-extensions/vscode-clangd)
- [vscode-eslint](https://open-vsx.org/extension/dbaeumer/vscode-eslint)
- [vscode-markdownlint](https://open-vsx.org/extension/DavidAnson/vscode-markdownlint)
