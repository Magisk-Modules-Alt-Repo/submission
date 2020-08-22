# Magisk Modules Alternative Repository Submissions
Just like the official Magisk Modules repository, this is where you can submit your modules.

# Differences
* Instead of only a few moderators, the Alt-Repo has plenty of volunteers who are constantly reviewing your submissions.
* Device-specific modules **are allowed**.
* "Trivial" modules **are allowed**. This includes simple boot scripts.

# Module Submissions
Create an [issue](https://github.com/Magisk-Modules-Alt-Repo/submission/issues) on this repository with `[Module]` in the title and include the link to your repo in the content, then wait for a moderator to approve or deny your module. Once approved, a moderator will mirror your personal repo to the Alt-Repo and give you ownership of it. It is best to then archive your personal repo and work soley here.

**Please make sure your repo name matches your module id, otherwise Magisk Manager will see that the module exists but will fail to pull data from it.**

# Mirror Submissions
You can create mirrors of already existing modules, which will be updated from the original repo automatically every 30 minutes. You should put `[Mirror]` at the start of the repo description and in the issue title. If you are a Moderator, you can use the internal [mmar-migrate](https://github.com/Magisk-Modules-Alt-Repo/mmar-migrate) tool to automate this process. If you don't know how to make the mirror yourself, or simply don't want to (understandable), follow the directions for the module submission, but instead of using the `[Module]` flair, use the `[Mirror]` flair to help the moderators differentiate your request.

# Modules vs Mirrors
There are a few key differences between Module submissions and Mirror submissions.

* Module submissions give developers their own working repository on the Alt-Repo, where they can push their code directly.  It **requires direct developer support** for updates to be created. This type of submission is best for developers who have created a module that they wish to maintain on the Alt-Repo.
* Mirror submissions simply clone an existing repository from a developer to the Alt-Repo, where it is updated automatically every 30 minutes. Modules **do not require human maintenance**. It also **does not require the consent of the original developer** in order to mirror the module. This type of submission is best for non-developers who simply want to put a module that somebody else made on the Alt-Repo for easy access.

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
| Request mirrors 	|    ✔   	|    ✔    	|       ✔       	|
| Request repos   	|    ✔   	|    ✔    	|       ✔       	|
| Create mirrors  	|    ✔   	|    ✔    	|       ❌       	|
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
