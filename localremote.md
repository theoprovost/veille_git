# How to synchro local / remote repository

- First of all, have an GitHub account
- For convenience, deploy a pair of SSH keys
- Fill your credentials (`git config`)
- Check everything is ok (`git config --list`)

<img src="https://whyisdifference.com/wp-content/uploads/2018/04/cdn_subdomain/Difference-Between-Git-Fetch-and-Git-Pull.png" style="width:100%; height:100%; margin:20px 0 20px 0">

## Git push

`> git push [options]`

"Updates remote refs using local refs, while sending objects necessary to complete the given refs." *Git's doc*

This command is used to sync your local version to your remote one.

## Git pull

`> git pull <remote> [options]`

This command gets the remote version to sync with the one one your desktop.

Pull grabs the remote copy of the branch and merges the changes with the local repository. Pull is basically a fetch followed by a merge command.
It brings a local branch of up-to-date with a remote

Conflicts ? Merge conflicts can occur with git pull when two (or more) work on the same code. Especially on the same branch.

## Git fetch

`> git fetch <remote> <branch> [options]`

Fetch retrieves all the changes from the remote repository without integrating them with the local repo.
It updates the repo data leaving your local repo unchanged.
It imports commit to local branches to keep you up-to-date with whats everybody is working on.

Conflicts ? No merging means no conflicts.
<br>

_____
***Refs:***
|Title|URL|
|--|--|
|Git's doc|https://git-scm.com/|
|Git magic PDF|[GitMagic.pdf](./GitMagic.pdf)
|