# baldnerd_base
Linux base creation tools for single board computers.

Before proceeding, the following must be achieved:

1) A Debian distro is imaged and booted. All updates / upgrades have been applied, and system is running well.
2) Date and time are set (best to run *locale* first).

Now, use these scripts:

1) *locale* - Set the timezone and locale. BaldNerd default is America/Toronto, en_US UTF-8.
2) *user* - Create the default user (baldnerd) and remove any existing user.
3) *hostname* - Set the hostname to *debian*.
4) *cleanup* - The final removal of logs, creation of the MOTD, and fill all empty space of disk with zeros before halting for image.
