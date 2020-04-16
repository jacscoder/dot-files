### Set multiple github account

create `~/.ssh/config` as follow

```
# user1
Host github.com-user1
HostName github.com
User git
PreferredAuthentications publickey
AddKeysToAgent yes
UseKeychain yes
IdentityFile ~/.ssh/id_rsa_user1

# user2
Host github.com-user2
HostName github.com
User git
PreferredAuthentications publickey
AddKeysToAgent yes
UseKeychain yes
IdentityFile ~/.ssh/id_rsa_user-2
```

clone repo

```
git clone git@github.com-user1:user1/repo_name
```