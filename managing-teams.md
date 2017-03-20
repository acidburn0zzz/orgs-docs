# Managing Teams

The key to managing package access in an Organization is Teams.
**Teams are sets of Organization Members that have defined privileges
for a set of packages that are controlled by the Organization**.
This page will teach you how to create and manage the 
membership of your Organization's team from the web interface.

If you would like to manage the membership of your Team from
the npm command line interface (CLI), you can use:

```
npm team
```

Learn more about `npm team` [here][2].

If you are looking for how to manage a Team's Package Access, check
out [this doc][1].

You will need to have the **Owner** or **Admin** Role to perform this
work. For more information on **Roles**, check out the 
[Roles and Privileges doc].

<hr/>

To manage your Organization's Teams, navigate to your
Organizations landing page. You can find it at
`https://www.npmjs.com/org/<org_name>`.

Once you are on your Organization's landing page, click the "Teams" tab.
You can also just point your browser at 
`https://www.npmjs.com/org/<org_name>/teams`.

## Creating a Team

To create a team:

1. Click the "Create a Team" button
2. Give your team a name. Your team name must be lower case and have no
  spaces or punctuation. Choose wisely! A team's name cannot be changed.
3. Optionally, give your team a description.
4. Optionally, add Organization members to your team. You can always
  add (or remove!) members later, so feel free to skip this.
5. Click the "make it so" button.

#### Notes

- Inviting an Organization Member to a new team does not send that user
  an email. Make sure to tell your new team member that you added them.
- New teams do not have any package access by default. Once you create
  a team, you should add Package Access to the Team. 
  ([Learn more about managing Package Access]).

## Managing Team Membership

To manage the membership of a Team, navigate to your Team's landing page.
You can find a list of your teams at `https://www.npmjs.com/org/<org_name>/teams`.

From this list, you can click the value in the "members" column. 

- If the Team has members, this value will be the current Member Count. Clicking
  this value will bring you to the Members tab for this team.
- If the Team does not have any members, this value will read "invite users".
  Clicking this value will bring you to the Team Member Invite page.

You can also navigate to your Team page directly by point your browser at
`https://www.npmjs.com/org/<org_name>/teams/<team_name>`.

From there, click the "Members" tab. You'll use this interface to manage the
membership of your Team.

### Adding a Member to a Team

To add a member to a team:

1. Enter the npm username of the user you would like to add to your Team.
2. Click the "add" button.
3. Repeat this until you have added all the members you would like to.
4. Click "make it so" button.

To save time, you can populate your team from an existing team. To populate
your team from an existing team:

1. Choose the team you would like to populate your new team from in the 
  dropdown at the top of the page.
2. When you release the dropdown, you should see the usernames of the members
  of that previously existing team appear in the list of Users to be added to
  your team.

#### Notes

- Adding a Organization member to a new Team does not send them an email. Let
  your new team member know that you added them to a new team!
- You cannot add a user who is not a member of your Organization to a Team. 
  Ask an Owner to invite them to the Organization so that you can add them to
  a Team. ([Learn more about managing Members]).
- Organization Members cost $7/member/month if the Organization has Private
  Packages even if the Teams the Member is a part of do not have access to
  Private Packages. 

### Removing a Member from a Team

To remove a member from a Team:

1. Locate the **Member** in the list of members.
2. Click the white X in the grey circle at the far right of the row.
3. The page will refresh. You should see a message telling you the status of your
   delete request. If your delete request was successful, you should no longer see
   the member you deleted in the list of members.

#### Notes

- Removing a Member from a Team, even if it is the only Team they are associated
  with, will **not** remove the Member from the Organization. If you would like to
  remove the Member from the Organization, you will need to be an Owner or ask
  an Owner. ([Learn more about managing Members]). 

[1]: managing-package-access.md
[Roles and Privileges doc]: roles-and-privileges.md
[Learn more about managing Package Access]: managing-package-access.md
[Learn more about managing Members]: managing-members.md
[2]: https://docs.npmjs.com/cli/team
