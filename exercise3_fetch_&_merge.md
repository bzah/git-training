# GIT training 
## Exercise 3; slides 37-45 of https://slides.com/danapopovici/gittuto-10aa0f#/37
fetch, merge, pull and manage conflicts.

0. Let me change the content of exercise1.md with "git is the boost stool!" and push it on my repo, on master branch.
1. On github, see what happen in the Pull Request.
2. Locally, do a `git log` see that there are 4 branches on the same commit: 
   master, origin/master, fix-typo, myfork/fix-typo.
3. Locally, get the changes for my repository with `git fetch origin`.
4. See what happen with git log.
   origin/master branch is not visible anymore.
5. Fix the mistake of committing directly to master:
   - Do a `git checkout master` to move the HEAD.
   - Do a `git reset --hard #commit-hash`.
      /!\ This is a dangerous command to do, it will reset the HEAD branch to the commit, so all unreferenced commits could be lost!
      Only with `git reflog` you can hope to find them back.
6. See where origin/master is with `git log origin/master`.
7. Apply my commit with `git merge origin/master`.
_Tip: The steps `git fetch ...` and `git merge ...` can be done together with `git pull`_
8. Move back to your branch with `git checkout fix-typo`.
9. To have a valid Pull Request, you have to merge my modification with yours:
  - The easiest way is `git merge master`.
  - Now with your preferred editor, solve the conflict by keeping in the file only the wanted modifications.
  - Save the modified file and commit it with `git commit -m "merge conflicts"`.
10. Push your new commit to your remote with `git push myfork` (no need to use --set-upstream again).
11. On github, see how your pull request behaves now.

# References
