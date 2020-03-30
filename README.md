Sample cloud shell pre-configuration

# Principe
Cloud Shell automatically runs the script, $HOME/.customize_environment, when your instance boots up. Unlike .profile or .bashrc, this script runs once when Cloud Shell boots (rather than once for each shell login).

your home is a persitent 5Go volume .  the purpose of this repo is to install system requirement which are outside your home/ or to be able to generate a, initial cloudshell env with ease

# How
simply copy this files in your cloudshell home and adapt them :

(to launch a cloudshell with a git repo and an editor: )

https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/xyzopowa/cshammer&page=editor&open_in_editor=README.md

```shell
.gitconfig              # git profile 
.profile                # env 
.customize_environment  # customize env
```

# Content
- update terraform
- add terraform-docs
- add tflint
- add pre-commit
- add kubect-krew
- add kubectl krew plugins :  rbac-lookup , tail , tree and view-secret
- add helm v3 as 'helm3'
- add velero 

# nota

