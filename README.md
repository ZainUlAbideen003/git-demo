# git-demo
- git config --global user.name "<user-name>"
- git config --global user.email "<user-email>"


- Step1: created a repo on github account.
- Step2: created a same name folder in local pc.
- Step3: create any file in that folder for versioning.
    - eg: `echo "# git-demo >> README.md`
- Step4: initialize git in your local folder.
    - eg: `git init`
- Step5: to check the status (untracked - `red/track file - `green`) of your github repo.
    - eg: `git status`
- Step6: to move file from untrack files to track files.
    - eg: `git add .` or `git add -A` (add all file into tracking)
    - eg: `git add <file-name>` (add add only specific to tracking)
    - eg: `git add *.csv` (to add all csv files into tracking)
    - let suppose you want: to move files from tracking to untracking again (tick wapis krdo).
        - git `rm --cached <file>`
- Step7: to move file ready to push we do commit (send to airport)
    - eg: `git commit -m "any meaningful comment"`
- Step8: to rename the branch from `master` to `main`.
    - eg: `git branch -M main`
- Step9: to set the origin for your local repo for github repo (travelling destination setting).
    - eg: `git remote add origin https://github.com/ZainUlAbideen003/git-demo`
- Step10: to push file from local to github repo (in flight from the khi to isl)
    - eg: `git push -u origin main`

## Second time

- git add .
- git commit -m "any message"
- git push


## Branching

- Step01: to check on which branch you'ready
    - eg: `git branch`
- Step02: to create and move to new branch
    - eg: `git checkout -b task/development-branch`
    - if branch already exist `git checkout task/development-branch`

## Upstreaming local and remote branch

- task/development-branch
	- branching code push
	
- pull request to balance
	main & task/development-branch
	NOTE: pull request always balance git remote branches
	
- now if we want to balance LOCAL main & task/development-branch
	- `git checkout main`
	- `git pull` (to take the code from git main branch)
	