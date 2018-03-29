
# npm Orgs

_This is a top-level introduction to Orgs. Skip ahead if you are ready to [get started](https://www.npmjs.com/docs/orgs/getting-started.html)._

<hr>

We created npm Orgs to make it easier to manage packages and teams of developers. 

Read this chapter to get some ideas about how you might use npm Orgs. You can find detailed instructions in the later chapters of this book.  

## Organizing Packages

When you create an Organization, you are granted an Organization _scope_, a unique namespace for packages. The Organization scope will match the name that you give your Organiation. For example, if your organization is called "the best", you would register
as "the-best" and get a scope, `@the-best`. 

### What is a scope? 

A scope multiplies the number of names you can give packages, because the packages you name will have the scope as part of their name. For example, if your scope is `@the-best` you can name a package `@the-best/puppy`, even though the name `puppy` by itself is taken. This gives you an entire world of possibilities for naming, because package names can only be used once. 
Scopes make it easier to:

- Maintain a fork of a package, e.g. `@the-best/request`.
- Avoid name disputes with popular names, e.g. `@the-best/cat`.
- Find packages within your organization.
- Group packages together for a single project. (Teams can also be used for this). 

#### npm Naming guidelines 

Even with scoped packages, keep npm naming guidelines in mind. These are similar to the general package name [guidelines](https://docs.npmjs.com/files/package.json#name). Basically, avoid using vulgar names, and avoid naming packages anything that might offend someone else, cause ownership confusion, or infringe a copyright. 


### Can I use my npm Org to manage packages that don't use my Org's scope? 
 
Yes. While you are granted a scope by default when registering as an Org, using the scope is optional. In fact, you can use Orgs to manage unscoped
packages, or even packages under a different scope, such as a user scope,
e.g. `@isaacs/hello`, where `isaacs` is an npm user.

## Organizing Access to Packages

A key benefit of npm Orgs is that it makes it easier, and in some cases,
simply *possible*, to manage access and visibility of packages across
a large team of contributors.

To get the biggest benefit from Orgs:

1. Organize your developers into teams. 
2. Grant team permissions (read/write) to packages you govern, which then
cascades to all Members of that team. 

This way, certain teams can develop a package (write access) while other teams can use the package but can't modify it (read access). You can set the access that makes sense for your project, for all of the packages that the Organization governs, public unscoped packages and public/private scoped packages 
alike. 

### Adding Members to an Org

Working with teams, adding packages, and setting access levels is easy using npmjs.com.

To add npm users to your Org, just type their npm username, and select an access level:

<img src="member-admin-owner-invite.png" style="border: 1px solid gray;">

### Adding Org Members to a Team
To add existing Org members to a team, just start typing their name. A drop-down menu will appear. 

<img src="org-add-users2.png" style="border: 1px solid gray;">


### Setting Team Package Access

To manage package and package access, click `read` or `read/write`: 

<img src="add-access-package.png" style="border: 1px solid gray;">

## What is the cost?

Orgs are **free** if your Organization only uses public packages.

If your Organization needs to also publish and install **private packages**, an Org will cost you $7/month/user, for each user, including yourself. 

It's easy to [upgrade](https://www.npmjs.com/docs/orgs/upgrading-and-downgrading.html) as your needs change. 

For detailed cost information, see the [pricing](https://www.npmjs.com/pricing) page. 

# Learn More 

This doc is focused on npm Orgs. For docs about other aspects of npm,  including [CLI docs](https://docs.npmjs.com/cli/help), visit the [docs page](https://docs.npmjs.com/). 

To learn how one customer uses npm Orgs, click [here](http://blog.npmjs.org/post/162404021573/customer-convo-dan-gebhardt-cerebris). Or read [another convo](http://blog.npmjs.org/post/160049089651/customer-convos-rob-tirserio-remedy-health-media).

For npm news, click [here](http://blog.npmjs.org).

