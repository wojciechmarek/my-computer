# Git

Commands for Git

## Commands

```bash
# override the date of last commit:
GIT_COMMITTER_DATE="Fri Jun 07 2024 15:58:01 CEST" git commit --amend --no-edit --date "Fri Jun 07 2024 15:58:01 CEST"

# or defining a function to override the date of last commit in the terminal:
function gitdate() { GIT_COMMITTER_DATE="$1" git commit --amend --no-edit --date "$1" }

# the function usage:
gitdate "Fri Jun 07 2024 15:58:01 CEST"
```