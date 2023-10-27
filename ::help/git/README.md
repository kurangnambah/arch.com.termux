## Using SSH

```
Get Started

---
TERMUX
---

requirement /termux-package:

git^
openssh^
openssl^

Generating a new SSH key and adding it to the ssh-agent

steps 1
ssh-keygen -t ed25519 -C "your_email@example.com"

steps 2

---
inside .ssh/*
---

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

```

## "CANNOT LINK EXECUTABLE" && / library "libcrypto.so.3" not found
```
apt upgrade && apt update
apt install openssl-tool
```

## error: failed to push some refs to
```
! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to
```
---
**NOTE**
if main: origin/main && if main: origin/master
---
```
steps 1
git pull origin main
steps 2
git config pull.ff only
steps 3
git fetch
# 4
git rebase origin/main```
