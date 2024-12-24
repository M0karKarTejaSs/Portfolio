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