# Roles and Privileges

This page will give you a top level overview of the roles and privileges
you can assign to members of your team.

<hr/>

Organizations allow you to manage privileges of multiple contributors. Roles
allow you to assign members of your Organization the ability to manage
different aspects of the Organization.

There are several types of management in an Organization:

- [Package access management]
- [Member management]
- [Team maangement]
- [Billing management]

There are three (3) roles in an Organization:

- **Owner**
- **Admin**
- **Member**

|                                             | **Owner** | **Admin** | **Member** |
|---------------------------------------------|-----------|-----------|------------|
| Manage billing                              | ✅         | ❌         | ❌          |
| Add/remove any **Member** to/from the Org   | ✅         | ❌         | ❌          |
| Change any Member's **Role**                | ✅         | ❌         | ❌          |
| Create/delete **Teams**                     | ✅         | ✅         | ❌          |
| Add/remove any **Member** from any **Team** | ✅         | ✅         | ❌          |
| Manage **Team** package access              | ✅         | ✅         | ❌          |

## Owner

The user who creates the Organization is automatically set up as an Owner.
An Owner is the highest level of privilege in the Organization and can
manage any and all aspects of the Organization..

An Owner is the **only Role** that can:

- Manage billing 
- Add/remove any **Member** to/from the Org
- Change any Org member's **Role** 

They can also:

- Create/delete **Teams**
- Add/remove any **Member** from any **Team**
- Manage **Team** package access

**You cannot remove the last owner from an Organization.** (This would
render the Organization inaccessible. If you are trying to delete your
organization, you can learn more [here][1].)

## Admin

An admin is a team leader. This is the second highest level of privilege.
Admin privileges allow a user to manage Teams and package access.

An Admin can:

- Create/delete **Teams**
- Add/remove any **Member** from any **Team**
- Manage **Team** package access

If an Admin would like to add an npm user to their team, they will need
to ask and Owner to first add that user as a member of the Organization.

## Member

Members are the lowest level of privilege in an Organization. They do not
have any management privileges.

[1]: renaming-and-or-deleting-an-org.md
[Package access management]: managing-package-access.md
[Member management]: managing-members.md
[Team maangement]: managing-teams.md
[Billing management]: managing-billing.md
