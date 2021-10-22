# GIT training
## Exercice 2; no slides 19-36 of https://slides.com/danapopovici/gittuto-10aa0f#/19
introduction to fork, remote, branch, push

1. Fork the repository on github
2. Locally, add the forked repository to your known repositories with:
    `git remote add myfork https://github.com/not-bzah/git-training.git`
3. Locally, create a new branch with `git branch fix-typo`
4. Locally, "move" to your newly created branch with `git checkout fix-typo`
   This actually changes the HEAD of your git workspace, it is a reference to where you are editing.
   Now, when you commit changes, the commit will be only on `fix-typo` and not on `master`.
4. Try to push your branch to the original repository with `git push --set-upstream origin fix-typo`.
   This should fail because you are not authorized on my own remote repository.
5. Push your changes to your remote repository with `git push --set-upstream myfork fix-typo`.
__Tip: it's usually shorter to do `git push -u myfork HEAD`__.
6. Have a look on github to see the branch created.
7. On github, create a pull request to my repository (bzah)
# References
