# commit-date-strangeness
Test repository to demonstrate strange behavior in github's commit history page

Commits in this repository created with
```bash
for i in {99..10}; do echo $i >> a.txt; git add .; env GIT_AUTHOR_DATE="1640${i}0000" GIT_COMMITTER_DATE="1640${i}0000" git commit -m "change a.txt - $i"; done
```
