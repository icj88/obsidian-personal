# Linux
1. Create the ssh key: `ssh-keygen -t ed25519 -C "my_email@example.com"
2. Copy the key: `cat ~/.ssh/id_ed25519.pub
3. Add the copied key to github:
	Go to Github -> Settings -> SSH and GPG keys -> New SSH Key
# Windows 
1. Create the ssh key: `ssh-keygen -t ed25519 -C "your_email@example.com"`
2. Start the SSH agent: `eval "$(ssh-agen -s)`
3. Add the ssh to the agent: `ssh-add ~/.ssh/id_ed25519`
4. Copy the key: `cat ~/.ssh/id_ed25519.pub
5. Add to GitHub
	Go to GitHub → Settings → SSH and GPG keys → New SSH key
	