# git_cli_notes
## version information
``` 
git --version
```
## Configure Git Identity
``` 
git config --global user.name "Your Full Name"
git config --global user.email "your_email@example.com"
```
## Create and Add SSH Key (for GitHub access without password)
Generate SSH key:
``` 
ssh-keygen -t ed25519 -C "your_email@example.com"
```
Add your SSH key to the ssh-agent:
``` 
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```
Copy the public key:
``` 
cat ~/.ssh/id_ed25519.pub
```
Add the key to GitHub:

  Go to: https://github.com/settings/keys

  Click “New SSH Key”

  Paste the key

  Click Add SSH Key
Verify Connection to GitHub
``` 
ssh -T git@github.com
```