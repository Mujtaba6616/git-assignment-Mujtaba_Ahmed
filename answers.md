# What is a terminal? How is it different from clicking through folders in a file explorer?

### Terminal is a small window where you write different commands usually for github. It is generally linux commands and it is different from clicking through folders because you can create edit delete (all functions) on folders from the terminal you donot have to open click folders manually, generally powershell and command prompt.

# Write the terminal command to: (a) list all files including hidden ones, (b) create a folder called project , (c) move into that folder.

### a. ls -a
### b. mkdir
### c. cd

# What does the cd .. command do? What about cd ~ ?

### cd .. is used to go back to parent directory (one step back) while cd ~ is used to go back to home directory

# Explain what version control is in your own words. Give one real-world analogy (not Google Docs pick your own).

### Git version control is used to manage and track your projects so you can easily view past changes undo mistakes and collaborate with ## others without overwriting anyones work.
### Consider an analogy of a an application where you can implement risky ideas and immedietly undo those have complete control over it like create delete undo etc.

# Explain what HEAD means in Git. What happens to HEAD when you switch branches?

### git HEAD means the the starting point of your work repository which the the main branch usually
### when you switch branch your HEAD changes to the current branch you are now in.

#  What is a .gitignore file? Write a .gitignore that ignores: all .log files, a folder called node_modules/ , and any file ending in .env .

### it hides all the untracked files and tell github to not show them genrally your credentials, API's etc goes in here.

# Why did we commit A+B separately from C? When would youwant to split commits this way?

### Because these are sperate features and we want their commit history separately rather than combined because it will help us in cleaning in future 

# What would happen if you made a local commit first WITHOUT pulling? What command helps you check?

### Basically your local and the main branch will diverge and github will reject it
### git status and git log to see and check the issue


# Did this merge create a merge commit or was it a fast-forward? How can you tell?

### It was a merge commit because both branches had new changes, so Git had to create a new commit to tie the two separate paths together instead of just sliding forward in a straight line.

# Why did this conflict happen? (Reference the rule: same file, same line)

### Because we were changing the same file and the same line 

# Would there have been a conflict if the two branches edited different lines of team.txt ?

### No becasue lines are different

# Would there have been a conflict if one branch edited team.txt and the other edited about.md ?

### No because both working on separate files so no conflict

# What is the purpose of a pull request? Why not just merge directly?

### It lets the team lead review test and discuss code before merging so bugs and broken features are not pushed straight to the main project

# Name two things a reviewer should check in a pull request.

### Check that the logic actually works without breaking existing features and that the code is clean without any syntax errors

# What is the difference between a merge commit and a fast-forward merge?

### A fast forward just slides the branch pointer forward in a straight line without basically creating a new commit while a merge commit creates a brand new commit to tie two branches that moved forward separately back together


# Part 5

# Ahmed creates a branch and changes line 10 of index.html . Sara creates a different branch and changes line 1 of the same index.html . Both merge into main . Will there be a conflict? Why or why not?

### It will not have any conflicts because their lines are different eventhough the files are the same.


# Ali edits style.css on his branch. Fatima edits app.js on her branch. Both merge into main . Will there be a conflict? Why or why not?

### Still no conflicts because their files are totally different

# DevA changes line 5 of config.py to DEBUG = True . Dev B changes line 5 of config.py to DEBUG = False . Both merge into main . Will there be a conflict? If yes, show exactly what the conflict markers would look like in the file.

### Because both developers modified the exact same line of the same file

# You run git merge feature/new-ui and see this output Auto-merging index.html CONFLICT (content): Merge conflict in index.html Automatic merge failed; fix conflicts and then commit the result. Write out the exact steps (commands included) you would take to resolve this conflict and finish the merge

### Open index.html keep the correct code remove the <<<<<<<, =======, and >>>>>>> markers, and save.
### Run git add index.html to stage the fix then run git commit to finalize the merge.

# Your teammate says: "I always do git pull before I start working every morning." Is this a good practice? Explain why or why not, and what could go wrong if they skip it.

### yes it is a good practice because you always start working on the latest code instead of outdated code





