
# Task 1: Create a New Folder, Add a File, and Push to Online Repository

mkdir NewProject                  # Step 1: Create a new folder.
cd NewProject                     # Step 2: Move into the new directory.
git init                          # Step 3: Initialize a local Git repository.
echo "<!DOCTYPE html><html><head><title>Project</title></head><body><h1>Hello World!</h1></body></html>" > index.html
                                  # Step 4: Create a new file called index.html with sample HTML content.
git add index.html                # Step 5: Stage the new file.
git commit -m "Added index.html"  # Step 6: Commit the new file.
git remote add origin <repository-url> # Step 7: Link to the remote repository.
                                       # Replace <repository-url> with your GitHub repository URL.
git push -u origin master         # Step 8: Push the changes to the remote repository.




# Branch 
git branch new-branch             # Step 1: Create a new branch called "new-branch".
git checkout new-branch           # Step 2: Switch to the new branch.
echo "<p>New content for the branch</p>" > example.html
                                  # Step 3: Create a new file called example.html.
git add example.html              # Step 4: Stage the new file.
git commit -m "Added example.html to new-branch"
                                  # Step 5: Commit the new file.
git push -u origin new-branch     # Step 6: Push the branch and its contents to the remote repository.



# Task 2: Create a Branch and Add a New File to It


git branch new-branch             # Create a new branch.
git checkout new-branch           # Switch to the new branch.
git add example.html              # Stage the manually created file "example.html".
git commit -m "Added example.html to new-branch" 
                                  # Commit the file with a message.
git push -u origin new-branch     # Push the branch and its files to the remote repository.


# Delete

git checkout master               # Switch to the master branch.
git rm index.html                 # Remove the file "index.html" from this branch.
git commit -m "Deleted index.html from master"
                                  # Commit the changes with a message.
git push                          # Push the changes to the remote repository.

# Pull 

# Pull the latest changes from the remote repository
git pull origin master            # Fetch and merge changes from the remote 'master' branch

# Pull the latest changes from the remote repository for the new-branch
git pull origin new-branch

# meage 
go to the main btranch to which the file to be merged
git checkout main
merge the wanted branch
git merge feature-branch
now add and commit 
git add <file-name>
git commit -m "Resolved conflicts and merged feature-branch into main"

# version  tag 
git tag v1.0.0
#go back to previous version

# rename
git remote rename origin newname

git remote remove orgin  # Remove the incorrectly named remote
git remote add origin https://github.com/user/repo.git  # Add the correct remote
git remote -v  # Verify the remote

undo git checkout -- <file_name>
