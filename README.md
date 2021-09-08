# JavaScript Code Style Guide

This guide is a set of suggestions rather than rules to enforce across all projects

## Formatting based on [StandardJS](https://standardjs.com/)

- 2 spaces for indentation
- No semi-colons (but be aware of the [edgecases](https://standardjs.com/rules.html#semicolons))
- Single quotes for strings

## Autoformatting with [Prettier](https://prettier.io)

### Prettier Config
**Recommended [Prettier settings](prettier.json)**

To use the shared Prettier config in your project, add this package as a dependency:

`npm i -D github:@archilogic-com/js-guide`

Then, add a `prettier` option to your `package.json`:

```
{
  "name": "ui-components",
  "version": "9000.0.1",
  "scripts": {...},
  "prettier": "@archilogic-com/prettier"
}
```

or create a `.prettierrc.json` file with the following line:
```
"@archilogic-com/prettier"
```

### Editor Integration
It is recommended you set up your editor to automatically format your code as you go.
For VSCode configuration, see the [Prettier extention docs](https://github.com/prettier/prettier-vscode).

### Formatting on commit
To enforce Prettier formatting in a project, you can configure it to run as a pre-commit hook.
See details [in Prettier docs](https://prettier.io/docs/en/precommit.html) (Option 1 recommended).



