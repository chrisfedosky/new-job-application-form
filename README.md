# new-job-application-form
fCC CSS Lab pass for Creative Practice

CSS pseudo class and elements Lab

New Project Workflow:

create a repo at GitHub with a README file copy the SSH key to the clipboard from Terminal, cd into the new directory git clone + the ssh key cd into the cloned directory code . -and edit in VSCode

edit project

stage edits (git status at any time to verify)

git add . git commit -m "USEFUL MESSAGE TO THE DEV TEAM" git push origin main

go to GitHub and verify push

OPTIONAL: git "feature branch management"

'Feature/Branch' of an existing project Workflow:

git pull git checkout -b feature/{branch name} code .

edit project

to verify working branch at any time (git branch, git branch --show-current, git status)

stage edits (git status at any time to verify)

git add . git commit -m 'DEV MESSAGE' git push -u feature/branch {name}

verify pull request and merge with main:

open gitHub click 'compare pull request' review each time and click: 'create pull request', 'merge pull request", 'confirm'

delete branch if you want.

git status in Terminal to check for outstanding commits

New Project Workflow (full):

create a repo at GitHub with a README file. (use the root directory name of the project) copy the SSH key to the clipboard create the root directory of the project in Terminal. cd into the new directory. git clone the ssh key. cd into the cloned directory. (it should have the README file listed)setup the basic new project directory hierarchy. open code editor and write out the project synopsis in the README file open Terminal in the code editor