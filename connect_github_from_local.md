
## Step 1: Check for existing SSH keys
```
ls -al ~/.ssh
```
If you see files named id_ed25519 and id_ed25519.pub: You already have a key! Skip directly to Step 3.

If you see an error like "No such file or directory" or the files are missing: Move to Step 2.

## Generate a new SSH key
Run the following command to generate a highly secure key pair. Make sure to replace the email with your GitHub account email:
```
ssh-keygen -t ed25519 -C "sureshsairam95@gmail.com"
```
## Step 3: Copy the SSH Public Key to your clipboard
```
cat ~/.ssh/id_ed25519.pub
```

## Step 4: Add the SSH key to your GitHub Account
Open your browser and go to your GitHub SSH Keys Settings.
Click the green New SSH Key button in the top right.
In the Title field, type a name for your computer (e.g., "My Work Laptop").
In the Key box, paste the text you copied in Step 3.
Click Add SSH Key. (GitHub may ask you to confirm your account password).

## Step 5: Update your local Git Repository to use SSH
Go back to your terminal, make sure you are inside your project folder (demo-repo), and swap the remote URL from HTTPS to SSH:
```
git remote set-url origin git@github.com:sureshsairam1995/demo-repo.git
```
