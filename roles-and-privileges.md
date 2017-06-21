# Roles and Privileges

This page will give you a top-level overview of the roles and privileges
you can assign to members of your Organization.

<hr/>

Organizations allow you to manage the privileges of multiple contributors. Roles
allow you to assign members of your Organization the ability to manage
different aspects of the Organization.

There are several types of management in an Organization:

- [Billing management]
- [Member management]
- [Team management]
- [Package access management]

There are three (3) roles in an Organization:

- **Owner**
- **Admin**
- **Member**

|                                             | **Owner** | **Admin** | **Member** |
|---------------------------------------------|-----------|-----------|------------|
| Manage billing                              | ✅         | ❌         | ❌          |
| Add/remove any **member** to/from the Org   | ✅         | ❌         | ❌          |
| Change any member's **role**                | ✅         | ❌         | ❌          |
| Create/delete **Ttams**                     | ✅         | ✅         | ❌          |
| Add/remove any **member** from any **team** | ✅         | ✅         | ❌          |
| Manage **team** package access              | ✅         | ✅         | ❌          |

## Owner

The user who creates the Organization is automatically set up as an owner.
An owner is the highest level of privilege in the Organization and can
manage any and all aspects of the Organization.

An owner is the **only role** that can:

- Manage billing.
- Add/remove any **member** to/from the Org.
- Change any Org member's **role**. 

They can also:

- Create/delete **teams**.
- Add/remove any **member** from any **team**.
- Manage **team** package access.

**You cannot remove the last owner from an Organization.** (This would
render the Organization inaccessible. If you are trying to delete your
Organization, you can learn more [here][1].)

## Admin

An admin is a team leader. This is the second highest level of privilege.
Admin privileges allow a user to manage teams and package access.

An admin can:

- Create/delete **teams**.
- Add/remove any **member** from any **team**.
- Manage **team** package access.

If an admin would like to add an npm user to their team, they will need
to ask an Owner to first add that user as a member of the Organization.

## Member

Members are the lowest level of privilege in an Organization. They do not
have any management privileges.

[1]: renaming-and-or-deleting-an-org.md
[Package access management]: managing-package-access.md
[Member management]: managing-members.md
[Team management]: managing-teams.md
[Billing management]: managing-billing.md
