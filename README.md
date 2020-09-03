# Magisk Modules Alternative Repository Submissions
Just like the official Magisk Modules repository, this is where you can submit your modules.

# Module Submissions
Create an [issue](https://github.com/Magisk-Modules-Alt-Repo/submission/issues) on this repository with `[Module]` in the title and include the link to your repo in the content, then wait for a moderator to approve or deny your module. Once approved, a moderator will mirror your personal repo to the Alt-Repo and give you ownership of it. It is best to then archive your personal repo and work soley here.

**Please make sure your repo name matches your module id, otherwise Magisk Manager will see that the module exists but will fail to pull data from it.**

# Submission Guidelines
We want to make sure that there are no dangerous modules on the Alt-Repo. Please abide by these guidelines.

* Device-specific modules **are allowed**.
* "Trivial" modules **are allowed**. This includes simple boot scripts.
* No malicious modules (deleting core files or breaking system intentionally).
* No broken modules (doesn't do what it says it will).
* No duplicate submissions.
* Module ID must match repo name (otherwise Magisk Manager fails to download it).

It is worth noting that the final approval decision comes from our moderators. If they do not see your module as being fit for the Alt-Repo, they have the choice to deny it. However, they are encouraged to stay unbaised when approving or rejecting modules.

# Migrating  Repositories
We have an internal (but publicly accessible) tool that makes migrating repositories to the Alt-Repo easy. Moderators should use [mmar-migrate](https://github.com/Magisk-Modules-Alt-Repo/mmar-migrate) (Magisk-Module-Alt-Repo Migrate) to migrate existing repositories to the Alt-Repo.

Here is an example use case for this tool:

1. User A creates an issue titled `[Module] My Custom Module`.
2. Moderator B approves the module submission.
3. Moderator B navigates to their private mmar-migrate fork.
4. Moderator B goes to the mmar-migrate Actions tab and enters the module information.
5. Moderator B submits the Action and waits for the completion message.
6. Moderator B navigates to the Alt-Repo clone / mirror and adds User A as a collaborator.
7. Moderator B closes User A's issue.
8. User A approves the invitation via email.

The benefit of such a system is that moderators can be away from their computers and can handle all necessary migrations online through the GitHub website. This should speed up the module approval process significantly.

# Permission Levels
These are the different levels that users can be assigned when choosing to contribute to this project.

* Collaborators are Magisk Module developers who must first make an issue and become approved.
* Members are moderators, they can create their own repos without requesting them beforehand.
* Owners are the admins, they have master control over the entire project.

|                 	| Admins 	| Moderators 	| Collaborators 	|
|-----------------	|--------	|---------	|---------------	|
| Commit changes  	|    ✔   	|    ✔    	|       ✔       	|
| Request repos   	|    ✔   	|    ✔    	|       ✔       	|
| Create repos    	|    ✔   	|    ✔    	|       ❌       	|
| Approve modules  	|    ✔   	|    ✔    	|       ❌       	|
| Manage members  	|    ✔   	|    ❌    	|       ❌       	|
| Remove repos    	|    ✔   	|    ❌    	|       ❌       	|
| Remove others   	|    ✔   	|    ❌    	|       ❌       	|
| Transfer repos  	|    ✔   	|    ❌    	|       ❌       	|

If you are interested in becoming a collaborator, please make an issue on this repo to get started with a project of your own. If you think you are qualified to become a moderator, please create an issue with `[Moderator]` in the title. We currently only consider existing moderators for the admin position, so you may not make a request for it.

# Contact
If you need assistance, feel free to contact any of our Alt-Repo moderators through email or Telegram. If you need direct support, I am always available in a timely manner.

* Telegram: https://t.me/tytydraco
* Email: tylernij@gmail.com
* XDA: tytydraco
