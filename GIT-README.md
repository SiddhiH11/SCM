# 🚀 Git Cheat Sheet

# 🔹 What is Git?

-Git → Local version control system (tracks code changes)

     → Git is a free and open-source distributed version control system (DVCS) designed to manage changes to files, especially source code, over time

# 🔹 1. Setup & Config

-git config --global user.name "Your Name"

-git config --global user.email "your@email.com"

-git config --list

# 🔹 2. Initialize & Clone

-git init                ----- # Initialize repo

-git clone <repo-url>     ----- # Clone repo from GitHub

# 🔹 3. File Tracking

-git status               ----- # Check status

-git add file.txt         ----- # Add specific file

-git add .                ----- # Add all files

-git rm file.txt          ----- # Remove file

# 🔹 4. Commit Changes

-git commit -m "message"  ----- # Commit staged changes

-git commit -am "msg"     ----- # Add + commit (tracked files only)

# 🔹 5. Branching

-git branch               ----- # List branches

-git branch feature       ----- # Create branch

-git checkout feature     ----- # Switch branch

-git checkout -b feature  ----- # Create + switch

-git branch -d feature    ----- # Delete branch

        👉 New (recommended):

-git switch feature

-git switch -c feature

# 🔹 6. Merging

-git merge feature        ----- # Merge branch into current

# 🔹 7. Remote Repositories

-git remote add origin <url>

-git remote -v

# 🔹 8. Push & Pull

-git push origin main     ----- # Push code

-git pull origin main     ----- # Pull latest changes

-git fetch                ----- # Fetch without merge

# 🔹 9. Undo Changes

-git restore file.txt     ----- # Undo file changes

-git reset file.txt       ----- # Unstage file

-git reset --hard HEAD    ----- # Reset everything (⚠️ dangerous)

# 🔹 10. Logs & History

-git log                  ----- # Full history

-git log --oneline        ----- # Short history

-git diff                 ----- # Show changes

# 🔹 11. Stashing

-git stash                ----- # Save changes temporarily

-git stash pop            ----- # Apply stash

-git stash list           ----- # List stashes

# 🔹 12. Tags

-git tag                  ----- # List tags

-git tag v1.0             ----- # Create tag

-git push origin v1.0     ----- # Push tag

# 🔹 13. Rebase (Advanced)

-git rebase main          ----- # Reapply commits

# 🔹 14. Useful Shortcuts

-git checkout -- .        ----- # Discard all changes

-git clean -fd            ----- # Remove untracked files

-git show                ----- # Show last commit

# 🎯 Common Workflow

-git clone <repo>

-git checkout -b feature

   " make changes"

-git add .

-git commit -m "feature added"

-git push origin feature
