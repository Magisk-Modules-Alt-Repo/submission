# Magisk Modules Alternative Repository Submissions
Just like the official Magisk Modules repository (now defunct), this is where you can submit your modules.

Note: You can browse and install those modules via [Fox's Magisk Module Manager](https://github.com/Fox2Code/FoxMagiskModuleManager/releases)

# Module Submissions
Create an [issue](https://github.com/Magisk-Modules-Alt-Repo/submission/issues) on this repository with `[Module] <Your module's name>` in the title and include the link to your repo in the content, then wait for a moderator to approve or deny your module. Once approved, a moderator will mirror your personal repo to the Alt-Repo and give you ownership of it. It is best to then archive your personal repo and work soley here or set up parallel remote push URLs with git.

# Submission Guidelines
We want to make sure that there are no dangerous modules on the Alt-Repo. Please abide by these guidelines.

## General Guidelines

* Your module must be a valid Magisk/Zygisk module. See the [Developer Guide](https://topjohnwu.github.io/Magisk/guides.html) for more info.
* Your module must have a README.md file in English with information about the module.
* Device-specific modules **are allowed**. Make sure to mention that they are device-specific in the README.
* "Trivial" modules **are allowed**. This includes simple boot scripts.
* No malicious modules (deleting core files, breaking system intentionally, adware, spyware, or any kind of module harmful to the end user).
* No broken modules (doesn't do what it says it will, or doesn't define correctly compatible devices).
* Module ID must match repo name. In the event that this isn't the case, your new module repo's name will be the same as the module ID.
* The issue author must be the owner of the module being submitted, or have permission from the owner.

## Source Code Guidelines

* You **must provide the source code** for any executables or APK files included in your submission. If you absolutely need to compile your code, please provide reproducible build instructions. An exception can be made for modules that provide compiled packages/binaries from trusted sources such as recognized developers on the Play Store. In such a case, you **cannot modify** the provided APKs unless doing so does not infringe on the author's copyright and you **must provide the source code** for modifications performed, if any.
* You **must not obfuscate** the source code of the scripts you provide or any binaries/packages provided unless you are providing a trusted third-party's binary/package where the source has been obfuscated by the third-party at the source.

We recommend that you publish your module under a license that explicitly permits redistribution of the software, such as the [GPLv3](https://www.gnu.org/licenses/gpl-howto.html) license. Any other FOSS license should work as well. Make sure the license is compatible with all code/binaries you provide — this is especially important if you provide a proprietary package with your module.

It is worth noting that the final approval decision comes from our moderators. If they do not see your module as being fit for the Alt-Repo, they have the choice to deny it. However, they are encouraged to stay unbaised when approving or rejecting modules.

Failure to abide by the guidelines will be pointed out after moderator review. In cases of larger problems, you may be asked to re-submit the module after corrections in a new issue. Infractions on the "no malicious modules" guideline (or straight up distributing malware) will result in a permanent ban from submitting new modules as well as the removal of ones previously submitted by the offender.

<!-- # Migrating  Repositories -->
<!-- We have an internal (but publicly accessible) tool that makes migrating repositories to the Alt-Repo easy. Moderators should use [mmar-migrate](https://github.com/Magisk-Modules-Alt-Repo/mmar-migrate) (Magisk-Module-Alt-Repo Migrate) to migrate existing repositories to the Alt-Repo. -->
<!--  -->
<!-- Here is an example use case for this tool: -->
<!--  -->
<!-- 1. User A creates an issue titled `[Module] My Custom Module`. -->
<!-- 2. Moderator B approves the module submission. -->
<!-- 3. Moderator B navigates to their private mmar-migrate fork. -->
<!-- 4. Moderator B goes to the mmar-migrate Actions tab and enters the module information. -->
<!-- 5. Moderator B submits the Action and waits for the completion message. -->
<!-- 6. Moderator B navigates to the Alt-Repo clone and adds User A as a collaborator. -->
<!-- 7. Moderator B closes User A's issue. -->
<!-- 8. User A approves the invitation via email. -->
<!--  -->
<!-- The benefit of such a system is that moderators can be away from their computers and can handle all necessary migrations online through the GitHub website. This should speed up the module approval process significantly. -->

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
If you need assistance, feel free to contact any of our Alt-Repo moderators through email or Telegram. If you need direct support, we are always available in a timely manner.

**Atrate**

* Email: Atrate[at]protonmail.com
* XDA: Atrate

**Tytydraco**

* Telegram: https://t.me/tytydraco
* Email: tylernij[at]gmail.com
* XDA: tytydraco
