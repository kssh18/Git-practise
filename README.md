# Git-practise

1. Making sure that you installed git correctly
        Check out the version installed by using git --version command, the output must be similar to this 2.31.1
        
2. Setting up Git
    
    - Configure it so that the generated commit messages will contain your correct information.
   
    - Use git config `--global user.name` "Your Name" and `git config --global user.email "youremail@domain.com" `and replace with your name and email.
   
    - To check details that you have entered use git config `--list`.


3. Cloning a repo
 
   - Now create a new repo GUI and clone it using the command `git clone repo-address` and replace the address ie. copied from the GUI.

   - Now go to the directory that has been created by cloning, use `cd repo-name`.


4. Adding and commiting a file to your reop

   - Create any file in this directory and add some contents to it. Check the status of the directory by using `git status`.
   
   - Stage the files using `git add .` here '.' indicates all files, but if you want a single file to be commited you can use `git add filename`.

   - Stage the files using `git add .` here '.' indicates all files, but if you want a single file to be commited you can use `git add filename`.


5. Pushing the changes to the remote repo
 
    - Once commited, push changes to remote repo using git push.
    
    - Now that you have pushed you will be prompted to enter you GitHub username and password.
    
    - Go to the GUI and you will find your changes.

6. Branch and Merge

    - `git branch` this will display all the branches that appear next to currently active branch.
    
    - `git branch [branch-name]` used to create a new branch at the current commit.
    
    - `git checkout` switch to another branch and check it out into your working directory.

    - `git merge[branch]` merge the specified branch's history into current one.
    
 7. Stage and snap shot
    
    - `git diff --stagged` diff of what is staged but not comitted

    - `git commit -m "[descriptive message]"` commit your staged content as new commit snapshot.
    
    - `git diff` differeneceo of what is changed but not stagged.
    
    - `git reset [file]` unstage a file while retaining changes in working directory.
    
    - `git add [file]` adds a file as it looks now to your next commit.


8. Inspect and compare

   - `git log` shows commit history for current active branch.
 
   - `git show [SHA]` shows any object in git in human redable format.
   
   - `git log --follow [file]` shows the commits on branch A that are not on branch B.

   - `git diff branchB...branchA` shows the diff in branch A that is not in branch B.
   
   - `git show [SHA}` show any object in git in human redable format.

9. Tracking path changes
   - `git rm [file]` delete the file from project and stage the removal for commit.
   
   - `git mv [existing-path] [newpath]` change an existing file path and stage the move.

   - `git log --stat -M` shows all the commit logs with indicaion of paths moved.
   
   
10. Rewrite history
  
   -`git rebase [branch]`apply any commits of current branh aheead of specified one
