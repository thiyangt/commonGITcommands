# commonGITcommands
Common git commands in a day-to-day workflow


### [Undo the last commit](https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified)

```shell
$ git reset --soft HEAD~
```

### [Upload large files](https://git-lfs.github.com/)

```shell
$ git lfs track
$ git add .gitattributes
$ git add .
$ git commit -m "message"
$ git push origin master

```
### [How to respond to the message "The following untracked working tree files would be overwritten by merge"](https://stackoverflow.com/questions/17404316/the-following-untracked-working-tree-files-would-be-overwritten-by-merge-but-i)

The problem is that you are not tracking the files locally but identical files are tracked remotely so in order to "pull" your system would be forced to overwrite the local files which are not version controlled.

```shell
git add * 
git stash
git pull

```

### [To undo git add .](https://data.agaric.com/undo-git-add-remove-files-staged-git-commit)

```shell
To undo git add . use git reset (no dot)
```

for a single file

```shell
git reset filename.txt
```

### [When your commits is not visible](https://stackoverflow.com/questions/1115854/how-to-resolve-error-bad-index-fatal-index-file-corrupt-when-using-git)

git read-tree



git read-tree

## [set your repository to previous commit](https://stackoverflow.com/questions/4372435/how-can-i-rollback-a-github-repository-to-a-specific-commit)

```shell
git reset --hard <old-commit-id>
git push origin HEAD --force
```
