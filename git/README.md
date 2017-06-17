# Git configs

The config includes a modified version of `.gitconfig` file to allow shortcut git commands.
Allow git completion through `.git-completion.bash`. Command to install git-completion and put it on `.bash_profile`:
```bash
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash && echo "source ~/.git-completion.bash" >> ~/.bash_profile && source ~/.bash_profile
```
