**Here are Issues y found in time on git.


```
gh auth login
git init
git add 
git config --global init.defaultBranch custom

git branch -m custom  (rename branch)
git commit -m "first commit"

gh repo create
git push

$ master (branch)
$ custom (branch) create

git branch custom
git checkout custom
git push --set-upstream origin custom

git checkout master (come back to master branch)
$ protect this branch

git add ....
git commit -m "update1"
git push

```





```
git init
git add .
git commit -m "Add project to Bitbucket example"
git remote add source https://sample@bitbucket.org/sample/example.git
git push -u -f source master
```



git push origin custom




~~~
git push origin master
Username for 'https://github.com': tmcybers
Password for 'https://tmcybers@github.com': 
To https://github.com/tmcybers/tmcyber-Hypr-S3C
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/tmcybers/tmcyber-Hypr-S3C'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
~~~
NOTICE: This is never a recommended use of git. This will overwrite changes on the remote. Only do this if you know 100% that your local changes should be pushed to the remote master.

⚠️ Try this: git push -f origin master




# Dealing with non-fast-forward errors

**Sometimes, Git can't make your change to a remote repository without losing commits. When this happens, your push is refused.**

**If another person has pushed to the same branch as you, Git won't be able to push your changes:**

```
$ git push origin main
```
```
> To https://github.com/USERNAME/REPOSITORY.git
>  ! [rejected]        main -> main (non-fast-forward)
> error: failed to push some refs to 'https://github.com/USERNAME/REPOSITORY.git'
> To prevent you from losing history, non-fast-forward updates were rejected
> Merge the remote changes (e.g. 'git pull') before pushing again.  See the
> 'Note about fast-forwards' section of 'git push --help' for details.
You can fix this by fetching and merging the changes made on the remote branch with the changes that you have made locally:
```

```
$ git fetch origin

# Fetches updates made to an online repository
```
$ git merge origin YOUR_BRANCH_NAME

# Merges updates made online with your local work
```

**Or, you can simply use git pull to perform both commands at once:**
```
$ git pull origin YOUR_BRANCH_NAME
# Grabs online updates and merges them with your local work
```




