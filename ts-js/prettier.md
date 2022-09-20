# Commands
```
npm install --save-dev prettier
touch .prettierrc
touch .prettierignore
```


# .prettierrc
```json
{
  "trailingComma": "es5",
  "tabWidth": 4,
  "semi": true,
  "singleQuote": false
}

```
# .prettierignore
```
typechain-types/*
```

# package.json
```json
{
  "scripts": {
    "prettier:fix": "prettier --write --config .prettierrc --check 'src/**/*.ts'",
    "prettier:lint": "prettier --config .prettierrc --check 'src/**/*.ts'",
  }
}
```