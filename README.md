# git_assignment_HeroVired
git_assignment_HeroVired’
Ans-1

1. create repository on by clicking plus button on  GitHub logged in by my user .
2. Repo link https://github.com/vijaykankane/git_assignment_HeroVired
3. git clone https://github.com/vijaykankane/git_assignment_HeroVired
4. git checkout -b dev
5. git add CalculatorPlus.py
6. git commit -m "commiting the CalculatorPlus.py"
7. git push --set-upstream origin dev
8.git checkout main
git pull origin main 
git merge dev
git tag -a v1.0.0 -m "Release version 1 of Calculator Plus App"
git push origin v1.0.0
 git checkout -b "feature/sqrt"
git add .\CalculatorPlus.py
git commit -m "adding sqrt funtion"
git push origin feature/sqrt
git checkout -b dev
git pull origin dev
  26 git checkout -b dev
  27 git pull orgin dev
  28 git merge feature/sqrt
  29 git commit -m "branch merged"
  30 git push origin dev
  31 git checkout -b main
  32 git pull origin main
  33 git merge dev
  34 git commit -m "dev merge to main"
  35 git push origin main
  36 git tag -a v2.0.0 -m "Release version 2 of the calculator plus app"
  37 git push origin v2.0.0


Ans 2

git checkout -b lfs
git lfs install

git lfs version
git lfs track "*.zip"
git lfs track "*.mp4"
git add mongodb-compass-1.46.2-win32-x64.zip
git commit -m "large file"
git push origin lfs


Ans 3.

git checkout -b feature/circle-area
git stash push -m "WIP: circle area calculation"
git status
git checkout -b feature/rectangle-area
git stash push -m "WIP: rectangle area calculation"
git status
git checkout feature/circle-area
git stash list
git stash apply stash@{1}
git add .
git commit -m "Complete: Circle area calculation feature"
git push origin feature/circle-area
git checkout feature/rectangle-area

git stash list
git stash apply stash@{0}
git add .
git commit -m "Complete: Rectangle area calculation feature"
git push origin feature/rectangle-area
git checkout -b dev
git create --base dev --head feature/circle-area --title "Add circle area feature" --body "Implemented circle area calculation."
git create --base dev --head feature/rectangle-area--title "Add rectangle area" --body "Implemented rectangle area calculation."
git push orign dev
git checkout -b main
git pull origin main
git merge dev
git commit -m "mergin dev to main"
git push origin main
