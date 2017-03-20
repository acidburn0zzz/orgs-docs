# Publishing an Org Scoped Package

One of the great benefits of using an Organization is that you can
publish packages, publicly or privately, under a shared namespace,
called the **Organization scope**. This is similar to a user 
namespace, or **User scope**, however an Organization scope makes
it much easier to manage package access for multiple packages and
multiple users.

This page will teach you how to publish an Organization scoped package,
both publicly and privately. This page will also teach you how to
configure you npm so that it automatically creates packages with your
Organization scope.

Don't forget that all Members of an Organization are immediately added
to a Developers team that automatically has Read/Write access to all
packages published under an Organization scope. 
([Learn more about the Developers Team])

<hr/>

## Creating a New Scoped Package

To create a new scoped package for your Organization scope, create
a directory with the name of the package you would like to create.
Navigate into that directory and use this command:

```
npm init --scope=<org_scope>
```

To verify that this worked, open the generated `package.json` with an
editor of your choice. You should see that the name of the package
will be `@org_scope/<pkg_name>`.

## Publishing a Private Scoped Package

By default, `npm publish` will publish a scoped package as private.
Therefore, to privately publish a scoped package as private, type:

```
npm publish
```

[Learn more about the CLI `publish` command].

You can verify that this worked by going to your npm profile or your
Organization's profile and look at the packages list. You should see
your newly published package listed there. You will know it is private
because there will be a small lock icon next to the package name.

## Publishing a Public Scoped Package

By default all scoped packages are published privately. To publish a
scoped package publicly, pass the `access` flag with the value 
`public`:

```
npm publish --access public
```

[Learn more about the CLI `publish` command].

You can verify that this worked by going to your npm profile or your
Organization's profile and look at the packages list. You should see
your newly published package listed there. You will know it is public
because there will *not* be a small lock icon next to the package name.

You can doubly verify this by opening a private browser tab and 
viewing your npm profile or your Organization's profile. The package
should be present on both package listings.

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

[Learn more about the Developers Team]: the-developers-team.md
[Learn more about the CLI `publish` command]: https://docs.npmjs.com/cli/publish
[Learn more about the `.npmrc` file]: https://docs.npmjs.com/files/npmrc
[Learn more about the CLI `config` command]: https://docs.npmjs.com/cli/config
[Learn more about configuring npm]: https://docs.npmjs.com/misc/config
