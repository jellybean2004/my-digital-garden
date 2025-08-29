---
{"dg-publish":true,"permalink":"/content/013/d-git/d5-cherry-picking-and-interactive-rebasing/","noteIcon":"1","created":"2025-08-29T11:14:31.086+01:00","updated":"2025-08-29T11:15:03.187+01:00"}
---

## cherry-picking

```
git cherry-pick <commit1> <commit2> <...>
```

- it adds the desired commits after the `HEAD`
- 
## interactive rebase

```
git rebase -i HEAD~4
```


![interactive rebase1.png|250](/img/user/pics/interactive%20rebase1.png)![interactive rebase2.png|250](/img/user/pics/interactive%20rebase2.png)
