# Commands
```
npm install --save-dev eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin typescript
touch .eslintrc
touch .eslintignore
```


# .eslintrc
```json
{
  "root": true,
  "parser": "@typescript-eslint/parser",
  "plugins": [
    "@typescript-eslint"
  ],
  "extends": [
    "eslint:recommended",
    "plugin:@typescript-eslint/eslint-recommended",
    "plugin:@typescript-eslint/recommended"
  ]
}
```
# .eslintignore
```
node_modules
dist
```

# package.json
```json
{
  "scripts": {
    "eslint": "eslint . --ext .ts",
  }
}
```