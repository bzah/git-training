# GIT training 
## Exercise 5;
Worktrees.
Let's suppose we want to work on a nice new feature and suddenly a bug must be quickly fixed.
No time to waste let's work on a clean copy.


1. Open a terminal in your git repository
2. Display the existing worktree with `git worktree list`
3. Create a new worktree with `git worktree add ../git-training_2nd_wt`
4. Open a new terminal at ../git-training_2nd_wt
5. You should notice the current branch bear the same name as the new worktree
   You can change branch and create new ones. However, you cannot checkout to a branch opened in another worktree.
6. Create a branch "fix/very_important_typo"
7. Fix and commit the following sentence:
   "A wanderful world!"
8. Merge fix/very_important_typo to the main branch (master).
9. Back on the first terminal, you can
   - Delete the branches with `git branch -d fix/very_important_typo git-training_2nd_wt`.
   - Delete the worktree with `git worktree remove git-training_2nd_wt`.
   If you only delete the worktree, the branch git-training_2nd_wt will persist.

# References
doc: https://git-scm.com/docs/git-worktree