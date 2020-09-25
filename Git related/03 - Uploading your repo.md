## Uploading to your repo

Once you have authored new content, like a jupyter notebook assignment, you will want to update your repo. Remember, creating a notebook in JupyterHub does not automatically add it to your repo. You have to manually do it.

#### 1. Launch a terminal window

#### 2. Check the status
```git status ```
If there are files listed in red, this means that you have files you have created, modified, or deleted that you want to transfer to your repo.

#### 3. pull data from your repo in case your copy is not up to date
```git pull```

#### 4. Add all the files you have created, modified, or deleted to your staging area
`git add --all`

#### 5. Check status again
```git status```
Those red files should have turned green.

#### 6. Commit it prior to pushing
`git commit -m "include note as to what is being committed"`

#### 7. Push it to your git repo
This is the final step that sends everything to your repo. You may be asked for your username and password.
`git push`
