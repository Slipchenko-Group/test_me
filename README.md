## repository to practice git tools

### To start with git

- on windows, install git 
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
`git pull origin master --rebase`
