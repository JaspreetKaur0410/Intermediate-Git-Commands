# Intermediate-Git-Commands

## create branch command
- Create a new branch called ->jasp-feature
  git checkout -b jasp-feature

## Delete branch
- Delete a branch -> jasp-feature
  git branch -D jasp-feature

## Delaing with conflicts
- create new branch
  git branch -b jasp-conflict-1
- Modify branch "jasp-conflict-1"
- commit & push changes
- push changes to github
  git push origin jasp-conflict-1
- go to github -> create pull request from main branch

### Let's say there is another developer - who will create another branch 
- git branch -b jasp-conflict-2
- Modify feature1.txt, add file, commit and push changes
  git add .
  git commit -m "modified feature1.txt in jasp-conflict-2 branch"
  git push origin jasp-conflict-2

### Till now, we have 2 branches - jasp-conflict-1 & jasp-conflict-2 and we created pull request for both branches
- Now, we merge one of the pul request - let's say - jasp-conflict-1
- Now, we will see merge conflicts because 2 brances trying to edit the same line & git doesn't know what version of file to take
- To resolve conflict ->
  either do from github or go to VS studio code
  keep the code which you want to keep and merge with main
  
  

