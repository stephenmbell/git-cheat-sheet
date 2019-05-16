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

# When making changes

1.  Get an updated copy of the repository on your local machine.  If there isn't already a local copy, use git clone https://url-of-repo.  If you have one already use `git fetch` or `git pull` from within the folder of the repository you are looking to work in.
     - `git fetch` command downloads commits, files, and refs from a remote repository to your local repo.
    - `git pull` is the more aggressive alternative, it will download the remote content for the active local branch and immediately execute `git merge` to create a merge commit for the new remote content.
1. Once you have an updated copy of the repository on your local machine, create a branch for the work you will be looking to complete using `git branch`
