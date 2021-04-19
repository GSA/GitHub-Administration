<h1>GSA GitHub Enterprise Cloud Reference</h1>
Follow this guide when using GitHub







## Table of Contents

[Introduction](#introduction)

[Joining the GSA Enterprise Organization](#joining-the-gsa-enterprise-organization)

[Complete your profile](#complete-your-profile)

[Set up two-factor authentication](#set-up-two-factor-authentication)

[Turning on notifications](#turning-on-notifications)

[Join the GSA organization](#join-the-gsa-organization)

[Outside Collaborators](#outside-collaborators)

[Make your membership public](#make-your-membership-public)

[Each repository should](#each-repository-should)

[Private vs. Public repository](#private-vs-public-repos)

[Standards for making a private repository](#standards-for-making-a-private-repo)

[Creating new public repositories](#creating-new-public-repositories)

[Creating new private repositories](#creating-new-private-repositories)

[Creating Teams in the GSA organization](#creating-teams-in-the-gsa-organization)

[Removing access to the GSA organization](#removing-access-to-the-gsa-organization)

[Reviewing system log and reporting any unusual activity](#reviewing-the-system-log)

[Third-party access](#third-party-access)

[Organizing Agency Users](#organizing-agency-users)


<h2 id="introduction">Introduction</h1>

GSA’s GitHub Enterprise Cloud provides corporate source code repository services to the various Offices throughout GSA. The Website & Platform Management Branch  (ICEW) in the Office of Corporate IT Services provides the management and administration of the service. Originally intended to support OMB Memorandum M-16-21 Achieving Efficiency, Transparency, and Innovation through Reusable and Open Source Software through the use of public repositories, the service now also supports private repositories for select programs with over 1,000 repositories in total.  You can find out more about the GSA Open Source effort at OpenGSA. GitHub is a web based service, so there’s no installation necessary.

<h2 id="joining-the-gsa-enterprise-organization">Joining the GSA Enterprise Organization</h1>

1.	You will need a GitHub account to join the GSA Org.  If you haven't created a GitHub account yet (https://github.com/), do so with your GSA email address.  A GSA email address is required to be a member of the GSA Org.

2.	If you already have a GitHub account, [simply add your GSA email to your existing account](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/adding-an-email-address-to-your-github-account). Do not create a new account. Make sure your commits are associated with your GSA mail address. 

3.	If you have another email specified in your [GitHub settings](https://github.com/settings/emails), they will both be tied to your GitHub account.

4.	Make sure you have [notifications turned on](https://github.com/settings/notifications) and make sure your notifications are set up the way you'd like them.

<h2 id="complete-your-profile">Complete your profile</h2>

Include the following:
* **Name:** Your first and last name.
* **Company:** Your company or government agency.
* **Location:** Your primary work location (city, state).

<h2 id="set-up-two-factor-authentication">Set up two-factor authentication</h2>

Two-factor authentication is required for all members and collaborators in the GSA org. You can choose among multiple options to add a second source of authentication to your account. You can configure two-factor authentication using a mobile app or via text message. You can also add a security key. See: [Configuring two-factor authentication](https://docs.github.com/en/github/authenticating-to-github/configuring-two-factor-authentication).

<h2 id="turning-on-notifications">Turning on notifications</h2>

Turn notifications on and adjust the settings as needed. Some people watch every repository; others only watch when they’re mentioned.

You will get a lot of emails when you turn notifications on. To help stem the tide, you can set up a Gmail filter to automatically archive emails from notifications@GitHub.com. However, you probably want to let through those emails that contain your GitHub username or are posted to a repo you’re watching.

Since each repository is considered to be its own mailing list, checking for the SMTP list-ID identifier is one reliable way to allow these notifications through. For example, if the repository name in GitHub is GSA/reponame, you can create a filter in Gmail with the condition: “has the words” **list:(reponame.gsa.GitHub.com)** and perform some standard gmail action such as “Apply a label.”

You can also find this by opening an email from the desired repository, clicking the “more info” arrow in the “To” field, and copying the bracketed address in the “mailing list” field. Adding **list:(reponame.GSA.GitHub.com)** to your filter’s exceptions will allow any issues posted to that repository to reach your inbox.

<h2 id="join-the-gsa-organization">Join the GSA organization</h2>

Email `gsa-GitHub.support@gsa.gov` the following: “Please add me `(https://GitHub.com/username)` to `https://GitHub.com/GSA`. Please supply your GitHub username and GSA email address.
 
Also, to make it easier, please describe any team(s) or repo(s) you will need access to. The owner or admin of the requested repo or team will need to grant access. An admin will verify compliance and add you, after which you’ll need to accept their invitation.

<h2 id="outside-collaborators">Outside Collaborators</h2>

Repositories within the GSA org can only be accessed by members in the organization. If a user needs access to a repository within the organization but is not a GSA employee or a contractor with a GSA email address, they will need to be invited as outside collaborators.

Only a member of the GSA Admin Team can invite an outside collaborator. Outside collaborators with access to a private repository incur charges (like a paid seat).

Outside collaborators will not be allowed access to a private repository, without justification from the requesting Program Office and final approval from a GSA Admin Team member. 

In addition, outside collaborators will not be allowed admin access to a repository within the GSA organization.

<h2 id="make-your-membership-public">Make your membership public</h2>

Go to the GSA org people page. Click where it says **private** next to your name. Change that to **public**.

**Each GSA user must**
*	Activate 2-factor Authentication
*	Add your information to your account
*	Make your membership public

<h2 id="each-repository-should">Each repository should</h2>
*	Have a simple and useful name
*	Have a user-friendly description
*	Have a useful README.md

The 18F Team has published a helpful [style guide](https://pages.18f.gov/open-source-guide/making-readmes-readable/) that can be referenced as guidance for describing and documenting repositories.

<h2 id="private-vs-public-repos">Private vs. Public repos</h2>

<h2 id="standards-for-making-a-private-repo">Standards for making a private repo</h2>

Since GSA is following its own Open Sources policy, by default, projects in gitgub.com/gsa should be public. They should only be made private if it contains information that legally cannot be made public. 

<h2 id="creating-new-public-repositories">Creating new public repositories</h1>

1. At https://github.com/gsa, Click '**+ New Repository'**. 
2.	When choosing the repository's name, try to pick a simple and useful name
3.	Include a brief description of the project. 
4.	Change the repository status to **“Public”** unless it needs to be private. 
5.	Note: we recommend the following when exposing your repositories to the public:
a.	Conduct a manual code review with your team. Go line by line through the code and check for sensitive content.
b.	Conduct static code analysis with a scanning tool (if available). SonarQube is approved as a standard. Teams can download it in their local environment and scan/remediate. Hopefully we can recommend other tools in the future. 
c.	Utilize a process to remediate security vulnerabilities within the code base or the environment.
d.	Make environmental variables private or store them on a server
6.	At a minimum, repositories should have a **README** and **LICENSE** file providing instructions to future contributors on how to setup and test the application in order to make suggestions. It is encouraged to have **CONTRIBUTING** and **CODE_OF_CONDUCT** files. See https://github.com/gsa/code-gov-front-end for some examples.
7.	You will usually not need to worry about adding a **“.gitignore”** unless you are going to store env variables or other dot file content. 
8.	GSA’s Office of General Counsel has determined that all GSA code should be Creative Commons Zero (CC0). Work with your program office / legal counsel if you have any questions. See description of the license types.
9.	Click **Create Repository**.
10.	If prompted, choose the most appropriate team that you are a member of that should be given permission to the repo.

<h2 id="creating-new-private-repositories">Creating new private repositories</h2>

The above directions are the same except that at step 4, you will choose Private instead of Public. 

<h2 id="creating-teams-in-the-gsa-organization">Creating Teams in the GSA organization</h2>

It is recommended to create teams to manage member’s access to a repository.  Establish separate teams for each access role: one for team admin users; a different team for your developers with write access; and one for users with read only access. You can assign the Team maintainer role to an individual(s) who would then be able to add / remove members to the repository’s teams. For help in creating teams, please see Creating a team or email gsa-github.support@gsa.gov 

<h2 id="removing-access-to-the-gsa-organization">Removing access to the GSA organization</h2>

*	Team managers should ensure that they monitor when a member of their GitHub team leaves the project or agency and no longer needs access to the GSA organization.  
*	At that point, they should email 'gsa-github.support@gsa.gov' with a request to remove the user from the GSA organization.
*	Organization admins should reply to the email with confirmation when the removal is complete. 
*	Team managers may delegate this responsibility but need to ensure that it is in place. 
**If a member leaves GitHub who is the sole owner of the repository,  and the repository is not archived or transferred to someone else, it will be deleted.**
 
<h2 id="reviewing-the-system-log">Reviewing the system log</h2>
  Users are respomnsible for reviewing their log file and reporting any unusual activity to the github admins. You can find guidance on accessing your security log at:  https://docs.github.com/en/github/authenticating-to-github/reviewing-your-security-log. Report any any usual activity to `gsa-GitHub.support@gsa.gov`
  
<h2 id="third-party-access">Third-party access</h2>

If you would like to have third-party access applications use GitHub, first you will need to ensure the application is shown as approved in the [GSA IT Enterprise Architecture (GEAR) listing](https://insite.gsa.gov/employee-resources/information-technology/do-it-yourself-self-help/software-and-applications/software-requests-and-software-updates/it-standards). The program office requesting 3rd-party integration is responsible for gaining IT Standards approval in GEAR and any cost for the application being integrated with GitHub.

<h2 id="organizing-agency-users">Organizing Agency Users</h2>

*	Identify Team Leads.
*	Ensure everyone has guidance going forward.
*	Repo owners should certify users to their own repos.  
*	It is recommended to make use of teams for better organization.  The repo admin should create a team with admin access for the repository, a team with read-only access, and a team for read/write access. They should then delegate a “team maintainer” for adding or removing members from the team.
*	Users will need to reply to the annual account recertification. If a user does not reply their account will be disabled.



