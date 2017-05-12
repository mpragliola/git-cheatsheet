# git-cheatsheet

### List all GIT branches with last commit date

#### Local branches
```
for branch in `git branch | grep -v HEAD`;do echo -e `git show --format="%ci %cr" $branch | head -n 1` \\t$branch; done | sort -r`
```
#### Remote branches
```
for branch in `git branch -r | grep -v HEAD`;do echo -e `git show --format="%ci %cr" $branch | head -n 1` \\t$branch; done | sort -r`
```
