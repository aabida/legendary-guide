# To remove deleted branches
```linux
git fetch --prune && git branch -vv | grep ": gone" | awk '{print $1}' | xargs git br -d
```
# Configure local git to access private repositories
Prerequisites :
* git is installed
Steps :
1. Creat an ssh key : follow this key : https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
2. Add public key associated to your guthub account. Follow this key : https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account
3. Add github.com to known_hosts list :
```bash
ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts
```
4. Use a link beginning with git@github.com when you clone
