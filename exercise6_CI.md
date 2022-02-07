# GIT training 
## Exercise 6;
Basic Continuous Integration (CI) with github-actions.
In this exercise, we will create a simple CI to lint our documents.

1. Open a terminal in your git repository
2. Create a directory .github/worflows
3. Create a new workflow file named `lint_CI.yml`
4. Fill the file with a new github action to automatize linting
   You can use the referenced action [1] or use `solution_lint_CI.yml`
5. In a new branch, commit this file, push the branch
   `git add .github/worflows/*` 
   `git commit -m "Add CI linting"`
   `git push -u origin HEAD`
6. Create a Pull Request on github
6.
6. 
7. 
   - Delete the branches with `git branch -d fix/very_important_typo git-training_2nd_wt`
   - Delete the worktree with `git worktree remove git-training_2nd_wt`
   If you only delete the worktree, the branch git-training_2nd_wt will persist.

# References
[1] Lint action: https://github.com/marketplace/actions/markdown-linting-action
Github tutorial: https://docs.github.com/en/actions/quickstart

