# ansible-role-simple-disk-space-notify
Install a cron job to periodically monitor disk use, and send a notification email if space exceeds the configured threshold

This is a trivial script for simple/legacy servers. You can use it as a backup, but you should have better monitoring in place.

See defaults/main.yml for config options.

## Requirements

- The `mail` command line util must be installed.
- You must have already configured your server to be able to deliver mail to the outside world.

The [acromedia.postfix](https://github.com/AcroMedia/ansible-role-postfix) is a good starting place for the above.
