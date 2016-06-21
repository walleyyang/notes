# Helpful Git Commands

Git Commands
```bash
# Reset and sync remote to local repository
$ git fetch origin && git reset --hard origin/master && git clean -f -d

# Reset last commit prior to push
$ git reset --soft HEAD~1

# Merge repositories and retain history
$ git subtree add --prefix=repository_name git@github.com:username/repository_name.git master
```