# Release 1.8.14.0 #
Released: 2015-04-08

## Features ##
  * Fixed [issue #2441](https://code.google.com/p/tortoisegit/issues/detail?id=#2441): A way to disable the sound that is played on errors
  * Updated shipped TortoiseGitPlink and putty binaries to version 0.64
> > If you are still using TortoisePlink, please switch to TortoiseGitPlink.
  * Fixed [issue #2466](https://code.google.com/p/tortoisegit/issues/detail?id=#2466): TortoiseGitUDiff tool cannot be localized
  * TGitCache: Improve reaction time for propagating changes to explorer
  * Fixed [issue #2031](https://code.google.com/p/tortoisegit/issues/detail?id=#2031): Missing option to disable displaying "FETCH\_HEAD" in "Switch/Checkout" dialog box
  * Log, RepoBrowser, and Rebase Dialogs: Allow to compare arbitrary files across commits
  * Fixed [issue #2534](https://code.google.com/p/tortoisegit/issues/detail?id=#2534): Use the current time for amending commit (also sets commit time)
  * TortoiseGitBlame: Implemented search forward (F3) and search backward (Shift+F3)
  * Allow to compare file with deleted file in CommitDlg (e.g., useful for renames)
  * Allow to use Explorer context menu options from TortoiseGit context menu
  * Sort remotes logically/case-insensitively

## Bug Fixes ##
  * Fixed [issue #2427](https://code.google.com/p/tortoisegit/issues/detail?id=#2427): "Submodule of Project: " cannot be localized
  * Fixed [issue #2432](https://code.google.com/p/tortoisegit/issues/detail?id=#2432): MessageBox buttons cannot be localized
  * Fixed [issue #2433](https://code.google.com/p/tortoisegit/issues/detail?id=#2433): Cannot see the log in Diff with previous version
  * Fixed [issue #2453](https://code.google.com/p/tortoisegit/issues/detail?id=#2453): The overlay icon of commited files in a submodule named with chinese characters is unversioned icon
  * Fixed [issue #2455](https://code.google.com/p/tortoisegit/issues/detail?id=#2455): "Diff with ..." menu cannot be localized
  * Fixed [issue #2431](https://code.google.com/p/tortoisegit/issues/detail?id=#2431): Add fails in submodule after upgrade from 1.8.12 to 1.8.13
  * Fixed [issue #2449](https://code.google.com/p/tortoisegit/issues/detail?id=#2449): wrong column info in tag reference dialog
  * Fixed [issue #2436](https://code.google.com/p/tortoisegit/issues/detail?id=#2436): Overlay icons gradually disappear or show files as unversioned after a short time
  * Fixed [issue #2374](https://code.google.com/p/tortoisegit/issues/detail?id=#2374): Rebase option in config not working anymore for pull
  * Fixed [issue #1440](https://code.google.com/p/tortoisegit/issues/detail?id=#1440): Different status of modifed renamed or moved files in Show log dialog, Check for Modifications dialog and Commit dialog
  * Fixed [issue #1501](https://code.google.com/p/tortoisegit/issues/detail?id=#1501): Unchanged files appears modified in Show Log dialog
  * Fixed [issue #2477](https://code.google.com/p/tortoisegit/issues/detail?id=#2477): Change "Split commit" label to "Edit/Split commit" in Rebase dlg
  * Fixed [issue #2481](https://code.google.com/p/tortoisegit/issues/detail?id=#2481): "Start registry editor" does not work properly in non-English locales
  * Fixed [issue #2480](https://code.google.com/p/tortoisegit/issues/detail?id=#2480): CommitDlg: auto-complete doesnt include removed items
  * Fixed [issue #2451](https://code.google.com/p/tortoisegit/issues/detail?id=#2451): Cleanup fails quietly if file is in use
  * Various bugfixes based on our newly added unit tests
  * Not all remotes showing in Push/Pull/Fetch/Sync dialogs (was limited to 25)

# Release 1.8.13.0 #
Released: 2015-02-15

## Features ##
  * Improved auto update
> > Version checks will use SSL (on Vista or newer systems)
> > New version.txt file format with more options
  * Fixed [issue #2243](https://code.google.com/p/tortoisegit/issues/detail?id=#2243): Submodule red-icon doesn't propagate to higher folders (configurable now)
  * Improved overlay icon accuracy
> > You might need to kill TGitCache.exe once using the TaskManager in order to reset its cache
  * Fixed [issue #2388](https://code.google.com/p/tortoisegit/issues/detail?id=#2388): See the exact time when the Relative time in log enabled
  * Fixed [issue #2346](https://code.google.com/p/tortoisegit/issues/detail?id=#2346): Add drag'n'drop to "Apply patches" window
  * Fixed [issue #2357](https://code.google.com/p/tortoisegit/issues/detail?id=#2357): Save the state of Search criteria checkboxes in Log dialog
  * Fixed [issue #2420](https://code.google.com/p/tortoisegit/issues/detail?id=#2420): Make push available in log for arbitrary commits (when pressing the shift key)
  * Fixed [issue #2351](https://code.google.com/p/tortoisegit/issues/detail?id=#2351): Allow upstream to be separate from onto in rebase
  * Fixed [issue #1400](https://code.google.com/p/tortoisegit/issues/detail?id=#1400): Allow the use of tags within the Git Rebase dialog
  * Fixes [issue #2417](https://code.google.com/p/tortoisegit/issues/detail?id=#2417): Resolving a conflict forces refresh of Commit Dialog
> > A new advanced option (RefreshFileListAfterResolvingConflict) was added which controls
> > whether file lists are refreshed after resolving conflicts. By default this is set to
> > true, but can be disabled in cases where refreshing the list takes lots of time or
> > people don't want the list to automatically scroll to the top (this also mitigates
> > [issue #1949](https://code.google.com/p/tortoisegit/issues/detail?id=#1949) until we have a cleaner fix). F5 for manual refresh is needed if enabled.
  * Fixed [issue #56](https://code.google.com/p/tortoisegit/issues/detail?id=#56): Ability to use Cygwin's git instead of msysGit
> > Check out the manual (keyword "Cygwin git") regarding Cygwin Git support and configuration hints.
> > Please note that Cygwin Git is not officially supported by TortoiseGit as the developers only
> > use Git for Windows. Bugreports, however, are welcome.

## Bug Fixes ##
  * Fixed [issue #2359](https://code.google.com/p/tortoisegit/issues/detail?id=#2359): Selected files counter not updated after revert
  * Fixed [issue #2362](https://code.google.com/p/tortoisegit/issues/detail?id=#2362): git.exe get stuck on Win XP
  * Fixed [issue #2372](https://code.google.com/p/tortoisegit/issues/detail?id=#2372): Remote Config Tags Dropdown doesn't enable Apply-Button when switching to Reachable
  * Updated libgit2 in order to fix CVE-2014-9390.
> > TortoiseGit is not affected in its default configuration (libgit2 has to be manually enabled for cloning).
> > Git for Windows and mSysGit < 1.9.5 are affected, so an update highly recommended.
  * Fixed [issue #2385](https://code.google.com/p/tortoisegit/issues/detail?id=#2385): 'Mail' - 'Use configured server' & 'none'... seems can not be localized
  * Fixed [issue #2356](https://code.google.com/p/tortoisegit/issues/detail?id=#2356): Rebase dialog should also auto-link to issue tracker
  * Fixed [issue #2390](https://code.google.com/p/tortoisegit/issues/detail?id=#2390): /command:log /outfile not written
  * Fixed [issue #2391](https://code.google.com/p/tortoisegit/issues/detail?id=#2391): Cannot clear "Load Putty Key" in clone dialog persistently
  * Fixed [issue #1789](https://code.google.com/p/tortoisegit/issues/detail?id=#1789): Tooltips not properly displayed in Log List if that commit has refs
  * Fixed [issue #2353](https://code.google.com/p/tortoisegit/issues/detail?id=#2353): Link to bug tracker not available in Show Log dialog on Win8+
  * Fixed [issue #2368](https://code.google.com/p/tortoisegit/issues/detail?id=#2368): CTRL+ENTER locks up GUI on Updating Index...
  * Fixed [issue #2414](https://code.google.com/p/tortoisegit/issues/detail?id=#2414): SendMail doesn't correctly place the mail in to list
  * Fixed several issues in libgit2 regarding SafeCrLf and AutoCrlf

# Release 1.8.12.0 #
Released: 2014-11-25

## Features ##
  * Fixed [issue #2272](https://code.google.com/p/tortoisegit/issues/detail?id=#2272): Export Dialog auto select tag if the revision has tag
  * We now use a 4096-bit RSA key with SHA2-512 for signing and verifying our releases instead of a 1024-bit DSA key with SHA1
> > The new key is signed by the old key. You can get the fingerprint from a trusted TortoiseGit installation by issuing
> > "TortoiseGitProc.exe /command:pgpfp"
  * Fixed [issue #1928](https://code.google.com/p/tortoisegit/issues/detail?id=#1928): Hotkeys in "Show log" dialog for navigating back / forward
  * Fixed [issue #1316](https://code.google.com/p/tortoisegit/issues/detail?id=#1316): Add git describe
  * Fixed [issue #2294](https://code.google.com/p/tortoisegit/issues/detail?id=#2294): Submodule Update dialog doesn't save its state
  * Fixed [issue #2176](https://code.google.com/p/tortoisegit/issues/detail?id=#2176): Color config for "View Patch" Window & Tortoise(Git)UDiff
  * Fixed [issue #2331](https://code.google.com/p/tortoisegit/issues/detail?id=#2331): Show prefix log asterisk in Log Dialog
  * Fixed [issue #2157](https://code.google.com/p/tortoisegit/issues/detail?id=#2157): TortoiseGitMerge does not delete temporary files on close (marking as "resolved" in TGit was necessary)
  * Fixed [issue #1950](https://code.google.com/p/tortoisegit/issues/detail?id=#1950): Log Dialog: File list filter
  * Fixed [issue #2330](https://code.google.com/p/tortoisegit/issues/detail?id=#2330): Optimize submodule conflict resolution
  * Fixed [issue #2332](https://code.google.com/p/tortoisegit/issues/detail?id=#2332): TortoiseGitMerge: Move "Create patch file" to the File menu
  * TortoiseGitMerge: Updated EditorConfig version to 0.12
  * Fixed [issue #2341](https://code.google.com/p/tortoisegit/issues/detail?id=#2341): Jump to search box when pressing CTRL+E
  * Custom dictionaries for the spell checker can now be put into the %APPDATA%\TortoiseGit\dic folder (w/o administrator privileges).
> > All other locations within the TortoiseGit installation folder (e.g. bin, dic, ...) except Languages are now deprecated.
> > See the manual for more information.
  * TGitCache: Overlay update improvements and speedups

## Bug Fixes ##
  * Fixed [issue #2260](https://code.google.com/p/tortoisegit/issues/detail?id=#2260): Clicking in blank space in Commit dialog causes all unversioned files to become selected
  * Fixed [issue #2290](https://code.google.com/p/tortoisegit/issues/detail?id=#2290): "Pulled Log" broken
  * Fixed [issue #2281](https://code.google.com/p/tortoisegit/issues/detail?id=#2281): TGit 1.8.11 is not using %HOME% correctly
  * Fixed [issue #2306](https://code.google.com/p/tortoisegit/issues/detail?id=#2306): TortoiseGitMerge ToolTip messages for Previous/next inline difference mixed up
  * Fixed [issue #2308](https://code.google.com/p/tortoisegit/issues/detail?id=#2308): Pressing ESC in the skip-worktree confirmation dialog box selects 'yes'
  * Fixed [issue #2309](https://code.google.com/p/tortoisegit/issues/detail?id=#2309): "Show log of aaaa..bbbb" on sub directory shows logs on root directory
  * Fixed [issue #2126](https://code.google.com/p/tortoisegit/issues/detail?id=#2126): Rebase: Squash after conflict causes additional commit
  * Fixed [issue #2313](https://code.google.com/p/tortoisegit/issues/detail?id=#2313): "Clean to recycle bin" after Clean-up dry run removes unexpected files
  * Fixed [issue #874](https://code.google.com/p/tortoisegit/issues/detail?id=#874): Add --rebase option to pull dialog
  * Fixed [issue #2316](https://code.google.com/p/tortoisegit/issues/detail?id=#2316): Error on comparing files when git config core.autocrlf ends with 2+ spaces and then a comment
  * Fixed [issue #2323](https://code.google.com/p/tortoisegit/issues/detail?id=#2323): TortoiseGit does not pull --tags despite checking Tags
  * Fixed [issue #2327](https://code.google.com/p/tortoisegit/issues/detail?id=#2327): Help button is broken in "SVN Commit Type" dialog
  * TGitCache now checks file sizes before checking file contents. This should mitigate possible "file is locked" problems.
  * Fixed [issue #2329](https://code.google.com/p/tortoisegit/issues/detail?id=#2329): Changes track remote branch when fast forward is used
  * Fixed [issue #1872](https://code.google.com/p/tortoisegit/issues/detail?id=#1872): Rebase edit doesn't amend files but only the commit message
  * Fixed [issue #2342](https://code.google.com/p/tortoisegit/issues/detail?id=#2342): Ignore whitespace blame option not work
  * Fixed [issue #2311](https://code.google.com/p/tortoisegit/issues/detail?id=#2311): Empty commits cannot be rebased
  * Fixed [issue #2312](https://code.google.com/p/tortoisegit/issues/detail?id=#2312): Fix UTF-8 AutoCRLF issues with libgit2
  * Fixed [issue #2345](https://code.google.com/p/tortoisegit/issues/detail?id=#2345): The Show Log dialog's View Patch side window is empty when the Working dir changes line is selected and no file is selected
  * Fixed [issue #2348](https://code.google.com/p/tortoisegit/issues/detail?id=#2348): Conflicts during rebase appends "conflicts" to commit message

# Release 1.8.11.0 #
Released: 2014-08-22

## Bug Fixes ##
  * Fixed [issue #2257](https://code.google.com/p/tortoisegit/issues/detail?id=#2257): Fetching & pushing using ssh.exe not working with TortoiseGit 1.8.10
  * Fixed crashes while opening the revision graph in the x64 version on some AMD CPUs
  * Fixed some other possible crashes when working with broken repositories or writing files failed
  * TortoiseGitMerge did not show ribbon bar with Portuguese (Brazil) language pack loaded

# Release 1.8.10.0 #
Released: 2014-08-12

## Features ##
  * Updated shipped libgit2 to version 0.21
  * Fixed [issue #1605](https://code.google.com/p/tortoisegit/issues/detail?id=#1605): Add TortoiseGit start and pre commit hooks
  * Fixed [issue #2170](https://code.google.com/p/tortoisegit/issues/detail?id=#2170): Please add interface to "git svn log -v"
  * Fixed [issue #1787](https://code.google.com/p/tortoisegit/issues/detail?id=#1787): auto-complete label when writing commit message
  * Fixed [issue #2241](https://code.google.com/p/tortoisegit/issues/detail?id=#2241): Cleanup: result window of dry run should offer to "really remove"
  * Fixed [issue #1596](https://code.google.com/p/tortoisegit/issues/detail?id=#1596): Added basic support for clean/smudge filters
  * Fixed [issue #2167](https://code.google.com/p/tortoisegit/issues/detail?id=#2167): Support git push --force-with-lease option
  * TortoiseGitMerge: Support EditorConfig indent\_style(space/tab) and indent\_size
  * TortoiseGitMerge: Can specify number of context lines or follow diff.context in a patch file
  * Can sort tags in reversed order
  * Can shallow pull/fetch a shallow clone repository
  * Revision Graph: Add filter to walk from Only Local Branches

## Bug Fixes ##
  * Fixed [issue #2216](https://code.google.com/p/tortoisegit/issues/detail?id=#2216): Add fails with message: libgit2: "failed to parse 'warn' as boolean"
  * Fixed [issue #2218](https://code.google.com/p/tortoisegit/issues/detail?id=#2218): Tortoise Git Extra Backslash with SUBST Drive Paths
  * Fixed [issue #1951](https://code.google.com/p/tortoisegit/issues/detail?id=#1951): Slow switch/checkout dialog
  * Fixed [issue #2064](https://code.google.com/p/tortoisegit/issues/detail?id=#2064): Broken characters when dragging the horizontal bar in TortoiseGitMerge
  * Fixed [issue #2143](https://code.google.com/p/tortoisegit/issues/detail?id=#2143): PowerShell not working in git hooks
  * Fixed [issue #2222](https://code.google.com/p/tortoisegit/issues/detail?id=#2222): 'Prune' in the pull dialog does not work
  * Fixed [issue #2223](https://code.google.com/p/tortoisegit/issues/detail?id=#2223): Move & revert operations not as expected if working tree root is directly on a drive
  * Fixed [issue #2225](https://code.google.com/p/tortoisegit/issues/detail?id=#2225): include.path does not understand tilde (~)
  * Fixed [issue #2228](https://code.google.com/p/tortoisegit/issues/detail?id=#2228): TortoiseGitUDiff incorrect font by non-ascii char name
  * Fixed [issue #2230](https://code.google.com/p/tortoisegit/issues/detail?id=#2230): First click on order dialog is ignored
  * Fixed [issue #2003](https://code.google.com/p/tortoisegit/issues/detail?id=#2003): TortoiseMerge uses wrong EOL with patches
  * Fixed [issue #2234](https://code.google.com/p/tortoisegit/issues/detail?id=#2234): Config file mess up if not end with LF
  * Fixed [issue #2238](https://code.google.com/p/tortoisegit/issues/detail?id=#2238): TortoiseGitMerge Default button in "Find" dialog does replace all
  * Fixed [issue #2250](https://code.google.com/p/tortoisegit/issues/detail?id=#2250): bugtraq.logregex Test incorrectly saves the order of the fields
  * TGitCache now does not check the contents of files with filesize > 10 MiB any more
> > and falls back to checking the timestamp of the files (as if TGitCacheCheckContent
> > is set to "false") according the the git index. This limit can be changed by adjusting
> > TGitCacheCheckContentMaxSize (measured in KiB) in TortoiseGit advanced settings.
> > The reason for this change is that libgit2 reads a file to memory for hashing and,
> > thus, locking the file and the repository for this time span.
> > Fixed [issue #2240](https://code.google.com/p/tortoisegit/issues/detail?id=#2240): TGitCache keeps crashing when I look at my folders or commit
  * Fixed [issue #2219](https://code.google.com/p/tortoisegit/issues/detail?id=#2219): "add cherry picked from" is not applied when squashing/editing the commits
  * TortoiseGitMerge: Fix some crashes when Wrap Long Lines is enabled
  * TortoiseGitMerge: Use the screen chars of the current view for the scrollbar page value
  * TortoiseGitMerge: Do not draw EOL mark in line number region
  * TortoiseGitMerge: No need to expand tab to spaces when finding inline diff positions
  * Repository Browser said commit not found in submodule

## Known Issues ##
  * If you use ssh.exe for pushing & pulling, please see [issue #2257](https://code.google.com/p/tortoisegit/issues/detail?id=#2257).
  * There seems to be a bug in the MFC library which occurrs when opening the revision graph in the x64
> > version on AMD CPUs, we cannot fix this. Please vote for this on Microsoft Connect:
> > https://connect.microsoft.com/VisualStudio/feedback/details/893171/c000001d-illegal-instruction-on-msvcr120-log-0x2d3-on-x64.

# Release 1.8.9.0 #
Released: 2014-06-09

## Features ##
  * Fixed [issue #2152](https://code.google.com/p/tortoisegit/issues/detail?id=#2152): Log window show whole commit in "View patch"
  * Fixed [issue #2149](https://code.google.com/p/tortoisegit/issues/detail?id=#2149): Can't search message in annotated tag or text in notes
  * Fixed [issue #2172](https://code.google.com/p/tortoisegit/issues/detail?id=#2172): Support num parameters of git blame -M and git blame -C
  * Fixed [issue #2179](https://code.google.com/p/tortoisegit/issues/detail?id=#2179): Revision comparisons against HEAD should not generate temporary files (allow to compare to working tree)
  * Fixed [issue #2168](https://code.google.com/p/tortoisegit/issues/detail?id=#2168): Add to the "Clean up" dialog "Recursive" option for submodules
  * Fixed [issue #2196](https://code.google.com/p/tortoisegit/issues/detail?id=#2196): Log dialog file list group headers show parent SHA-1
  * Fixed [issue #2144](https://code.google.com/p/tortoisegit/issues/detail?id=#2144): TortoiseGit should support configuring pushurl for remotes
  * Fixed [issue #2155](https://code.google.com/p/tortoisegit/issues/detail?id=#2155): Make "Delete Remote Tags..." more discoverable
  * Fixed [issue #2164](https://code.google.com/p/tortoisegit/issues/detail?id=#2164): allow Commit from Log > Working dir changes of selected files
  * Fixed [issue #2096](https://code.google.com/p/tortoisegit/issues/detail?id=#2096): Allow to disable blue text-label about git.exe execution timings on progress dialog
  * Fixed [issue #968](https://code.google.com/p/tortoisegit/issues/detail?id=#968): Rebase / Cherry Pick dialogs should update "conflict" status when conflicts are resolved
  * Fixed [issue #1706](https://code.google.com/p/tortoisegit/issues/detail?id=#1706): Show log in different branch reverts to active branch
  * Fixed [issue #1973](https://code.google.com/p/tortoisegit/issues/detail?id=#1973): Support INS/OVR mode in TortoiseMerge
  * Fixed [issue #1970](https://code.google.com/p/tortoisegit/issues/detail?id=#1970): Provide replacement function in TortoiseGitMerge
  * Use libgit2 for more operations instead of calling git.exe

## Bug Fixes ##
  * Fixed [issue #2158](https://code.google.com/p/tortoisegit/issues/detail?id=#2158): TortoiseGit sometimes crashes when doing Sync > Pull
  * Fixed [issue #2159](https://code.google.com/p/tortoisegit/issues/detail?id=#2159): URL combo box in Submodule Add is not case sensitive
  * Fixed [issue #2171](https://code.google.com/p/tortoisegit/issues/detail?id=#2171): blame setting 'detect moved or copied line' does not work for the case 'from modified files'
  * Fixed [issue #2174](https://code.google.com/p/tortoisegit/issues/detail?id=#2174): Submodule update shows wrong submodule list
  * Fixed [issue #2175](https://code.google.com/p/tortoisegit/issues/detail?id=#2175): TortoiseGitBlame fails to search if line has non-ascii chars and system locale is not US
  * Fixed [issue #2141](https://code.google.com/p/tortoisegit/issues/detail?id=#2141): libgit2 still added the file with mixing EOL, while autocrlf and safecrlf are true
  * Fixed [issue #2183](https://code.google.com/p/tortoisegit/issues/detail?id=#2183): Explorer Property Page "Last modified" stays empty
  * Fixed [issue #2180](https://code.google.com/p/tortoisegit/issues/detail?id=#2180): When opening revision graph, scroll to current branch
  * Fixed [issue #2104](https://code.google.com/p/tortoisegit/issues/detail?id=#2104): Opening log for non-git folder results in multiple error messages
  * Fixed [issue #2192](https://code.google.com/p/tortoisegit/issues/detail?id=#2192): Shell context menu not detecting submodule if submodule name differs from submodule path
  * Fixed [issue #2187](https://code.google.com/p/tortoisegit/issues/detail?id=#2187): Misshowed branch on many dialogs in the new version
  * Fixed [issue #2191](https://code.google.com/p/tortoisegit/issues/detail?id=#2191): Skip-worktree or assume-valid flagged files are not always listed if subfolder is selected
  * Fixed [issue #2199](https://code.google.com/p/tortoisegit/issues/detail?id=#2199): Fetch dialog does not delete remote in remote list after managing remotes
  * Fixed [issue #2200](https://code.google.com/p/tortoisegit/issues/detail?id=#2200): Add remote name starts with # should not fetch all
  * Fixed [issue #2190](https://code.google.com/p/tortoisegit/issues/detail?id=#2190): "Force Rebase" after "Squash ALL" does not mark commits for squashing
  * Fixed [issue #2073](https://code.google.com/p/tortoisegit/issues/detail?id=#2073): Remove Entry of remote in "Remote Url" box in sync window
  * Fixed [issue #2207](https://code.google.com/p/tortoisegit/issues/detail?id=#2207): "Do you want to stash pop now?" dialog shows "Stash" labeled button instead of "Pop"
  * Fixed [issue #2161](https://code.google.com/p/tortoisegit/issues/detail?id=#2161): Windows explorer slow/very long delays with shell extension enabled and accessing network folders
  * Fixed [issue #2198](https://code.google.com/p/tortoisegit/issues/detail?id=#2198): MSVCR110.dll error with TortoisePlink. However, using TortoiseGitPlink is recommended

# Release 1.8.8.0 #
Released: 2014-04-01

## Features ##
  * Fixed [issue #2065](https://code.google.com/p/tortoisegit/issues/detail?id=#2065): Add link to fetch to screen when push failed
  * Fixed [issue #1855](https://code.google.com/p/tortoisegit/issues/detail?id=#1855): Support negative log filter syntax
  * Fixed [issue #1029](https://code.google.com/p/tortoisegit/issues/detail?id=#1029): Add function to control the TGitCache module
  * Fixed [issue #2086](https://code.google.com/p/tortoisegit/issues/detail?id=#2086): Rebase autoskip patches that are already in upstream
  * Fixed [issue #2112](https://code.google.com/p/tortoisegit/issues/detail?id=#2112): Disable option for Drag & Drop Handler
  * Fixed [issue #2114](https://code.google.com/p/tortoisegit/issues/detail?id=#2114): Allow to swap rebase refs
  * Updated libgit to version 1.9.0
  * Fixed [issue #1920](https://code.google.com/p/tortoisegit/issues/detail?id=#1920): Diff in log dialog like in commit dialog
  * Fixed [issue #2134](https://code.google.com/p/tortoisegit/issues/detail?id=#2134): Easier to select lines to partial commit in TortoiseGitMerge
  * Fixed [issue #2135](https://code.google.com/p/tortoisegit/issues/detail?id=#2135): Add menu button to open Explorer when clone finishes

## Bug Fixes ##
  * Fixed [issue #2067](https://code.google.com/p/tortoisegit/issues/detail?id=#2067): Normalize email with capital letters when calculating gravatar hash
  * Fixed [issue #2071](https://code.google.com/p/tortoisegit/issues/detail?id=#2071): TGitCache blocks Windows to eject USB drive
  * Fixed [issue #2074](https://code.google.com/p/tortoisegit/issues/detail?id=#2074): Time field not large enough
  * Fixed [issue #1648](https://code.google.com/p/tortoisegit/issues/detail?id=#1648): Issue with handles being kept when there are uncommitted changes
  * Fixed [issue #2083](https://code.google.com/p/tortoisegit/issues/detail?id=#2083): TortoiseGitBlame 'show unified diff' actually performs compare
  * Fixed [issue #2087](https://code.google.com/p/tortoisegit/issues/detail?id=#2087): Rebase ComboBox DropDown List too short
  * Fixed [issue #2088](https://code.google.com/p/tortoisegit/issues/detail?id=#2088): log entries have space in front of message without labels if right side drawing is enabled
  * Fixed [issue #2075](https://code.google.com/p/tortoisegit/issues/detail?id=#2075): Commit do not show merged files after merge
  * Fixed [issue #2097](https://code.google.com/p/tortoisegit/issues/detail?id=#2097): Wrong context menu when selecting ignored file in Status dialog
  * Fixed [issue #2099](https://code.google.com/p/tortoisegit/issues/detail?id=#2099): Cannot cancel "Delete and add to ignore list"
  * Fixed [issue #2109](https://code.google.com/p/tortoisegit/issues/detail?id=#2109): Checkout Tag without creating Branch - Remove Pull Option
  * Fixed [issue #2106](https://code.google.com/p/tortoisegit/issues/detail?id=#2106): "All local branches" option is not remembered
  * Fixed [issue #2076](https://code.google.com/p/tortoisegit/issues/detail?id=#2076): Issue Tracker Integration is broken in 1.8.7.0
  * Fixed [issue #2124](https://code.google.com/p/tortoisegit/issues/detail?id=#2124): Rebase icon not properly displayed
  * Fixed [issue #2113](https://code.google.com/p/tortoisegit/issues/detail?id=#2113): JiraSvn bugtraq provider's commit behavior is broken
  * Fixed [issue #2128](https://code.google.com/p/tortoisegit/issues/detail?id=#2128): tagopt not saved when asked to disable tag fetching
  * Fixed [issue #2127](https://code.google.com/p/tortoisegit/issues/detail?id=#2127): After delete last tag in Browse references, tree of refs disappeared
  * Fixed [issue #2131](https://code.google.com/p/tortoisegit/issues/detail?id=#2131): Commit message not used when merging with "squash" option
  * Fixed [issue #2147](https://code.google.com/p/tortoisegit/issues/detail?id=#2147): Resolve not dealing correctly with (modify/delete) conflicts
  * Fixed [issue #2148](https://code.google.com/p/tortoisegit/issues/detail?id=#2148): Cherry pick with conflicts does not add "Cherry picked from..."
  * Fixed [issue #2150](https://code.google.com/p/tortoisegit/issues/detail?id=#2150): Integrate with issue tracker - bug Id can not be larger than 6 digit number

# Release 1.8.7.0 #
Released: 2014-01-12

## Features ##
  * Fixed [issue #1943](https://code.google.com/p/tortoisegit/issues/detail?id=#1943): Add "Ignore N items by extension" in Commit dialog
  * Fixed [issue #1952](https://code.google.com/p/tortoisegit/issues/detail?id=#1952): Export specific folder
  * Fixed [issue #1002](https://code.google.com/p/tortoisegit/issues/detail?id=#1002): No right-drag context menu (git copy & add, git move)
  * Fixed [issue #1956](https://code.google.com/p/tortoisegit/issues/detail?id=#1956): Ship more overlay icon sets as TortoiseSVN does
  * Add Ref Compare List in Sync Dialog
  * Fixed [issue #1975](https://code.google.com/p/tortoisegit/issues/detail?id=#1975): Pull Dialog should remember fast forward only
  * Fixed [issue #1981](https://code.google.com/p/tortoisegit/issues/detail?id=#1981): Hotkey to focus on file list in commit dialog
  * Fixed [issue #1979](https://code.google.com/p/tortoisegit/issues/detail?id=#1979): Comments are not stripped from commit message
  * Fixed [issue #1991](https://code.google.com/p/tortoisegit/issues/detail?id=#1991): Disable (by default) certain operations with stash commits
  * Updated shipped libgit2 to version 0.20
  * Fixed [issue #2010](https://code.google.com/p/tortoisegit/issues/detail?id=#2010): Conflict dialog show local and remote commits
  * Autocompletion for language-dependent keywords (usually class/method/variable names) in the commit dialog
  * Fixed [issue #2034](https://code.google.com/p/tortoisegit/issues/detail?id=#2034): Show gravatar in TortoiseGitBlame
  * Fixed [issue #871](https://code.google.com/p/tortoisegit/issues/detail?id=#871): Blame copy/move detection and other options
  * Fixed [issue #1990](https://code.google.com/p/tortoisegit/issues/detail?id=#1990): TortoiseGitBlame always takes whitespace into account
  * Fixed [issue #1988](https://code.google.com/p/tortoisegit/issues/detail?id=#1988): Allow tag selection in From/To fields instead of dates only
  * Fixed [issue #2015](https://code.google.com/p/tortoisegit/issues/detail?id=#2015): Save and load ref lists (selections) in "Show log" -> "Browse references"
  * Fixed [issue #1847](https://code.google.com/p/tortoisegit/issues/detail?id=#1847): Option to show all local branches in log view
  * Fixed [issue #1823](https://code.google.com/p/tortoisegit/issues/detail?id=#1823): Pressing tab key can insert spaces instead of tab in TortoiseGitMerge
  * Fixed [issue #2047](https://code.google.com/p/tortoisegit/issues/detail?id=#2047): Create a log file with git commands and output
  * Fixed [issue #1129](https://code.google.com/p/tortoisegit/issues/detail?id=#1129): Add Fetch/Pull operations in Show Log window
  * Fixed [issue #2048](https://code.google.com/p/tortoisegit/issues/detail?id=#2048): Add date to stash list / reflog
  * Fixed [issue #2049](https://code.google.com/p/tortoisegit/issues/detail?id=#2049): Add pull to after commit actions
  * Fixed [issue #1980](https://code.google.com/p/tortoisegit/issues/detail?id=#1980): Add Show Unified Diff entry to context menu in TortoiseGitBlame in Revision List
  * Fixed [issue #1820](https://code.google.com/p/tortoisegit/issues/detail?id=#1820): Show Assume valid/unchanged files in repo status dialog on a separate list
  * Fixed [issue #1603](https://code.google.com/p/tortoisegit/issues/detail?id=#1603): Make "Show Whole Project" in log and commit dialog autosaved
  * Fixed [issue #827](https://code.google.com/p/tortoisegit/issues/detail?id=#827): add the option to autoclose the "Git command progress" window
  * Fixed [issue #1913](https://code.google.com/p/tortoisegit/issues/detail?id=#1913): SVN DCommit Button in successful merge Dialog
  * Fixed [issue #1978](https://code.google.com/p/tortoisegit/issues/detail?id=#1978): Use file directory on Save revision to path in Repository Browser and log dialog
  * Updated libgit to version 1.8.5.2
  * Fixed [issue #2059](https://code.google.com/p/tortoisegit/issues/detail?id=#2059): "Go to line" CLI argument support for diff command

## Bug Fixes ##
  * Fixed [issue #1947](https://code.google.com/p/tortoisegit/issues/detail?id=#1947): When editing git notes, spurious reformatting is done
  * Fixed [issue #1951](https://code.google.com/p/tortoisegit/issues/detail?id=#1951): Slow switch/checkout dialog
  * Fixed [issue #1958](https://code.google.com/p/tortoisegit/issues/detail?id=#1958): Revision graph crashes when trying to switch/checkout via context menu
  * Fixed [issue #1963](https://code.google.com/p/tortoisegit/issues/detail?id=#1963): TortoiseGitMerge: Missing color config when an added line is changed
  * Fixed [issue #1976](https://code.google.com/p/tortoisegit/issues/detail?id=#1976): Commit log crashes if it receives a WM\_PRINTCLIENT while opening
  * Fixed [issue #1974](https://code.google.com/p/tortoisegit/issues/detail?id=#1974): bugtraq logregex does not save correctly
  * Fixed [issue #1977](https://code.google.com/p/tortoisegit/issues/detail?id=#1977): Commit log: cannot select multiple branches if a branch name matches a filename
  * Fixed [issue #1992](https://code.google.com/p/tortoisegit/issues/detail?id=#1992): Compare selected refs fails if tag object is selected
  * Fixed [issue #1985](https://code.google.com/p/tortoisegit/issues/detail?id=#1985): TortoiseGitBlame does not follow renames when comparing line with previous version
  * Fixed [issue #2008](https://code.google.com/p/tortoisegit/issues/detail?id=#2008): Wrong reflog if hash repeated
  * Fixed [issue #2004](https://code.google.com/p/tortoisegit/issues/detail?id=#2004): In create patch serial dialog, number of commits up down buttons reversed
  * Fixed [issue #2013](https://code.google.com/p/tortoisegit/issues/detail?id=#2013): Double-clicking on ref log list doesn't work until after right-clicking it
  * Fixed [issue #2016](https://code.google.com/p/tortoisegit/issues/detail?id=#2016): Changed files list forgets sort order after switching versions in compare revisions dialog
  * Fixed [issue #2014](https://code.google.com/p/tortoisegit/issues/detail?id=#2014): "Show log" doesn't update properly when a window is dragged over it if aero is not enabled
  * Fixed [issue #2021](https://code.google.com/p/tortoisegit/issues/detail?id=#2021): Disable commit template when combine commits
  * Fixed [issue #2024](https://code.google.com/p/tortoisegit/issues/detail?id=#2024): Unnamed "remote" should not be created
  * Fixed [issue #2027](https://code.google.com/p/tortoisegit/issues/detail?id=#2027): Failed to preserve selected commit when filter is removed
  * Fixed [issue #2030](https://code.google.com/p/tortoisegit/issues/detail?id=#2030): TortoisePlink crash on x64
  * Fixed [issue #2037](https://code.google.com/p/tortoisegit/issues/detail?id=#2037): TortoiseGit.dll sometimes does not close it's handles in explorer.exe
  * Fixed [issue #2040](https://code.google.com/p/tortoisegit/issues/detail?id=#2040): "fatal: pathspec did not match any files" error when resolving deleted/modified conflict
  * Fixed [issue #1866](https://code.google.com/p/tortoisegit/issues/detail?id=#1866): Check for newer version of tgit behind proxy
  * Fixed [issue #1927](https://code.google.com/p/tortoisegit/issues/detail?id=#1927): Clicking on a hyperlinked commit hash leaves the target's log message un-hyperlinked
  * Fixed [issue #1835](https://code.google.com/p/tortoisegit/issues/detail?id=#1835): Question mark icons on committed unchanged files
  * Fixed [issue #2053](https://code.google.com/p/tortoisegit/issues/detail?id=#2053): Can't do "Combine to one commit"; changed file list wrongly empty
  * Fixed [issue #2051](https://code.google.com/p/tortoisegit/issues/detail?id=#2051): Submodule update error when fetchRecurseSubmodules has value on-demand
  * Fixed [issue #1860](https://code.google.com/p/tortoisegit/issues/detail?id=#1860): Race condition in git.exe Progress Dialog
  * Fixed [issue #2020](https://code.google.com/p/tortoisegit/issues/detail?id=#2020): Passworddialog in background after requesting username
  * Fixed [issue #1802](https://code.google.com/p/tortoisegit/issues/detail?id=#1802): submodule update module selection not always accurate
  * Fixed [issue #1579](https://code.google.com/p/tortoisegit/issues/detail?id=#1579): Log Dialog sometimes forgets the dialog height

## Known Issues ##
  * If you upgraded Windows 8 to 8.1 and you experience problems with the installer, please see [issue #2061](https://code.google.com/p/tortoisegit/issues/detail?id=#2061).
  * If you experience problems/crashes while starting !Tortoise(Git)Merge, please see [issue #2063](https://code.google.com/p/tortoisegit/issues/detail?id=#2063).

# Release 1.8.6.0 #
Released: 2013-10-20

## Features ##
  * Revision Graph: Can generate output graph file through command line
  * Fixed [issue #1858](https://code.google.com/p/tortoisegit/issues/detail?id=#1858): Switch-and-merge as a single command
  * Log Dialog: Support Gravatar
  * Implement git checkout --merge
  * TortoiseGitIDiff: Conflict resolving for images
  * Fixed [issue #1795](https://code.google.com/p/tortoisegit/issues/detail?id=#1795): Allow to put branch labels on right side of message column in log view
  * Fixed [issue #1870](https://code.google.com/p/tortoisegit/issues/detail?id=#1870): Commit subset of changes selected from diff dialog
  * Fixed [issue #1785](https://code.google.com/p/tortoisegit/issues/detail?id=#1785): If PuTTY defaults to anything other than type SSH port 22, TortoiseGit acts up on SSH cloning (fixed in TortoiseGitPlink.exe)
  * Add setting to confirm to kill running git process in progress dialog
  * Added support for tgit://-links to start cloning from browser (e.g. tgit://clone/https://code.google.com/p/tortoisegit/)
  * Added optional support for git://-links to start cloning from browser
  * Added optional support for smartgit:// and github-windows://-links to start cloning from browser
> > In order to be able to use github-windows://-links on github.com web page, you have to enable them for your GitHub profile once.
> > Right now the only way is to install the official GitHub client and sign in with your GitHub profile (on any Windows machine).
  * Allow to edit hierarchical git settings
> > If you have set "i18n.commitencoding" to something different than UTF-8 check your "user.name" setting
  * Fixed [issue #1645](https://code.google.com/p/tortoisegit/issues/detail?id=#1645): enable/disable spell checking in commit dialog
  * Fixed [issue #1806](https://code.google.com/p/tortoisegit/issues/detail?id=#1806): Compressed graph in the log view
  * Fixed [issue #1926](https://code.google.com/p/tortoisegit/issues/detail?id=#1926): Add "No Merges" checkbox in Log Messages window
  * Fixed [issue #1779](https://code.google.com/p/tortoisegit/issues/detail?id=#1779): tortoisegit does not understand include.path in global config
> > If you have relevant settings for TGitCache in an included file, you have to restard TGitCache or modify the global, system, or local config file in order to reload any included file.
  * Support project icon as task button overlay
  * Fixed [issue #1946](https://code.google.com/p/tortoisegit/issues/detail?id=#1946): In "Compare revisions", please show something to confirm when there are no differences

## Bug Fixes ##
  * Fixed [issue #1859](https://code.google.com/p/tortoisegit/issues/detail?id=#1859): Log too long when using Switch to New Branch option in Create Branch dialog
  * Fixed [issue #1864](https://code.google.com/p/tortoisegit/issues/detail?id=#1864): Commit button did not work after revert
  * Fixed [issue #1862](https://code.google.com/p/tortoisegit/issues/detail?id=#1862): Some labels not wide enough for translations to fit in
  * Fixed [issue #1790](https://code.google.com/p/tortoisegit/issues/detail?id=#1790): "Clean up" window position is not preserved on multi-monitor setup
  * Fixed [issue #1876](https://code.google.com/p/tortoisegit/issues/detail?id=#1876): Up/down buttons in Rebase dialog desynchronise the bottom view
  * Fixed [issue #1875](https://code.google.com/p/tortoisegit/issues/detail?id=#1875): Commit selection is lost with focus in Rebase dialog
  * Fixed [issue #1873](https://code.google.com/p/tortoisegit/issues/detail?id=#1873): Squash doesn't preserve original author date
  * Fixed [issue #1863](https://code.google.com/p/tortoisegit/issues/detail?id=#1863): never-ending wait due to lost messages
  * Fixed [issue #1883](https://code.google.com/p/tortoisegit/issues/detail?id=#1883): Option Buttons in Hook script not wide enough
  * Fixed [issue #1893](https://code.google.com/p/tortoisegit/issues/detail?id=#1893): Unified diff for merge commit always shows inverted changes
  * Fixed [issue #1896](https://code.google.com/p/tortoisegit/issues/detail?id=#1896): Switch/Checkout Branch name resets itself after browsing for a branch
  * Fixed [issue #1895](https://code.google.com/p/tortoisegit/issues/detail?id=#1895): Context menu incomplete if working tree is located on network share
  * Fixed [issue #1618](https://code.google.com/p/tortoisegit/issues/detail?id=#1618): In "Show log", mouseover triggers improper redraw of ClearType font log descriptions in "Message" column
  * Fixed [issue #1891](https://code.google.com/p/tortoisegit/issues/detail?id=#1891): Cleanup dialog unexpectedly sizable
  * Bring back templates when creating repository with libgit2, it was "cancelled" in since TortoiseGit 1.8.0
  * Fixed [issue #1908](https://code.google.com/p/tortoisegit/issues/detail?id=#1908): "Export selection to.." fails to checkout files which names (or paths) renamed in working dir
  * Fixed [issue #1914](https://code.google.com/p/tortoisegit/issues/detail?id=#1914): Repository Browser give an error (libgit2) after change branch
  * Fixed [issue #1915](https://code.google.com/p/tortoisegit/issues/detail?id=#1915): Submodule Update Dialog behaves curious
  * Fixed [issue #1919](https://code.google.com/p/tortoisegit/issues/detail?id=#1919): Submodule visibility with square brackets
  * Fixed [issue #1918](https://code.google.com/p/tortoisegit/issues/detail?id=#1918): Settings dialog forces to use remotes
  * Fixed [issue #1923](https://code.google.com/p/tortoisegit/issues/detail?id=#1923): Once Credential node is activated, pressing apply button in Settings dialog will close the dialog
  * Fixed [issue #1769](https://code.google.com/p/tortoisegit/issues/detail?id=#1769): "Show Log" missing from context menu if "Shell Extended" and a file was Added but not committed
  * Fixed [issue #1917](https://code.google.com/p/tortoisegit/issues/detail?id=#1917): Avoid request to stash if there is nothing to rebase or fast forward is possible
  * Fixed [issue #1929](https://code.google.com/p/tortoisegit/issues/detail?id=#1929): Using "Find" in "Show log" doesn't move to commits it finds, it only selects them
  * Fixed [issue #1948](https://code.google.com/p/tortoisegit/issues/detail?id=#1948): Case sensitive authors switch throw an error

## Known Issues ##
  * If you experience problems with PuTTY ssh, please see [issue #1880](https://code.google.com/p/tortoisegit/issues/detail?id=#1880).

# Release 1.8.5.0 #
Released: 2013-08-18

## Features ##
  * Fixed [issue #1831](https://code.google.com/p/tortoisegit/issues/detail?id=#1831): Allow Origin Remote Renaming on Clone
  * Fixed [issue #1839](https://code.google.com/p/tortoisegit/issues/detail?id=#1839): Conflict dialog does not allow resolving multiple or all conflicts with the same option
  * Allow to send (patch)mails over relay servers (e.g. the one from your ISP)
  * When adding second and more remotes, prompt user to disable tag fetching to avoid fetching wrong tags
  * Fixed [issue #1845](https://code.google.com/p/tortoisegit/issues/detail?id=#1845): Add "pull" button on "git switch" window
  * Fixed [issue #1848](https://code.google.com/p/tortoisegit/issues/detail?id=#1848): TortoiseGitBlame doesn't scroll to the previously selected line on "Blame previous revision"
  * Underline git hash in log message view and jump to that commit when clicking on the hash
  * Fixed [issue #1829](https://code.google.com/p/tortoisegit/issues/detail?id=#1829): You have not concluded your merge (MERGE\_HEAD exists) - allow to abort merge more easily.
  * Commit Dialog: Add "Pick commit hash" in message text box context menu
  * Can set log graph line width and node size
  * Updated shipped PuTTY PLink to version 0.63 (which contains some securiuty fixes)
  * Fixed [issue #1746](https://code.google.com/p/tortoisegit/issues/detail?id=#1746): Pressing "Delete" on keyboard should delete selected non versioned file in commit dialog
  * Sync Dialog: Add stash menu button
  * Fixed [issue #1852](https://code.google.com/p/tortoisegit/issues/detail?id=#1852): Add command-line argument to tortoisegitproc that specifies value for Directory field

## Bug Fixes ##
  * Fixed [issue #1833](https://code.google.com/p/tortoisegit/issues/detail?id=#1833): Fast-Forward rebase does not preserve SHA-1 of commits
  * Fixed [issue #1832](https://code.google.com/p/tortoisegit/issues/detail?id=#1832): TortoiseGitMerge has an empty menue when German language pack is loaded
  * Fixed [issue #497](https://code.google.com/p/tortoisegit/issues/detail?id=#497): TGitCache.exe won't let user delete folder
  * Mitigated [issue #1011](https://code.google.com/p/tortoisegit/issues/detail?id=#1011): "git svn" commands create "sys$command" file

# Release 1.8.4.0 #
Released: 2013-07-09

## Features ##
  * Fixed [issue #1765](https://code.google.com/p/tortoisegit/issues/detail?id=#1765): Pull button when push (after commit) fails
  * Updated shipped libgit2 to version 0.19
  * Updated libgit to version 1.8.3
  * Support diff.context config key
  * Fixed [issue #1778](https://code.google.com/p/tortoisegit/issues/detail?id=#1778): Add Submodule with Putty key
  * Fixed [issue #1800](https://code.google.com/p/tortoisegit/issues/detail?id=#1800): Automatically remove "git clone " from URL in Clone dialog
  * Fixed [issue #1807](https://code.google.com/p/tortoisegit/issues/detail?id=#1807): Handle new descriptions of detached head introduced in git 1.8.3
  * TortoiseGitMerge: Encoding and EOL conversion
  * TortoiseGitMerge: Tab / spaces conversion and trim trailing space
  * TortoiseUDiff: Add Printing function
  * Fixed [issue #553](https://code.google.com/p/tortoisegit/issues/detail?id=#553): Pull the latest version of all submodules
  * TortoiseGitMerge: Improved applying a patch with conflicts
  * Rename touch.exe as tgittouch.exe to avoid filename collision
  * Support SOCKS proxy
  * Include submodules in RepositoryBrowser

## Bug Fixes ##
  * Fixed [issue #1763](https://code.google.com/p/tortoisegit/issues/detail?id=#1763): Unable to re-download TortoiseGit packages due to caching
  * Fixed [issue #795](https://code.google.com/p/tortoisegit/issues/detail?id=#795): Switch/Checkout Dialog, "Switch To Version" is confusing
  * Fixed [issue #722](https://code.google.com/p/tortoisegit/issues/detail?id=#722): Pull/Push sometimes does not gets the right remote branch
  * Fixed [issue #1781](https://code.google.com/p/tortoisegit/issues/detail?id=#1781): Sync dialog fails with "Encountered an improper argument" when closing log tab with escape
  * Fixed [issue #1773](https://code.google.com/p/tortoisegit/issues/detail?id=#1773): "Show changes as unified diff" on "Working dir changes" show inverted diff operation
  * Fixed [issue #1753](https://code.google.com/p/tortoisegit/issues/detail?id=#1753): On dialog box for SSH certificate's passphrase, some certificate filenames aren't fully displayed
  * Fixed [issue #1726](https://code.google.com/p/tortoisegit/issues/detail?id=#1726): Rebasing issues with empty commits
  * Fixed [issue #1782](https://code.google.com/p/tortoisegit/issues/detail?id=#1782): Do not reset changed lines/files statistics after toggling "Authors case sensitive" checkbox
  * Fixed [issue #1783](https://code.google.com/p/tortoisegit/issues/detail?id=#1783): TortoiseGit does not work on WinXP/2003 x64
  * Fixed [issue #1798](https://code.google.com/p/tortoisegit/issues/detail?id=#1798): "Paste Recent commits" during Please wait in Commit dialog does not work
  * Fixed [issue #1106](https://code.google.com/p/tortoisegit/issues/detail?id=#1106): Stairs in log view
  * Fixed [issue #1304](https://code.google.com/p/tortoisegit/issues/detail?id=#1304): TortoiseGit doesn't see a bare repo within a non-bare one
  * "Delete (keep local)" did not work on folders
  * Fixed [issue #1756](https://code.google.com/p/tortoisegit/issues/detail?id=#1756): Rebase trips over merge commits
  * Fixed possible crashes while applying a patch in TortoiseGitMerge
  * Fixed [issue #1809](https://code.google.com/p/tortoisegit/issues/detail?id=#1809): Overlay shows changes in parent folder if a file with a second extension exists
  * TortoiseGitMerge: Fixed bugs regarding multi-view edit
  * Fixed [issue #1814](https://code.google.com/p/tortoisegit/issues/detail?id=#1814): Squash rebase fills message too much
  * Reverting newly added file in Commit-dialog misbehaving
  * Fixed [issue #1589](https://code.google.com/p/tortoisegit/issues/detail?id=#1589): Clone Dialog's URL case sensitivity causes issues with folder creation
  * Fixed [issue #1786](https://code.google.com/p/tortoisegit/issues/detail?id=#1786): Committing 25 or more files causes hidden progress dialog
  * Fixed [issue #1732](https://code.google.com/p/tortoisegit/issues/detail?id=#1732): Tortoisegit always crashes when viewing the history log of blink
  * Fixed [issue #1824](https://code.google.com/p/tortoisegit/issues/detail?id=#1824): Rebase Dialog sometimes not showing after running Fetch and Rebase in Sync Dialog
  * Fixed [issue #1725](https://code.google.com/p/tortoisegit/issues/detail?id=#1725): 'Git Show Log' doesn't work on folders created by git-new-workdir script

# Release 1.8.3.0 #
Released: 2013-05-05

## Features ##
  * Press F5 can refresh Submodule Diff Dialog
  * Fixed [issue #1359](https://code.google.com/p/tortoisegit/issues/detail?id=#1359): Drag support for files listed as being changed in the commit/log/modifications window
  * log list: indicate annotated tag in tag shape
  * TortoiseGitBlame: Allow to highlight lines by age of last modification
  * Fixed [issue #1376](https://code.google.com/p/tortoisegit/issues/detail?id=#1376): Daemon starting from Tortoise UI
  * Fixed [issue #1737](https://code.google.com/p/tortoisegit/issues/detail?id=#1737): Make a button to rename remote
  * Repository Browser: Allow to copy tree / blob hashes to clipboard
  * Added sound support for indicating warnings and errors
  * Fixed [issue #1755](https://code.google.com/p/tortoisegit/issues/detail?id=#1755): Add "Remove All" and "Ignore All" options in Remove from Index Prompt
  * Fixed [issue #1747](https://code.google.com/p/tortoisegit/issues/detail?id=#1747): Add interface to log window to view range log

## Bug Fixes ##
  * Fixed [issue #1729](https://code.google.com/p/tortoisegit/issues/detail?id=#1729): crash when commit
  * Fixed [issue #1728](https://code.google.com/p/tortoisegit/issues/detail?id=#1728): TortoiseGitMerge show fake difference in the same lines if line end falls to 0x40000 byte
  * Fixed [issue #1741](https://code.google.com/p/tortoisegit/issues/detail?id=#1741): Push / Pull Dialog URL combo box should not be filled unless enabled
  * Fixed [issue #1735](https://code.google.com/p/tortoisegit/issues/detail?id=#1735): diff-xls.vbs not found
  * Fixed [issue #1750](https://code.google.com/p/tortoisegit/issues/detail?id=#1750): Repository Browser fails for empty repository
  * Fixed [issue #1743](https://code.google.com/p/tortoisegit/issues/detail?id=#1743): Remove "The target folder is not empty!" warning
  * Fixed [issue #1757](https://code.google.com/p/tortoisegit/issues/detail?id=#1757): Compare single new file against working tree
  * Fixed [issue #1760](https://code.google.com/p/tortoisegit/issues/detail?id=#1760): Unified diff of two revisions is inversed
  * Fixed various possible crashes

# Release 1.8.2.0 #
Released: 2013-03-26

## Features ##
  * Fixed [issue #1270](https://code.google.com/p/tortoisegit/issues/detail?id=#1270): Log dialog can revert selected files to parent revision
  * Fixed [issue #1500](https://code.google.com/p/tortoisegit/issues/detail?id=#1500): Support git merge --log option
  * Can disable log cache (tortoisegit.data, tortoisegit.index)
  * Revision Graph can save as graphviz dot language (`*`.gv)
  * Support merge strategies except octopus
  * Fixed [issue #1597](https://code.google.com/p/tortoisegit/issues/detail?id=#1597): Reduce chance of committing old submodule revision on cherry-pick / rebase conflicts
  * Can specify specific paths of submodules to update
  * Fixed [issue #1661](https://code.google.com/p/tortoisegit/issues/detail?id=#1661): TortoiseGitBlame: show line date time
  * Fixed [issue #1662](https://code.google.com/p/tortoisegit/issues/detail?id=#1662): skip-worktree should not be exposed via context menus or anything without confirmation
  * Fixed [issue #330](https://code.google.com/p/tortoisegit/issues/detail?id=#330): Implement --author option gui interface in the commit dialog
  * Fixed [issue #1147](https://code.google.com/p/tortoisegit/issues/detail?id=#1147): Ability to filter out branches in Log dialog
  * Fixed [issue #1628](https://code.google.com/p/tortoisegit/issues/detail?id=#1628): Support commit ranges in log list (from Reference Browser)
  * Fixed [issue #832](https://code.google.com/p/tortoisegit/issues/detail?id=#832): Compare commits between branches (branch1...branch2, from Reference Browser)
  * Fixed [issue #515](https://code.google.com/p/tortoisegit/issues/detail?id=#515): Sort the log window by date
  * Fixed [issue #1676](https://code.google.com/p/tortoisegit/issues/detail?id=#1676): Automatically check "Make it Bare" when repository path ends in ".git"
  * Fixed [issue #1677](https://code.google.com/p/tortoisegit/issues/detail?id=#1677): Clicking "revert" on a file should automatically check the file in the revert dialog
  * Fixed [issue #1667](https://code.google.com/p/tortoisegit/issues/detail?id=#1667): Ability to ignore a folder in commit dialog
  * Fixed [issue #1674](https://code.google.com/p/tortoisegit/issues/detail?id=#1674): Option "Push all branches" leaves out tags on pushed changes
  * Fixed [issue #1663](https://code.google.com/p/tortoisegit/issues/detail?id=#1663): F5 does not refresh the revision graph
  * Fixed [issue #522](https://code.google.com/p/tortoisegit/issues/detail?id=#522): Store password for HTTP
  * Fixed [issue #1660](https://code.google.com/p/tortoisegit/issues/detail?id=#1660): Save Push Dialog "Push all branches" and "Use Thin Pack" options
  * Fixed [issue #1542](https://code.google.com/p/tortoisegit/issues/detail?id=#1542): Can send pull request email
  * Fixed [issue #1493](https://code.google.com/p/tortoisegit/issues/detail?id=#1493): Remember Push Dialog "Push to all remotes" option state
  * Enhanced Windows 7 taskbar grouping and highlighting of windows belonging to the same working tree
  * .mailmap is now used for Log-Dialog Statistics
  * Fixed [issue #1610](https://code.google.com/p/tortoisegit/issues/detail?id=#1610): Average values on statistics dialog graph
  * Fixed [issue #1708](https://code.google.com/p/tortoisegit/issues/detail?id=#1708): Merge dialog have no saving of log message
  * Fixed [issue #1716](https://code.google.com/p/tortoisegit/issues/detail?id=#1716): TortoiseGitBlame added line parameter
  * Allow to set a default value for ssh client in HKLM (Software\TortoiseGit\SSH)

## Bug Fixes ##
  * Fixed [issue #1642](https://code.google.com/p/tortoisegit/issues/detail?id=#1642): Incorrect behavior if repo is located on root of drive
  * Fixed [issue #1643](https://code.google.com/p/tortoisegit/issues/detail?id=#1643): TortoiseGitMerge window do not maximize correctly on screeen with right-side docked start bar
  * Fixed [issue #1639](https://code.google.com/p/tortoisegit/issues/detail?id=#1639): Does not work on older CPU without SSE2
  * Fixed [issue #1682](https://code.google.com/p/tortoisegit/issues/detail?id=#1682): Rebase ignores commits after an error is received
  * Fixed [issue #1429](https://code.google.com/p/tortoisegit/issues/detail?id=#1429): Blame: copy sha to clipboard copies the log message
  * Fixed [issue #1654](https://code.google.com/p/tortoisegit/issues/detail?id=#1654): Git blame commit message tooltip flashes when tooltip window is tall
  * Fixed [issue #1658](https://code.google.com/p/tortoisegit/issues/detail?id=#1658): Checkbox 'add "cherry picked from"' has wrong anchor
  * Fixed [issue #1657](https://code.google.com/p/tortoisegit/issues/detail?id=#1657): Dirty submodule commit does not open the underling submodule commit dialog
  * Fixed [issue #1552](https://code.google.com/p/tortoisegit/issues/detail?id=#1552): TGitCache prevents a git clone from performing successfully
  * Fixed [issue #1631](https://code.google.com/p/tortoisegit/issues/detail?id=#1631): Set focus to branch menu in Switch/Checkout window
  * Fixed [issue #1646](https://code.google.com/p/tortoisegit/issues/detail?id=#1646): TortoiseGit Log gives undeterministic results (log does not apply --boundary any more by default)
  * Fixed [issue #1085](https://code.google.com/p/tortoisegit/issues/detail?id=#1085): Small commit with lots of unversioned and not ignored files takes very long
  * Fixed [issue #1675](https://code.google.com/p/tortoisegit/issues/detail?id=#1675): delete/ignore does not delete folder from repo when local copy is kept
  * Fixed [issue #1679](https://code.google.com/p/tortoisegit/issues/detail?id=#1679): Reset dialog pick another revision has no effect
  * Fixed [issue #1609](https://code.google.com/p/tortoisegit/issues/detail?id=#1609): remember my remote branch choice precisely
  * Fixed [issue #1268](https://code.google.com/p/tortoisegit/issues/detail?id=#1268): Paths in Windows Explorer changed to all lower case
  * Fixed [issue #1681](https://code.google.com/p/tortoisegit/issues/detail?id=#1681): High screen DPI breaks TortoiseGitMerge's ribbon UI sprites
  * Fixed [issue #1685](https://code.google.com/p/tortoisegit/issues/detail?id=#1685): Deleting remote branch blocks UI
  * Fixed [issue #1686](https://code.google.com/p/tortoisegit/issues/detail?id=#1686): Wrong stash list after "Stash Apply" in RefLog
  * Fixed [issue #1689](https://code.google.com/p/tortoisegit/issues/detail?id=#1689): Option to make Git Commit GUI look different from TortoiseSVN equivalent
  * Fixed [issue #1693](https://code.google.com/p/tortoisegit/issues/detail?id=#1693): Cherry pick progress bar doesn't stay green
  * Fixed [issue #1276](https://code.google.com/p/tortoisegit/issues/detail?id=#1276): Cannot show diff of renamed file
  * Fixed [issue #1696](https://code.google.com/p/tortoisegit/issues/detail?id=#1696): Fetch from switch dialog does not refresh branches list
  * Fixed [issue #1701](https://code.google.com/p/tortoisegit/issues/detail?id=#1701): Changing commit order in rebase dialog doesn't auto scroll
  * Fixed [issue #1702](https://code.google.com/p/tortoisegit/issues/detail?id=#1702): Original commit message is showen even though it is changed during rebase
  * Fixed [issue #1223](https://code.google.com/p/tortoisegit/issues/detail?id=#1223): Workaround endless waiting when git.exe already exited
  * Fixed [issue #1709](https://code.google.com/p/tortoisegit/issues/detail?id=#1709): Right click -> assume unchanged is irreversible
  * Fixed [issue #1713](https://code.google.com/p/tortoisegit/issues/detail?id=#1713): Pre-populate commit message on squash merges
  * Fixed [issue #1566](https://code.google.com/p/tortoisegit/issues/detail?id=#1566): Frequent crashes when searching log

# Release 1.8.1.0 #
Released: 2013-02-07

## Features ##
  * Fixed [issue #1623](https://code.google.com/p/tortoisegit/issues/detail?id=#1623): Search by email in Log window
  * Fixed [issue #1624](https://code.google.com/p/tortoisegit/issues/detail?id=#1624): Easier navigation in revision graph with mouse

## Bug Fixes ##
  * Fixed [issue #1611](https://code.google.com/p/tortoisegit/issues/detail?id=#1611): Changing Search criteria with empty search field refreshes log content
  * Fixed [issue #1620](https://code.google.com/p/tortoisegit/issues/detail?id=#1620): Apply Patch serial can't open file dialog on WinXP
  * Fixed [issue #1533](https://code.google.com/p/tortoisegit/issues/detail?id=#1533): Could not parse git.exe version number
  * Fixed [issue #1619](https://code.google.com/p/tortoisegit/issues/detail?id=#1619): TortoiseGitMerge: Ribbon UI/toolbars can be toggled
  * Fixed [issue #1627](https://code.google.com/p/tortoisegit/issues/detail?id=#1627): TortoiseGit gets the wrong revision if the branch name looks like git-describe format
  * Fixed [issue #1617](https://code.google.com/p/tortoisegit/issues/detail?id=#1617): TortoiseGitPLink does not work with interactive ssh logins
  * Fixed [issue #1384](https://code.google.com/p/tortoisegit/issues/detail?id=#1384): Commit Dialog autocompletion does not work for some pattern

# Release 1.8.0.0 #
Released: 2013-01-27

## Features ##
  * Fixed [issue #1377](https://code.google.com/p/tortoisegit/issues/detail?id=#1377): Log Dialog Working dir changes should include untracked files
  * Fixed [issue #1541](https://code.google.com/p/tortoisegit/issues/detail?id=#1541): Show progress dialog when running git request-pull
  * Fixed [issue #1513](https://code.google.com/p/tortoisegit/issues/detail?id=#1513): Easier to clean TortoiseGit temporary files
  * Fixed [issue #1540](https://code.google.com/p/tortoisegit/issues/detail?id=#1540): Add jump to previous / next commit in Log Dialog
  * Fixed [issue #1529](https://code.google.com/p/tortoisegit/issues/detail?id=#1529): Can show and set tagopt
  * Fixed [issue #1554](https://code.google.com/p/tortoisegit/issues/detail?id=#1554): Unwanted text formatting in commit dialogue (styling can be disabled using advanced settings now)
  * Fixed [issue #1563](https://code.google.com/p/tortoisegit/issues/detail?id=#1563): Show repository dir on Settings Dialog title bar
  * Fixed [issue #1577](https://code.google.com/p/tortoisegit/issues/detail?id=#1577): Add a retry button on Reset failure
  * Fixed [issue #1571](https://code.google.com/p/tortoisegit/issues/detail?id=#1571): Warn author not set when editing notes
  * Fixed [issue #221](https://code.google.com/p/tortoisegit/issues/detail?id=#221): After resolving all merge conflicts, it's not obvious the project needs a commit
  * Fixed [issue #1568](https://code.google.com/p/tortoisegit/issues/detail?id=#1568): Add support for recurse-submodules on push dialog
  * Fixed [issue #1578](https://code.google.com/p/tortoisegit/issues/detail?id=#1578): Warn author not set when merging
  * Fixed [issue #1557](https://code.google.com/p/tortoisegit/issues/detail?id=#1557): Submodule Diff Dialog should launch diff with working copy if the submodule is dirty
  * Fixed [issue #1066](https://code.google.com/p/tortoisegit/issues/detail?id=#1066): Add 'Revision Graph' Feature
  * Fixed [issue #1435](https://code.google.com/p/tortoisegit/issues/detail?id=#1435): EXE Name collision with TortoiseSVN
    * Renamed:
      * TortoiseIDiff.exe to TortoiseGitIDiff.exe
      * TortoiseMerge.exe to TortoiseGitMerge.exe
      * TortoiseProc.exe to TortoiseGitProc.exe
      * TortoisePLink.exe to TortoiseGitPLink.exe (TortoisePLink.exe is still shipped for compatibility reasons)
      * TortoiseUDiff.exe to TortoiseGitUDiff.exe
  * Fixed [issue #1433](https://code.google.com/p/tortoisegit/issues/detail?id=#1433): Can reset to remote tracking branch after fetch
  * Fixed [issue #763](https://code.google.com/p/tortoisegit/issues/detail?id=#763): "Clean up" should show a list of to-be-deleted files
  * Fixed [issue #1581](https://code.google.com/p/tortoisegit/issues/detail?id=#1581): Show/Hide tags in the log
  * Synced TortoiseGitMerge code with TortoiseMerge of TortoiseSVN code (trunk)
  * Log Dialog specially highlights branches that have a remote tracking branch
  * Added search mechanism to reflog dialog
  * Add No fetch, Merge and Rebase options in Submodule Update Dialog
  * Fixed [issue #1467](https://code.google.com/p/tortoisegit/issues/detail?id=#1467): put remote branches at the bottom in "branches" dropdowns (can be disabled using advanced settings)
  * Fixed [issue #1285](https://code.google.com/p/tortoisegit/issues/detail?id=#1285): Show Log Filter on Tags
  * Uncheck "Track" checkbox when creating a branch with different name to remote branch
  * Add button to push notes in Sync Dialog

## Bug Fixes ##
  * Fixed [issue #1535](https://code.google.com/p/tortoisegit/issues/detail?id=#1535): Unclear UI in prompt dialog of Stash Save
  * Fixed [issue #1538](https://code.google.com/p/tortoisegit/issues/detail?id=#1538): Deleting multiple stash list entries skips some and delete the wrong ones
  * Fixed [issue #1543](https://code.google.com/p/tortoisegit/issues/detail?id=#1543): TortoiseGit Comboboxes trim input if longer than their width
  * Fixed [issue #1544](https://code.google.com/p/tortoisegit/issues/detail?id=#1544): TortoiseGit Init warning message is not appropriate
  * Fixed [issue #1555](https://code.google.com/p/tortoisegit/issues/detail?id=#1555): Commit dialog fails to warn submodule dirty state
  * Fixed [issue #1556](https://code.google.com/p/tortoisegit/issues/detail?id=#1556): Narrower treeview when launching Settings Dialog with default page Remote
  * Fixed [issue #1383](https://code.google.com/p/tortoisegit/issues/detail?id=#1383): Pageant is not always auto-loaded if using sync remote update (some without keys)
  * Fixed [issue #1536](https://code.google.com/p/tortoisegit/issues/detail?id=#1536): Committing via log causes hidden progress dialog
  * Fixed [issue #1593](https://code.google.com/p/tortoisegit/issues/detail?id=#1593): Sync dialog In ChangeList shows wrong diff when pressing enter

# Release 1.7.15.0 #
Released: 2012-11-20

## Features ##
  * Fixed [issue #1436](https://code.google.com/p/tortoisegit/issues/detail?id=#1436): Clone Dialog add --branch and --no-checkout options
  * Fixed [issue #1450](https://code.google.com/p/tortoisegit/issues/detail?id=#1450): Option to fetch when adding a remote
  * Fixed [issue #1411](https://code.google.com/p/tortoisegit/issues/detail?id=#1411): Commit dialog checks submodule dirty state
  * Fixed [issue #1485](https://code.google.com/p/tortoisegit/issues/detail?id=#1485): Implement a Goto-Line dialog in TortoiseMerge
  * Upgraded gitdll and libgit to 1.8.0
  * Fixed [issue #1461](https://code.google.com/p/tortoisegit/issues/detail?id=#1461): Add progress indicator for stash operations
  * Fixed [issue #1484](https://code.google.com/p/tortoisegit/issues/detail?id=#1484): Settings dialog default to Git page
  * Fixed [issue #1505](https://code.google.com/p/tortoisegit/issues/detail?id=#1505): Tell user that author not set in Rebase Dialog
  * Fixed [issue #1503](https://code.google.com/p/tortoisegit/issues/detail?id=#1503): Passing full file paths and revisions into diff viewer
  * Fixed [issue #1518](https://code.google.com/p/tortoisegit/issues/detail?id=#1518): Add "Export selection to" menu item in Log Dialog
  * Fixed [issue #1497](https://code.google.com/p/tortoisegit/issues/detail?id=#1497): Systemwide gitconfig may require UAC elevation when editing
  * Fixed [issue #1512](https://code.google.com/p/tortoisegit/issues/detail?id=#1512): In Rebase Dialog, ask user to retry after failed "git checkout" and "git reset"
  * Fixed [issue #1330](https://code.google.com/p/tortoisegit/issues/detail?id=#1330): Preparing for git 1.7.12 new config file location
  * Fixed [issue #1515](https://code.google.com/p/tortoisegit/issues/detail?id=#1515): Allow Changed Files Dialog to revert selected files
  * Fixed [issue #1458](https://code.google.com/p/tortoisegit/issues/detail?id=#1458): Shell context menu shows "Commit submodule" if the selected folder is submodule root
  * Fixed [issue #1211](https://code.google.com/p/tortoisegit/issues/detail?id=#1211), [issue #1472](https://code.google.com/p/tortoisegit/issues/detail?id=#1472): Commit dialog can amend message only without affecting any files
  * Fixed [issue #1200](https://code.google.com/p/tortoisegit/issues/detail?id=#1200): Ignored folders can be destroyed by "git stash -u"
  * Fixed [issue #1508](https://code.google.com/p/tortoisegit/issues/detail?id=#1508): Indicate change type in Submodule Diff Dialog
  * Fixed [issue #1527](https://code.google.com/p/tortoisegit/issues/detail?id=#1527): Rebase Dialog shows Log menu button after rebasing if not launched from log dialog
  * Fixed [issue #1252](https://code.google.com/p/tortoisegit/issues/detail?id=#1252): wrap commit logs per git conventions (set tgit.logwidthmarker using git-config)
  * Added basic support for localized spellcheckers in commit dialog (see help file, keyword "spellchecker")
  * Fixed [issue #1531](https://code.google.com/p/tortoisegit/issues/detail?id=#1531): Clean up should show progress dialog

## Bug Fixes ##
  * Fixed [issue #1427](https://code.google.com/p/tortoisegit/issues/detail?id=#1427): Combine to one commit: Commit-window doesn't show changes from oldest commit
  * Fixed [issue #1443](https://code.google.com/p/tortoisegit/issues/detail?id=#1443): git svn dcommit: unclear behavior for dirty working tree
  * Fixed [issue #1457](https://code.google.com/p/tortoisegit/issues/detail?id=#1457): Confusing amend commit behaviour
  * Fixed [issue #1466](https://code.google.com/p/tortoisegit/issues/detail?id=#1466): Checkout Dialog always track remote branches
  * Fixed [issue #1396](https://code.google.com/p/tortoisegit/issues/detail?id=#1396): Sync Dialog Pull show wrong commit range in "In commits"
  * Fixed [issue #1465](https://code.google.com/p/tortoisegit/issues/detail?id=#1465): Clean up does not work with core.quotepath=true
  * Fixed [issue #1419](https://code.google.com/p/tortoisegit/issues/detail?id=#1419): Push window doesn't load PuTTY key when pushing to multiple remotes
  * Fixed [issue #1482](https://code.google.com/p/tortoisegit/issues/detail?id=#1482): Allow to show log of other branches if current HEAD points to an orphan branch
  * Fixed [issue #1487](https://code.google.com/p/tortoisegit/issues/detail?id=#1487): Do not use libgit in TortoiseShell for displaying HEAD commit (might set %GIT\_DIR% permanently)
  * Fixed [issue #1475](https://code.google.com/p/tortoisegit/issues/detail?id=#1475): Installer resets your SSH preference to ssh.exe when run silently
  * Fixed [issue #1470](https://code.google.com/p/tortoisegit/issues/detail?id=#1470): Log Dialog: Selected item not remembered after refresh if item is one of the first 100
  * Fixed [issue #1499](https://code.google.com/p/tortoisegit/issues/detail?id=#1499): Allow to show log if current HEAD and selected ref is orphan branch when show all branches checked
  * Fixed [issue #1507](https://code.google.com/p/tortoisegit/issues/detail?id=#1507): Submodule Diff Dialog should show dirty state only on working copy revision
  * Fixed [issue #1511](https://code.google.com/p/tortoisegit/issues/detail?id=#1511): Changed Files Dialog cannot show icons as folder for submodule
  * Fixed [issue #1516](https://code.google.com/p/tortoisegit/issues/detail?id=#1516): SVN clone strips trailing slashes
  * Fixed [issue #1486](https://code.google.com/p/tortoisegit/issues/detail?id=#1486): Rebase/Cherry-pick Dialog conflict list fail to refresh the status of resolved deleted file
  * Fixed [issue #1521](https://code.google.com/p/tortoisegit/issues/detail?id=#1521): Directories with period at beginning are recognized as file extensions showing `*`.dir
  * Fixed [issue #1519](https://code.google.com/p/tortoisegit/issues/detail?id=#1519): Quotes in notes break Merge command
  * Fixed [issue #1524](https://code.google.com/p/tortoisegit/issues/detail?id=#1524): Log dialog failed to view revision in alternative editor of the same file more than once
  * Fixed [issue #1459](https://code.google.com/p/tortoisegit/issues/detail?id=#1459): Refreshing Log Dialog may freeze up to 20 seconds
  * Fixed [issue #1523](https://code.google.com/p/tortoisegit/issues/detail?id=#1523): Bugtraq Number is checked for number only (inconsistent default value)

# Release 1.7.14.0 #
Released: 2012-10-14

## Features ##
  * Fixed [issue #1424](https://code.google.com/p/tortoisegit/issues/detail?id=#1424): Better Indicate submodule diff error
  * Fixed [issue #1425](https://code.google.com/p/tortoisegit/issues/detail?id=#1425): Indicate dirty state in Submodule Diff Dialog
  * Fixed [issue #1430](https://code.google.com/p/tortoisegit/issues/detail?id=#1430): Diff: allow multiple files unified diff
  * Fixed [issue #1453](https://code.google.com/p/tortoisegit/issues/detail?id=#1453): Allow Log List to copy multiple SHA-1 hashes
  * Fixed [issue #1454](https://code.google.com/p/tortoisegit/issues/detail?id=#1454): Show git progress time spent and end time in Progress Dialog and Sync Dialog
  * Fixed [issue #1434](https://code.google.com/p/tortoisegit/issues/detail?id=#1434): Easier to copy to file text to clipboard in TortoiseGitBlame

## Bug Fixes ##
  * Fixed [issue #1426](https://code.google.com/p/tortoisegit/issues/detail?id=#1426): Pull Dialog: Unknown option 'no-ff' when using no-tags
  * Fixed [issue #1423](https://code.google.com/p/tortoisegit/issues/detail?id=#1423): Update Dialog downloads the wrong language pack
  * Fixed [issue #1429](https://code.google.com/p/tortoisegit/issues/detail?id=#1429): Blame: copy sha to clipboard copies the log message
  * Fixed [issue #1439](https://code.google.com/p/tortoisegit/issues/detail?id=#1439): In Show log, long messages don't have the triple dots appended, when a Tag/Branch lable is visible
  * Fixed [issue #1444](https://code.google.com/p/tortoisegit/issues/detail?id=#1444): Cannot launch settings dialog from shell context menu when selecting a file
  * Fixed [issue #1265](https://code.google.com/p/tortoisegit/issues/detail?id=#1265): MSVC crashing unloading TortoiseGit32.dll (faulting module TortoiseGit32.dll\_unloaded)
  * Fixed [issue #772](https://code.google.com/p/tortoisegit/issues/detail?id=#772): Rebase may take extremely long time to open window

# Release 1.7.13.0 #
Released: 2012-09-30

## Features ##
  * Fixed [issue #1224](https://code.google.com/p/tortoisegit/issues/detail?id=#1224): Still can't delete a remote tag
  * Fixed [issue #366](https://code.google.com/p/tortoisegit/issues/detail?id=#366): Log - multiline search
  * Fixed [issue #696](https://code.google.com/p/tortoisegit/issues/detail?id=#696): Allow specifying execute bit
  * Fixed [issue #1335](https://code.google.com/p/tortoisegit/issues/detail?id=#1335): Available the branch edit description
  * Fixed [issue #494](https://code.google.com/p/tortoisegit/issues/detail?id=#494): Implement a commit button in the sync dialog
  * Fixed [issue #1333](https://code.google.com/p/tortoisegit/issues/detail?id=#1333): Added support for "update-index --skip-worktree"
  * Fixed [issue #1350](https://code.google.com/p/tortoisegit/issues/detail?id=#1350): Commit Dialog set focus to message editor after clicking amend checkbox
  * Fixed [issue #811](https://code.google.com/p/tortoisegit/issues/detail?id=#811): Log the history of a submodule not its contents
  * Fixed [issue #1344](https://code.google.com/p/tortoisegit/issues/detail?id=#1344): Log list add copy to clipboard only with commit message
  * Fixed [issue #1336](https://code.google.com/p/tortoisegit/issues/detail?id=#1336): Have visible the name of the branch in Repository Browser
  * Fixed [issue #1351](https://code.google.com/p/tortoisegit/issues/detail?id=#1351): Add Hotkey to (de)select all files and commit
  * Fixed [issue #1363](https://code.google.com/p/tortoisegit/issues/detail?id=#1363): copy email in the log window
  * Fixed [issue #1373](https://code.google.com/p/tortoisegit/issues/detail?id=#1373): The only available remote should be set on PUSH
  * Fixed [issue #1216](https://code.google.com/p/tortoisegit/issues/detail?id=#1216): Revamp update dialog
  * Fixed [issue #1381](https://code.google.com/p/tortoisegit/issues/detail?id=#1381): Sync Dialog log message add colored "success" or "git did not exit cleanly" at the end
  * Fixed [issue #1372](https://code.google.com/p/tortoisegit/issues/detail?id=#1372): Support git pull --no-tags

## Bug Fixes ##
  * Fixed [issue #1062](https://code.google.com/p/tortoisegit/issues/detail?id=#1062): Log window should refresh automatically after reset --hard
  * Fixed [issue #641](https://code.google.com/p/tortoisegit/issues/detail?id=#641): Failure trying to revert a "merge"
  * Fixed [issue #1338](https://code.google.com/p/tortoisegit/issues/detail?id=#1338): Assume Unchanged and Executable Bit checkboxes not show in TortoiseShell tab page on x86
  * Fixed [issue #1341](https://code.google.com/p/tortoisegit/issues/detail?id=#1341): Overlays missing in TotalCommander (x86) with TGitCache on x64
  * Fixed [issue #1355](https://code.google.com/p/tortoisegit/issues/detail?id=#1355): Added files are no-longer auto-checked for commit
  * Fixed [issue #1356](https://code.google.com/p/tortoisegit/issues/detail?id=#1356): File ignoring works not well with unicode filenames
  * Fixed [issue #1354](https://code.google.com/p/tortoisegit/issues/detail?id=#1354): Remote archive in push dialog not remembered, even if selected
  * Fixed [issue #1358](https://code.google.com/p/tortoisegit/issues/detail?id=#1358): Sync Dialog Pull cannot show updated ref labels in "In commits"
  * Disabled Direct2D by default for textboxes (in Commit Dialog, Patch Viewer, TortoiseGitBlame and TortoiseUDiff).
  * Fixed [issue #1362](https://code.google.com/p/tortoisegit/issues/detail?id=#1362): Merge Dialog cannot automatically select the annotated tag
  * Fixed [issue #1357](https://code.google.com/p/tortoisegit/issues/detail?id=#1357): Cannot add file in submodule
  * Fixed [issue #1343](https://code.google.com/p/tortoisegit/issues/detail?id=#1343): should not set SCI\_SETFONTQUALITY to SC\_EFF\_QUALITY\_LCD\_OPTIMIZED which bypasses user preference
  * Fixed [issue #1361](https://code.google.com/p/tortoisegit/issues/detail?id=#1361): git push: Entered source ref is ambiguous
  * Fixed [issue #1076](https://code.google.com/p/tortoisegit/issues/detail?id=#1076): Error trying to delete remote branch named 1.0.0
  * Fixed [issue #1375](https://code.google.com/p/tortoisegit/issues/detail?id=#1375): Wrong default action on dialog to delete references
  * Fixed [issue #1378](https://code.google.com/p/tortoisegit/issues/detail?id=#1378): Ignoring a file into info/exclude with seperate .git directory failed
  * Fixed [issue #1371](https://code.google.com/p/tortoisegit/issues/detail?id=#1371): Log window does not always remember column order correctly
  * Fixed [issue #1380](https://code.google.com/p/tortoisegit/issues/detail?id=#1380): When chosing Pull Remote Branch using Browse Reference the remote branch name won't get updated
  * Fixed [issue #1287](https://code.google.com/p/tortoisegit/issues/detail?id=#1287): Setting Remote URL not translated to '/' when clicking Apply or OK
  * Fixed [issue #1382](https://code.google.com/p/tortoisegit/issues/detail?id=#1382): Log messages with PGP signatures showing badly
  * Fixed [issue #1394](https://code.google.com/p/tortoisegit/issues/detail?id=#1394): Submodule Diff Dialog cannot jump to a commit that not belongs to current branch
  * Fixed [issue #1387](https://code.google.com/p/tortoisegit/issues/detail?id=#1387): Submodule Diff Dialog might display wrong submodule revision
  * Fixed [issue #1390](https://code.google.com/p/tortoisegit/issues/detail?id=#1390): TortoiseMerge cannot diff files after calling Export in Log Dialog
  * Fixed [issue #1395](https://code.google.com/p/tortoisegit/issues/detail?id=#1395): Problem restoring from earlier commit for file in a subdirectory
  * Fixed [issue #1392](https://code.google.com/p/tortoisegit/issues/detail?id=#1392): Window with rebase results is non-manageable via keyboard (no focus, can't press Done)
  * Fixed [issue #1405](https://code.google.com/p/tortoisegit/issues/detail?id=#1405): Cannot show branch description in Browse Reference Dialog with separate .git directory
  * Fixed [issue #1406](https://code.google.com/p/tortoisegit/issues/detail?id=#1406): Commit dialog cannot check MERGE\_HEAD with separate .git directory
  * Fixed [issue #861](https://code.google.com/p/tortoisegit/issues/detail?id=#861): TGitCache gets confused about file status (should detect touched file as unmodified)
> > TGitCache only checked timestamps of files in order to get their state since 1.7.0.
> > This fix makes TortoiseGit check the content of the files.
> > If you want to restore the old behavior, you can disable checking the contents via
> > the Settings dialog -> Advanced and set TGitCacheCheckContent to "false".
  * Fixed [issue #1300](https://code.google.com/p/tortoisegit/issues/detail?id=#1300): TortoiseProc LogDialog might crash if tortoisegit.index or tortoisegit.data is broken
  * Fixed [issue #1413](https://code.google.com/p/tortoisegit/issues/detail?id=#1413): Submodule Diff Dialog: show log button should be right-aligned
  * Fixed [issue #1418](https://code.google.com/p/tortoisegit/issues/detail?id=#1418): Submodule Diff Dialog labels disappeared

# Release 1.7.12.0 #
Released: 2012-08-10

## Features ##
  * Fixed [issue #238](https://code.google.com/p/tortoisegit/issues/detail?id=#238): submodule update should be recursive
  * Fixed [issue #1234](https://code.google.com/p/tortoisegit/issues/detail?id=#1234): Abbreviate renamings in the Log dialog as in the Commit Progress dialog
  * Fixed [issue #822](https://code.google.com/p/tortoisegit/issues/detail?id=#822): allow push to all remotes defined by checking a mark
  * Fixed [issue #1192](https://code.google.com/p/tortoisegit/issues/detail?id=#1192): fetch --all via dialog
  * Allow users to store pushremote and pushbranch on push dialog for local branches
  * Fixed [issue #1205](https://code.google.com/p/tortoisegit/issues/detail?id=#1205): Add "Last modified" column to commit dialog
  * Fixed [issue #1295](https://code.google.com/p/tortoisegit/issues/detail?id=#1295): Browse Ref Dialog ref name order consider numbers in string
  * Added unicode big-endian text file support to TortoiseMerge and TortoiseGitBlame
  * Fixed [issue #277](https://code.google.com/p/tortoisegit/issues/detail?id=#277): Add the ability to run the 'assume-unchanged' command
  * Fixed [issue #626](https://code.google.com/p/tortoisegit/issues/detail?id=#626): add "show log" in Git Sync dialog
  * Fixed [issue #884](https://code.google.com/p/tortoisegit/issues/detail?id=#884): Blame dialog Commit Info doesn't allow copy-paste
  * Fixed [issue #1165](https://code.google.com/p/tortoisegit/issues/detail?id=#1165): sort UI items alphabetically

## Bug Fixes ##
  * Fixed [issue #913](https://code.google.com/p/tortoisegit/issues/detail?id=#913): Merge does not cope with ambiguous tag and branch names
  * Fixed [issue #1266](https://code.google.com/p/tortoisegit/issues/detail?id=#1266): gitdll can cause stack overflow because of endless recursion in mark\_parents\_uninteresting (revision.c)
> > Upgraded gitdll and libgit to 1.7.11.1
  * Fixed [issue #1267](https://code.google.com/p/tortoisegit/issues/detail?id=#1267): Tortoisegit adding gitignore backslash instead of slash
  * Fixed [issue #1260](https://code.google.com/p/tortoisegit/issues/detail?id=#1260): TortoiseGit crashes if index is broken
  * Fixed [issue #1280](https://code.google.com/p/tortoisegit/issues/detail?id=#1280): TortoiseProc might crash after displaying libgit error
  * Fixed [issue #1235](https://code.google.com/p/tortoisegit/issues/detail?id=#1235): TortoiseGIT commit dialog freezes if index.lock file already exists
  * Fixed [issue #1283](https://code.google.com/p/tortoisegit/issues/detail?id=#1283): TortoiseProc might crash after LogDialog is closed
  * Fixed [issue #1282](https://code.google.com/p/tortoisegit/issues/detail?id=#1282): gitdll.dll might crash if a pack file is closed which is still in use
  * Fixed [issue #1290](https://code.google.com/p/tortoisegit/issues/detail?id=#1290): When pushing, 'remote' should default to the tracked archive, or empty
  * Optimized remembering of checked/unchecked files on the commit dialog
  * Fixed [issue #767](https://code.google.com/p/tortoisegit/issues/detail?id=#767): Default column widths in log commit file list are off
  * Fixed [issue #1294](https://code.google.com/p/tortoisegit/issues/detail?id=#1294): TortoiseGit might crash on concurrent access on CGitHeadFileList
  * Fixed [issue #1279](https://code.google.com/p/tortoisegit/issues/detail?id=#1279): Nothing seen in Repository Browser without config core.bare=false
  * Fixed [issue #1296](https://code.google.com/p/tortoisegit/issues/detail?id=#1296): Closing log dialog might cause crash
  * Fixed [issue #1255](https://code.google.com/p/tortoisegit/issues/detail?id=#1255): Adding non-versioned files from the commit dialog does not always work
  * Fixed [issue #620](https://code.google.com/p/tortoisegit/issues/detail?id=#620): Unmodified files appear in the Modified File list while committing
  * Fixed [issue #774](https://code.google.com/p/tortoisegit/issues/detail?id=#774): Revert does not work for submodules
  * Fixed [issue #1303](https://code.google.com/p/tortoisegit/issues/detail?id=#1303): Past Recent Message command in commit dialog doesn't work
  * Fixed [issue #1311](https://code.google.com/p/tortoisegit/issues/detail?id=#1311): Open With is broken
  * Fixed [issue #898](https://code.google.com/p/tortoisegit/issues/detail?id=#898): Committed everything even though I only selected one file
  * Fixed [issue #693](https://code.google.com/p/tortoisegit/issues/detail?id=#693): Ignoring `*`.`[`mime`]` in the commit window doesn't refresh file list
  * Fixed [issue #1318](https://code.google.com/p/tortoisegit/issues/detail?id=#1318): Higher dir combox box in format patch dialog
  * Fixed [issue #830](https://code.google.com/p/tortoisegit/issues/detail?id=#830): Renaming file with differences only in casing doesn't work
> > Added basic support only: the overlay status might be wrong (file shown as clean or modified instead of added)
  * Fixed [issue #867](https://code.google.com/p/tortoisegit/issues/detail?id=#867): Add should not run a new Git process for each file

# Release 1.7.11.3 #
Released: 2012-07-07

## Bug Fixes ##
  * Fixed [issue #1256](https://code.google.com/p/tortoisegit/issues/detail?id=#1256): TortoiseProc crashes on composing invalid ref error message
  * Fixed [issue #1254](https://code.google.com/p/tortoisegit/issues/detail?id=#1254): Adding file extensions to root .gitignore
  * Fixed [issue #1261](https://code.google.com/p/tortoisegit/issues/detail?id=#1261): gitdll.dll can crash if an already closed handle is closed again
  * Fixed [issue #1257](https://code.google.com/p/tortoisegit/issues/detail?id=#1257): HOME environment variable is not set up correctly on x86
  * Fixed [issue #1262](https://code.google.com/p/tortoisegit/issues/detail?id=#1262): TortoiseProc might crash if git.exe version is not parseable
  * Fixed [issue #1264](https://code.google.com/p/tortoisegit/issues/detail?id=#1264): TortoiseProc might crash if commands are executed w/o a working tree directory

# Release 1.7.11.0 #
Released: 2012-07-02

## Features ##
  * Push Dialog: Allow to enter SHA-1 or more complex refs as source ref
  * Fixed [issue #746](https://code.google.com/p/tortoisegit/issues/detail?id=#746): Make tortoisegit more gerrit friendly
  * Optimized TGitCache overlay calculation (deleted but kept files are now displayed as such)
  * Fixed [issue #1067](https://code.google.com/p/tortoisegit/issues/detail?id=#1067): Add clear button into "stash list"
  * Fixed [issue #1230](https://code.google.com/p/tortoisegit/issues/detail?id=#1230): Filter/Search for Branches in Reference Browser
  * Fixed [issue #1228](https://code.google.com/p/tortoisegit/issues/detail?id=#1228): Ignore by mask work recursively
  * Fixed [issue #1086](https://code.google.com/p/tortoisegit/issues/detail?id=#1086): Partial commit resets "Added" status on files omitted from checkin
  * Fixed [issue #1250](https://code.google.com/p/tortoisegit/issues/detail?id=#1250): Sync Dialog should reload remote combo box after clicking "Manage"
  * Fixed [issue #462](https://code.google.com/p/tortoisegit/issues/detail?id=#462): Implement 'All' and 'None' opportunities in the Set Extended menu settings dialog
  * TortoiseGit 1.7.11 comes with a new crash handler (crash-server.com) and lots of crash fixes (found using crash reports in our preview releases)

## Bug Fixes ##
  * Fixed [issue #1213](https://code.google.com/p/tortoisegit/issues/detail?id=#1213): cannot diff renamed files with Revision Diff Dialog
  * Fixed [issue #1215](https://code.google.com/p/tortoisegit/issues/detail?id=#1215): Branch name in the right click menu (for commit) does not support utf-8
  * Fixed [issue #652](https://code.google.com/p/tortoisegit/issues/detail?id=#652): "Clean up" should use recycle bin
  * Fixed [issue #1166](https://code.google.com/p/tortoisegit/issues/detail?id=#1166): Unreadable error message in TortoiseMerge
  * Fixed [issue #665](https://code.google.com/p/tortoisegit/issues/detail?id=#665): Problem with temporary file creation
  * Fixed [issue #1221](https://code.google.com/p/tortoisegit/issues/detail?id=#1221): Log Dialog revert files shows wrong number of files in message
  * Fixed [issue #1207](https://code.google.com/p/tortoisegit/issues/detail?id=#1207): TortoiseGit 1.7.10 crashes directly when trying to start
  * Fixed [issue #1226](https://code.google.com/p/tortoisegit/issues/detail?id=#1226): Show log crash when path contain some unicode symbols
  * Fixed [issue #1229](https://code.google.com/p/tortoisegit/issues/detail?id=#1229): Progress Window Gains Focus on Command Completion
  * Fixed [issue #1231](https://code.google.com/p/tortoisegit/issues/detail?id=#1231): incorrect behavior of squash in rebase/cherry pick
  * Fixed [issue #1233](https://code.google.com/p/tortoisegit/issues/detail?id=#1233): Could not go to annotated tag
  * Fixed [issue #947](https://code.google.com/p/tortoisegit/issues/detail?id=#947): The "Git check for modifications" form does not remember the setting for "Show unversioned files"
  * Fixed [issue #1093](https://code.google.com/p/tortoisegit/issues/detail?id=#1093): Directory incorrectly shown as changed (overlay icon)

# Release 1.7.10.0 #
Released: 2012-06-03

## Features ##
  * Updated shipped zlib library to version 1.2.7
  * Synced TortoiseIDiff with TortoiseSVN
  * Synced TortoiseUDiff with TortoiseSVN
  * Fixed [issue #1150](https://code.google.com/p/tortoisegit/issues/detail?id=#1150): Add support for ANSI Color Codes in log Outputs
  * Fixed [issue #969](https://code.google.com/p/tortoisegit/issues/detail?id=#969): Support for localization (you can download/create language packs for TortoiseGit, see http://redir.tortoisegit.org/translate)
  * Added Repository Browser
  * Updated shipped libgit2 to version 0.17.0
  * Fixed [issue #1169](https://code.google.com/p/tortoisegit/issues/detail?id=#1169): Show Branch for Commits
  * Fixed [issue #337](https://code.google.com/p/tortoisegit/issues/detail?id=#337): TortoiseGit Log doesn't apply --follow (added basic support for --follow)

## Bug Fixes ##
  * Fixed [issue #1162](https://code.google.com/p/tortoisegit/issues/detail?id=#1162): Sync dialog should use same font as progress dialog (use log font for both)
  * Fixed [issue #1174](https://code.google.com/p/tortoisegit/issues/detail?id=#1174): Clone Dialog incorrectly extracts name from URL that contains ".git" in the middle
  * Fixed [issue #1184](https://code.google.com/p/tortoisegit/issues/detail?id=#1184): diff of "Working dir changes" uses incorrect line endings (AutoCrLf=true)
  * Fixed [issue #1193](https://code.google.com/p/tortoisegit/issues/detail?id=#1193): Not properly handling submodule meta information (.git-file contains relative path)
  * Fixed [issue #1167](https://code.google.com/p/tortoisegit/issues/detail?id=#1167): TGitCache.exe crashes under Win7/64bit
  * Fixed [issue #1195](https://code.google.com/p/tortoisegit/issues/detail?id=#1195): Problems with tags containing non-ascii chars
  * Fixed [issue #1185](https://code.google.com/p/tortoisegit/issues/detail?id=#1185): In TortoiseGit log dialog info text, diff dialog and TortoiseGitBlame, git shows 7 chars of the hash by default (as git does)
  * Fixed [issue #1197](https://code.google.com/p/tortoisegit/issues/detail?id=#1197): Create branch: Alt+S doesn't mark "Switch to new branch"
  * Fixed [issue #1152](https://code.google.com/p/tortoisegit/issues/detail?id=#1152): Log-Dialog constantly crashes when diffing a file while loading
  * Fixed [issue #719](https://code.google.com/p/tortoisegit/issues/detail?id=#719): TortoiseGit is ignoring Global excludesfile for overlays
  * Fixed [issue #1199](https://code.google.com/p/tortoisegit/issues/detail?id=#1199): TortoiseGitBlame shows wrong revision history
  * Fixed [issue #1157](https://code.google.com/p/tortoisegit/issues/detail?id=#1157): Custom screen DPI causes wrong text size calculation

# Release 1.7.9.0 #
Released: 2012-05-05

## Features ##
  * Allow to fetch from log dialog
  * Fixed [issue #1058](https://code.google.com/p/tortoisegit/issues/detail?id=#1058): Allow to create tag after commit
  * Fixed [issue #101](https://code.google.com/p/tortoisegit/issues/detail?id=#101): UTF-8 support
> > This makes TortoiseGit msysgit 1.7.10 compatible. If you have non-ascii chars in filenames in your repository you should consider rewriting your history
> > (see https://github.com/kblees/git/wiki#wiki-Migrating_old_Git_for_Windows_repositories).
  * Added "prune/cleanup stale remote tracking branches" option to sync dialog

## Bug Fixes ##
  * Fixed [issue #1123](https://code.google.com/p/tortoisegit/issues/detail?id=#1123): Apply patch serial does not correctly add patches to list if >3 patches are selected
  * Fixed [issue #1061](https://code.google.com/p/tortoisegit/issues/detail?id=#1061): Enviroment variables ignored: GIT\_AUTHOR\_NAME and GIT\_AUTHOR\_EMAIL
  * Fixed [issue #1028](https://code.google.com/p/tortoisegit/issues/detail?id=#1028): overlays with separate-git-dir (e.g. .git\modules\... for submodules) not working
  * Fixed [issue #1131](https://code.google.com/p/tortoisegit/issues/detail?id=#1131): "Whole project" checkbox in commit dialog selects all files
  * Fixed [issue #1065](https://code.google.com/p/tortoisegit/issues/detail?id=#1065): Explorer crashes when rendering a file conflict icon
  * Fixed [issue #1027](https://code.google.com/p/tortoisegit/issues/detail?id=#1027): When post-receive hook contains more than 1 echo bash command, only the LAST echo is displayed in dialog
  * Fixed [issue #1136](https://code.google.com/p/tortoisegit/issues/detail?id=#1136): Proxy password with @ symbol not parsed/saved correctly
  * Fixed [issue #1135](https://code.google.com/p/tortoisegit/issues/detail?id=#1135): branch name does not get updated in show log
  * Fixed [issue #153](https://code.google.com/p/tortoisegit/issues/detail?id=#153): Empty error messagebox when starting rebase dialog
  * Fixed [issue #1140](https://code.google.com/p/tortoisegit/issues/detail?id=#1140): Settings page does not inherit msysgit system-wide config
  * Fixed [issue #1146](https://code.google.com/p/tortoisegit/issues/detail?id=#1146): Add hotkey for option "All Branches" in log dialog
  * Fixed [issue #1141](https://code.google.com/p/tortoisegit/issues/detail?id=#1141): Sync dialog local branch combo box too short
  * Fixed [issue #1130](https://code.google.com/p/tortoisegit/issues/detail?id=#1130): Sync dialog forgets the remote branch every time
  * Fixed [issue #1144](https://code.google.com/p/tortoisegit/issues/detail?id=#1144): Cancel button on commit dialog works very slow
  * Fixed [issue #1155](https://code.google.com/p/tortoisegit/issues/detail?id=#1155): TortoiseGit SVN rebase finish dialog produces very big dialog box

# Release 1.7.8.0 #
Released: 2012-04-01

## Features ##
  * Updated shipped zlib library to version 1.2.6
  * Updated shipped apr library to version 1.4.6
  * Updated shipped libgit2 to version 0.16.0
  * When deleting remote branch on log dialog one can also delete branch in remote repository now.
  * Fixed [issue #1103](https://code.google.com/p/tortoisegit/issues/detail?id=#1103): cherrypick option to indicate original commit
  * Fixed [issue #1094](https://code.google.com/p/tortoisegit/issues/detail?id=#1094): Support filter command line options for log
  * Fixed [issue #435](https://code.google.com/p/tortoisegit/issues/detail?id=#435) and [issue #1102](https://code.google.com/p/tortoisegit/issues/detail?id=#1102): Feature: "Save as patch" from Diff window

## Bug Fixes ##
  * Fixed [issue #1085](https://code.google.com/p/tortoisegit/issues/detail?id=#1085): Small commit with lots of unversioned and not ignored files takes very long
  * Fixed [issue #1098](https://code.google.com/p/tortoisegit/issues/detail?id=#1098): 'In ChangeList' is cleared when you click a table header
  * Fixed [issue #1073](https://code.google.com/p/tortoisegit/issues/detail?id=#1073): Correct default name in Switch/Checkout dialog
  * Fixed [issue #1110](https://code.google.com/p/tortoisegit/issues/detail?id=#1110): Tracking branches when you don't want to/incorrectly
  * Fixed [issue #1115](https://code.google.com/p/tortoisegit/issues/detail?id=#1115): Detached HEAD message has no cancel/abort option
  * Fixed [issue #1112](https://code.google.com/p/tortoisegit/issues/detail?id=#1112): Rebase corrupt commit message (ignores windows codepage and converts everything to utf-8)
  * Fixed [issue #985](https://code.google.com/p/tortoisegit/issues/detail?id=#985): Correctly store status for view patch in commit dialog
  * Fixed [issue #1116](https://code.google.com/p/tortoisegit/issues/detail?id=#1116): Make remote branch in pull dialog default to the current branch (or remote tracking branch)
  * Fixed [issue #1060](https://code.google.com/p/tortoisegit/issues/detail?id=#1060): tgit rebase process can get stuck
  * Fixed [issue #1107](https://code.google.com/p/tortoisegit/issues/detail?id=#1107): Wrong font used in MessageBoxes on Windows XP
  * Fixed [issue #1105](https://code.google.com/p/tortoisegit/issues/detail?id=#1105): Wrong status for missing files
  * Fixed some TortoiseMerge patch apply issues (includes [issue #1117](https://code.google.com/p/tortoisegit/issues/detail?id=#1117))
  * Fixed [issue #718](https://code.google.com/p/tortoisegit/issues/detail?id=#718): When pulling it should be possible to directly open the modifications window for editing conflicts
  * Fixed [issue #982](https://code.google.com/p/tortoisegit/issues/detail?id=#982): TortoiseGit messes up TortoiseSVN and TortoiseCVS menu icons on WinXP
  * Fixed [issue #1118](https://code.google.com/p/tortoisegit/issues/detail?id=#1118): Exporting from Changed Files dialog stops on checkout failure
  * Fixed [issue #1108](https://code.google.com/p/tortoisegit/issues/detail?id=#1108): Allow users to disable the "show unversioned files" messagebox in commit dialog

## Known Issue ##
  * separate-git-dir .git-directories do not work for overlays

# Release 1.7.7.0 #
Released: 2012-02-09

## Features ##
  * Fixed [issue #758](https://code.google.com/p/tortoisegit/issues/detail?id=#758): Make the log of a bare repository available
  * Fixed [issue #880](https://code.google.com/p/tortoisegit/issues/detail?id=#880): Allow sync / fetch / push on bare repository
  * Fixed [issue #818](https://code.google.com/p/tortoisegit/issues/detail?id=#818): SafeCRLF = warn should be available
  * Fixed [issue #855](https://code.google.com/p/tortoisegit/issues/detail?id=#855): moved up Git page in settings dialog
  * Fixed [issue #999](https://code.google.com/p/tortoisegit/issues/detail?id=#999): Added "Diff submodule" dialog
  * Fixed [issue #1019](https://code.google.com/p/tortoisegit/issues/detail?id=#1019): better indicate errors to user on progress dialog
  * Added "Show Log before rename/copy" on log dialog file list
  * Added basic support for separate-git-dir (Overlays are not working yet)
  * Fixed [issue #1042](https://code.google.com/p/tortoisegit/issues/detail?id=#1042): Allow to delete branch after successful merge
  * Fixed [issue #1040](https://code.google.com/p/tortoisegit/issues/detail?id=#1040): Commit to new branch
  * Fixed [issue #1043](https://code.google.com/p/tortoisegit/issues/detail?id=#1043): Add 'Stash' to 'Working dir changes' context menu in log dialog
  * Added support for Windows 7 libraries
  * Fixed [issue #222](https://code.google.com/p/tortoisegit/issues/detail?id=#222): support partially committing a file

## Bug Fixes ##
  * Updated shipped PuTTY binaries to version 0.62
  * Fixed [issue #1000](https://code.google.com/p/tortoisegit/issues/detail?id=#1000): Git commit doesn't work
  * Fixed [issue #587](https://code.google.com/p/tortoisegit/issues/detail?id=#587): Log entries with tag/branch/head marker don't highlight correctly
  * Fixed [issue #1004](https://code.google.com/p/tortoisegit/issues/detail?id=#1004): git svn fetch/rebase/clone return an error for ssh authorization
  * Reenabled --topo-order for log. Users who do not want this, can disable it on settings dialog
  * Fixed [issue #1024](https://code.google.com/p/tortoisegit/issues/detail?id=#1024): commit freezes after click on ok with a lot of files
  * Fixed [issue #1026](https://code.google.com/p/tortoisegit/issues/detail?id=#1026): Cannot configure (and autoload) putty key for submodules with new mSysGit.
  * Fixed [issue #849](https://code.google.com/p/tortoisegit/issues/detail?id=#849): Searching in log breaks graph/branch-line
  * Fixed [issue #1030](https://code.google.com/p/tortoisegit/issues/detail?id=#1030): Does not close handle after export to zip
  * Fixed [issue #1025](https://code.google.com/p/tortoisegit/issues/detail?id=#1025): branch is not recognized correctly with separate-git-dir
  * Fixed [issue #1022](https://code.google.com/p/tortoisegit/issues/detail?id=#1022): Cannot add files to submodules with-separate-git-dir
  * Fixed [issue #1008](https://code.google.com/p/tortoisegit/issues/detail?id=#1008): Bug Id not displayed in Log Messages (multiline comment)
  * Fixed [issue #1020](https://code.google.com/p/tortoisegit/issues/detail?id=#1020): Incorrect Overlays on large repos (> 2 GiB), upgraded libgit2
  * Fixed [issue #607](https://code.google.com/p/tortoisegit/issues/detail?id=#607) and [issue #1005](https://code.google.com/p/tortoisegit/issues/detail?id=#1005): Tortoisegit overlay icons are not correctly shown for new create local repo
  * Fixed [issue #1051](https://code.google.com/p/tortoisegit/issues/detail?id=#1051): Adding files using the add files dialog doesn't normalize line endings
  * Fixed [issue #582](https://code.google.com/p/tortoisegit/issues/detail?id=#582), [issue #956](https://code.google.com/p/tortoisegit/issues/detail?id=#956), [issue #960](https://code.google.com/p/tortoisegit/issues/detail?id=#960), [issue #973](https://code.google.com/p/tortoisegit/issues/detail?id=#973), [issue #980](https://code.google.com/p/tortoisegit/issues/detail?id=#980), [issue #959](https://code.google.com/p/tortoisegit/issues/detail?id=#959) and [issue #1016](https://code.google.com/p/tortoisegit/issues/detail?id=#1016): 100% CPU, icons blinking and refreshing bugs in TGitCache
  * Fixed [issue #1044](https://code.google.com/p/tortoisegit/issues/detail?id=#1044): Add file to index with special character (ei – "dash") or accent fail without any message

## Known Issue ##
  * separate-git-dir .git-directories do not work for overlays

# Release 1.7.6.0 #
Released: 2011-12-10

## Features ##
  * Fixed [issue #972](https://code.google.com/p/tortoisegit/issues/detail?id=#972): Add "fast forward only" checkbox in pull dialog
  * Fixed [issue #976](https://code.google.com/p/tortoisegit/issues/detail?id=#976): Compare Revisions should inherit path filter
  * Fixed [issue #869](https://code.google.com/p/tortoisegit/issues/detail?id=#869): TortoiseProc CloneCommand is ignoring "url" command line parameter
  * Fixed [issue #820](https://code.google.com/p/tortoisegit/issues/detail?id=#820): Missing menu item for "git svn fetch"
  * Fixed [issue #792](https://code.google.com/p/tortoisegit/issues/detail?id=#792): Fetch progress window should have a "Log" button
  * Fixed [issue #451](https://code.google.com/p/tortoisegit/issues/detail?id=#451): rebase (maybe be for any conflicts) select multiple files to mark
  * Fixed [issue #894](https://code.google.com/p/tortoisegit/issues/detail?id=#894): Make images "open with" TortoiseIDiff
  * Fixed [issue #985](https://code.google.com/p/tortoisegit/issues/detail?id=#985): Store status for view patch in commit dialog
  * Fixed [issue #977](https://code.google.com/p/tortoisegit/issues/detail?id=#977): Fetch does not have an option to fetch tags
  * Fixed [issue #801](https://code.google.com/p/tortoisegit/issues/detail?id=#801): Be able to enter a custom stash message
  * Fixed [issue #933](https://code.google.com/p/tortoisegit/issues/detail?id=#933): implement git stash --include-untracked
  * Fixed [issue #987](https://code.google.com/p/tortoisegit/issues/detail?id=#987): Add Stash save/pop to "Working Dir Changes" dialog
  * Fixed [issue #988](https://code.google.com/p/tortoisegit/issues/detail?id=#988): Stash pop/apply fail should have a button for viewing conflicts
  * Fixed [issue #676](https://code.google.com/p/tortoisegit/issues/detail?id=#676): Add remove remote tag ability
  * Fixed [issue #678](https://code.google.com/p/tortoisegit/issues/detail?id=#678): TortoiseGitBlame log incomplete (integrated --follow into TortoiseGitBlame)

## Bug Fixes ##
  * Fixed [issue #747](https://code.google.com/p/tortoisegit/issues/detail?id=#747): TortoiseProc & less process not closing
  * Fixed [issue #808](https://code.google.com/p/tortoisegit/issues/detail?id=#808): Less: file viewer stop work when use show-low
  * Fixed [issue #931](https://code.google.com/p/tortoisegit/issues/detail?id=#931), [issue #934](https://code.google.com/p/tortoisegit/issues/detail?id=#934) and [issue #948](https://code.google.com/p/tortoisegit/issues/detail?id=#948): TortoiseProc crashes when repo contains huge files (on x86)
> > Upgraded gitdll, libgit and tgit.exe to 1.7.7.2
  * Fixed [issue #936](https://code.google.com/p/tortoisegit/issues/detail?id=#936): Applying a stash from the list fails
  * Fixed [issue #962](https://code.google.com/p/tortoisegit/issues/detail?id=#962): git\_init in gitdll.c uses USERPROFILE for creating home
  * Fixed [issue #964](https://code.google.com/p/tortoisegit/issues/detail?id=#964): Can't mark conflict as resolved
  * Fixed [issue #867](https://code.google.com/p/tortoisegit/issues/detail?id=#867): Add should not run a new Git process for each file
  * Fixed [issue #981](https://code.google.com/p/tortoisegit/issues/detail?id=#981): After Aborting a Rebase a different Commit is checked out
  * Fixed [issue #670](https://code.google.com/p/tortoisegit/issues/detail?id=#670): Cannot delete/apply individual stash entries
  * Fixed [issue #863](https://code.google.com/p/tortoisegit/issues/detail?id=#863): Commit and revert gets stuck on repositories with mixed line-endings
  * Fixed [issue #378](https://code.google.com/p/tortoisegit/issues/detail?id=#378): CRLF/LF conversion causes commit dialog to freeze
  * Fixed [issue #858](https://code.google.com/p/tortoisegit/issues/detail?id=#858): Tortoise Git Client crash when showing the log dialog
  * Fixed [issue #920](https://code.google.com/p/tortoisegit/issues/detail?id=#920): TortoiseGitBlame and UTF-16 LE
  * updated documentation
  * Fixed [issue #994](https://code.google.com/p/tortoisegit/issues/detail?id=#994): Git clone from SVN - Depth field is useless
  * Fixed [issue #996](https://code.google.com/p/tortoisegit/issues/detail?id=#996): Compare with Working Copy error on renamed files

# Release 1.7.5.0 #
Released: 2011-11-09

## Features ##
  * Fixed [issue #260](https://code.google.com/p/tortoisegit/issues/detail?id=#260): Added support for bisect
  * Fixed [issue #916](https://code.google.com/p/tortoisegit/issues/detail?id=#916): Fixed wrong contextmenu icon display position with installed TSVN 1.7
  * Add new command to diff two selected files in the CGitStatusListCtrl.

## Bug Fixes ##
  * Fixed [issue #931](https://code.google.com/p/tortoisegit/issues/detail?id=#931): TGitCache: Missing NULL check
  * Fixed [issue #935](https://code.google.com/p/tortoisegit/issues/detail?id=#935): TortoiseMerge removes newlines at file end
  * Fixed [issue #931](https://code.google.com/p/tortoisegit/issues/detail?id=#931): libgit2 had problems with big pack files
  * Fixed [issue #486](https://code.google.com/p/tortoisegit/issues/detail?id=#486): Resolving conflicts can result in nothing to commit and branch merge not concluded
  * Fixed [issue #938](https://code.google.com/p/tortoisegit/issues/detail?id=#938): **Backlash** between user name and domain name is incorrectly replaced by **Slash**
  * Fixed [issue #941](https://code.google.com/p/tortoisegit/issues/detail?id=#941): Performing diff on an unchanged file behaves like a diff with an added file
  * Fixed [issue #928](https://code.google.com/p/tortoisegit/issues/detail?id=#928): Mark diff-tempfiles as read-only
  * Fixed [issue #951](https://code.google.com/p/tortoisegit/issues/detail?id=#951): Alt+S conflict for sign and set date
  * Fixed [issue #949](https://code.google.com/p/tortoisegit/issues/detail?id=#949): TortoiseMerge does not allow copying to the clipboard via Ctrl+Insert
  * Fixed [issue #950](https://code.google.com/p/tortoisegit/issues/detail?id=#950): avoid possible crash if .git/packed-refs contains annotated tags
  * Fixed [issue #915](https://code.google.com/p/tortoisegit/issues/detail?id=#915): TortoiseProc memory corruption on empty repo
  * Fixed [issue #959](https://code.google.com/p/tortoisegit/issues/detail?id=#959): Overlay icons are not updated immediately

# Release 1.7.4.0 #
Released: 2011-10-10

## Features ##
  * Add Show Environment variables at setting dialog to help debug user problem.
  * Allow users to be warned if there is no Signed-Off-By line in a commit message
  * Fixed [issue #375](https://code.google.com/p/tortoisegit/issues/detail?id=#375): Implement --date/time option gui interface in the commit dialog
  * Fixed [issue #814](https://code.google.com/p/tortoisegit/issues/detail?id=#814): Remember last selected commit/line on log filtering
  * Allow to "Update submodules" after pull or hard reset
  * Fixed [issue #780](https://code.google.com/p/tortoisegit/issues/detail?id=#780): "Merge to `[`branch`]`..." should pre-select the chosen commit's branch or tag name
  * Fixed [issue #459](https://code.google.com/p/tortoisegit/issues/detail?id=#459): Implement more talkative name than just 'Revert fail'

## Bug Fixes ##
  * Fixed [issue #899](https://code.google.com/p/tortoisegit/issues/detail?id=#899): Push via Showlog  use Push with force option
  * Fixed [issue #893](https://code.google.com/p/tortoisegit/issues/detail?id=#893): "Show Unified Diff" on file entry in "show log" has changes backwards
  * Fixed [issue #881](https://code.google.com/p/tortoisegit/issues/detail?id=#881): "Create repository here" should warn if target directory is not empty
  * Fix wrong contextmenu icon display position when install TSVN 1.7 on WinXP
  * TGitCache: Fix sometime project root show as unversioned icon
  * Fixed [issue #862](https://code.google.com/p/tortoisegit/issues/detail?id=#862) and [issue #870](https://code.google.com/p/tortoisegit/issues/detail?id=#870): TGitCache: Fix sometime show "+" at tracked items
  * Upgraded libgit2 to 0.15.0
  * Fixed [issue #716](https://code.google.com/p/tortoisegit/issues/detail?id=#716): Aborted clone leaves git process running
  * Fixed [issue #787](https://code.google.com/p/tortoisegit/issues/detail?id=#787): Problem of setting proxy for work using HTTPS
  * Fixed [issue #908](https://code.google.com/p/tortoisegit/issues/detail?id=#908): TortoiseGit crashes if .git/config-file is broken
  * Fixed [issue #909](https://code.google.com/p/tortoisegit/issues/detail?id=#909): Cannot amend initial commit
  * Fixed [issue #829](https://code.google.com/p/tortoisegit/issues/detail?id=#829): "Remote" combobox in "Push" window updates only after losing focus
  * Fixed [issue #906](https://code.google.com/p/tortoisegit/issues/detail?id=#906): Add ability to add files with options -force.
  * Fixed [issue #914](https://code.google.com/p/tortoisegit/issues/detail?id=#914): unifiled diff always show wrong changes (base files compare with new files)
  * Fixed [issue #673](https://code.google.com/p/tortoisegit/issues/detail?id=#673): Applying a patch does not honour CRLF in files
  * Fixed [issue #713](https://code.google.com/p/tortoisegit/issues/detail?id=#713): apply serial patch window need to improve
  * Fixed [issue #922](https://code.google.com/p/tortoisegit/issues/detail?id=#922): Settings / Git / Config / Edit global .gitconfig uses wrong path

# Release 1.7.3.0 #
Released: 2011-08-24

## Features ##
  * Fixed [issue #872](https://code.google.com/p/tortoisegit/issues/detail?id=#872): 32 shell extension should be made optional on x64 installation

## Bug Fixes ##
  * Fixed [issue #833](https://code.google.com/p/tortoisegit/issues/detail?id=#833): Password with Percent (%) is not accepted
  * Fixed [issue #852](https://code.google.com/p/tortoisegit/issues/detail?id=#852): Incorrect current version string in Check For Updates dialog on x86
  * Fixed [issue #850](https://code.google.com/p/tortoisegit/issues/detail?id=#850): 32bit application can't show icon overlay at 64bit system.
  * Fixed [issue #864](https://code.google.com/p/tortoisegit/issues/detail?id=#864): Show log crashes when commit with "encoding" in comment exists
  * Fixed [issue #851](https://code.google.com/p/tortoisegit/issues/detail?id=#851): Windows Explorer Shell Crashed when empty repository
  * Fixed open handles in TGitCache
> > Fixed [issue #497](https://code.google.com/p/tortoisegit/issues/detail?id=#497), [issue #623](https://code.google.com/p/tortoisegit/issues/detail?id=#623) and [issue #892](https://code.google.com/p/tortoisegit/issues/detail?id=#892): TortoiseGit locks repository folders so that the user can't delete them
  * Fixed [issue #870](https://code.google.com/p/tortoisegit/issues/detail?id=#870): Wrong overlay icons
  * Fixed [issue #793](https://code.google.com/p/tortoisegit/issues/detail?id=#793): Context menu for files does not contain "Add to ignore list"
  * Fixed [issue #860](https://code.google.com/p/tortoisegit/issues/detail?id=#860): Commit file moves does not properly remove the source file
  * Fixed [issue #386](https://code.google.com/p/tortoisegit/issues/detail?id=#386): Commit dialog does not preserve selection when toggling "Whole project"

# Release 1.7.2.0 #
Released: 2011-08-08

## Features ##
  * Added shortcuts to the Windows 7 taskbar jumplist
  * Allow to clone recursively
  * Fixed [issue #841](https://code.google.com/p/tortoisegit/issues/detail?id=#841): Pull dialog should have "no fast-forward" option like the merge dialog

## Bug Fixes ##
  * Fixed blame crash at XP system.
  * Upgraded TortoisePlink to TortoiseSVN rev. 21694, fixes a bug with shipped Pageant under x64
  * Updated shipped apr library to version 1.4.5
  * Updated shipped apr-util library to version 1.3.12
  * Updated shipped zlib library to version 1.2.5
  * Fixed [issue #783](https://code.google.com/p/tortoisegit/issues/detail?id=#783): Git Command Progress window should close with Escape
  * Fixed [issue #499](https://code.google.com/p/tortoisegit/issues/detail?id=#499): Git Command Progress window does not close from X-closebutton
  * Fixed [issue #844](https://code.google.com/p/tortoisegit/issues/detail?id=#844): Git Command Progress window, "Writing Objects" , progress info refresh with glitches.

# Release 1.7.1.0 #
Released: 2011-07-29 (internal release)

## Features ##
  * Fixed [issue #828](https://code.google.com/p/tortoisegit/issues/detail?id=#828): disable the commit button if there's no comment entered

## Bug Fixes ##
  * Fixed [issue #796](https://code.google.com/p/tortoisegit/issues/detail?id=#796): plz add code page name "cp949"
  * Fixed [issue #795](https://code.google.com/p/tortoisegit/issues/detail?id=#795): Switch/Checkout Dialog, "Switch To Version" is confusing
  * Fixed [issue #757](https://code.google.com/p/tortoisegit/issues/detail?id=#757): TortoiseGit Blame not working from working dir with autocrlf-enabled.
  * Fixed [issue #691](https://code.google.com/p/tortoisegit/issues/detail?id=#691): 64-bit version should include the 32-bit shell extension too
  * Updated shipped PuTTY binaries to version 0.61
  * Updated shipped notepad2 binaries to version 4.2.25 and added x64 version
  * Updated shipped TortoiseOverlay to version 1.1.3.21564
  * Fix crash for init repository
  * Fixed [issue #799](https://code.google.com/p/tortoisegit/issues/detail?id=#799): Explore crash with empty directory
  * Fixed [issue #816](https://code.google.com/p/tortoisegit/issues/detail?id=#816): Output in Git Command Progress is broken

# Release 1.7.0.0 #
Released: 2011-05-11

## Features ##
  * Fixed [issue #724](https://code.google.com/p/tortoisegit/issues/detail?id=#724): BrowseRefs: Made branch renaming possible.
  * Use fetch-dialog for "Fetch" in BrowseRefs
  * Allow to edit user signingkey in TortoiseGit->Settings->GitConfig
  * Allow to sign tags (requires GPG and a key without passphrase)
  * Allow to enter CC recipients with MAPI
  * Do not add Signed-off-by if already included
  * Do not add another empty line if there are already some Reviewed-by or Signed-off-by lines at the end of the commit message on signing.
  * Allow to start push dialog from log
  * Show changes to revision before the last commit on amend and perform actions relatively to this revision (old behavior is still possible)
  * Remember (de)selected files in "Commit dialog" after refreshing or ordering the list
  * Fixed [issue #745](https://code.google.com/p/tortoisegit/issues/detail?id=#745): Added checkbox to commit dialog to disable autoselection of submodules
  * Show status on taskbar button on Windows 7
  * Allow to add a "Signed-Off-By" line to patches on applying
  * Fixed [issue #781](https://code.google.com/p/tortoisegit/issues/detail?id=#781): Allow to push all branches at once
  * Fixed [issue #784](https://code.google.com/p/tortoisegit/issues/detail?id=#784): Rebase window should allow easier selection of Pick/Squash/Edit/Skip (keys: space: shifts the state, s: skip, e: edit, p: pick, q: squash)
  * Fixed [issue #785](https://code.google.com/p/tortoisegit/issues/detail?id=#785): Rebase window should list the contents of a commit just like Log window does
  * Fixed [issue #768](https://code.google.com/p/tortoisegit/issues/detail?id=#768): Display modified files in "Reset" dialog

## Bug Fixes ##
  * Fixed tab indices (activation order)
  * Fixed missing putty-key for deleting a remote branch
  * Fixed [issue #728](https://code.google.com/p/tortoisegit/issues/detail?id=#728): Shell "Diff With Previous" doesn't work when there are more than 2 revisions for that file and diff working copy to HEAD~1
  * Fixed 32/64-bit MAPI inconsistency-issues
  * Do not include patch in mail if user selected attachment
  * Fix attaching of patches to mails with some MAPI clients
  * Fixed sending patches combined in one mail w/o attachments (files were always attached)
  * Make change setting "hide TGit menu" work
  * Fixed [issue #729](https://code.google.com/p/tortoisegit/issues/detail?id=#729): SVN DCommitt incorrectly executes with --rmdir
  * Fixed [issue #732](https://code.google.com/p/tortoisegit/issues/detail?id=#732): Synch-dialog layout broken
  * Fixed [issue #734](https://code.google.com/p/tortoisegit/issues/detail?id=#734): git not found: Fixed possible problems with folders containing spaces
  * Fixed [issue #735](https://code.google.com/p/tortoisegit/issues/detail?id=#735): Log generates file stats from shown parent instead of actual parent
  * Do not show "Diff with previous" for added files
  * Fixed [issue #737](https://code.google.com/p/tortoisegit/issues/detail?id=#737): Diffing of added files does not work with Shell
  * Fixed [issue #738](https://code.google.com/p/tortoisegit/issues/detail?id=#738): Lost the commit id on file name when use a external diff tool
  * Fixed [issue #714](https://code.google.com/p/tortoisegit/issues/detail?id=#714): add "FETCH\_HEAD" to reference drop down list
  * Fixed [issue #548](https://code.google.com/p/tortoisegit/issues/detail?id=#548):  tortoisegit use incorrect case sensitive comparison
  * Fixed [issue #727](https://code.google.com/p/tortoisegit/issues/detail?id=#727): /CloseOnEnd not working for commit
  * Fixed [issue #754](https://code.google.com/p/tortoisegit/issues/detail?id=#754): Allow to show log for files in "Changes files" dialog
  * Fixed [issue #749](https://code.google.com/p/tortoisegit/issues/detail?id=#749): Ask before delete files.
  * Fixed [issue #125](https://code.google.com/p/tortoisegit/issues/detail?id=#125): Export files from revision or range of revisions in "Changes files" dialog.
  * Fixed [issue #512](https://code.google.com/p/tortoisegit/issues/detail?id=#512): Git sync lose local commits (remote update, fetch and rebase)
  * Fixed [issue #766](https://code.google.com/p/tortoisegit/issues/detail?id=#766): "Switch/Checkout" dialog: "Track" should be disabled when no new branch is created
  * Fixed [issue #765](https://code.google.com/p/tortoisegit/issues/detail?id=#765): "Check for Updates" in about box doesn't work
  * Fixed [issue #731](https://code.google.com/p/tortoisegit/issues/detail?id=#731): Git Command Progress Window text box doesn't have a context menu.
  * Rebase failed at revision with empty commit message.
  * Fixed sorting of columns of file lists (e.g. commit dialog).
  * Fixed [issue #757](https://code.google.com/p/tortoisegit/issues/detail?id=#757): TortoiseGit Blame not working from working dir.
  * Fixed layout issues with Windows 7 Aero
  * TortoiseProc.exe sometimes didn't exit correctly after closing the log dialog
  * Fixed [issue #761](https://code.google.com/p/tortoisegit/issues/detail?id=#761): Settings should correctly deal with backslashes (windows path separators) in entered remote URLs
  * Patch Viewer might display no horizontal scrollbar
  * Fixed [issue #779](https://code.google.com/p/tortoisegit/issues/detail?id=#779): Show correct text in taskbar when rebasing finished.
  * Pushing required a remote-branch name
  * Fixed [issue #790](https://code.google.com/p/tortoisegit/issues/detail?id=#790): Add minimize button to progress window
  * Fixed some optical issues in Rebase-Dialog
  * Fixed [issue #791](https://code.google.com/p/tortoisegit/issues/detail?id=#791): /CloseOnEnd not working for switch
  * TortoiseGitCache
> > Partly rewritten to fix various issues.
  * Fixed [issue #415](https://code.google.com/p/tortoisegit/issues/detail?id=#415): Fix the Settings/General/Context menu/Apply operation (missing LF trimming)

# Release 1.6.5.0 #
Released: 2011-02-20

## Bug Fixes ##
  * Fixed [issue #715](https://code.google.com/p/tortoisegit/issues/detail?id=#715): Unable to show log when there are old version cache file
  * Fixed [issue #611](https://code.google.com/p/tortoisegit/issues/detail?id=#611): Add "copy all information" to "Changed Files" dialog
  * Fixed new file miss when combine commits at log dialog
  * Fixed [issue #720](https://code.google.com/p/tortoisegit/issues/detail?id=#720): Infinite loop at search in Show Log when there are notes

# Release 1.6.4.0 #
Released: 2011-02-14

## Features ##
  * Significantly Improve Log fetch speed for big repository
> > Fetch modified file list asynchronous.
> > Time filter (From, to) use git built-in --max-age and --min-age.
> > Text filter use git grep.
> > Fixed [issue #590](https://code.google.com/p/tortoisegit/issues/detail?id=#590): wasteful use of memory with very large repository
> > Fixed [issue #531](https://code.google.com/p/tortoisegit/issues/detail?id=#531): Git synchronization UI opened so slowly
> > Fixed [issue #541](https://code.google.com/p/tortoisegit/issues/detail?id=#541): show log is extremely slow
> > Fixed [issue #364](https://code.google.com/p/tortoisegit/issues/detail?id=#364): Log - hot key for "browse refs" dialog

  * Improve TortoisePLink 3x transfer perfomance
> > Update TortoisePlink to plink 9078

  * Implemented [issue #664](https://code.google.com/p/tortoisegit/issues/detail?id=#664): Warn when committing to detached HEAD
  * The context menu can be hidden completely for unversioned items ([issue 674](https://code.google.com/p/tortoisegit/issues/detail?id=674))
  * Only show DCommit type dialog if "svn.rmdir" is unset
  * Optionally remember DCommit type setting
  * enable git status column in TortoiseShell
  * Fixed [issue #644](https://code.google.com/p/tortoisegit/issues/detail?id=#644): Dropped "Check repository" button on check for modifications dialog
  * Allow to diff two revisions of a file by calling TortoiseProc
  * Fixed [issue #480](https://code.google.com/p/tortoisegit/issues/detail?id=#480): Implement text copying opportunities in the dialogs
  * Allow to change EOL by pressing CTRL+Return in TortoiseMerge
  * Allow to replace (previously hardcoded) Notepad2 by any other editor
  * Optionally send/mail patches via MAPI, if a default mail client is set up
  * Fixed [issue #248](https://code.google.com/p/tortoisegit/issues/detail?id=#248): Allow to reorder commits on rebase
  * Fixed [issue #702](https://code.google.com/p/tortoisegit/issues/detail?id=#702): Added request-pull functionality

  * TortoiseGitBlame
> > Clicking on a line automatically selects the log entry in the loglist
> > Allow to diff to previous revision of a file
> > Added new context menu
> > Allow to toggle author column

## Bug Fixes ##
  * Fixed [issue #669](https://code.google.com/p/tortoisegit/issues/detail?id=#669): cannot open help from clean window
  * Fixed [issue #671](https://code.google.com/p/tortoisegit/issues/detail?id=#671): Help not working when choose switch dialog and dcommit dialog
  * Fixed [issue #690](https://code.google.com/p/tortoisegit/issues/detail?id=#690): Superfluous line in displayed commit message
  * Do not allow to delete-ignore working copy root-directory
  * Starting TortoiseGitBlame might fail to start if folder contains spaces
  * Fixed window titles of log and statistics window
  * Fixed [issue #697](https://code.google.com/p/tortoisegit/issues/detail?id=#697): /CloseOnEnd was not working, fixed for fetch&pull

  * Fixed issues with the send mail dialog
> > If all three attempts failed, do not show success
> > If all three attempts failed, do not go on sending more patches
> > Correctly show retries
> > Interpret user cancel as failure

  * TortoiseGitBlame
> > Fixed [issue #448](https://code.google.com/p/tortoisegit/issues/detail?id=#448): Disable personalized menu behaviour
> > After blaming an older revision, TortoiseGitBlame was fixed to this.

  * Fixed [issue #704](https://code.google.com/p/tortoisegit/issues/detail?id=#704): cannot open help from diff from previous, browse refs
  * Fixed [issue #694](https://code.google.com/p/tortoisegit/issues/detail?id=#694): "Clean Up" executes on top level directory
  * Fixed [issue #680](https://code.google.com/p/tortoisegit/issues/detail?id=#680): StatGraphDlg.cpp min-avg statistics are incorrect
  * Fixed [issue #705](https://code.google.com/p/tortoisegit/issues/detail?id=#705): Fixed comparing added/deleted files on diffing whole revisions
  * Improved "Combine commits" process (prevents possible loss of data)

# Release 1.6.3.0 #
Released: 2011-01-14

## Features ##
  * Improved log dialog
> > Fixed [issue #662](https://code.google.com/p/tortoisegit/issues/detail?id=#662): Allow to filter for paths
> > Added hash column
> > Show BugID when user config bugtraq.logregex

  * Improved commit dialog
> > Removed useless options from the contextmenu (e.g. file operations for directories/submodules)
> > allow to ignore deleted or unversioned files

  * Improved changed files dialog
> > Removed useless options from the contextmenu (e.g. file operations for directories/submodules)
> > Fixed [issue #618](https://code.google.com/p/tortoisegit/issues/detail?id=#618): Added a commit button
> > allow to ignore deleted or unversioned files

  * Rewrite patch import dialog
> > Patch import dialog look like sync dialog.
> > User can know which patch fail import easily.
> > Show patch import progress.
> > Add 3way and ignore space option.
> > Fix many issues about patch import dialog ([issue #252](https://code.google.com/p/tortoisegit/issues/detail?id=#252), [issue #324](https://code.google.com/p/tortoisegit/issues/detail?id=#324), [issue #332](https://code.google.com/p/tortoisegit/issues/detail?id=#332) and [issue #430](https://code.google.com/p/tortoisegit/issues/detail?id=#430))

  * Include version information for all executables

  * Improved TortoiseBlame
> > Fixed [issue #490](https://code.google.com/p/tortoisegit/issues/detail?id=#490) and [issue #436](https://code.google.com/p/tortoisegit/issues/detail?id=#436): Allow to blame older revisions in TortoiseGitBlame
> > Removed useless options from the contextmenu (e.g. compare to working copy)
> > Fixed [issue #658](https://code.google.com/p/tortoisegit/issues/detail?id=#658): Added author column

  * Fixed [issue #323](https://code.google.com/p/tortoisegit/issues/detail?id=#323): implement DCommit type

  * ask user if he wants to stash pop after "SVN fetch"

  * allow to override branch on switch/checkout dialog

  * allow to prune on fetch

  * allow to edit global and local .gitconfig

  * Fixed [issue #655](https://code.google.com/p/tortoisegit/issues/detail?id=#655): remember previously selected features on upgrade

## Bug Fixes ##
  * Fixed [issue #663](https://code.google.com/p/tortoisegit/issues/detail?id=#663), [issue #656](https://code.google.com/p/tortoisegit/issues/detail?id=#656) and [issue #77](https://code.google.com/p/tortoisegit/issues/detail?id=#77): allow to diff added or deleted files
  * Commit and changed files dialog
> > Fixed possible hangs
> > double-click default to open files for unversioned files
> > make double-click on newly added file for diff work
  * TortoiseShell
> > Fixed an assertion (when executed on ignored files)
  * Optical and smaller optimizations/fixes (missing spaces and typos, [issue #654](https://code.google.com/p/tortoisegit/issues/detail?id=#654), [issue #595](https://code.google.com/p/tortoisegit/issues/detail?id=#595) and [issue #543](https://code.google.com/p/tortoisegit/issues/detail?id=#543))
  * Fixed [issue #666](https://code.google.com/p/tortoisegit/issues/detail?id=#666): Remote names with dots (e.g., john.doe) do not show properly in fetch dialog box
  * Fixed [issue #661](https://code.google.com/p/tortoisegit/issues/detail?id=#661): TProc crash when choose file and Git Sync dialog loads

# Release 1.6.2.0 #
Released: 2010-12-22

## Bug Fixes ##
  * Fixed [issue #650](https://code.google.com/p/tortoisegit/issues/detail?id=#650): Settings crashes on setting user name and email address
  * Fixed [issue #648](https://code.google.com/p/tortoisegit/issues/detail?id=#648): TortoiseProc crash when cloning from a working copy repo

# Release 1.6.1.0 #
Released: 2010-12-19

## Bug Fixes ##
  * Fixed [issue #645](https://code.google.com/p/tortoisegit/issues/detail?id=#645): Context menu diff crashes/errors

# Release 1.6.0.0 #
Released: 2010-12-17

## Bug Fixes ##
  * Fixed [issue #639](https://code.google.com/p/tortoisegit/issues/detail?id=#639): Tortoise Git crashes on Settings | Git | Config dialogue
  * Fixed [issue #640](https://code.google.com/p/tortoisegit/issues/detail?id=#640): Sentence is grammatically poor on Windows installer

# Release 1.5.9.0 #
Released: 2010-12-08

## Features ##
  * Fixed [issue #220](https://code.google.com/p/tortoisegit/issues/detail?id=#220): Enhancement, support creating bare repositories

  * Improve log dialog
> > Add "checkout to branch" menu at log dialog
> > Show icon for sub menu at log dialog
> > Show bisect flag at log dialog

  * Support multi-parent diff
> > Enhance GNU Diff for merge commit by choose Parent.
> > Add gnu diff combine option for merge commit
> > Support compare 1st parent, 2nd parent at merge commit
> > Show diff with multi parent at merge commit at log dialog
> > Support multi parent compare with udiff and view diff
> > Show merged file group at log dialog
> > show combine udiff at merged files
> > Add Three way diff for merge commit at log dialog

  * Compare multi parent at reflog log dialog

  * Add "Show log" in reflog context menu

  * Add --init in Submodule update from sync dialog

## Bug Fixes ##
  * Fixed [issue #270](https://code.google.com/p/tortoisegit/issues/detail?id=#270): Clone fails: bash: X.X.X.X: command not found
  * Fixed [issue #568](https://code.google.com/p/tortoisegit/issues/detail?id=#568): push using ssh private key with a password fails the first time
  * Fixed [issue #577](https://code.google.com/p/tortoisegit/issues/detail?id=#577): Commit warning "svn:externals"
  * Fixed [issue #586](https://code.google.com/p/tortoisegit/issues/detail?id=#586): Ampersand in log description underlines next character
  * Fixed [issue #323](https://code.google.com/p/tortoisegit/issues/detail?id=#323): GIT SVN dcommit --rmdir
  * Fix stash list can't show stash at reflog default
  * Fixed [issue #603](https://code.google.com/p/tortoisegit/issues/detail?id=#603): Columns not sorted in Compare revisions dialog box
  * Fixed [issue #598](https://code.google.com/p/tortoisegit/issues/detail?id=#598): Background color of log messages changed when mouse is over tag or branch indicator
  * Fixed [issue #616](https://code.google.com/p/tortoisegit/issues/detail?id=#616): Problem encoding Cyrillic characters in Author name
  * Fixed [issue #612](https://code.google.com/p/tortoisegit/issues/detail?id=#612): "Copy all information to clipboard" copies incorrect header
  * Fixed [issue #602](https://code.google.com/p/tortoisegit/issues/detail?id=#602): Rebase shows overlapping branches
  * Fixed [issue #542](https://code.google.com/p/tortoisegit/issues/detail?id=#542): Difference between line endings in compared files (external Diff Viewer)
  * Fixed [issue #468](https://code.google.com/p/tortoisegit/issues/detail?id=#468): Non-ASCII characters in user info aren't stored correctly
  * Fixed [issue #593](https://code.google.com/p/tortoisegit/issues/detail?id=#593): Fetch and push fails with TortoiseGit but succeeds with git bash

# Release 1.5.8.0 #
Released: 2010-10-02

## Bug Fixes ##
  * Fixed [issue #571](https://code.google.com/p/tortoisegit/issues/detail?id=#571): missing annotated  tags display in log dialog
  * Fix don't show tag info at log dialog
  * Fixed [issue #570](https://code.google.com/p/tortoisegit/issues/detail?id=#570): Check for modifications dialog's controls not functioning correctly
  * Fixed [issue #573](https://code.google.com/p/tortoisegit/issues/detail?id=#573): Upgrading to 1.5.7.0 removes gitdll.dll
  * Fixed [issue #572](https://code.google.com/p/tortoisegit/issues/detail?id=#572): Commit dialog becomes unresponsive after hitting F5 to refresh

# Release 1.5.7.0 #
Released: 2010-09-28

## Bug Fixes ##
  * Fix progressdlg show mass data when clone

# Release 1.5.6.0 #
Released: 2010-09-24

## Bug Fixes ##
  * Fixed [issue #556](https://code.google.com/p/tortoisegit/issues/detail?id=#556): "bad revision" in log of "Submodule Add"
  * Fix "amend last commit" can't get last commit message.
  * Fix icons were just white when using 125% display magnification mode
  * Fix ref is not updated when refresh at log dialog
  * Fix Git property page information show wrong

# Release 1.5.5.0 #
Released: 2010-09-22

## Features ##
  * Support msysgit 1.7.2.3

  * Upgrade gitdll.dll to 1.7.2.3
> > Use gitdll to fetch reflog, branch, tag information.

  * Enhance Column manage for commit list.
> > At log, rebase, sync dialog, reflog, blame. User can customize column position. User can show\hide column. Add commiter date, commiter name, email.

  * BrowseRefs: Put focus on a tree node after a branch is deleted.s

  * Add Note Support

  * Icon Overlay (TGitCache)
> > Add RW Lock to reduce tgitcache crash.

  * SyncDlg: Log output is now in Courier font. This way characters are aligned like in the console.

## Bug Fixes ##
  * Fixed [issue #535](https://code.google.com/p/tortoisegit/issues/detail?id=#535): Wandering label when drag top of progress dialog
  * Fixed [issue #478](https://code.google.com/p/tortoisegit/issues/detail?id=#478): Fix Blame timing because it shows wrong date and 00000.... commit hash
  * Fix outlook can't get correct attachment send by TortoiseGit-1.5.3.0-32bit.msi
  * Fixed [issue #537](https://code.google.com/p/tortoisegit/issues/detail?id=#537): Glitch at "merge to the right" in graph display at log dialog
  * Fixed [issue #546](https://code.google.com/p/tortoisegit/issues/detail?id=#546): Exporting without specifying a zip filename sends all zip output to stdout and confuses the GUI
  * Fixed [issue #545](https://code.google.com/p/tortoisegit/issues/detail?id=#545): Switch/Checkout Dialog: Checkbox "Create New Branch" not responding
  * Fixed [issue #160](https://code.google.com/p/tortoisegit/issues/detail?id=#160): Browse Refs dialog: Parameter is incorrect.
  * Fix Sync dialog crash when using msysgit 1.7.2.3
  * Fixed [issue #191](https://code.google.com/p/tortoisegit/issues/detail?id=#191): No Progress Indicator making one believe a hang or some failure.

# Release 1.5.3.0 #
Released: 2010-04-21

## Features ##
  * Add pre and post push hook support
  * Don't show remote branch name if remote branch is track branch at syncdlg
  * RebaseDlg: working at no branch, not upstream branch.

## Bug Fixes ##
  * Fixed [issue #475](https://code.google.com/p/tortoisegit/issues/detail?id=#475): Fix 'Save revision to' for 'Working copy'
  * Fixed [issue #486](https://code.google.com/p/tortoisegit/issues/detail?id=#486): Resolving conflicts can result in nothing to commit
  * Fixed [issue #493](https://code.google.com/p/tortoisegit/issues/detail?id=#493): Add username option at clone dialog
  * Fixed [issue #482](https://code.google.com/p/tortoisegit/issues/detail?id=#482): View message details of a tag
  * Fixed [issue #495](https://code.google.com/p/tortoisegit/issues/detail?id=#495): Push dialog does not select remote branch correctly
  * Fixed [issue #505](https://code.google.com/p/tortoisegit/issues/detail?id=#505): Delete (keep local) results in commit error
  * Fixed [issue #503](https://code.google.com/p/tortoisegit/issues/detail?id=#503): remote branch drop down doesn't allow enough characters at sync dialog
  * Fixed [issue #506](https://code.google.com/p/tortoisegit/issues/detail?id=#506): TortoiseGit-1.5.2.0-32bit.msi does not recognize msysGit-fullinstall-1.7.1-preview20100612.exe
  * Fixed [issue #492](https://code.google.com/p/tortoisegit/issues/detail?id=#492): Remember AutoLoad Putty Key status in Sync dialog
  * Fixed [issue #492](https://code.google.com/p/tortoisegit/issues/detail?id=#492): Remember AutoLoad Putty Key status in Pull dialog
  * Fixed [issue #492](https://code.google.com/p/tortoisegit/issues/detail?id=#492): Fix AutoLoad Putty Key operation in push dialog
  * Fixed [issue #513](https://code.google.com/p/tortoisegit/issues/detail?id=#513): Remember "Git Command Progress" window size
  * Fixed [issue #519](https://code.google.com/p/tortoisegit/issues/detail?id=#519): Icon overlay not working for exclude files
  * Fixed [issue #507](https://code.google.com/p/tortoisegit/issues/detail?id=#507): Help Spell error and push wrongly link to sync
  * Fixed [issue #507](https://code.google.com/p/tortoisegit/issues/detail?id=#507): context menu spell error and description error
  * Fixed [issue #517](https://code.google.com/p/tortoisegit/issues/detail?id=#517): Context menu for folder does not contain "Add to ignore list"
  * Fixed [issue #380](https://code.google.com/p/tortoisegit/issues/detail?id=#380): TortoiseMerge "Created unified diff file" doesn't work
  * Fixed [issue #528](https://code.google.com/p/tortoisegit/issues/detail?id=#528): Whole repository context menu actions not visible in Win 7 folders in libraries
  * Fixed [issue #412](https://code.google.com/p/tortoisegit/issues/detail?id=#412): Create new branch default check at switch\checkout dialog.
  * Fixed [issue #477](https://code.google.com/p/tortoisegit/issues/detail?id=#477): Commit from "GitShowLog" doesn`t show not versioned files
  * Fixed [issue #527](https://code.google.com/p/tortoisegit/issues/detail?id=#527): Fix the dialog after commit for us to be able to continue committing
  * Fixed [issue #472](https://code.google.com/p/tortoisegit/issues/detail?id=#472): TortoiseGit allows to commit without setting up a username + email
  * Fixed [issue #464](https://code.google.com/p/tortoisegit/issues/detail?id=#464): Push and pull missing from context menu
  * Fixed [issue #470](https://code.google.com/p/tortoisegit/issues/detail?id=#470): auto stash apply/pop for SVN dcommit

# Release 1.5.2.0 #
Released: 2010-06-10

## Bug Fixes ##
  * Fixed [issue #454](https://code.google.com/p/tortoisegit/issues/detail?id=#454): Fix "check Now" can't work at setting dialog
  * Fixed [issue #457](https://code.google.com/p/tortoisegit/issues/detail?id=#457): Git copy versioned item(s) here adds all unversioned files
  * put pull, push and fetch to external manual.
  * Fixed [issue #460](https://code.google.com/p/tortoisegit/issues/detail?id=#460): "Show changes as unified diff" compares files in reverse order.
  * Fix history combobox show twice item

# Release 1.5.1.0 #
Released: 2010-06-03 (internal release)

## Features ##
  * TortoiseMerge
> > Tip show "new file" "delete file" "rename file" status at tortoisemerge

  * TortoiseGitBlame
> > Add encode support for blame

  * Sync Dialog
> > Fixed [issue #392](https://code.google.com/p/tortoisegit/issues/detail?id=#392): refresh branch info when press "F5"
> > Improve user experience when input remote branch and url

  * Log Dialog
> > [issue #371](https://code.google.com/p/tortoisegit/issues/detail?id=#371): Log offer per-file "revert ..." of working dir changes
> > Add AntiAlias at show log
> > Fix version tree graphic line break at Win 7
> > Fixed [issue #427](https://code.google.com/p/tortoisegit/issues/detail?id=#427): Implement enter operation to open a file in the 'Show Log' window

  * Fixed [issue #355](https://code.google.com/p/tortoisegit/issues/detail?id=#355): Implement Show log like history in the Changed Files window after a git pull operation

  * ProgressDlg Post Cmd support menubutton

  * Update the translations.txt for translators

  * Fixed [issue #421](https://code.google.com/p/tortoisegit/issues/detail?id=#421): Implement ctrl+a standard 'Select all' facility

  * Change FormatPatch dialog default output directory is project root

  * Fixed [issue #431](https://code.google.com/p/tortoisegit/issues/detail?id=#431): Implement commit button in the git add dialog

## Bug Fixes ##
  * Fixed [issue #401](https://code.google.com/p/tortoisegit/issues/detail?id=#401): TGitCache.exe keeps open pack-xxx.idx on git repo
  * Fix issue review patch fail when there are new FilePatchesDlg.cpp
  * Fix all file show "+" icon after run git gc
  * Fixed [issue #449](https://code.google.com/p/tortoisegit/issues/detail?id=#449): Files not in the Commit dialog are committed if in index
  * Fixed [issue #450](https://code.google.com/p/tortoisegit/issues/detail?id=#450): Log Messages file list wrong when choose children dir firstly.
  * Fixed [issue #387](https://code.google.com/p/tortoisegit/issues/detail?id=#387): "Automatically check for newer versions every week" remains disabled
  * Show correct file when Add new file at tortoisemerge
  * Fixed [issue #381](https://code.google.com/p/tortoisegit/issues/detail?id=#381): About screen of TortoiseMerge shows invalid build information
  * Fixed [issue #382](https://code.google.com/p/tortoisegit/issues/detail?id=#382): TGitBlame encoding problem
  * Fixed [issue #400](https://code.google.com/p/tortoisegit/issues/detail?id=#400): CrLf options are missing in the help file
  * Fixed [issue #397](https://code.google.com/p/tortoisegit/issues/detail?id=#397): Settings/Set Extended menu/Help button doesn't work
  * Fixed [issue #396](https://code.google.com/p/tortoisegit/issues/detail?id=#396): Fix 'Copy paths to clipboard' option
  * Fixed [issue #398](https://code.google.com/p/tortoisegit/issues/detail?id=#398): Settings/Revision Graph/Help button doesn't work
  * Fixed [issue #392](https://code.google.com/p/tortoisegit/issues/detail?id=#392): Implement refresh button in sync dialog
  * Fixed [issue #395](https://code.google.com/p/tortoisegit/issues/detail?id=#395): `[`BUG`]` Infomation error when "Switch the comparison"
  * Fixed [issue #385](https://code.google.com/p/tortoisegit/issues/detail?id=#385): Bug In properties->Git dialog
  * Clear HOME at gitdll dll after load git config
  * Fixed [issue #403](https://code.google.com/p/tortoisegit/issues/detail?id=#403): Diff Show changes, but commit not
  * Fixed [issue #404](https://code.google.com/p/tortoisegit/issues/detail?id=#404): GetOpenFileName does not work in Cygwin
  * Fixed [issue #411](https://code.google.com/p/tortoisegit/issues/detail?id=#411): Fix the refresh button operation in 'Check for modifications' when only file time change.
  * Fixed [issue #406](https://code.google.com/p/tortoisegit/issues/detail?id=#406): Putty key can't save when clone
  * Fixed [issue #419](https://code.google.com/p/tortoisegit/issues/detail?id=#419): wrong error message for empty commit
  * Fixed [issue #418](https://code.google.com/p/tortoisegit/issues/detail?id=#418): Misleading button title in Sync dialog leads to loss of uncommitted changes
  * Fixed [issue #402](https://code.google.com/p/tortoisegit/issues/detail?id=#402): Revert Renamed File Fail
  * Fixed [issue #429](https://code.google.com/p/tortoisegit/issues/detail?id=#429): When applying patches, tortoise doesn't remember last file location
  * Fixed [issue #428](https://code.google.com/p/tortoisegit/issues/detail?id=#428): Blame of an old version
  * Fixed [issue #410](https://code.google.com/p/tortoisegit/issues/detail?id=#410): Change some menu item name to make it clear
  * Fixed [issue #440](https://code.google.com/p/tortoisegit/issues/detail?id=#440): Don't enable 'Apply' button until the data are ok in Settings/Git/Remote
  * Fixed [issue #439](https://code.google.com/p/tortoisegit/issues/detail?id=#439): Fix the Help action in the TortoiseGitBlame window
  * Fixed [issue #438](https://code.google.com/p/tortoisegit/issues/detail?id=#438): Slow load Switch/Checkout dialog
  * Fixed [issue #221](https://code.google.com/p/tortoisegit/issues/detail?id=#221): After resolving all merge conflicts, it's not obvious the project needs a commit
  * Fixed [issue #437](https://code.google.com/p/tortoisegit/issues/detail?id=#437): Blame should be available when there are local changes
  * Fixed [issue #444](https://code.google.com/p/tortoisegit/issues/detail?id=#444): Crash rebase  dialog when press ESC and move split bar
  * Fixed [issue #445](https://code.google.com/p/tortoisegit/issues/detail?id=#445): Resolve conflict does not delete temporary files
  * Fixed [issue #446](https://code.google.com/p/tortoisegit/issues/detail?id=#446): TortoiseMerge crash when "Edit Conflicts"
  * Fixed [issue #405](https://code.google.com/p/tortoisegit/issues/detail?id=#405): Merge commit message when there is a conflict

# Release 1.4.4.0 #
Released: 2010-04-13

## Features ##
  * #379:  Create Branch for remote branch do not set branch name

## Bug Fixes ##
  * Fix log show mass when encode is cp1251
  * Fixed [issue #357](https://code.google.com/p/tortoisegit/issues/detail?id=#357): Fix line endings merging issue

# Release 1.4.3.0 #
Released: 2010-04-10

## Bug Fixes ##
  * Fix explore crash when there are ignore patten at .git/info/exclude
  * Fixed [issue #367](https://code.google.com/p/tortoisegit/issues/detail?id=#367): Last line of .gitignore ignored
  * Fixed [issue #368](https://code.google.com/p/tortoisegit/issues/detail?id=#368): TortoiseGitBlame should not spell check by default
  * Fixed [issue #369](https://code.google.com/p/tortoisegit/issues/detail?id=#369): TortoiseGitBlame should expand its menu items by default
  * Fixed issue: Compare submodule dialog show wrong subject at log dialog
  * Fixed [issue #365](https://code.google.com/p/tortoisegit/issues/detail?id=#365): Log - enter closes dialog
  * Fixed [issue #358](https://code.google.com/p/tortoisegit/issues/detail?id=#358): Renamed files are not properly committed, after refreshing the commit dialog
  * Fixed issue .git/`*` locked when remove git repository

# Release 1.4.2.0 #
Released: 2010-04-06

## Features ##
  * Log dialog find support search tag and branch
  * Fixed [issue #354](https://code.google.com/p/tortoisegit/issues/detail?id=#354): impliment revert of this commit at log dialog
  * Add Merge command at log context menu
  * Fixed [issue #350](https://code.google.com/p/tortoisegit/issues/detail?id=#350): Implement "Copy and rename" from context menu

## Bug Fixes ##
  * Fixed [issue #346](https://code.google.com/p/tortoisegit/issues/detail?id=#346): can't remove remote repos
  * Fixed [issue #280](https://code.google.com/p/tortoisegit/issues/detail?id=#280): "Use recycle bin when reverting" does not work
  * Fix ignore over lay show wrong when second level directory exist .gitignore file
  * Fixed [issue #240](https://code.google.com/p/tortoisegit/issues/detail?id=#240): Setting "Do not show the context menu for following paths:" not working properly

# Release 1.4.1.0 #
Released: 2010-04-04

## Features ##
  * Fixed [issue #349](https://code.google.com/p/tortoisegit/issues/detail?id=#349): Offer "DCommit" instead of "Push" when working as SVN client

## Bug Fixes ##
  * Fixed clone fail if msysgit version below 1.7.0.2
  * Fixed Folder keep "X" delete icon after commit
  * Fixed some small repository can't reflect "add"
  * Fixed show "?" at second level directory when icon overlay using "shell"
  * Fixed [issue #351](https://code.google.com/p/tortoisegit/issues/detail?id=#351): "Search log messages..." in Log context menu does nothing
  * Fixed [issue #226](https://code.google.com/p/tortoisegit/issues/detail?id=#226): tortoisegit is searching for .git share on network drives
  * Fixed number of files selected is wrong at commit dialog
  * Fixed [issue #353](https://code.google.com/p/tortoisegit/issues/detail?id=#353): Fix Help button in the git sync dialog

# Release 1.4.0.0 #
Released: 2010-03-31

## Features ##
  * Improve Icon Overlay
> > Rewrite icon overlay implement. TGitCache will call gitdll.dll to get HEAD tree. And direct read index files. Read .gitignore file and call gitdll.dll to judge ignore files.
> > Can't watch untracked directroy to reduce TGitCache loading.

  * Git Clone
> > Add --progress at clone dialog

  * Log Dialog
> > Add antiAlias when draw cycle at log dialog

  * Add minimize and maximize button at rebase and sync dialog

## Bug Fixes ##
  * Fixed [issue #344](https://code.google.com/p/tortoisegit/issues/detail?id=#344): Force is the default in the sync dialog
  * Fixed [issue #343](https://code.google.com/p/tortoisegit/issues/detail?id=#343): Wrong behaviour of Show Unversioned Files checkbox at Commit dialog
  * Fixed [issue #281](https://code.google.com/p/tortoisegit/issues/detail?id=#281): show wrong character after finish commit
  * Fix commitdlg can close after commit and progress scroll too much
  * Fixed [issue #299](https://code.google.com/p/tortoisegit/issues/detail?id=#299): Do nothing "Check For Updates..."  at about dialog
  * Fixed [issue #333](https://code.google.com/p/tortoisegit/issues/detail?id=#333): Can't abort CherryPick
  * Fixed [issue #336](https://code.google.com/p/tortoisegit/issues/detail?id=#336): Text of context menu slightly wrong; replace svn with git
  * Fixed [issue #340](https://code.google.com/p/tortoisegit/issues/detail?id=#340): OpenSSH password dialog focus
  * Fixed [issue #312](https://code.google.com/p/tortoisegit/issues/detail?id=#312): The number of changed files in 'Show log' window
  * Fixed [issue #325](https://code.google.com/p/tortoisegit/issues/detail?id=#325): Would be nice to see current directory in the commit dialog
  * Fixed [issue #329](https://code.google.com/p/tortoisegit/issues/detail?id=#329): path wrong at "Save revision to...
  * Fixed [issue #327](https://code.google.com/p/tortoisegit/issues/detail?id=#327): Crash in the commit dialog after you changed a file for Linux formatted
  * Fixed [issue #321](https://code.google.com/p/tortoisegit/issues/detail?id=#321): Wrong Company/Product name in Metadata
  * Fixed [issue #309](https://code.google.com/p/tortoisegit/issues/detail?id=#309): Mispelled words in the Git Synchronization dialog
  * Fixed [issue #304](https://code.google.com/p/tortoisegit/issues/detail?id=#304): Adding a file in the commit dialog resets selection
  * Fixed [issue #305](https://code.google.com/p/tortoisegit/issues/detail?id=#305): Filtering showlog make crash

# Release 1.3.6.0 #
Released: 2010-02-05

## Bug Fixes ##
  * Fixed log crash when no body message at commit
  * Fixed [issue #298](https://code.google.com/p/tortoisegit/issues/detail?id=#298): State of "View Patch/Hide Patch" link (commit window) is wrong in some ways
  * Fixed [issue #301](https://code.google.com/p/tortoisegit/issues/detail?id=#301): Show Log crashes with empty repo

# Release 1.3.5.0 #
Released: 2010-02-03

## Features ##
  * Support Annotated tags
> > Implemented [issue #274](https://code.google.com/p/tortoisegit/issues/detail?id=#274): Enhancement: Annotated tags

  * shallow clones support --depth at clone dialog
> > Fixed [issue #290](https://code.google.com/p/tortoisegit/issues/detail?id=#290): Shallow clones support --depth at clone dialog

  * Improve Diff Dialog
> > Change commit at diff dialog
> > Diff commit context menu show in git repository

  * Log Dialog
> > Direct Launch external diff when open dialog at file
> > Log can refresh when Click Rev button.

  * Context menu
> > Use setting dialog to control which menuitem is external menu.

  * Sync Dialog
> > Add remote update at sync dialog

## Bug Fixes ##
  * Fixed [issue #294](https://code.google.com/p/tortoisegit/issues/detail?id=#294): commit template not supported and support msysgit unix path
  * Fixed [issue #282](https://code.google.com/p/tortoisegit/issues/detail?id=#282): Fom/To/Messages/Authors/Paths filters are eventually disabled
  * Fixed [issue #292](https://code.google.com/p/tortoisegit/issues/detail?id=#292): Very large dialog when merging
  * Fixed [issue #291](https://code.google.com/p/tortoisegit/issues/detail?id=#291): Blame makes empty "UserImages.bmp" file
  * Fix crash when copy several log message to clipboards
  * Fixed [issue #284](https://code.google.com/p/tortoisegit/issues/detail?id=#284): Show Log crashes when switching branches wait for log thread exit
  * Fixed [issue #285](https://code.google.com/p/tortoisegit/issues/detail?id=#285): Cherry picking no longer works
  * Fix fetch command can't sync remote branch at sync dialog

# Release 1.3.2.0 #
Released: 2010-01-21

## Bug Fixes ##
  * Fixed [issue #276](https://code.google.com/p/tortoisegit/issues/detail?id=#276): Crash on seeing diff with previous version
  * Fixed [issue #275](https://code.google.com/p/tortoisegit/issues/detail?id=#275): Load gitweb for 'Browse' button
  * Fixed [issue #265](https://code.google.com/p/tortoisegit/issues/detail?id=#265): Log dialog: Date picker throws multiple error messages when date is before 1.1.1970
  * Fix RefLogDlg crash

# Release 1.3.1.0 #
Released: 2010-01-18

## Features ##
  * Improve Log Dialog. Speed up log fetch speed.
> > Build Git source as a DLL. LogDialog will call gitdll to fetch log instead of capture git.exe output.
> > Improve refresh and all branch user experience. refresh can abort runing fetch log commit.

  * Improve icon-overlay
> > Give up igit.exe and use tgit which build from git source by VS.
> > use tgit.exe statusex to get file status.
> > Don't list all untracked files.

  * Improve commit and checkout modify dialog
> > Don't show file that is only time stamp change and no context change.
> > Run git-update-index first when open commit and checkout out modify dialog.

## Bug Fixes ##
  * Fixed [issue #234](https://code.google.com/p/tortoisegit/issues/detail?id=#234): First log(first commit in history) was missing...
  * Fixed [issue #232](https://code.google.com/p/tortoisegit/issues/detail?id=#232): "No Commit" Option always acitve
  * Fixed [issue 236](https://code.google.com/p/tortoisegit/issues/detail?id=236): CGit::GetRemoteList uses bad regular expression
  * Fix blame show wrong when first char is '^'
  * Workaround show "fail" even git run success at sometime by remove "fail" message.
  * Fixed [issue #265](https://code.google.com/p/tortoisegit/issues/detail?id=#265): Log dialog: Date picker throws multiple error messages when date is before 1.1.1970

# Release 1.2.1.0 #
Released: 2009-11-12

## Features ##
  * Add color success and fail at ProgressDlg

  * Log Dialog
> > Show work copy to log dialog. User can commit change at log dialog.
> > Easy to compare with working copy difference

  * Allow Alt+O in commit dialog for OK

  * Sync Dialog remote URL support save history

  * Add remote branch and current branch at proptery page

  * Add no-commit option at merge dialog

  * Enable IBugTraqProvide CheckCommit and OnCommitFinished

## Bug Fixes ##
  * Fixed [issue #219](https://code.google.com/p/tortoisegit/issues/detail?id=#219): Blame Error when git repository is at root directory and path use "/"
  * Fixed [issue #214](https://code.google.com/p/tortoisegit/issues/detail?id=#214): installer inserts unused or faulty registry key
  * Fixed [issue #179](https://code.google.com/p/tortoisegit/issues/detail?id=#179): Log dialog lacks information about changed files
  * Fixed [issue #209](https://code.google.com/p/tortoisegit/issues/detail?id=#209): High CPU usage in tortoiseproc.exe & limit line number
  * Fixed [issue #212](https://code.google.com/p/tortoisegit/issues/detail?id=#212): Disable the "Select items automaticlly" option has no effect to commit files dialog
  * Fixed [issue #209](https://code.google.com/p/tortoisegit/issues/detail?id=#209): High CPU usage in tortoiseproc.exe & Append text to edit ctrl
  * Fixed [issue #203](https://code.google.com/p/tortoisegit/issues/detail?id=#203): Remote URL select box in sync dialog is not populated with remotes.
  * Fixed [issue #208](https://code.google.com/p/tortoisegit/issues/detail?id=#208): During push (from context menu), branches missing from drop down list.
  * Fixed [issue #86](https://code.google.com/p/tortoisegit/issues/detail?id=#86): Globally sets HOME affecting third-party applications (GNU Emacs)
  * Fixed [issue #188](https://code.google.com/p/tortoisegit/issues/detail?id=#188): Add Git Properties tab into Windows File Properties

# Release 1.1.1.0 #
Released: 2009-10-13

## Features ##
  * Improve Rebase Dialog
> > Allow lanuch new rebase dialog again after finish rebase dialog
> > Disable "force rebase" checkbox during rebase.

  * Git SVN
> > Append svn:ignore settings to the default git exclude file Add shell extension command to import svn ignore settings.
> > Need press "Shift" key to show "import svn ignore" command.

  * Drag-drop copy\move support
> > File only

  * Add paste command at shell extension
> > Copy and paste file is okay. But there are problems when including directory.
> > Cut and paste working

  * Update notepad2 to 4.022

  * Sync Dialog
> > Ability to sync submodules in TGit sync dialog

  * Statics
> > Sort commits by dates before processed by StatGraphDlg

  * Log Dialog
> > Show <No branch> replace ref error message at log dialog

  * Add Check software updater support.

## Bug Fixes ##
  * Fixed [issue #185](https://code.google.com/p/tortoisegit/issues/detail?id=#185). "Can't find Super-project" when pathname include space.
  * Fixed [issue #190](https://code.google.com/p/tortoisegit/issues/detail?id=#190): Access violation in Blame and wrong path name when root dir is git repository
  * Fixed [issue #180](https://code.google.com/p/tortoisegit/issues/detail?id=#180): Create patch serial doesn't work when there is "\" at end of path
  * Fixed [issue #173](https://code.google.com/p/tortoisegit/issues/detail?id=#173): SVN Rebase does not work The correct handle below case git config svn-remote.svn.fetch myproject/trunk:refs/remotes/trunk
  * Fixed [issue #169](https://code.google.com/p/tortoisegit/issues/detail?id=#169): Force rebase checkbox is fixed
  * Fixed [issue #163](https://code.google.com/p/tortoisegit/issues/detail?id=#163): Conflict "theirs" and "mine" are reversed during a rebase
  * Fixed [issue #165](https://code.google.com/p/tortoisegit/issues/detail?id=#165): Incorect path to Notepad2
  * Fixed [issue #158](https://code.google.com/p/tortoisegit/issues/detail?id=#158): Rebase can act on the wrong branch

# Release 1.0.2.0 #
Released: 2009-09-05

## Bug Fixes ##
  * Fixed [issue #155](https://code.google.com/p/tortoisegit/issues/detail?id=#155): Fix SVN Rebase sets upstream as remotes/trunk
  * Fixed [issue #157](https://code.google.com/p/tortoisegit/issues/detail?id=#157): Move progress dlg before rebase dialog SVN Rebase doesn't fast-forward

# Release 1.0.1.0 #
Released: 2009-08-29

## Features ##
  * Improve Commit Dialog
> > Show line and column number
> > Add view/hide patch windows

  * Improve Log Dialog
> > Bolad subject at log dialog

  * Setting Config Dialog
> > Add core.autocrlf and core.safecrlf

  * Add more option to resolve conflict
> > Add Resolve "Their" and Resolve "Mine" at conflict item.

  * Improve Merge dialog
> > Add message box to allow input message when merge

  * Improve Stash
> > Add Stash pop.
> > Add delete stash at logview.

## Bug Fixes ##
  * Fix don't show "push" after commit
  * Fixed [issue #133](https://code.google.com/p/tortoisegit/issues/detail?id=#133): Command fails on folder with leading dash And -- to separate file and git options
  * Fixed [issue #133](https://code.google.com/p/tortoisegit/issues/detail?id=#133): (mv\rename  problem) Command fails on folder with leading dash And -- to separate file and git options
  * Fixed [issue #140](https://code.google.com/p/tortoisegit/issues/detail?id=#140): Incorrect treatment of "Cancel" action on "Apply patch serial" command
  * Fixed [issue #135](https://code.google.com/p/tortoisegit/issues/detail?id=#135): Taskbar text says "TortoiseSVN"
  * Fixed [issue #142](https://code.google.com/p/tortoisegit/issues/detail?id=#142): TortoiseGit Clone of SVN repo does not use PuTTY session for non-standard SSH port
  * Fixed [Issue #138](https://code.google.com/p/tortoisegit/issues/detail?id=#138): "Format patch" in "Show log" dialog doesn't work
  * Fixed [issue #141](https://code.google.com/p/tortoisegit/issues/detail?id=#141): Bizarre ordering in commit dialog
  * Fixed [issue #137](https://code.google.com/p/tortoisegit/issues/detail?id=#137): Proxy Authentification fails
  * Fixed [issue #131](https://code.google.com/p/tortoisegit/issues/detail?id=#131): Missing SVN DCommit Command
  * Fixed [issue #139](https://code.google.com/p/tortoisegit/issues/detail?id=#139): "Format patch" with a range of revisions doesn't export the first revision in the range
  * Fix Pathwatcher thread can't stop when commitdlg exit.
  * Fixed [issue #150](https://code.google.com/p/tortoisegit/issues/detail?id=#150): When pushing, 'remote' should default to the tracked branch, or empty

# Release 0.9.1.0 #
Released: 2009-07-31

## Features ##
  * Add Sync Dialog like TortoiseHg.
> > Put pull, fetch, push, apply patch and email patch together. You can Know what change pull and push. Show changed file list.

  * Enhance Rebase dialog. Add force rebase checkbox. Disable start button when no item rebase. Don't show merge commit

  * Add post action button for rebase dialog. Such as send patch by email
> > After rebase, you can click button to send patch email directly.

  * Add  launch rebase option at fetch dialog.

  * Improve push dialog.
> > Default settings from local repositories pushing to remote repository Choose track remote and remote branch! Add short-cut at push dialog
> > Add "F5" refresh remote and branch info at push dialog

  * Add Clean Untracked version type
> > User can choose clean untracked file, clean ignore file, clean all.

  * Enhancement: "Git Clone" from SVN repository with additional start revision number option (-r xxx:HEAD)

  * Improve Commit dialog
> > Add recent message back to context menu.
> > The "Message" field of the Commit dialog should have a shortcut key (Alt-M is a good choice)
> > Make "Whole project" directory checked by default when the user commits in the root of the project.
> > When using "Commit" to also add files, if you forget to check the new files and press "Ok", you get the dialog "Nothing Commit" and then the whole Commit dialog closes. Keep the dialog open after this message.

  * Improve setting dialog
> > Settings: Git -> Remote: When creating the first remote, the "Remote" should have "origin" as default.
> > Fix setting dialog remote page tab order
> > Push: When you press "Manage" under Destinations, the Settings dialog opening should have "Git -> Remote" selected by default.

## Bug Fixes ##
  * Fixed [issue #124](https://code.google.com/p/tortoisegit/issues/detail?id=#124): Incorrect Date header in patch e-mail
  * Fixed [issue #122](https://code.google.com/p/tortoisegit/issues/detail?id=#122): Garbage text in "Git Command Progress" / suspected buffer overflow Improve commit speed when many added files.
  * Fixed [issue #121](https://code.google.com/p/tortoisegit/issues/detail?id=#121): Refresh in "Check for modifications" dialog duplicates added state entries when new repository
  * Fixed [issue #71](https://code.google.com/p/tortoisegit/issues/detail?id=#71): (TortoiseProc problem)Icon Overlays don't work in root of drive When m_CurrentDir =C:\, not C:,  pathlist calulate wrong.
  * Fixed [issue #116](https://code.google.com/p/tortoisegit/issues/detail?id=#116): SVN Rebase doesn't work
  * Fixed [issue #115](https://code.google.com/p/tortoisegit/issues/detail?id=#115): Windows XP: Initial "Git Clone..." from SVN Repository doesn't work
  * Fix "ESC" = "push" when after commit and Add Alt-P  for Push
  * Fixed [issue #111](https://code.google.com/p/tortoisegit/issues/detail?id=#111): Undo Add does not work (keep added file) and enable "F5" at revert dialog
  * Fixed [issue #109](https://code.google.com/p/tortoisegit/issues/detail?id=#109): clone on bare local repository fails Clear trail slash \ or/
  * Fixed [issue #104](https://code.google.com/p/tortoisegit/issues/detail?id=#104): Doubleclicking changed submodule dir in Check For Modifications dlg, crashes TGit Fix log dialog double click submodule problem_

# Release 0.8.1.0 #
Released: 2009-07-03

## Features ##
  * Improve work flow and reduce click
> > Commit: Made user able to push after successful commit
> > Show Push Dialog after close commit dialog
> > Add messagebox to ask if stash change when rebase at dirty work space
> > Show GUI friendly diffstat after pull

  * Rebase: Select default upstream based on current tracked remote

  * Improve BrowseRef Dialog
> > Add Option to delete multiple refs
> > Added 'Switch to this Ref' option
> > Fetch context menu item added.
> > Add "BrowseRef" to shell extension command.
> > Add ability to diff two commits
> > Added option to delete remote branch
> > Always set initial ref
> > Show context menu icons
> > Save / Restore window size

  * Add Basic Git-SVN Operation
> > Add SVN DCommit Command
> > Add "SVN Rebase" and "SVN DCommit" command at shell contextmenu
> > Support Git svn-clone at clone dialog.

  * Help Document Updated
> > Add git basic book.

  * Add Help button at many dialog

  * Improve Format Patch
> > May also select 'format patch...' if selection is continuous.
> > Implemented browse buttons and added browsebutton for 'since'.

  * Add TortoiseIDiff to compare picture

  * Enable Bugtraq setting dialog

  * Improve Log dialog
> > Ajust label colors when selected. (Not on Vista with themes enabled)
> > Add compare with working copy at log dialog
> > Ref label borders

  * FileDiffDlg: Make shift right-left button work

  * Branch/Tag dlg: Update 'track' option after browse-refs

  * StatusListCtrl: Implemented delete unversioned file.

  * RebaseDlg: Update rebase lines after browserefs

## Bug Fixes ##
  * Fixed [issue #64](https://code.google.com/p/tortoisegit/issues/detail?id=#64): When the graph column is small, the graph sometimes appears through the text of the next column on Vista
  * Fix log graph tree mass when dragon scroll bar from left to right
  * Fixed [issue #104](https://code.google.com/p/tortoisegit/issues/detail?id=#104): Doubleclicking changed submodule dir in Check For Modifications dlg, crashes TGit
  * Pull: Fixed bug that when pulling from the configured remote branch, git did not update the remote tracking branches.
  * Fix stash problem when svn dcommit at dirty working space
  * Modify Create repository error message
  * Fixed [issue #102](https://code.google.com/p/tortoisegit/issues/detail?id=#102): Invalid patch e-mails generated
  * Fix submodule update Crash when repository have not submodule
  * Fixed [issue #88](https://code.google.com/p/tortoisegit/issues/detail?id=#88): Ambiguous dialog message
  * Correct format patch command -num argument
  * PushDlg: Fix: Wrong remote selected after selection via ref-browser.
  * Rebase: Skip in context-menu appeared twice. First one should be pick.
  * Fixed [issue #89](https://code.google.com/p/tortoisegit/issues/detail?id=#89): Can't locate msysgit on x64
  * Fixed [issue #95](https://code.google.com/p/tortoisegit/issues/detail?id=#95): TortoiseBlame Icon disappears when selected in the settings treeview
  * Fixed [issue #94](https://code.google.com/p/tortoisegit/issues/detail?id=#94): Commit log showing incorrect timestamps
  * Fix pull don't launch putty key file

# Release 0.7.2.0 #
Released: 2009-06-05

## Features ##
  * Add bug track plug-in support
> > Compatible with TortoiseSVN. The typical plug in is gurtl(google code issue plug-in).
> > https://code.google.com/p/gurtle/.

  * Support browse reference.
> > Show all branch, tags information. Support add remote, del branch\tag.

  * Show merged file at log dialog.

  * Update version graphic tree.
> > Update graphic tree to qgit2.3

  * Add option -p for TortoisePLink.
> > -p is the same as -P. So it is compatible with OpenSSH port option

## Bug Fixes ##
  * Fixed [issue #91](https://code.google.com/p/tortoisegit/issues/detail?id=#91): clone dialog generates bad directory name based on URL, ignores overrid
  * Fixed [issue #85](https://code.google.com/p/tortoisegit/issues/detail?id=#85): Installer: warns of downgrade when running 0.6.2.0 on top of 0.6.1.0
  * Fix i18n.logOutputEncoding doesn't work at log\commit dialog.

# Release 0.6.2.0 #
Released: 2009-05-06

## Feature ##
  * Improve fetch overlay speed
> > rebase igit.exe to msysgit 1.6.2.2, which is major application to get git status.

  * TortoiseMerge Support git format patch file.
> > TortoiseMerge can open git patch file and review diff and merge change.

  * SendMail support
> > Right click .patch or .diff file, click "send mail..." to send patch out.

  * improve clone dialog
> > Add auto fill module name at directory when change URL. Fix tab order.

## Bug Fixes ##
  * Fixed [issue #73](https://code.google.com/p/tortoisegit/issues/detail?id=#73): Error while reading/writing the registry key MSysGit Access is denied
  * Fixed [issue #11](https://code.google.com/p/tortoisegit/issues/detail?id=#11): Show differences as unified diff does not use selected item
  * Fixed [issue #77](https://code.google.com/p/tortoisegit/issues/detail?id=#77): "Show differencess" against a deleted file will cause TortoiseMerge to error
  * Fixed [issue #74](https://code.google.com/p/tortoisegit/issues/detail?id=#74): Add multiple files from commit dialog only adds first two in multi-selection
  * Fixed [issue #75](https://code.google.com/p/tortoisegit/issues/detail?id=#75): About box does not show version information
  * Wrong error message when fail launch pageant
  * Setup will launch old version msi to remove old version. Directly update to new version without remove old version
  * Double click conflict item to launch diffview, not conflict edit.
  * Fixed [issue #66](https://code.google.com/p/tortoisegit/issues/detail?id=#66): Some log lines lose color or disappear after you click on them
  * Fixed [issue #81](https://code.google.com/p/tortoisegit/issues/detail?id=#81): Cannot have x86 and x64 versions installed at the same time.

# Release 0.5.1.0 #
Released: 2009-04-03

## Features ##
  * Submodule Support.
> > Support submodule add, sync and update.
> > "Submodule Sync" is located in explore context external menu, which need press "shift" key when right click.

  * Improve show log speed at big repository, such as git.git

  * OpenSSH can prompt password dialog

  * Clone, pull push support both OpenSSH and Plink.
> > Support both key and password mode.
> > Show progress when clone at git and SSH protocol.

  * Stash Save\Apply support

  * Reflog support. Need press "shift" to show reflog menu item at context menu.

  * Add save special version to another file at file list, such as log dailog.

  * Add external diff merge and undiff setting at settings page

  * Add Diff with workcopy at file list

  * Add MessageBox Tell user Revert Finished

  * Add Notepad2 to setup script to view text file

  * Add view in notepad2 at file list

  * Add Copy File list to clipboard

  * Choose Default SSH client when install TortoiseGit

  * Add user config and remote manage at setting dialog

  * Pull and push can autoload putty private key.

## Bug Fixes ##
  * Fixed [issue #52](https://code.google.com/p/tortoisegit/issues/detail?id=#52): TortoiseMerge crashes on x64
  * Fixed [issue #55](https://code.google.com/p/tortoisegit/issues/detail?id=#55): "resolved" function doesn't delete temporary files.
  * Fixed [issue #57](https://code.google.com/p/tortoisegit/issues/detail?id=#57): Data duplication when Clicking Check repository in Check for modification dialog
  * Fix GetString error when edit at HistoryCombo
  * win2k context menu fix (had an issue when shift key was pressed)
  * Fix crash in logviewer on invalid time strings
  * Fixed [issue #61](https://code.google.com/p/tortoisegit/issues/detail?id=#61): Add/Commit of files with umlauts in filename not working

# Release 0.4.2.0 #
Released: 2009-03-07

## Features ##
  * Full Overlay Icon Support.
> > Show "Conflict, ignore file, untracked file, modified, Add, staged" icon according to file status.

  * Rebase Support.
> > Support "Pick" "Sqaush" "Edit" and "Skip" commit when rebase branch.
> > Support abort.

  * Combine Multi-commits to one commit.
> > Combine continous commits to one commit. The limition is the only single line(no merge point) above combined commit.

  * Cherry Pick multi commits.
> > User can use multi commits at log dialog and then choose cherry pick these. Cherry Pick dialog guide you finish whole work.
> > Support "Pick" "Squash" "Edit" and "Skip" commits.

  * First x64 version.

  * Support version "browse" at switch, export, new branch/tag and merge dialogs.

  * Add context menu item "Revert" at Commit dialog File List.

  * Show bold font for HEAD at log dialog.

  * Add "Whole Project" checkbox at commit dialog

  * First Version Help Document.

## Bug Fixes ##
  * Fix Shell menu disappear because ATL library have not installed.
  * Fix Commit Dialog and Log Dialog default column is wrong
  * Fix some dialog can't show after resize and close and open again
  * Fix ProgressDlg Sometime thread is dead blocked.
  * Fixed x64 build of TortoiseProc crashed due to received unexpected messages
  * Fix tag to head when **force** check box checked
  * Add Git document to help
  * Fixed [issue #36](https://code.google.com/p/tortoisegit/issues/detail?id=#36): Push not working if no remote branch is specified
  * Default UnCheck untrack file at commit dialog
  * Fixed [issue #40](https://code.google.com/p/tortoisegit/issues/detail?id=#40): Commit from subfolder shows unversioned files in parent
  * Fix diff problem when filenames have embedded spaces
  * Fixed [issue #24](https://code.google.com/p/tortoisegit/issues/detail?id=#24) and [issue #45](https://code.google.com/p/tortoisegit/issues/detail?id=#45): Commit results not in window with scroll bars
  * Fix for win2k context menu icons
  * Fixed [issue #46](https://code.google.com/p/tortoisegit/issues/detail?id=#46): The about window title still displays TortoiseSVN
  * Fixed [issue #37](https://code.google.com/p/tortoisegit/issues/detail?id=#37): When the file name contains Chinese char, Diff doesn't work.
  * Fixed [issue #28](https://code.google.com/p/tortoisegit/issues/detail?id=#28): "Add" status icon overlay is not correct.

# Release 0.3.3.0 #
Released: 2009-02-08

## Features ##
  * Icon Overlay
> > Show different icon overlay at git repository. Support File and directory icon overlay.

  * Show version tree in log dialog.
> > Show version graphic tree at log list dialog. Use QGit style.

  * Enable log cache to improve log show speed.

  * VS2008 Style Blame application.
> > Show different back color according to line age. Show blame file log list to know which line is newer.

  * Enable conflict handle
> > Show conflict status at any file list, such as commit dialog. User just need right click and choose resolve conflict, tortoisemerge will be launch.

  * Related time show support.

  * Setting dialog support.

  * Enable TortoisePlink.
> > Passwork dialog can prompt when use tortoiseplink as ssh client.

  * Git Reset support.
> > User can right click log list at log dialog. Choose reset to reset current branch to chosen commit.

  * Current handle renamed file at file list.

## Bug Fixes ##
  * Disable file overlay icon at vista system to avoid explore crash
  * File overlay default is enable at XP system. User can disable it by setting dialog.
  * Fixed [issue #20](https://code.google.com/p/tortoisegit/issues/detail?id=#20): Add To Ignore from Commit dialog not working
  * Fixed [issue #31](https://code.google.com/p/tortoisegit/issues/detail?id=#31): Init Repository, Commit dialog can not show added file
  * Fixed [issue #30](https://code.google.com/p/tortoisegit/issues/detail?id=#30): Clone does not support UNC path to repository
  * Fix when setting ssh client is null. GIT\_SSH environment variable is not clear
  * Fixed [issue #29](https://code.google.com/p/tortoisegit/issues/detail?id=#29): F5 should refresh TGit log
  * Fix log filter don't filter commit hash
  * Fixed [issue #25](https://code.google.com/p/tortoisegit/issues/detail?id=#25): Log refresh does not pick up new tags on top line, or move 'master' up
  * Fixed [issue #27](https://code.google.com/p/tortoisegit/issues/detail?id=#27): Deleted files not committed
  * Fixed [issue #22](https://code.google.com/p/tortoisegit/issues/detail?id=#22): Error deleting file from context menu if filename contains spaces
  * Fixed [issue #6](https://code.google.com/p/tortoisegit/issues/detail?id=#6): Add does not work.
  * Fixed [issue #8](https://code.google.com/p/tortoisegit/issues/detail?id=#8): Clone of git via HTTP Creates repo in wrong location
  * Fixed [issue #9](https://code.google.com/p/tortoisegit/issues/detail?id=#9): Error commit file with chinese filename.
  * Fixed [issue #10](https://code.google.com/p/tortoisegit/issues/detail?id=#10): Switch and Create Branch drop-downs only display 25 items
  * Fixed [issue #13](https://code.google.com/p/tortoisegit/issues/detail?id=#13): Create branch fail if branch name is invalidate
  * Fixed [issue #14](https://code.google.com/p/tortoisegit/issues/detail?id=#14): Commit dialog don't report error when no message input
  * Fixed [issue #16](https://code.google.com/p/tortoisegit/issues/detail?id=#16): Commit dialog, F5 don't work.
  * Fix "explore to" in context menu in commit dialog.
  * Fix redraw all when loading thread finish load log.

# Release 0.2.0.0 #
Released: 2009-01-04

## Features ##
  * Add TortoiseMerge as default compare tools
  * Pull, Fetch, Push
  * Create Branch\Tag
  * Switch branch\Chechout
  * Compare with previous version
  * Clone(only support local repository, see known issue for detail)
  * Log Dialog support filter
  * Check for modifications
  * Revert local change
  * Create Patch Serial
  * Apply Patch Serial
  * Add file to repository(see know issue)
  * Export to zip file

## Bug Fixes ##
  * A2W cause stack overwrite bug when git output is long.

## Known Issue ##
  * ProgressDlg will wait for ever when clone remote repository(ssh, http,git).
  * push fetch and pull don't support password mode. Just support public key problem.
  * Just fetch first 100 log item.
  * If install TortoiseGit before MsysGit, you need modify register
> > HKEY\_LOCAL\_MACHINE\Software\TortoiseGit\\MsysGit\
> > Let it point to correct msysgit install path.
  * Add File, please commit and show unversion file, the choose add file, then right clict, Choose Add file
  * To new initial repository, You will not see add file again in commit dialog box if give up commit when choose add


# Release 0.1.0.0 #
Released: 2008-12-12

## Features ##
  * Context menu(subset of TortoiseSVN)
  * Icon Overlay(version controled\unversion controled at directory)
  * Unified DIFF
  * Use third part diff tools (such kdiff3)
  * Commit change
  * Show Log
  * Create Repository