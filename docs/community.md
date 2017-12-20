# Community

## Persons

### Persons properties
Phis community is composed of persons which can be either:
- **persons** identified by their names and email. Persons have to be created within Phis before being refered to by projects and expertiments.
- **users**, term refering to persons linked to a Phis account: they are provided with a password that they can change at any time (see [Manage a user account](../community/#manage-a-user-account)).

### New users: get an access to PHIS2
*todo*
ask Phis developpers..
ask smone w/ a Phis account
accounts and authorization access

### Manage a user account
*todo*.
`Tools > Persons`
`ORCID`. Open Researcher and Contributor ID. Optionnal.
You can create and get your orcid at [orcid.org](https://orcid.org/).

### Create a person without account
*todo*
not necessarily existing email adress
no check by mail
from person to user: possible if a awner user updates the person account

### Create an account (admins only)

## Access rights

### User account levels of access
User access rights depend on users groups.

`Classic`: a classic user gets access to public data and data accessible to the groups the user belongs to.

`Admin`: on top of the guest user access rights, an admin can create or delete user accounts.
An admin can also create groups and assign users to those groups.
An admin are usually platform or installation managers, as well as data managers.
There is generally no more than one or two admin per platform.

### Restrictions to a group
A given information can be visible to specific groups. A Phis user not belonging to those groups will not be able to view the data linked to them.
The concepts that can be assigned to groups are experiments and the agronomical objects it contains.
Currently, access rights are managed by experiment.

### Public data
An information assigned to no group is by default set as public. For instance, an experiment not belonging to any group will be viewable to every Phis user, e.g. to every person owning a Phis account.
Research data requiring authrorizations to be accessed to could become public data after several years. *to confirm*

### Groups levels of access
`Guest`: members of a guest group can visualize the data linked to this guest group.

`Owner`: in addition to the visualization rights given to guest groups members, owner groups members can modify the data belonging to the group.

## Groups of users

### Groups properties
Only admin-users are able to view the list of user groups within the `Tools > Groups` menu, not visible from a guest user account.
For instance, the public account *guestphis* has no access to this menu.

From the `Tools > Groups` menu, admin-users get an overview the main properties of all users groups:
- the group URI (standardized, unique and persistent)
- the group name
- the group level of access (guest or owner), cf. [Access rights](../community/#access-rights)

From **Home / Groups**, admin-users can click on the eye icon on the right of a given group in order to view its information sheet.
The additional informations provided by the group sheet are a short description and the persons included in the group, identified by their email address.

Groups informations can be modified with the <span class="btn btn-primary">Update</span> button by the admin-users.

### Create a group (admins only)
Within the `Groups` menu, one can create a new one with the
<span class="btn btn-success">Create Group</span> button.

`URI`. The group URI is automatically created by Phis web service which uses the **Name** of the group provided by the user.

`Name`. Group name composed of an **Organism** name and additional informations on the group (e.g. laboratory and team) provided by the user.
No spaces or hyphen are accepted: they are automatically replaced by dots.
The group **Name** is automatically created in capital letters.

`Organism`. Name of the organism employing the group members.
If a group includes persons from various organisms, instead of an organism name, a project name, or else, can be provided.
No spaces or hyphen are accepted: they are automatically replaced by dots.
The group **Organism** is automatically formatted in capital letters.

Once the group created, its **URI**, **Name** and **Organism** name can no longer be modified.

`Level`. Group's level of access to the experiments it will be involved in: *guest* or *owner*.
A scientific supervisor can consider creating two distinct groups acceding to the same experiments : an owner group that includes the few users susceptible to add and modify experimental data and persons accessing it, and a guest group of persons not involved in the data production, but provided with an access to the data.

`Description`. Complete plain text description of the user group, preferably provided in English language.

`Members`. Email of the Phis persons that will be part of the new group.
This field in the group creation is crucial, but can also be modified at a later time.
Persons are selected from a predefined list of the email identifiying them in Phis.

Note that even persons without an account (persons that are not users) can be added to the new group.

Completing the group creation within Phis is then achieved by clicking on the <span class="btn btn-success">Create</span> button.
