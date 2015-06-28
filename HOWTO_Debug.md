# Introduction #

This guide will show you how to Debug TortoiseGit. In general there are three stages of debugging with increasing need of work:

  1. [Capturing debug strings](HOWTO_Debug#Capture_Debug_Strings.md)
  1. [Using a debugger (to generate a stack trace)](HOWTO_Debug#How_to_use_a_debugger.md)
  1. [Compile your own debug version](HOWTO_Debug#Compile_your_own_debug_version.md)

## Capture Debug Strings ##

TortoiseGit has some debug statements build in which are not generated and visible by default.

You can enable the generation of those debug strings by setting _DebugOutputString_ to _true_ in TortoiseGit advanced settings.

After restarting your computer (or TGitCache.exe, explorer.exe and/or TortoiseGitProc.exe) you can capture the debug strings using a tools like [DebugView](http://technet.microsoft.com/en-us/sysinternals/bb896647.aspx) from the SysInternals suite or [WinDbg](http://msdn.microsoft.com/en-us/windows/hardware/gg463009.aspx).

If you use DebugView and wish to report the values in Time column, you need to save the log file or log to file. Time column is not copied to clipboard.

## How to use a debugger ##

In order to generate a stack trace you can use a debugger like [WinDbg](http://msdn.microsoft.com/en-us/windows/hardware/gg463009.aspx) or a Visual Studio IDE and attach it to a TortoiseGit process.

To get a nice stack trace and resolve symbols, you can use our symbol server

http://www.crash-server.com:8080/public/TortoiseGit/7fbde3fc-94e9-408b-b5c8-62bd4e203570/symsrv/

or download the [debug symbols](http://download.tortoisegit.org/tgit/) which are only available for our releases.

In WinDbg the symbol server can be used by issuing _.sympath+ srv`*`c:\tmp`*`http://www.crash-server.com:8080/public/TortoiseGit/7fbde3fc-94e9-408b-b5c8-62bd4e203570/symsrv/_; the URL for the Microsoft symbol server is _srv\*c:\tmp\*http://msdl.microsoft.com/download/symbols_.

## Compile your own debug version ##

See TortoiseGit\_Overall\_Architecture and http://code.google.com/p/tortoisegit/source/browse/build.txt.