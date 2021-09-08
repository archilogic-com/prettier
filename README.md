# JavaScript Code Style Guide

This guide is a set of suggestions rather than rules to enforce across all projects

#### Formatting based on [StandardJS](https://standardjs.com/)

- 2 spaces for indentation
- No semi-colons (but be aware of the [edgecases](https://standardjs.com/rules.html#semicolons))
- Single quotes for strings

#### Autoformatting with [Prettier](https://prettier.io)

To use the shared Prettier config, add this package as a dependency:

`npm i -D github:@archilogic-com/js-guide#al-1099-publish-prettier-config-as-archilogic`

Then, add a `prettier` option to your `package.json` or a `.prettierrc.json` file with the following value:
`@archilogic-com/prettier`.

Recommended [prettier] settings:

```
{
  "printWidth": 100,
  "semi": false,
  "singleQuote": true,
  "tabWidth": 2,
  "jsxBracketSameLine": true,
  "htmlWhitespaceSensitivity": "ignore",
  "trailingComma": "none",
  "arrowParens": "avoid"
}
```
