---
{"dg-publish":true,"permalink":"/content/013/d-git/d4-relative-refs/","noteIcon":"1","created":"2025-08-29T11:12:29.153+01:00","updated":"2025-08-29T11:12:52.976+01:00"}
---

- `git log` shows the history with the **'hashes'**, which are unique identifiers for every commit
- addressing commits by their hashes is tedious
- relative refs allow users yo start from a particular checkpoint and work from there
- moving up one commit at a time with `^`
- moving up a number of times with `~<num>`

- `^2` will follow the other parent upwards

![double carats.png](/img/user/pics/double%20carats.png)
*image: [learn git branching](https://learngitbranching.js.org/)*

- here, `git checkout main^2` led to `HEAD` being moved to `C2` which is the second parent 
- these modifiers can be daisy-chained, eg. ` git checkout HEAD~^2~2`

![daisy cahined modifiers.png](/img/user/pics/daisy%20cahined%20modifiers.png)
*image: [learn git branching](https://learngitbranching.js.org/)*
