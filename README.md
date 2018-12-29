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
