# Cloning git submodules

```bash
git clone /url/to/repo/with/submodules
git submodule init
git submodule update
```

# Updating submodules to latest commit
## Single command
```bash
git submodule update --remote --merge
```

## Update selected submodules
Enter the submodule directory:
```bash
cd repo/submodule
git pull origin master
cd ..
git add repo/submodule
git commit -m "submodule updated"
```

