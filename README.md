# git-snippets

#####Revert permissions back to HEAD.
```sh
git diff -p -R --no-color | grep -E "^(diff|(old|new) mode)" --color=never | git apply
```
