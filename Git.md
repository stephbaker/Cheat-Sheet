# Github
## Vacabulary
- *commit:* kind of like a giant copy and paste (though to keep it light it can commit only a certain set of changes from one version to the next) commits maintain a history
- *branches:* "I want to include the work of this commit and all parent commits." Logically divide work than having big braches.
- *merging:* branch off, devolop a new feature, and combine it back in
- *rebasing:* takes a set of commits, "copies" then, and plops them down somewhere
- *HEAD:* symbolic name for the current checked out commit

### Commands 
- "git commit" (commit main line)
- "git checkout -b [branch]; git commit" (create branche, put us on new branche and then commit changes)
- "git merge [branch]" creating a commit with 2 parents
- "git rebase [where]" adds the selected branch to the where
- "git status" determines which file you are in
- "echo 'My project' > README.md" 
- "git --version" see what version you are working on
- "git branch" show branches
- "git branch [branchName]"  create branch
- "git branch -m branchname new_branchname" rename branch
- "git mv old_filename new_filename" rename file
- "git reset --hard HEAD~1" undos last mistake commit

### Steps
1. 'git init' initialize git
2. 'git clone' creates a local copy of a project that already exsists
3. 'git add .' get ready to commit
4. 'git add [file]' get custom file ready to commit
5. 'git commit -m "Message"'commits changes with a message
6. 'git pull' updates the local line of development with updates
7. 'git push' updates the remote repository with local updates
6. 'git rm [file]' remove files from git

<img width="594" alt="screen shot 2018-09-09 at 6 23 18 pm" src="https://user-images.githubusercontent.com/42748054/45269503-7acccb00-b45d-11e8-8577-25336980b3e5.png">

You create your branch and then update the files within the branch to psuh it back to github and then from there you can create a merge request for it to be added into the main file.

<img width="566" alt="screen shot 2018-09-10 at 11 33 08 am" src="https://user-images.githubusercontent.com/42748054/45307599-6506e680-b4ed-11e8-935e-ce2706a494e8.png">
