## How to upload local scripts to Github 
echo "# crawler4fun" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/alfredzj/crawler4fun.git
git pull origin master
git push -u origin main
