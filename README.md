# Magisk Modules Alternative Repository Submissions
Just like the official Magisk Modules repository (now defunct), this is where you can submit your modules.

Note: You can browse and install those modules via [MMRL](https://github.com/DerGoogler/MMRL) or the [Androidacy Module Manager](https://github.com/Androidacy/MagiskModuleManager), a continuation of the [Fox's Magisk Module Manager](https://github.com/Fox2Code/FoxMagiskModuleManager/releases) project. Alternatively you can use the [Telegram Channel](https://t.me/MagiskModulesAltRepo) to receive Magisk modules updates.

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

* You **must provide the source code** for any executables or APK files included in your submission. If you absolutely need to compile your code, please provide reproducible build instructions. An exception can be made for modules that provide compiled packages/binaries from trusted sources such as recognized developers on the Play Store. In such a case, you **cannot modify** the provided APKs unless doing so does not infringe on the author's copyright and you **must provide the source code/APKtool configuration** for modifications performed, if any.
* You **must not obfuscate** the source code of the scripts you provide or any binaries/packages provided unless you are providing a trusted third-party's binary/package where the source has been obfuscated by the third-party at the source.

You can provide the source code in various ways, including, but not limited to:
* On the project's Wiki page
* As a separate repository
* On a separate, empty branch
* Directly in the main branch, with instructions in `customize.sh` that delete it during installation

### Anti-Features

The new `json-v2` format supports Anti-Features like F-Droid, this gives more transparency about the modules and helps the user if a module includes non-free dependencies etc.

<details><summary>Click here to see all supported Anti-Features</summary>

| Name                      | ID                | Description                                                                                  |
| ------------------------- | ----------------- | -------------------------------------------------------------------------------------------- |
| Ads                       | `Ads`             | Advertising                                                                                  |
| Tracking                  | `Tracking`        | Tracks and/or reports your activity to somewhere, even when it can be turned off             |
| Non-Free Network Services | `NonFreeNet`      | Promotes or depends entirely on a non-changeable or non-free network service                 |
| Non-Free Addons           | `NonFreeAdd`      | Promotes other non-libre module or plugins                                                   |
| Non-Free Dependencies     | `NonFreeDep`      | Needs a non-libre module to work (e.g. Google Maps, Market)                                  |
| NSFW                      | `NSFW`            | Contains content that the user may not want to be publicized or visible everywhere           |
| Upstream Non-Free         | `UpstreamNonFree` | Upstream source code is not libre, and this version has those parts replaced or rewritten    |
| Non-Free Assets           | `NonFreeAssets`   | Non-libre media in things that are not code (e.g. images, sound, music, 3D-models, or video) |
| Known Vulnerability       | `KnownVuln`       | Known security vulnerability                                                                 |
| No Source Since           | `NoSourceSince`   | Source code no longer available, making new releases impossible                              |
| Obfuscation               | `Obfuscation`     | Module includes obfuscated code                                                              |
| Unasked removal           | `UnaskedRemoval`  | Module removes app, permissions and other modules without approval                           |

</details>

We recommend that you publish your module under a license that explicitly permits redistribution of the software, such as the [GPLv3](https://www.gnu.org/licenses/gpl-howto.html) license. Any other FOSS license should work as well. Make sure the license is compatible with all code/binaries you provide — this is especially important if you provide a proprietary package with your module.

## Concluding remarks

It is worth noting that the final approval decision comes from our moderators. If they do not see your module as being fit for the Alt-Repo, they have the choice to deny it. However, they are encouraged to stay unbaised when approving or rejecting modules.

Failure to abide by the guidelines will be pointed out after moderator review. In cases of larger problems, you may be asked to re-submit the module after corrections in a new issue. Infractions on the "no malicious modules" guideline (or straight up distributing malware) will result in a permanent ban from submitting new modules as well as the removal of ones previously submitted by the offender.

You should maintain your module for as long as possible and remove your repository if it stops working completely and you can't maintain it. We may perform changes without developer approval on any broken modules that are abandoned by their maintainers. This only includes simple fixes, heavily broken, unmaintained modules will simply be deleted.

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

# Disclaimer

We do our best to check modules as they are submitted into MMAR for any
malicious/broken functionality, but we cannot reasonably check every commit from
the time the modules are accepted. As such we withhold any responsibility for
bricked devices, unintended behavior, malware, or other problems arising from
using modules submitted to MMAR. If you notice such a module, though, please let
us know (see below).

# Reporting modules

If you notice a broken module or one containing malware, please create an issue
here with the `Module Takedown Request` template. In case of matters requiring
urgent attention, such as modules that brick devices or malware, please *also*
ping us in the issue and send an e-mail message about that (see the `Contact`
section below).

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

**HuskyDG**

* Telegram: https://t.me/HuskyDG
* Email: deadboltsx303[at]gmail.com
* XDA: huskydg

**Der_Googler**

* Telegram: https://t.me/Der_Googler
* Email: jimmy[at]dergoogler.com
* XDA: Der_Googler

**Tytydraco**

* Telegram: https://t.me/tytydraco
* Email: tylernij[at]gmail.com
* XDA: tytydraco
