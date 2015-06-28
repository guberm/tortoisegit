

# How to add new Wiki pages or update Wiki pages? #
Feel free to clone https://code.google.com/p/tortoisegit.wiki/ or https://github.com/TortoiseGit/wiki and send a pull request. Also everyone who is on our mailing list (https://groups.google.com/group/tortoisegit-dev) can edit the wiki using the web editor.

# TortoiseGit icons are not displayed (correctly) #

Windows explorer can just handle a fixed number different overlay providers and TortoiseGit is using 6 of these (these 6 are handled by TortoiseOverlays and, thus, shared with TortoiseSVN and TortoiseCVS).

If the TortoiseGit icons are not correctly displayed this is likely caused by other programs which provide overlays (like Dropbox, Owncloud, BoxSync and various others) and register with a higher priority.

See https://code.google.com/p/tortoisegit/issues/detail?id=692#c45 for a few steps on how to solve this. The TortoiseSVN team also has a nice FAQ for this: http://tortoisesvn.net/faq.html#ovlnotshowing

You can see which ones the Tortoise clients use in the TortoiseGit settings dialog (https://tortoisegit.org/docs/tortoisegit/tgit-dug-settings.html#tgit-dug-settings-overlay-handlers). Here also a button with direct access to the registry is provided where all overlay handlers are configured.

# How to delete branch and tag #
Press "Shift" key, right-click -> Browse Reference,
Choose branch or tag, right-click, choose "delete". Branches and tags can also be deleted using the Log Dialog, however, tags will only be deleted locally (see [[here](#How_to_delete_a_remote_tag.md)] to find out how to delete tags on a remote repository).

Or open log dialog -> choose commit with branch\tag, right->click->delete

# What to do if a crash happened? #
  * Check if "git gc" resolves the problem
  * Check if "git fsck" resolves the problem
  * Test our [preview release](http://download.tortoisegit.org/tgit/previews/) if the problem is still there. If yes: File a [bugreport](https://code.google.com/p/tortoisegit/issues/list). Mention your Windows Version (also x64 or x86), your msysgit version and the used TortoiseGit version there.

# What to do if log dialog shows inaccurate information? #
  * Close all log dialogs of that repository, then go to .git folder, delete tortoisegit.data and tortoisegit.index

# There are no icon overlays on Network drives/RAM drives/Removable drives or CD drives. How to enable them? #
You have to enable overlay icons for these devices in TortoiseGit settings -> Icon overlays.

# How to make TortoiseGit use OpenSSH or plink? #
Go to TortoiseGit settings -> Network and enter "SSH.exe" resp. TortoiseGitPLink.exe into the SSH client text field:
![http://tortoisegit.googlecode.com/git/doc/images/en/SettingsProxy.png](http://tortoisegit.googlecode.com/git/doc/images/en/SettingsProxy.png)

# How to delete a remote tag #
  * Since 1.7.12.1: Go to the "Browse References" dialog, right click on a remote and select "Delete remote tags...".
  * Before 1.7.12.1: Open the push dialog, select the remote archive, no local branch, fill in the tag name into the remote branch field and click on OK.

# How to remove file from version control and keep local copy #
Press "shift" key, right-click -> Delete (keep local)

# How to use PuTTY for git cli and git bash? #
Create an environment variable called "GIT\_SSH" with the path to the PuTTY plink.exe or preferably to TortoiseGitPLink.exe.
This can be done on the command line by executing "set GIT\_SSH=PATH\_TO\_PLINK.EXE" ("C:\Program Files\TortoiseGit\bin\TortoiseGitPLink.exe" on default installations) or [permanently](http://www.computerhope.com/issues/ch000549.htm).

# How to show extended menu items? #
Press "shift" key, right-click

# How to hide some menu items #
setting -> Set Extend Menu Item.
Choose the menu items you want to hide (by default), however, these items can be shown by pressing the "shift" key while doing the right-click.

# How to use 32bit extension at 64bit system #
Since version 1.7.2 the 32-bit extension is also included in the 64-bit installer.

# TortoiseGitBlame shows menu in wrong language #
You have to reset the menu bar (even if you did not make any changes to it). Left click -> Customize -> Menu tab and hit Reset/Restore.