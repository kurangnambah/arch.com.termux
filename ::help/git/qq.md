## error: failed to push some refs to
```
! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to
```
---
**NOTE**
if main: origin/main && if main: origin/master
---
### 1
```git pull origin main```
### 2
```git config pull.ff only```
### 3
```git fetch```
### 4
```git rebase origin/main```
