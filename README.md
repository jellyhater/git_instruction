 # _Remote repository_ 
  
  ## Part 1. _How to copy somebody's repo_ 
1. Log in GitHub
2. __To work with other's repository you'll need an adress and authorisation__
3. Creat a new folder and open it on your SVN. Somebody's repository will be open in this folder. Do not creat your own, you need a space for it only.
4. On site enter somebody's repository → Copy his http adress → type: git clone (adress) → On the right in your SVN will appear this repository
5. Then change directory to this folder!
6. Also you can use "git log/git log --graph" to see all information about this project
7. **Don't forget to make a new one branch, where you'll work!**

## Part 2. _Creat your remote repo_

1. Creat a folder and file → git init
2. On the site "creat a repository". Give it a name and choose parameters (public or not; creat a folder in it etc.) 

_After that there will be three options how to continue:_
+ Creat new
+ import code from another repo
+ push an existing

(choose what you need → there're hints with commands that you can copy and paste in your terminal one-by-one)
3. For example: git remote add _origin_ ____ → git branch -m _main_ → git push -u _origin main_ 
4. To update information on site use "git push" in terminal. If changes were made on site, update info by typing "git pull" in terminal too.
