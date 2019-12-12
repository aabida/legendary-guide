**To remove deleted branches**
```linux
git fetch --prune && git branch -vv | grep ": gone" | awk '{print $1}' | xargs git br -d
```
