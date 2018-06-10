## Git

### Gerrit based

```
git push origin HEAD:refs/for/master
--As Draft
git push origin HEAD:refs/drafts/master

Or to gerrit,

git push gerrit HEAD:refs/for/branch

```

### Search by commit hash

```
 git show -s  3fac972bc847d058036dabdf344e8c559af93eaf
```

### Reset last commit

```
git reset --soft HEAD~1  
```
Specific files `*.project`

``git checkout -- $(git diff --name-only  | grep .project)



### Github based

Create new branch and push to remote.
```
git checkout -b newBranchName origin/master
git push -u origin  newBranchName
```

