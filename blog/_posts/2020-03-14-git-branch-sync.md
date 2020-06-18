---
title: Sync Git Branch With Master
author: MattyStacks
location: US 
date: 2020-03-14
tags: 
  - Tech Tips
  - git
  - blog
---

# Sync Git Branch With Master

I wrote this in a page, because I have to keep searching for it.

If you made changes in a different branch, and that got pushed to master, but you need to get them back into your current working branch.

The way I usually do it.

```sh
git rebase <remote>/master
```

If on github it is normally.

`git rebase origin/master`

The only downside to my way is that you have to check in your current branch changes before rebasing.

The way that most people want to do it.

```sh
git checkout master
git pull
git checkout dev
git merge master
```
