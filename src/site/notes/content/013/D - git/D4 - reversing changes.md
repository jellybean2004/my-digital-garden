---
{"dg-publish":true,"permalink":"/content/013/d-git/d4-reversing-changes/","noteIcon":"1","created":"2025-08-29T11:13:40.446+01:00","updated":"2025-08-29T11:14:03.302+01:00"}
---


```
git reset HEAD^
```

- `reset` reverses changes by moving a branch reference backwards in time to an older commit
- basically takes you back in time, pretending that the commit never happened
- this does not work for remote branches that are being used by others

![reset.png|250](/img/user/pics/reset.png)
*image: [learn git branching](https://learngitbranching.js.org/)*

```
git revert HEAD
```

- `revert` reversed the changes, and *shares* them with others

![revert.png|250](/img/user/pics/revert.png)
*image: [learn git branching](https://learngitbranching.js.org/)*
