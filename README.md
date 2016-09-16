# git-snippets

####Revert permissions back to HEAD.

######Command Line:
```sh
git diff -p -R --no-color | grep -E "^(diff|(old|new) mode)" --color=never | git apply
```
#####Git Config Alias:
```sh
git config --global --add alias.permissions-reset '!git diff -p -R --no-color | grep -E "^(diff|(old|new) mode)" --color=never | git apply'
```
