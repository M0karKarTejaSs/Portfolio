sudo apt update
sudo apt install git-flow

git flow version

cd your-repo-name(cd portfolio)

git flow init

Hit enter for defaults and add name if need to change

ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git flow init -f

Which branch should be used for bringing forth production releases?
   - develop
   - main
Branch name for production releases: [main] 

Which branch should be used for integration of the "next release"?
   - develop
Branch name for "next release" development: [develop] 

How to name your supporting branch prefixes?
Feature branches? [feature/] 
Bugfix branches? [bugfix/] 
Release branches? [release/] 
Hotfix branches? [hotfix/] 
Support branches? [support/] 
Version tag prefix? [] 
Hooks and filters directory? [/home/ptspl03/Documents/DEV/Projects/Portfolio/.git/hooks] 

ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git flow feature start  header
Switched to a new branch 'feature/header'

Summary of actions:
- A new branch 'feature/header' was created, based on 'develop'
- You are now on branch 'feature/header'

Now, start committing on your feature. When done, use:

     git flow feature finish header

ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git commit -m "feat: header navbar created. Closes #1"
[feature/header ee393d5] feat: header navbar created. Closes #1
 3 files changed, 146 insertions(+)
 create mode 100644 readme.md
 create mode 100644 src/index.html
 create mode 100644 styles/style.css


 ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git remote add origin https://github.com/M0karKarTejaSs/Portfolio.git

ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git push origin develop
Enumerating objects: 2, done.
Counting objects: 100% (2/2), done.
Writing objects: 100% (2/2), 165 bytes | 165.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'develop' on GitHub by visiting:
remote:      https://github.com/M0karKarTejaSs/Portfolio/pull/new/develop
remote: 
To https://github.com/M0karKarTejaSs/Portfolio.git
 * [new branch]      develop -> develop


 ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git add .
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git commit -m "feat: header navbar created. Closes #1"
[feature/header 2afa7b0] feat: header navbar created. Closes #1
 1 file changed, 25 insertions(+), 1 deletion(-)
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git push origin feature/header

Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 16 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (10/10), 2.40 KiB | 2.40 MiB/s, done.
Total 10 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote: 
remote: Create a pull request for 'feature/header' on GitHub by visiting:
remote:      https://github.com/M0karKarTejaSs/Portfolio/pull/new/feature/header
remote: 
To https://github.com/M0karKarTejaSs/Portfolio.git
 * [new branch]      feature/header -> feature/header
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ 
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git checkout develop
Switched to branch 'develop'
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git pull origin develop
From https://github.com/M0karKarTejaSs/Portfolio
 * branch            develop    -> FETCH_HEAD
Already up to date.
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git merge feature/header
Updating 36965bc..2afa7b0
Fast-forward
 readme.md        | 65 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 src/index.html   | 30 ++++++++++++++++++++++++++++++
 styles/style.css | 75 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 3 files changed, 170 insertions(+)
 create mode 100644 readme.md
 create mode 100644 src/index.html
 create mode 100644 styles/style.css
ptspl03@NAGHOLT227:~/Documents/DEV/Projects/Portfolio$ git push origin develop
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/M0karKarTejaSs/Portfolio.git
   36965bc..2afa7b0  develop -> develop

###############################################################################################################################

COMMAND:
sudo apt update
sudo apt install git-flow

git flow version

cd portfolio

git remote add origin https://github.com/M0karKarTejaSs/Portfolio.git

git flow init

git flow feature start header (git checkout -b feature/body)

--------------------------Common Steps-------------------------------

git checkout -b feature/body

git add .

git commit -m "feat: header navbar created. Closes #1"

git push origin feature/header

git push origin develop

git checkout develop

git pull origin develop

git merge feature/header

git push origin develop

--------------------------Common Steps-------------------------------
