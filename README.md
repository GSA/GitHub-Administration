
## GSA Standards

#### Each GSA user must

* [Activate 2-factor Authentication](https://github.com/fisma-ready/github#activate-2-factor-authentication)
* [Add your information to your account](https://github.com/fisma-ready/github#add-your-information-to-your-account)
* [Add a profile avatar](https://github.com/fisma-ready/github#add-a-profile-avatar)
* [Make your membership public](https://github.com/fisma-ready/github#make-your-membership-public)

#### Each repository should: 

* [Have a simple and useful name](https://pages.18f.gov/open-source-guide/naming-your-project/)
* [Have a user-friendly description](https://pages.18f.gov/open-source-guide/writing-the-repo-description/)
* [Have a useful README.md](https://pages.18f.gov/open-source-guide/making-readmes-readable/)

#### Standards for making a private repo:  

By default, projects in GitHub.com/GSA should be public.  They should only be made private under certain circumstances.  

* A repository can be made private if it containts information that legally cannot be made public.  

## Workflows 

#### Creating a GitHub account

1. If you haven't created a GitHub account yet (https://github.com/), do so with your government email, which will assist with [records retention](http://ben.balter.com/open-source-for-government/#records).  
2. If you already have a GitHub account, simply [add your goverment email to your existing account](https://help.github.com/articles/adding-an-email-address-to-your-github-account/). Do not create a new account. You can also set up custom email routing through the [Notifications Center](https://github.com/settings/notifications). Make sure your commits are [associated with your government email address](https://help.github.com/articles/setting-your-email-in-git).
3. Update the `Settings` in your account to match the [GSA Standards](#gsa-standards).
4. Note that associating commits with an email address is different from [setting notifications to go to one or another email address](https://help.github.com/articles/configuring-notification-emails-for-organizations/). You also have to change the official commit email address attached to each repo.
5. If you’re using your work computer for personal projects on GitHub and want your personal email tied to those commits, you can set your GSA email as part of the global `.gitconfig`, then [override on a repository level](http://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration) with your personal email. If you have both emails [in your GitHub settings](https://github.com/settings/emails), though, they will both be tied to your GitHub account.
6. Make sure you have [notifications turned on](https://github.com/settings/notifications) and make sure your notifications are set up they way you'd like them.

#### Requesting access to the GSA organization

1. Ensure that you have created a GitHub account that matches the standards above.  
2. If your group already has a team in the GSA organization, ask your point of contact to email 'gsa-github.support@gsa.gov' with your Github username and request that you be given access.  
3. If your group does not yet have a team in the GSA organization, email 'gsa-github.support@gsa.gov' to coordinate a team be created.  You will need to list the usernames of any others who should be added.   
4. You will receive a notification when you've been given access.  

#### Creating new public repositories

1. At https://github.com/GSA, Click `+ New Repository`.  
2. When choosing the repo's name, try to pick [a simple and useful name](https://pages.18f.gov/open-source-guide/naming-your-project/)
3. Include a brief description of the project.  
4. Change the repo status to `Public` unless it does must be private.  
5. It is usually convenient to check the box to `Initialize this repository with a README`.  
6. You will usually not need to worry about adding a `.gitignore`.  
7. Please choose the type of license from the dropdown.  For a description of the license types, see https://help.github.com/articles/licensing-a-repository  
8. Click Create Repository
9. If prompted, choose the most appropriate team that you are a member of that should be given permission to the repo.  

#### Creating new private repositories

...

The above directions are the same except that at step 4, you will choose Private instead of Public.  

#### Removing access to the GSA organization

1. [Team managers](https://github.com/GSA/GitHub-Administration/blob/master/team-management.md#team-points-of-contact) should ensure that they monitor when a member of their GitHub team leaves the project or agency and no longer needs access to the GSA organization.  
2. At that point, they should email 'gsa-github.support@gsa.gov' with a request to remove the user from the GSA organization. 
3. Organization admins should reply to the email with confirmation when the removal is complete.  
4. Team managers may delegate this responsibility but need to ensure that it is in place.  

#### Third-party access

If you are requesting third-party access apps to access GitHub,  the app needs to be in the GSA IT Enterprise Architecture GEAR listing as approved ( https://ea.gsa.gov/#!/itstandards ) and whoever wants to use the app needs to shepherd it through the GEAR process for approval.  Once it is approved in the It Standards, it can be approved in GitHub. 

## Organize Agency Users

* Identify Team Leads
* Plan and implement the application of the standards 
* Ensure everyone has guidance going forward


