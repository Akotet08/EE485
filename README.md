# EE485

Git stores snapshots(like a photograph of the state), not differences in each version.
GitHUb is just a website that uses git.

Install git and configure 
`git config --global user.name 'Your name'`
`git config --global user.email 'Your Email address'`

### Git Transport Commands
`workspace -> index -> Local repository -> Remote repository`

Developers work on workspace. The changes are tracked by the index. Then whatever is updated is added to the local repository when committed. Finally the local repo can be pushed to the remote repo.

`git clone` - copies all data from remote repo to the local repo.
The local rep is in the .git file.

`git add` - addes changes to the staging area doesn't affect the local repo.
`git commit` - affects only the local repo. `git commit -a` commit all changes even if they are not staged in the index. Each commit as a hash value of 40 characters using SHA-1 that is used as an ID

`git log` - show the history of the commits.

### Git file status
Untracked - status not under version control
unmodified - not changed since last update
modified - Status that the contents of the file being versioned have changed 
statged - changes added to index that can be commited to the local repo


### Branches
A git branch is a file that stores a particular commit hash value. Braches don't affect each other, so this allows paraller development.

HEAD is the current branch that is being worked on.

Merge two brances
    Fast Forward merge: merge with a parent when the parent hasn't changed
    3-way merge: merging with a parent that has new commits. Resolve conflict manually

### Pull/Push
push to change the remote repo
synchronize with fetch and then merge with the main. git pull does fetch and merge automatically

