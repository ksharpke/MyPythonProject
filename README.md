# MyPythonProject
mkdir MyPythonProject
cd MyPythonProject
git init
# main.py
print("Hello, Git!")
git add main.py
git commit -m "Initial commit"
git branch feature-branch
git checkout feature-branch
# main.py
print("Hello, Git! This is a feature.")
git add main.py
git commit -m "Implementing feature X"
git checkout main
git merge feature-branch
git push origin main
git pull origin main
git checkout main
# Make conflicting changes in main.py
git merge feature-branch
# main.py
print("Hello, Git! This is a feature with conflict resolution.")
git add main.py
git merge --continue
git commit -m "Merge feature-branch with conflict resolution"
git push origin main
