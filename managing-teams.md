# Managing Teams

The key to managing package access in an Organization is teams.
**Teams are sets of Organization members that have defined privileges
for a set of packages that are controlled by the Organization**.
This page will teach you how to create and manage the 
membership of your Organization's team from the web interface.

If you would like to manage the membership of your team from
the npm command line interface (CLI), you can use:

```
npm team
```

Learn more about `npm team` [here][2].

If you are looking for how to manage a team's package access, check
out [this doc][1].

You will need to have the **owner** or **admin** role to perform this
work. For more information on **roles**, check out the 
[Roles and Privileges doc].

<hr/>

To manage your Organization's teams, navigate to your
Organization's landing page. You can find it at
`https://www.npmjs.com/org/<org_name>`.

Once you are on your Organization's landing page, click the "Teams" tab.
You can also just point your browser at 
`https://www.npmjs.com/org/<org_name>/teams`.

## Creating a Team

To create a team:

1. Click the "Create a Team" button.
2. Give your team a name. Your team name must be lower case and have no
  spaces or punctuation. Choose wisely! A team's name cannot be changed.
3. Optionally, give your team a description.
4. Optionally, add Organization members to your team. You can always
  add (or remove!) members later, so feel free to skip this.
5. Click the "make it so" button.

#### Notes

- Inviting an Organization member to a new team does not send that user
  an email. Make sure to tell your new team member that you added them.
- New teams do not have any package access by default. Once you create
  a team, you should add package access to the team. 
  ([Learn more about managing Package Access]).

## Managing Team Membership

To manage the membership of a team, navigate to your team's landing page.
You can find a list of your teams at `https://www.npmjs.com/org/<org_name>/teams`.

From this list, you can click the value in the "Members" column. 

- If the team has members, this value will be the current member count. Clicking
  this value will bring you to the members tab for this team.
- If the team does not have any members, this value will read "invite users".
  Clicking this value will bring you to the team member invite page.

You can also navigate to your team page directly by pointing your browser at
`https://www.npmjs.com/org/<org_name>/teams/<team_name>`.

From there, click the "Members" tab. You'll use this interface to manage the
membership of your team.

### Adding a Member to a Team

To add a member to a team:

1. Enter the npm username of the user you would like to add to your team.
2. Click the "add" button.
3. Repeat this until you have added all the members you would like to.
4. Click "make it so" button.

To save time, you can populate your team from an existing team. To populate
your team from an existing team:

1. Choose the team you would like to populate your new team from in the 
  dropdown at the top of the page.
2. When you release the dropdown, you should see the usernames of the members
  of that previously existing team appear in the list of users to be added to
  your team.

#### Notes

- Adding a Organization member to a team does not send them an email. Let
  your new team member know that you added them to a team!
- You cannot add a user who is not a member of your Organization to a team. 
  Ask an Owner to invite them to the Organization so that you can add them to
  a team. ([Learn more about managing members]).
- Organization members cost $7/member/month if the Organization has private
  packages even if the teams the member is a part of do not have access to
  private packages. 

### Removing a Member from a Team

To remove a member from a team:

1. Locate the **member** in the list of members.
2. Click the white X in the grey circle at the far right of the row.
3. The page will refresh. You should see a message telling you the status of your
   delete request. If your delete request was successful, you should no longer see
   the member you deleted in the list of members.

#### Notes

- Removing a member from a team, even if it is the only team they are associated
  with, will **not** remove the member from the Organization. If you would like to
  remove the member from the Organization, you will need to be an Owner or ask
  an Owner. ([Learn more about managing members]). 

[1]: managing-package-access.md
[Roles and Privileges doc]: roles-and-privileges.md
[Learn more about managing Package Access]: managing-package-access.md
[Learn more about managing Members]: managing-members.md
[2]: https://docs.npmjs.com/cli/team
