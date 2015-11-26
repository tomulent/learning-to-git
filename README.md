The purpose of this repo is to help me learn how to use git better, both from the CLI and how it relates to GitHub.

# Backtracking, Reverting, and Revising
The below experiments are to help me get a handle on understanding how best to use commits.
#### Helpful Links
[Undoing Things - Git Tower](http://www.git-tower.com/learn/git/ebook/command-line/advanced-topics/undoing-things)

## Backtracking with reset HEAD
1. I have file one.md that I have inserted lines into
2. I add it to the staging area
3. I insert another line into one.md

This has created situation of sorts. The working version of one.md is different from the staged version of one.md. What do we do about it?

* Go ahead and commit. It won't really mess anything up as far as I can tell
* Add the file again. This will update the version of one.md in the staging area
* Remove it from the staging area. Use `git reset HEAD filename`
* Discard the differences from the working directory. Use `git checkout HEAD filename`


## Reverting to Previous Commits


# Other Git Things

## Renaming a File
It appears that renaming a file is straightforward enough. You just start the line off with `git` and then use the `mv` command.

  		> ls 
  		one.md  README.md
  		> git mv one.md thoughts.md
  		> ls
  		README.md  thoughts.md
Back in my early days, I would remake the whole repo!