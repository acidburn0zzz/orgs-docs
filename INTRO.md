# npm Orgs

*This is a top-level introduction to Orgs. If you already know what Orgs are
and want to get up and running, you should jump ahead to "Getting Started".*

<hr>

Orgs is a tool for organization, both of packages and teams of developers.
It was created out of the need by many package publishers to handle
large numbers of contributors over a set of many packages.

## Organizing Packages

Creating an organization on npm gives you an organization scope under
which you can have your own namespace for packages. The organization
scope is the name of the organization, as registered on npm. For
example, if your organization is called "the best", you would register
as "the-best" and get a scope, `@the-best`. From there, you could name
your packages whatever you want (according to our guidelines).

Scopes are great for many reasons, some examples:

- maintain a fork of a package, e.g. `@the-best/request`
- avoiding name disputes with popular names, e.g. `@the-best/cat`
- improving internal discovery of organization supported packages
  (they're all in a single namespace!)

While you get a scope by default when registering as an Org, that doesn't
mean you *have* to use it. In fact, you can use Orgs to manage unscoped
packages, or even packages under a different scope, such as a user scope,
e.g. `@ag_dubs/hello`, where `ag_dubs` is an npm user.

## Organizing People

The real benefit of Orgs is that it makes it better, and in some cases,
simply *possible*, to manage access and visibility of packages across
a large team of contributors.

When using Orgs, you organize your developers into Teams. You can then
grant team permissions (read/write) to packages you govern, which then
cascades to all members of that team. By doing this, you can have certain
teams that develop a package (write access) and then some teams that can use
that package (read access). You can do this for all of the packages that
the organization governs, public unscoped packages and public/private
scoped packages alike.

## What does Orgs cost?

Orgs are **free** if your organization only has public packages.

If your organization needs to also publish and install **private packages**,
an Org will cost you $7/user/month, for all users.
