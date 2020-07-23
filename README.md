
# GSA github Reference
 
## Setup
GitHub is a web application, so there’s no installation necessary

## Creating a GitHub account
1.	 If you haven't created a GitHub account yet (https://github.com/), do so with your GSA email address.
2.	 If you already have a GitHub account, simply [add your GSA email to your existing account](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/adding-an-email-address-to-your-github-account)   Do not create a new account. Make sure your commits are [associated with your GSA mail address](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/setting-your-commit-email-address) 
3.	 If you have another email specified  in your [GitHub settings](https://github.com/settings/emails), they will both be tied to your GitHub account.
4.	Make sure you have [notifications turned on](https://github.com/settings/notifications) and make sure your notifications are set up the way you'd like them.

## Complete your profile

Include the following:
* Name: Your first and last name.
* Company: Your government agency.
* Location: Your primary work location (city, state).

## Set up two-factor authentication

Two-factor authentication is required for all members and collaborators in the GSA org. You can choose among multiple options to add a second source of authentication to your account. You can configure two-factor authentication using a mobile app or via text message. You can also add a security key.  See: [Configuring two-factor authentication](https://docs.github.com/en/github/authenticating-to-github/configuring-two-factor-authentication)

## Turn notifications on 
[Turn notifications on](https://github.com/settings/notifications) and adjust the settings as needed. Some people watch every repo; others only watch when they’re mentioned.

You will get a lot of emails when you turn notifications on. To help stem the tide, you can set up a Gmail filter to automatically archive emails from
`notifications@github.com`. However, you probably want to let through those emails that contain your GitHub username or are posted to a repo you’re watching. 

Since on GitHub, each repo is considered its own mailing list, checking for that identifier is one reliable way to allow these notifications through. For example, if the repo name in GitHub is GSA/reponame, the mailing list will be reponame.gsa.github.com. 

You can also find this by opening an email from the desired repo, clicking the “more info” arrow in the “To” field, and copying the bracketed address in the “mailing list” field. Adding list:(reponame.GSA.github.com) to your filter’s exceptions will allow any issues posted to that repo to reach your inbox.

# Join the GSA organization
Email `gsa-github.support@gsa.gov` the following: 
“Please add me `<https://github.com/username>` to `<https://github.com/GSA>`”.  Please supply your github username and GSA email address.
 
Also, to make it easier, please describe any team(s) or repo(s) you will need access to.  The owner or admin of the requested repo or team will need to grant access. An admin will verify compliance and add you, after which you’ll need to accept their invite by going [here](https://github.com/GSA).

## Outside Collaborators:
Repositories with the GSA org can only be accessed by members in the organization.  If a user needs access to a repository with the organization but is not a GSA employee or a contractor with a GSA email address, they will need to be invited as outside collaborators.

Only a member of the GSA Admin Team can invite an outside collaborator. Outside collaborators with access to a private repository incur charges (like a paid seat).  

Outside collaborators will not be allowed access to a private repository, without justification  from the requesting Program Office and final approval from a GSA Admin Team member. 
In addition,  outside collaborators will not be allowed admin access to a repository within the GSA organization.
  
## Make your membership public
Go to the GSA org people page. Click where it says private next to your name. Change that to public.
Each GSA user must
*	Activate 2-factor Authentication
*	Add your information to your account
*	Add a profile avatar
*	Make your membership public

Each repository should:
*	Have a simple and useful name
*	Have a user-friendly description
*	Have a useful README.md
 
## Standards for making a private repo: 
Since GSA is following its own Open Sources policy,  by default, projects in GitHub.com/GSA should be public.  They should only be made private under certain circumstances. 

A repository should be made private if it contains information that legally cannot be made public. 

## Creating new public repositories
1. At https://github.com/GSA, Click `+ New Repository`. 
2.	When choosing the repo's name, try to pick a simple and useful name
3.	Include a brief description of the project. 
4.	Change the repo status to `Public` unless it needs to be private. 
5.	Note: we recommend the following when exposing your repositories to the public:
a.	Conduct a manual code review with your team.  Go line by line through the code and check for sensitive content.
b.	Conduct static code analysis with a scanning tool (if available). SonarQube is approved as a standard. Teams can download it in their local environment and scan/remediate. Hopefully we can recommend other tools in the future. 
c.	Utilize a process to remediate security vulnerabilities within the code base or the environment.
d.	Make environmental variables private or store them on a server
6.	Repos at a minimum should have a README and LICENSE file providing instructions to future contributors on how to setup and test the application in order to make suggestions. It is encouraged to have CONTRIBUTING and CODE_OF_CONDUCT files.See https://github.com/GSA/code-gov-front-end for some examples.
7.	You will usually not need to worry about adding a `.gitignore` unless you are going to store env variables or other dot file content. 
7.	GSA Legal has determined that all GSA code should be CC0.   Work with your program office / legal counsel if you have any questions.  See  description of the license types
8.	Click Create Repository
9.	If prompted, choose the most appropriate team that you are a member of that should be given permission to the repo. 

## Creating new private repositories
The above directions are the same except that at step 4, you will choose Private instead of Public. 

## Creating Teams in the GSA organization
It is recommended to create teams to manage member’s access to a  repository.  Establish separate teams for each access role:  one for team admin users; a different team for your developers with write access; and one for users with read only access.  You can assign the Team maintainer role to an individual(s) who would then be able to add / remove members to the repository’s teams.   For help in creating teams, please see [Creating a Team](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/creating-a-team) or email gsa-github.support@gsa.gov 

## Removing access to the GSA organization
*	 Team managers should ensure that they monitor when a member of their GitHub team leaves the project or agency and no longer needs access to the GSA organization.  
*	At that point, they should email 'gsa-github.support@gsa.gov' with a request to remove the user from the GSA organization.
*	Organization admins should reply to the email with confirmation when the removal is complete. 
*	Team managers may delegate this responsibility but need to ensure that it is in place. 
If a member leaves github and they are the sole owners of the repository,  if the repository is not archived or transferred to someone else,  it will be deleted.  

## Third-party access
If you are requesting third-party access apps to access GitHub,  the app needs to be in the GSA IT Enterprise Architecture GEAR listing as approved ( https://ea.gsa.gov/#!/itstandards ) and whoever wants to use the app needs to shepherd it through the GEAR process for approval.  Once it is approved in the It Standards, it can be approved in GitHub.  If there is a cost involved in the third-party app, the requesting program office is required to pay for it.

## Organize Agency Users
*	Identify Team Leads
*	Ensure everyone has guidance going forward
*	Repo owners should certify users to their own repos.  
*	It is recommended to make use of teams for better organization.  The repo admin could create a team with admin access for the repo,  a team with read-only access, and a team for read/write access.   They would then delegate a ‘team maintainer ‘ for adding/.removing members from the team
*	Users will need to reply to the annual recertification

 
