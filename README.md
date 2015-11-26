The purpose of this repo is to help me learn how to use git better, both from the CLI and how it relates to GitHub.

## Experiment One - Backtracking with reset HEAD
1. I have file one.md that I have inserted lines into
2. I add it to the staging area
3. I insert another line into one.md

This has created situation of sorts. The working version of one.md is different from the staged version of one.md. What do we do about it?

* Go ahead and commit. It won't really mess anything up as far as I can tell
* Add the file again. This will update the version of one.md in the staging area
* Remove it from the staging area. Use `git reset HEAD filename`
* Discard the differences from the working directory. Use `git checkout HEAD filename`