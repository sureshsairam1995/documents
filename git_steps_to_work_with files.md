### connect your local project directory directly to your online GitHub repository
```
cd ~/git_demmo
```
> [!NOTE]
>  All the commands and steps should be executed inside the project directory of system.
<img width="642" height="241" alt="image" src="https://github.com/user-attachments/assets/16cd2cf9-8160-4b39-94a5-7967b5a85331" />

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
### If GitHub rejects it because the remote has files you don't have locally, run below command first, then push again
```
git pull origin main --allow-unrelated-histories
```
### Push smoothly to GitHub
```
git push -u origin main
```



