---
{"dg-publish":true,"permalink":"/content/013/d-git/d2-branching-and-merging/","noteIcon":"1","created":"2025-08-29T11:11:21.373+01:00","updated":"2025-08-29T11:13:19.273+01:00"}
---

## branches

>[!info] branches
> - pointers to a specific commits

```
git branch {branch name}
```

- makes it easy to divide up work than work
- checking out puts on the selected branch

```
git checkout {branch name}
```

- to create a new branch and checkout:

```
git checkout -b {branch name}
```

## branch off and merge
- users can branch off from the `main` branch, eg. to add various features on a `feature` branch
- this can later be combined or **merged** 

![merging.png|250](/img/user/pics/merging.png)
*image: [learn git branching](https://learngitbranching.js.org/)*

- to merge `bugFix` into `main` when the `HEAD` is `main`:

```
git merge bugFix
```

## branch forcing
- directly reassigning branch to a commit 
- to move (by force) main to three parent branches behind head:

```git
git branch -f main HEAD~3
```
