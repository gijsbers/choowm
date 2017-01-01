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
without having to authenicate.
Run it as the last command in your `~/.xinitrc` file.
