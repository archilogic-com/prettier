# Archilogic's shared [Prettier](https://prettier.io) configuration

## Using this config

To use the shared Prettier config in your project, add this package as a dev dependency (along with Prettier itself):

`npm i -D prettier @archilogic/prettier`

Then, add a `prettier` option to your `package.json`:

```
{
  "name": "ui-components",
  "version": "9000.0.1",
  "scripts": {...},
  "prettier": "@archilogic/prettier"
}
```

or create a `.prettierrc.json` file with the following line:

```
"@archilogic/prettier"
```

### Adding a format script

To format all your files, run `npx prettier --write .`.
Or add a script to `package.json`

```
"scripts": {
  "format": "prettier --write ."
}
```

### Formatting on commit (recommended)

To enforce Prettier formatting in a project, you can configure it to run as a pre-commit hook.
See [pre-commits docs](https://prettier.io/docs/en/precommit.html) (Option 1 recommended).

### Editor Integration

It is recommended that you set up your editor to automatically format the code as you go.
See [editor integration docs](https://prettier.io/docs/en/editors.html).

## Recommended settings

Recommended [Prettier settings](prettier.json) in this config are based on [StandardJS](https://standardjs.com/):

- 2 spaces for indentation
- No semi-colons (Prettier takes care of the [edgecases](https://standardjs.com/rules.html#semicolons))
- Single quotes for strings

If you need to extend the configuration or overwrite some of its settings, import the file in a `.prettierrc.js` file and export the modifications, e.g:

```
module.exports = {
  ...require("@company/prettier-config"),
  semi: false,
};
```
