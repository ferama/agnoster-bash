# agnoster-bash
Agnoster Theme for Bash

agnoster's Theme - https://gist.github.com/3712874
A Powerline-inspired theme for BASH

(Converted from ZSH theme by Kenny Root)
https://gist.github.com/kruton/8345450

# README

In order for this theme to render correctly, you will need a
[Powerline-patched font](https://gist.github.com/1595572).
I recommend: https://github.com/powerline/fonts.git
```
git clone https://github.com/powerline/fonts.git fonts
cd fonts
install.sh
```

Install:

I recommend the following:
```
cd $HOME
mkdir -p .bash/themes/agnoster-bash
git clone https://github.com/ferama/agnoster-bash.git .bash/themes/agnoster-bash
```

then add the following to your .bashrc:

```
export THEME=$HOME/.bash/themes/agnoster-bash/agnoster.bash
if [[ -f $THEME ]]; then
    export DEFAULT_USER=`whoami`
    source $THEME
fi
alias su='su -m'
alias sudo='sudo '

```

# Goals

The aim of this theme is to only show you *relevant* information. Like most
prompts, it will only show git information when in a git working directory.
However, it goes a step further: everything from the current user and
hostname to whether the last call exited with an error to whether background
jobs are running in this shell will all be displayed automatically when
appropriate.

![ScreenShot](agnoster-bash-sshot.png)
