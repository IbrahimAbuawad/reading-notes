## what is git 

#### Snapshots

##### Git is a DVCS that stores data in a file system made up of snapshots.

#### Local Operations

##### Git mostly relies on local operations because most necessary information can be found in local resources.

#### Tracking Changes

##### Every single change applied to any file or directory is tracked by Git.

## Cloning
##### You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL: git clone .
##### Example:
##### https://github.com/test 

## Local Repository Structure
### The local Git repository has three components:

##### 1. Working Directory: The actual files reside here.
##### 2. Index: The area used for staging
##### 3. Head

## Check File Status
##### To determine the state of files, utilize the git status command:

##### Example:
##### $ git status

## Committing a File
##### After staging one or multiple files, you should commit the changes and record what you did within the commit message:

##### Example:
##### $ git commit -m “made change x,y,z”

## Pushing Changes
##### Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

##### Example:

##### $ git push origin master