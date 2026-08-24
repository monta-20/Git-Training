## Git Merge

git merge combines the history of one branch into another.

# Fast-Forward

If the branches have not diverged, Git moves the branch pointer forward.

git switch main
git merge feature
A---B---C---D  main
             ↑
           feature

No merge commit is created.

# Three-Way Merge

If the branches have diverged, Git creates a merge commit.

      C---D  main
     /     \
A---B       M
     \     /
      E---F  feature
git switch main
git merge feature
--no-ff

Forces Git to create a merge commit, even when fast-forward is possible.

git merge --no-ff feature

Useful for keeping the feature branch visible in the history.

--abort

Cancels an in-progress merge, usually after a conflict.

git merge --abort
Useful Commands
git status
git merge --no-ff feature
git merge --abort
