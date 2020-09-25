<<<<<<< HEAD
## Uploading to your repo

Once you have authored new content, like a jupyter notebook assignment, you will want to update your repo. Remember, creating a notebook in JupyterHub does not automatically add it to your repo. You have to manually do it.

#### Launch a terminal window
#### pull data from your repo in case your copy is not up to date
```git pull```
#### add all the files you have created, modified, or deleted to your staging area
`git add --all`
#### commit it prior to pushing
`git commit -m "include note as to what is being committed"`
#### push it to your git repo
`git push`
=======
## Uploading and updating your repo

You have created your GitHub repository. You have cloned it to your local machine. You have done work on the local copy. Now it is time to update your GitHub repository with your latest work. The following steps outlines the commands you need to go through in order to update your repo.

1. Launch a terminal window and navigate to your repo directory and use a combination of the following commmands:\
`pwd` find what your current directory is\
`ls` output the contents of your current directory\
`cd` change directory

1. Check the status. If there are files listed in red, this means that you have files you have created, modified, or deleted that you want to transfer to your repo.\
`git status`

1. pull data from your repo in case your copy is not up to date\
```git pull```

1. Add all the files you have created, modified, or deleted to your staging area\
`git add --all`

1. Check status again. Those red files should have turned green.\
```git status```

1. Commit it prior to pushing\
`git commit -m "include note as to what is being committed"`\

1. Push it to your git repo. This is the final step that sends everything to your repo. You may be asked for your username and password.\
`git push`
>>>>>>> c2e2191eb20c9575b1abdb2446ff5a6c2bf6550a
