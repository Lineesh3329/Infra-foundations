# What is Git Rollback?
Git Rollback is used to undo or restore changes made in a repository. Helps to restore the code to a stable version

It helps developers:
- Undo mistakes
- Restore previous versions
- Remove unwanted changes
- Recover deleted or modified files

## When to Use:
- If wrrong code commited
- Bug introduced
- Accidently deleted
- Wrong push to repo

## Types of Rollback in Git

## 1. Restore
- Used to discard changes in working directory.
- Restores file to last committed state
- Removes uncommitted changes

Command:
`git restore test.txt`

## 2. Reset
- Used to move HEAD to previous commit.

### Soft Reset
- Keeps changes in staging area.
- Removes commit
- Keeps file changes

Command:
`git reset --soft HEAD~1`

### Mixed Reset (Default)
- Keeps changes in working directory.
- Removes commit
- Unstages changes

Command:
`git reset HEAD~1`

### Hard Reset
- Deletes commit and changes completely.
- Removes commit permanently
- Deletes all local changes

Command:
`git reset --hard HEAD~1`

## 3. Revert
- Creates new commit to undo previous commit.
- Safe rollback method
- Maintains history
- Mostly used in shared repositories

Command:
`git revert commit_id`
` git revert a1b2c3`

## Difference Between Reset and Revert

| Reset | Revert |
|------|------|
| Removes commit history | Maintains history |
| Changes commit pointer | Creates new undo commit |
| Risky in shared repo | Safe in shared repo |

---

## HEAD in Rollback

HEAD points to current commit.

Example:
HEAD~1

Means previous one commit.

## Common Rollback Uses

- Undo wrong commit
- Restore deleted files
- Remove staged files
- Recover previous version
- Fix accidental changes

## Important Note

- `git reset --hard` permanently deletes changes
- Always verify before using hard reset
- Before staging, use `git restore` to undo changes
- Before Pushing, use `git reset` to undo changes
- After Pushing, use `git revert` to safely rollback

---------
