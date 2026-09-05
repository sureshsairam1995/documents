### connect your local project directory directly to your online GitHub repository
```
cd ~/git_demmo
```
### Initialize Git
```
git init
```
### Rename your default branch from "master" to "main":
```
git branch -M main

```
### Link the remote repository: Replace the URL below with your actual repository URL
```
git remote add origin git@github.com:sureshsairam1995/demo-repo.git

```
### Stage your changes
This prepares all your local changes (like your new .github/workflows folder) to be committed.
```
git add .
```
### Save the snapshot to your local computer's history. (Tip: Changed to a conventional commit style to match your preferences!)
```
git commit -m "ci: add github actions workflow and connect remote"
```
### Push smoothly to GitHub
```
git push -u origin main
```



