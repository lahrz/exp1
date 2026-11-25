# exp1
prog 1:
mkdir GitProject
cd GitProject

git init

echo "Hello, Git!" > main.txt

git add main.txt
git commit -m "Add initial source file"

echo "*.tmp" > .gitignore
echo "*.log" >> .gitignore

echo "Temporary data" > temp.tmp
echo "Application log" > app.log

git status

git check-ignore temp.tmp app.log

git add .gitignore
git commit -m "Add gitignore for temporary and log files"




git status
git log --oneline
git ls-files
