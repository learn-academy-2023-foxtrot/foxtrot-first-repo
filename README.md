# foxtrot-first-repo

## Git and Github Intro 8/29/2023 Foxtrot

### vocabulary
- git: version control software
- version control: a system that manages that changes that are made to files over time
- repositories: storage location for files and folders for a project
- local: refers to code that only exist on your local machine
- remote: refers to code that exists on a server
- github: web-based platform that serves as a hosting service for git repositories, allows developers to share, store, and contribute to a project
- branch: way to store the current version of the codebase you have changed
- main branch: "source of truth", stores the working version of the project
- checkout: switching to a different branch within a repository
- staging: selecting files (changes) to be included in a commit
- commit: a snapshot of the changes made to files in a repository and includes a descriptive message
- merging: combining the changes from one branch into another
- stale branch: a branch that is no longer relevant, changes have been merged

### Process Notes
Anything wrapped in < > is an indication that this will be named uniquely, the < > are NOT included in the command
$ is an indication of a command line prompt, the $ is not included
Anything in ( ) is informational and not included in the command

### Naming Conventions
Branches and file names should be in all lowercase letters with no spaces

### Informational Commands
Use this informational command to tell you what files have been modified and what phase of the git process you are on:

`$ git status`
Use this informational command to the branches you have locally on a repo:

`$ git branch`
The branch that you are on currently will be denoted with an asterisk.

### Cloning the Repo
Use this command if you don't have the repository (folder) on your local machine:

`$ git clone <repo-url>` (the url is the https address copied and pasted from the code dropdown button on GitHub)

### Create a Branch
Use this command if you need to create a branch that does not exist on either repos locally or remotely:

`$ git checkout -b <topic-initials1-initials2>`

### Changing to a Local Branch
Use this command to move to a branch that exists on your local machine:

`$ git checkout <branch-name>`
`$ git pull origin <branch-name>`

### Pushing Local Code to GitHub
Use these commands to add the code you have on your local machine to GitHub:

$ git status
$ git add <file-name>
$ git commit -m "message describing the work that was accomplished"
$ git push origin <branch-name>

### Switching Drivers
- Second driver will run the following commands after verifying that the shared repo is cloned on both sides locally

$ git fetch origin <branch-name-of-team>
$ git checkout <branch-name-of-team>

- After changes have been made and the team is ready to switch again, revisit the Pushing Local Code to Github steps above.