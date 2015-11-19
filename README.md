This utility uses the hpasmcli command line utility
to check the temperature on HP hardware. It can be used
as a nagios plugin or directly from the command line

This script only checks temperature sensors

It requires Python version 2.6 and has been tested on the following:
RHEL 6

You have to run hpasmcli as root so marke sure your NRPE Command looks like this:
```
command[check_temp]=/usr/bin/sudo /usr/lib64/nagios/plugins/check_hp_temp
```
