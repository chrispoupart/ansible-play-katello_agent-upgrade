# Update the Katello Agent to 6.2

This play will likely have to be run in two passes. On the first pass, there
will be many of the older servers that will fail on "become" becuase they use
the Quest SUDO package. 

Re-run the play useing the `katello-update.retry` script, and change the become
option in `ansible.cfg` to `/opt/quest/bin/sudo`.
