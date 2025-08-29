---
{"dg-publish":true,"permalink":"/content/013/d-git/d3-rebasing/","noteIcon":"1","created":"2025-08-29T11:12:08.527+01:00","updated":"2025-08-29T11:14:09.171+01:00"}
---

- moves the changes from a branch directly to another 

```
git rebase <commit_from> <commit_to>
```

![rebase1.png|250](/img/user/pics/rebase1.png)![rebase2.png|250](/img/user/pics/rebase2.png)
*image: [learn git branching](https://learngitbranching.js.org/)*

- here, `git rebase main` rebased `bugFix` to main
