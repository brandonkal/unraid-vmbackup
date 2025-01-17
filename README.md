# unraid-vmbackup

Script for use with unRAID's CA User Scripts plugin. See [here](https://lime-technology.com/forums/topic/48286-plugin-ca-user-scripts/ "CA User Scripts") for more information.

Currently the script is in a relatively stable state, and most of the features have been implemented. I have tested them as well as I can, but I cannot guarantee they will work correctly for everyone, so be sure to test thoroughly on your system before depending on this script for backups. Please review the Change Log and To-Do List if you would like to know more.

v1.1.4 - 2018/05/19

## Installation

- Add the script and description files to the CA User Scripts plugin. No other files are necessary to make the script work.

- Set the variables in the script file.

- Choose a schedule in the CA User Scripts plugin.

### Script options

- Choose a backup location.

- List VMs to be backed up.

- List specific vdisks to skip, if any.

- Option to kill a VM that won't shutdown cleanly.

#### VM restart options

- Option to have VMs start after backup based on their previous state.

- Advanced: Option to have VMs start after successful backup regardless of previous state.

- Advanced: Option to have VMs start after failed backup regardless of previous state.

#### Backup retention options

- Choose the number of days to keep backups.

- Choose the number backups to keep.

#### Logging and notification options

- Option to log to file.

- Choose the number of log files to keep.

- Option to log messages through unRAID notification system.

  - Option to only receive error notifications

  - Option to receive detailed notifications.

    - sends notifications when vm backups are started and stopped.

    - sends notifications when old backups are deleted.

#### Additional options

- Option to compress backups.

- Option to timestamp backups.

- Option to disable delta syncs.

- Option to only use rsync.

- Advanced: Option to enable reconstruct write during backups.

- Advanced: Option to compare files and retry backup in the event of failure.

- Advanced: Option to skip backing up xml configuration.

- Advanced: Option to skip backing up nvram.

- Advanced: Option to skip backing up vdisks.

- Advanced: Option to ignore iso files when checking for valid vdisks.

- Advanced: Choose the number of times to check if a VM is shut down.

- Advanced: Choose the number of seconds to wait between checks to see if a VM is shut down.

##### Disclaimer

I do not make any guarantees as to the function of this script. It is provided as-is. Use at your own risk.

###### Originally from unraid-autovmbackup by Daniel Jackson (danioj) [here](https://lime-technology.com/forums/topic/46281-unraid-autovmbackup-automate-backup-of-virtual-machines-in-unraid-v04/ "unraid-autovmbackup")

###### Includes additions for removing old backups added by Deeks [here](https://lime-technology.com/forums/topic/46281-unraid-autovmbackup-automate-backup-of-virtual-machines-in-unraid-v04/?do=findComment&comment=589821 "unraid-autovmbackup Deek's script")
