# NextJS (Boilerplate)

## auto eslint on commit

### dev steps

_.eslintrc.json_

```json
{
  "extends": ["next", "next/core-web-vitals"],
  "rules": {
    "no-unused-vars": "error",
    "indent": ["error", 2]
  }
}
```

_package.json_

```
 "pre-commit": "yarn lint --fix && git add -A ."
```

- `yarn add husky`
- `npm set-script prepare "husky install"`
- `yarn prepare`
- `yarn husky add .husky/pre-commit "yarn pre-commit"`
