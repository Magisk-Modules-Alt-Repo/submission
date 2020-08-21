# Magisk Modules Alternative Respository Submissions
Just like the official Magisk Modules repository, this is where you can submit your modules.

# Differences
* Instead of only a few moderators, the Alt repository has plenty of volunteers who are constantly reviewing your submissions.
* Device-specific modules **are allowed**.
* "Trivial" modules **are allowed**. This includes simple boot scripts.

# Module Submissions
1. Create an [issue](https://github.com/Magisk-Modules-Alt-Repo/submission/issues) on this repository with `[Module]` in the title and include the link to your repo in the content.
2. Wait for a moderator to approve or deny your module.

Please make sure your repo name matches your module id, otherwise Magisk Manager will see that the module exists but will fail to pull data from it.

# Mirrors
You can create mirrors of already existing modules. You should put `[Mirror]` at the start of the repo description and in the issue title. If you want your module to auto-update, add a GitHub Action like this:

```
name: Update Mirror
on:
  schedule:
    - cron: '*/30 * * * *'
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Update mirrored repo
        uses: actions/checkout@v2
      - run: git remote update --prune |
             git pull
```

Title it something like `update.yml`. The suggested Action above will check for updates every hour and merge the changes to the current repository. This will cause issues when the original repo owner force-pushes to their master branch.

If you don't know how to make the mirror yourself, or simply don't want to (understandable), follow the directions for the module submission, but instead of using the `[Module]` flair, use the `[Mirror]` flair to help the moderators differentiate your request.

# Permission Levels
These are the different levels that users can be assigned when choosing to contribute to this project.

* Collaborators are Magisk Module developers who must first make an issue and become approved
* Members are moderators, they can create their own repos without requesting them beforehand
* Owners are the admins, they have master control over the entire project

|                 	| Owners 	| Members 	| Collaborators 	|
|-----------------	|--------	|---------	|---------------	|
| Commit changes  	|    ✔   	|    ✔    	|       ✔       	|
| Request mirrors 	|    ✔   	|    ✔    	|       ✔       	|
| Request repos   	|    ✔   	|    ✔    	|       ✔       	|
| Create mirrors  	|    ✔   	|    ✔    	|       ❌       	|
| Create repos    	|    ✔   	|    ✔    	|       ❌       	|
| Manage members  	|    ✔   	|    ❌    	|       ❌       	|
| Remove others   	|    ✔   	|    ❌    	|       ❌       	|
| Transfer repos  	|    ✔   	|    ❌    	|       ❌       	|

If you are interested in becoming a collaborator, please make an issue on this repo to get started with a project of your own. If you think you are qualified to become a moderator, please create an issue with `[Moderator]` in the title. We currently only consider existing moderators for the admin position, so you may not make a request for it.

# Contact
If you need assistance, feel free to contact any of our Alt Repo moderators through email or Telegram. If you need direct support, I am always available in a timely manner.

* Telegram: https://t.me/tytydraco
* Email: tylernij@gmail.com
* XDA: tytydraco
