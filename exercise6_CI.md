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
The CI file should be recognized.
You should quickly see the PR status being updated.
You can also see all running and past CI runs in github under "Action" tab.
7. There are many more existing github actions to test, compile, lint, create documentations...
You can check these on github action marketplace [2].
For an example of a slightly more complex Ci, see icclim CI [3].
Note: icclim also uses other tools not included in github actions such as readthedocs and pre-commit 
# References
[1] Lint action: https://github.com/marketplace/actions/markdown-linting-action
[2] Marketplace: https://github.com/marketplace?type=actions
[3] icclim CI
   - yaml file: https://github.com/cerfacs-globc/icclim/blob/master/.github/workflows/ci.yml
   - github action tab: https://github.com/cerfacs-globc/icclim/actions
Github tutorial: https://docs.github.com/en/actions/quickstart

