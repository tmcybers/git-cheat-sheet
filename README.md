**Here is my personal git Cheat-Sheet, and Issues y found in time on git.


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










