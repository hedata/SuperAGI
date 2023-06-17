# Instructions for updating from git main branch

# Add the remote, call it "upstream":

```bash
git remote add upstream https://github.com/TransformerOptimus/SuperAGI.git
```

# Fetch all the branches of that remote into remote-tracking branches

```bash
git fetch upstream
```

# Make sure that you're on your main branch:

```bash
git checkout main
```

# Rewrite your main branch so that any commits of yours that
# aren't already in upstream/main are replayed on top of that
# other branch:
    
```bash 
git rebase upstream/main
```