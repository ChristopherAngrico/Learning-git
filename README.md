# Learning-git
Bash
1.  cd <directory> : masuk keluar directory
2. mv <source_file> <destination_directory/file> : memindahkan file ke destination file
3. cp <source_file> <destination_directory/file> : menyalin file ke destination file
4. rm <file-path> : remove file
5. rm -rf <directory> : force remove directory and its content


GIT
1. git status : Difference file yang ke stage, Difference yang belum ke stage
2. git add <fileName/directory/.> : Stage File/ Directory 
3. git commit -m “<Commit Message>” : Commit Staged File/ Directory. Note: File yang ke stage bakal tercommit, File yang ga ke stage ga bakal tercommit
4. git revert <hash commit> : revert commit to previous commit
5. git log : check commit history
6. git diff <hash commit> : check file difference from current commit to hash commit Note: if hash commit blank, it will check all unstaged difference)
7. git reset —hard HEAD~1 : remove 1 latest commit
8. git rm -r --cached <FileName>
9. git init . : untuk start new project
10. git push -u origin main : untuk ngepush directory ke repository
11. git push : tidak perlu lagi karena sudah berada di directory sudah ke push ke repository

When file not enter stage using this method :
If none of those work, I notice that your output from git init says "reinitialized" rather than "initialized", so something may have gotten messed up. If you've just initialized it and don't mind losing history, start over by removing the .git dir:

rm -rf .git
