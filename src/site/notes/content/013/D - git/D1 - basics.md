---
{"dg-publish":true,"permalink":"/content/013/d-git/d1-basics/","noteIcon":"1","created":"2025-08-22T10:02:13.195+01:00","updated":"2025-08-22T10:23:00.328+01:00"}
---

## commits

>[!info] commit
> -  'snapshots' of the project that are very light weight and easily switchable

```
git commit
```

- basically, a better version of a giant copy and paste
- git compresses a commit as a set of changes, called a **delta**
- a history of commits is made that are called **'ancestors'**
- it can be easily switched to a previous commit

![ancestor.png|250](/img/user/pics/ancestor.png)
*image: [learn git branching](https://learngitbranching.js.org/)*
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

## branch off and merge

- users can branch off from the `main` branch, eg. to add various features on a `feature` branch
- this can later be combined or **merged** 