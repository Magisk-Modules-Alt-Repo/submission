# Magisk Modules Alternative Respository Submissions
Just like the official Magisk Modules repository, this is where you can submit your modules.

# Differences
* Instead of only a few moderators, the Alt repository has plenty of volunteers who are constantly reviewing your submissions.
* Device-specific modules **are allowed**.
* "Trivial" modules **are allowed**. This includes simple boot scripts.

# Steps
1. Create an [issue](https://github.com/Magisk-Modules-Alt-Repo/submission/issues) on this repository with the link to your repo.
2. Wait for a moderator to approve or deny your module.

# Mirrors
You can create mirrors of already existing modules. You should put `[Mirror]` at the start of the repo description and in the issue title. If you want your module to auto-update, add a GitHub Action like this:

```
name: Update Mirror
on:
  schedule:
    - cron: '*/60 * * * *'
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

# Contact
If you need assistance, feel free to contact any of our Alt repo moderators through email or Telegram.
