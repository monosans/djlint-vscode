# djlint-vscode

Visual Studio Code extension for formatting and linting Django/Jinja HTML templates using [djLint](https://djlint.com).

## Installation

Search for `djLint` in VS Code extensions.

[Visual Studio Code Marketplace page](https://marketplace.visualstudio.com/items?itemName=monosans.djlint)

## Usage

`djlint-vscode` automatically sets djLint's `profile` setting in accordance with language ID.

| Language ID | djLint profile |
| ----------- | -------------- |
| html        | html           |
| django-html | django         |
| jinja-html  | jinja          |
| jinja       | jinja          |
| nj          | nunjucks       |
| njk         | nunjucks       |
| nunjucks    | nunjucks       |

Some djLint options, such as `indent` and `ignore`, can be configured directly in the VSCode settings. Other djLint options can be set through the configuration file, as indicated in the [corresponding documentation](https://djlint.com/docs/configuration/). Please do not change the `linter_output_format` setting, otherwise linter will work incorrectly.

Add this to your `settings.json` to format all supported file types with `djLint`:

```json
"[html]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[django-html]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[jinja-html]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[jinja]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[nj]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[njk]": {
  "editor.defaultFormatter": "monosans.djlint"
},
"[nunjucks]": {
  "editor.defaultFormatter": "monosans.djlint"
},
```

## Disclaimer

This extension is not affiliated with the authors of [djLint](https://djlint.com).
