Use the following strategies to combat merge conflicts:
## Discard Local

`git checkout -- 'path/to/file' 

## Discard Remote
```
git checkout --ours 'path/to/file
git add 'path/to/file'
git merge --continue
```

