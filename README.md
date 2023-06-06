## repository to practice git tools

### To start with git

- if you do not have WSL installed on Wondows, install git. Otherwise, WSL already has git installed. Just work from the WSL terminal
- add ssh keys to your machine via `ssh-keygen` command
- add public ssh keys to git web (in settings, add new ssh keys)
- do `git config`

### Basic git commands 

Clone repository to a local machine
`git clone ...`

Create your own branch "my_branch"
`git checkout -b my_branch`

Check all branches
`git branch`

Switch to a branch "branch_name"
`git branch branch_name`

Add all your changes to local repository
`git add .`

Add specific file to local repository
`git add file_name`

Commit changes to a branch on a local machine
`git commit -m "description of my changes"`

Push your changes in branch "branch_name" to the remote (cloud)
`git push origin branch_name`
This creates or updates "branch_name" on cloud github

Merge your branch with master: on git website, submit merge request for your branch 

Update local master branch
`git pull origin main --rebase`

**Explanation of the `-- rebase` option from [https://www.gitkraken.com](https://www.gitkraken.com/learn/git/git-rebase#:~:text=Git%20pull%20rebase%20is%20a,behind%20the%20origin%2Fmain%20branch.)**

So, what’s the difference between Git pull rebase and Git pull merge? While both of these options will combine the changes fetched from your remote, the outcome will look very different in your Git history.

Git pull merge is the default method for combining changes in Git, and will merge the unpublished changes with the published changes, resulting in a merge commit.

With Git pull rebase, on the other hand, the unpublished changes will be reapplied on top of the published changes and no new commit will be added to your history.

With this in mind, you can see that Git pull rebase will result in a linear and cleaner project history by removing the unneeded merge commit.
