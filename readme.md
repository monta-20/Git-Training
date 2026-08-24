# Git — Push to a Remote Branch

Explain the **_steps_** to push a local repository to a remote branch.

## Commands

```bash
git init
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

git remote add origin git@github.com:user/project.git

git add .
git commit -m "Initial commit"

git push -u origin main
