# JavaScript Code Style Guide

This guide is a set of suggestions rather than rules to enforce across all projects

#### Formatting based on [StandardJS](https://standardjs.com/)

- 2 spaces for indentation
- No semi-colons (but be aware of the [edgecases](https://standardjs.com/rules.html#semicolons))  
- Single quotes for strings

#### Autoformatting

Recommended [prettier](https://prettier.io) settings:

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
