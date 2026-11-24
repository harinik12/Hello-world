git --version
mkdir program3
cd program3
git init
git branch -M master
echo "This is the original content" > sample.txt
cat sample.txt
git add sample.txt
git status
git commit -m "Initial commit"
git branch feature-branch
git branch
echo "This is my new uncommitted change" >> sample.txt
cat sample.txt
git status
git stash
git stash list
git status
git checkout feature-branch
git branch
git checkout master
git stash apply
cat sample.txt
git status
git stash list
