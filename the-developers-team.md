# The Developers Team

The **Developers Team** is a *special* Team that is automatically
created when you create an Organization. This page will teach you about
the special properties of this Team, as well as walk through what
happens when you delete this Team, and how to reinstate it.

<hr/>

## Special Defaults

When an Organization is first created, a Team called "developers". This
team is *special* because it has pre-built membership and package access
defaults created for your convenience.

### Members

Members are automatically added to the Developers team:

- The user who created the Organization is added to this team automatically.
- Any member added to the Organization is also added to this
  team automatically.

If an Owner adds a new Member to an Organization and **does not** want
that Member to be on the Developers team, an Owner can remove them. 
([Learn more about managing teams]).

### Package Access

**By default, the developers team has read/write access to all new packages
created under the Organization's scope.** 

A nice side effect of this default is that the [`maintainers` field] in 
the [`package.json`] of any newly created packages under the Organization scope
is automatically populated with the members of the current Developers team. 

If you create a new package under your Organization's scope and you do not
want members of the Developers Team to have Read/Write access to that 
package, an Owner or Admin can remove the Developers Team's access to that
package. ([Learn more about managing Package Access]).

## Removing the Developers Team

An Owner or an Admin can delete the Developers team. If the Developers team
is deleted:

- Newly added Members of the Organization will not be automatically added to
  any team.
- Any package access that current Members had because they were a member of
  the Developers Team will be removed.
- npm will attempt to fill the [`maintainers` field] in [`package.json`] of
  any newly created packages under the Organization scope with the members of
  a Team the publishing user is a Member of. This behavior is not predictable.

## Reinstating the Developers Team

An Owner or Admin can "reinstate" the Developers team by creating a new team
with the name "developers". This "new" Developers team will have all the 
default behavior of the original Developers team:

- All Members added to the Organization after the Developers Team is 
  reinstated will be automatically added to the Developers Team
- All Members of the Developers team will automatically have Read/Write access
  to all new packages created under the Organization scope

You **will** need to manually add any members of the Organization that existed
before the Developers team was "reinstated" if you'd like them to also 
experience the special Developers Team defaults. 
([Learn more about managing teams]).

[Learn more about managing teams]: managing-teams.md
[Learn more about managing Package Access]: managing-package-access.md
[`maintainers` field]: https://docs.npmjs.com/files/package.json#people-fields-author-contributors
[`package.json`]: https://docs.npmjs.com/files/package.json
