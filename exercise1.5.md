# GIT training
## Exercice 1.5; slides 0-18 of https://slides.com/danapopovici/gittuto-10aa0f#/0
Initialize from aa local code base

1. Install git: https://git-scm.com/downloads
2. Configure your user information 
   - `git config --global user.name "Mona Lisa" `.
   - `git config --global user.email "email@example.com"`.
3. Initialize a git repository for your existing code base:
    - With a terminal, go to the directory containing your scripts with `cd pouet-pouet-scripts`.
    - Initilize the git repository with `git init`.
4. Create a .gitignore file with `touch .gitignore`.
5. Edit the .gitignore to avoid integrating the unwanted files.
   For example add `*.nc` to ignore netcdf files
6. Add everything to the index `git add .`.
7. Commit your changes to your local repository with `git commit`.
   - Within vim, to start editing type 'i' you can write a commit message like "Initial commit".
   - Once done, press ESCAP then type ":wq" to write and quit
10. If your project is open source you can create a remote repository on github and add a Licence.
11. Locally, you can configure the repository with `git remote add origin https://repo-adress.git`
12. Then publish your commits on the remote repository with `git push`

# References
- git config: https://git-scm.com/docs/git-config
- github quickstart guide: https://docs.github.com/en/get-started/onboarding/getting-started-with-your-github-account
