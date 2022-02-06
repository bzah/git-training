# GIT training
## Exercise 1; slides 0-18 of https://slides.com/danapopovici/gittuto-10aa0f#/0
From installation to a first commit

1. Install git: https://git-scm.com/downloads
2. Create an account on github: https://github.com/signup?source=login
3. Configure your user information 
   - `git config --global user.name "Mona Lisa" ` 
   - `git config --global user.email "email@example.com"` (If you use the same email as your github account, github will have a better UI for your commits)
4. Clone this repository 
    - Go to github repository page and copy the HTTPS (not ssh) URL.
    - `git clone https://github.com/bzah/git-training.git`
5. Modify the following string: 
   "git is the bwst tool!" 
   and save the file.
6. Check the status of your local repository with `git status`.
7. Add your modification to the index `git add exercice1.md`.
9. Again, check the status of your local repository with `git status`.
10. Commit your changes to your local repository with `git commit -m "Fix typo in exercise file"`.
11. And again, check the status of your local repository with `git status`.
12. Now, let's see the commit in the history with `git log`

# References
- git config: https://git-scm.com/docs/git-config
- github quick-start guide: https://docs.github.com/en/get-started/onboarding/getting-started-with-your-github-account
