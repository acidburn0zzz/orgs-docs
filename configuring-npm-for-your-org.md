# Configuring npm for Your Org

## Configuring npm for Your Scope

The npm CLI is configurable! [Learn more about configuring npm].

If you intend on publishing packages with your Organization scope more
often that not, you may want to add your Organization scope to your
global `.npmrc` file. [Learn more about the `.npmrc` file].

To set your Organization scope globally for your instance of the npm
CLI, use this command:

```
npm config set scope <org_scope> --global
```

[Learn more about the CLI `config` command].

Once you issue this command, all packages that you create with 
`npm init` will be scoped to your Organization scope. 

To verify this, create a new package with `npm init`. Open the
generated `package.json` and view the `name` property. If you 
successfully configured npm, you should see your Organization's
scope preceding the packages name in the `name` property.

For packages you do not want to publish with the Organization's
scope, you can manually edit the generated `package.json`, removing
the Organization scope from the `name` field.

## Configuring npm for Your Org Plan

[Learn more about the `.npmrc` file]: https://docs.npmjs.com/files/npmrc
[Learn more about the CLI `config` command]: https://docs.npmjs.com/cli/config
[Learn more about configuring npm]: https://docs.npmjs.com/misc/config
