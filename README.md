#first step

https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/xyzopowa/cshammer&page=editor&open_in_editor=README.md

#second step
Environment customization script

Cloud Shell automatically runs the script, $HOME/.customize_environment, when your instance boots up. Unlike .profile or .bashrc, this script runs once when Cloud Shell boots (rather than once for each shell login).

This script runs as root and you can install any packages that you want to exist in each Cloud Shell session using Debian package management commands.

For example, if you'd like to have erlang installed on Cloud Shell, your .customize_environment file will look like this:
```shell
#!/bin/sh
apt-get update
apt-get -y install erlang
``` 
Execution logs of your .customize_environment script can be found at /var/log/customize_environment. The .customize_environment script runs as a background process and on successful execution, will touch /google/devshell/customize_environment_done. Because package installation runs in parallel with your logging in, the installed packages may become available a few moments after you reach the login prompt.

#


# files

```shell
.gitconfig              # git profile
.profile                # env 
.customize_environment  # customize env
```
