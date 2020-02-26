# JavaScript Code Style Guide

#### Respect the style of the repository you are working in

Different projects have different requirements and tradeoffs to make. This guide is a set of suggestions rather than rules to enforce across all projects.

#### Formatting based on [StandardJS](https://standardjs.com/)

- 2 spaces for indentation
- No semi-colons (but be aware of the [edgecases](https://standardjs.com/rules.html#semicolons))  
- Single quotes for strings

#### Separate formatting commits from implementation commits

This can make the code-review process easier, and can make it easier to rollback changes if something has broken.

#### Autoformatting

We recommend using [prettier](https://prettier.io) for automatting with the following default settings  

```
{
  "printWidth": 100, 
  "semi": false,
  "singleQuote": true,
  "tabWidth": 2,
  `"htmlWhitespaceSensitivity": "ignore"
}
```
