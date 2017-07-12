# Git configs

The config includes a modified version of `.gitconfig` file to allow shortcut git commands.
Allow git completion through `.git-completion.bash`. Command to install git-completion and put it on `.bash_profile`:
```bash
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash && echo "source ~/.git-completion.bash" >> ~/.bash_profile && source ~/.bash_profile
```

## List of git shortcut commands available:

### Branches:
  - **git br**: List all local branches.
  - **git branches**: List all remote-tracking and local branches.
  - **git cb**: Show the current checked out branch.
  - **git chkm**: Checkout the remote (origin) master.
  - **git chkb <`branch`>**: Checkout a given branch.
  - **git delb <`branch`>**: Delete a given branch.
  - **git purge**: Delete all local branches that has been merged.

### Commits:
  - **git st**: Show the working tree status.
  - **git dl**: Decoratively print out commit status.
  - **git addup <`file`>**: Stage a changed file.
  - **git stage**: Stage all changed files.
  - **git rmv <`file`>**: Unstage a changed file.
  - **git amend**: Amend changes to a previous commit.
  - **git cp <`hash`>**: Cherry pick a commit hash.

### Repositories:
  - **git rem**: List set of tracked repositories.
  - **git remadd <`name`> <`org`> <`repo`>**: Add a remote with the given name, org and repo.
  - **git remaddu <`org`> <`repo`>**: Add a remote as an upstream with the given org and repo.
  - **git remrmv <`name`>**: Remove a remote with the given name.

### Push:
  - **git fet**: Prune and fetch the latest from remote (origin) master.
  - **git fetu**: Prune and fetch the latest from upstream master.
  - **git rbm**: Interactively rebase against the remote (origin) master.
  - **git rb <`remote`> <`branch`>**: Interactively rebase against a given remote and branch.
  - **git fp <`remote`> <`branch`>**: Force push to a given remote and branch.
  - **git fpo <`branch`>**: Force push to a given branch in remote (origin).
  - **git fpoc**: Force push to the current checked out branch.
  - **git prep <`file`>**: Stage a file by amending it to a previous commit.
  - **git prepup <`file`>**: Stage a file and push it by amending it to a previous commit.
  - **git send**: Push all staged files by amending to previous commit.
