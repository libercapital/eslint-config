# ESLint Libercapital

## Basic setup

### .editorconfig

```text
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true

[*.md]
trim_trailing_whitespace = false

[*.txt]
trim_trailing_whitespace = false
insert_final_newline = false

[{Makefile,**.mk}]
indent_style = tab
```

### .eslintrc

```json
{
  "extends": ["@libercapital/eslint-config"]
}
```

### .prettierrc

```json
{
  "singleQuote": false,
  "tabWidth": 2
}
```

### .prettierignore

```text
.gitignore
.prettierignore
yarn.lock
yarn-error.log
package-lock.json
LICENSE
*.ejs
dist
coverage
pnpm-lock.yaml
```

## VSCode

### .vscode/extensions.json

```json
{
  "recommendations": [
    "editorconfig.editorconfig",
    "dbaeumer.vscode-eslint",
    "esbenp.prettier-vscode"
  ]
}
```

### .vscode/settings.json

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
}
```
