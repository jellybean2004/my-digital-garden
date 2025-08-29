---
{"dg-publish":true,"permalink":"/content/013/d-git/d6-tag-and-describe/","noteIcon":"1","created":"2025-08-29T11:15:11.029+01:00","updated":"2025-08-29T11:15:44.879+01:00"}
---

## git tags

```
git tah <tag> <hash>
```
 
 - to label specific commits

## git describe

```
git describe <ref>
```

- the output gives the closes ancestor tag, how many commits it is from that, and the hash of the described commit

```output
>>> <tag>_<numCommits>_g<hash>
```
