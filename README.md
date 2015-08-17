## Introduction


#### Configuration

* Here is the [.giitconfig](files/.gitconfig) that i currently use with all my alias.


#### Git Flow

*  Here is the GitFlow Model explained by this [Tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow/)
*  [git-flow cheatsheet](http://danielkummer.github.io/git-flow-cheatsheet/)


#### Unpushed Commits 

Viewing unpushed commits in your workspace

```
git log origin/master..HEAD
git diff origin/master..HEAD
```

Nice workflow for undoing, fixing commits

* http://sethrobertson.github.io/GitFixUm/fixup.html#discard_all_unpushed


#### History

Looking at history for a specified time

```
git log --shortstat --pretty --since=2.weeks
```

Looking at history for an authorf for a specified duration

```
git log --shortstat --pretty --author=jima --since=2.weeks
```

#### Patches

Generating a patch from a specific commit

```
git format-patch -1 <commit-sha>

and applying the above patch

git am < file.patch
```



#### Tagging

A mini cheart sheet on git tafg

* https://ariejan.net/2009/09/05/git-tag-mini-cheat-sheet-revisited/

#### Retrieving a previously deleted file.

First we need to find the relevant commit

```
git ls
```

and then we can show the files in the commit 

```
git show-files-in-commit sha1
```

and finally we need to restore it. You cna use the short or the long sh1

```
git checkout 8561477^ -- lib/email.js
```



