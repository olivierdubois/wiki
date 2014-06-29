# Working with existing remotes




## Start a project from an existing remote repository

The following instructions assume that:
  * the project already exists on a remote repository;
  * the project uses a Gitflow workflow.


#### Create a local branch

If the `develop` branch does not already exist on the local repository, create it by running:
```
$ git checkout -b develop
```


#### Download the remote branch

Download `develop` from the remote repository:
```
$ git pull -u origin develop
```
The `-u` option will set the local branch to track upstream changes from the remote. It will provide feedback about how many commits ahead or behind the local branch is compared to the remote when `$ git status` is run.


#### Initiate Gitflow

Initiate the Gitflow workflow by running:
```
$ git flow init
```
This is only required to run once when work is being started on a local repository. If the `master` and `develop` branches are present on the local repository, the following command can be run safely and will apply all the defaults:
```
$ git flow init -d
```


#### Create a feature branch

Create a new `feature` branch to work on:
```
$ git flow feature start [feature-name]
```

