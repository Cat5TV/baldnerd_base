# baldnerd_base
Linux base creation tools for single board computers.

You can download pre-built base images from my blog at https://baldnerd.com/sbc-build-base/

Before proceeding, the following must be achieved:

1) A Debian distro is imaged and booted. All updates / upgrades have been applied, and system is running well.
2) Date and time are set (best to run *locale* first).

Now, use these scripts:

1) *prep* - Prepare the system before building. Will force a reboot.
2) *locale* - Set the timezone and locale. BaldNerd default is America/Toronto, en_US UTF-8.
3) *base* - Install a very simple base set of tools (this is only a base OS, developers can add what they really need, but I'll install what I think is crucial out of the box).
4) *user* - Create the default user (baldnerd) and remove any existing user.
5) *hostname* - Set the hostname to *debian*.
6) Reboot at this point, and when reconnecting, login as baldnerd/baldnerd, then use sudo su to become root.
7) *rc* - Configure and then open rc.local for first-boot (do not reboot after this)
8) *cleanup* - The final removal of logs, creation of the MOTD, and fill all empty space of disk with zeros before halting for image.
