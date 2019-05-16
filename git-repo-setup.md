# basic repository setup

We use git in a distributed - or - de-centralized model.  This basically means that each contributor has a copy of the *ENTIRE* repository locally on their machine.  All work is done in the *LOCAL* repository and then pushed to the *REMOTE* repository.

The *REMOTE* repository is the one that is hosted in Azure Devops, Github, Bitbucket, etc.  This is the *OFFICIAL* project repository OR *CENTRAL* repository.  Contributors never work on the central repository.  Instead, they clone it and work independently on their local copy.

## cloning an existing repository
`# create a folder where you would like to store your local repository, and cd to it`
cd ~/gitrepos
mkdir my-repo
git clone https://url-to-repository

This will download a copy of the repository to your machine.















