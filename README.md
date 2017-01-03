# choowm -- Choose your window manager

Choowm is a bash shell script which
allows the user to choose which
window manager to run.

Choowm will examine the system for nearly
all known window managers.
Those found are shown in a graphical dialog.
The user can pick one and choowm will run it.
If the chosen window manager exits then
choowm repeats the process.
If the user aborts selection then choowm will stop.

This script enables fast switching
between different window managers
without having to authenticate.
Run it as the last command in your `~/.xinitrc` file.

Choowm accepts the following command line options:

- -i initialwm: This forces the given window
manager to be run immediately on startup,
bypassing the dialog selection process once. Only
if this window manager exits is the selection
dialog presented.
- -l: Just print a listing of the available
window managers to stdout and exit.
- -n: No execution. This _dryrun_ option only
prints the selected window manager and then
exits. This is used for testing.

## Screenshots

By default `zenity` will be used to show the dialog
if it is installed:

![choowm using zenity](/images/choowm-zenity.png)

Otherwise `xmessage` is used:

![choowm using xmessage](/images/choowm-xmessage.png)

