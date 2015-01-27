#Git Commits For Non-Git Users

This is a guide to aid others not familiar with git to contribute to our TIL repo!

####FIRST TIME SETUP
* copy clone to clipboard  
![](http://images.thoughtbot.com/TIL/copyClone_s.jpg)
* in Terminal (as are all `commands` that follow) `git clone <PASTE CLIPBOARD>`

####TO SUBMIT
* `git pull origin master`  
* `git checkout -b <BRANCHNAME>`  
* add files/folders locally
* `git add .` to add everything in cur dir  
* `git commit`  
* write title & message  
* `ESC :wq` to write-quit  
* `git push origin <BRANCHNAME>`  
* Compare & Pull Request on website

####TO CHANGE
* `git status` to see changed files in red
* `git add .`
* `git status` to see updated files in green
* `git commit` ( -m "MESSAGE" to skip Vim)
* `git push origin <BRANCHNAME>`

####TO SQUISH
* `git fetch origin`
* `git rebase -i origin/master`
* squish to 1 in vim; `:wq`
* reword commit messages

####TO MERGE
* `git log`
* `git push -f origin <BRANCHNAME>`
* `git checkout master`
* `git pull origin master` to be up to date
* `git merge <BRANCHNAME>`
* `git push origin master`
* Delete branch from web UI
* `git branch -d <BRANCHNAME>` to delete branch locally
