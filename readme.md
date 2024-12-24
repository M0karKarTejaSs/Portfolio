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

 