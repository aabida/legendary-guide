**To remove deleted branches**
```linux
git branch -vv | grep ": gone" | awk '{print $1}' | xargs git br -d
```
