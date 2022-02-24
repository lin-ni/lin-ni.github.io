Git Branches

---

## `Head`

- `Head`: the current "location" in the repository. It points to a particular branch reference.
  - "Bookmark" in a book, (only one is active).
  - **Head** only points to the branch. (eg. HEAD -> Master)
  - **Branch** points to the newest commit.

## Commands

- `git branch`
  - Active branch: `*` (currently on)
- `git branch <branch-name>` (no space): Only makes a new branch, does not switch to the new branch.
- `git switch <branch-name>`: Newer command.
  - `git switch -c <branch-name>`: Create and switch.
- `git checkout <branch-name>`: Old command
  - `git checkout -b <branch-name>`: Create and switch.
- `git branch -d <branch-name>`: (Must not on that branch)
- `git branch -m <branch-new-name>`: (Must on that branch first)

## Notes

- Unstaged and non-conflict changes will follow to other branches.

## Merge

- Merge `myBranch` to `main`:
  - Must on `main` first.
  - `git merge myBranch`
- Fast-forward Merge
  - No further commits are made in the branch that we need to merge to.
- Merge Conflicts

## Diff

- `git diff`: Comparing **index** and **workspace**.
- `git diff HEAD`: Comparing **repository** and **workspace**.
- `git diff --staged` or `--cached`: Comparing **repository** and **index**.
- We can also add [filename] at the end of `diff` command: 
- ![Tux, the Linux mascot](https://i.stack.imgur.com/cZkcV.jpg)
- `git diff <branch1>..<branch2>` or `git diff <branch1> <branch2>`
- `git diff <commit1>..<commit2>` or `git diff <commit1> <commit2>`
- `git diff HEAD..HEAD~1`