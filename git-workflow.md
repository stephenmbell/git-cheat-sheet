# basic git workflow

## Where do I do my work?

Contributors never work on the central repository.  Instead, they clone it and work independently on their local copy.  Again - *NEVER* work in the central OR remote repository.  All work is done locally then pushed to the central repository.

## General Workflow

Link to the [Github workflow](https://guides.github.com/introduction/flow/)

Another link describing the [Github workflow](http://scottchacon.com/2011/08/31/github-flow.html)

Takeaways:

- `master` branch is *ALWAYS* deployable.  Should represent stable working history of code
- branch names should be descriptive
- *NEVER* work directly in the `master` branch

## When making changes

1. Get an updated copy of the repository on your local machine.  If there isn't already a local copy, use git clone https://url-of-repo.  If you have one already use `git fetch` or `git pull` from within the folder of the repository you are looking to work in.
    - `git fetch` command downloads commits, files, and refs from a remote repository to your local repo.
    - `git pull` is the more aggressive alternative, it will download the remote content for the active local branch and immediately execute `git merge` to create a merge commit for the new remote content.
1. Once you have an updated copy of the repository on your local machine, create a branch for the work you will be looking to complete using `git branch`
Example: `git branch my-new-branch`

    - Once the branch is created, switch to that branch: `git checkout my-new-branch`

1. As you make changes to the code you will iterate over the following process:
    - Run `git status` to view any unstaged changes / untracked files
    - To add the changes / files to the index to be tracked, run `git add -A` (A for all).  (This will add all staged changes)
    - To add changes individually, run `git add ..\path\to\changes.txt`
    - Once all changes have been staged, you can commit the changes by running `git commit -m "descriptive message about included changes"`
    - Once the changes have been committed to your local repository, run `git push` to push your local copy of the branch to the origin (cloud) repository.
  
## Deploying your code

Once your testing is completed, you can deploy the code from your newly created branch
## Once your code has been validated in production

To integrate the changes from your newly created branch into master, you need to create a `pull request`.  This can be done within your editor (vscode), or from the web (Azure Devops, Github).  Creating a pull request will initiate a merge between your branch and master and present you with any conflicts.

