## 1. Clone git files to local VS code 
- `git clone` : clone the repositories from your GitHub and download them to local;
- `git status` : check the status of your files; 
- `git add .` : track the untracked files, you can check **certain files** or **all files** by adding a `.`;
- `git commit -m "your message" -m "your description"` : add some description to what you have added and save it;、
- `git push`：push your new file to your github.

## 2. SSH keys
### Generate your SSH keys
- `ssh-keygen -t rsa -b 4096 -C "example@email.com"`
- name the key;
- set password or empty password to your key;
- you get a **public key** and a **private key.**
- search for your key: `ls | grep yourkeyname`;
- **public key** : You put on your GitHub;
- **private key** : You show your private key to GitHub;
- `cat yourkeyname.pub`: You get your public key;

### Copy your SSH through SSH agent
- the process can be find on the GitHub page： https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
- Remember: You **must have the ssh key in your ./ssh fileholder** (I have spent 1 hour to check this stupid thing.) if they are not in ./ssh holder, just **type command+space and find them, drag them to ./ssh holder.**
 

## 3. Git Push: Push your local code to repository
- `git init`: initialize the local file 
-  `git remote add origin +pasted SSH`: you paste your repository SSH info to local terminal. So that local terminal can have idea what you have done. 
- `git remote -v`: show what repository you have created on GitHub. 
- `git push origin master`: push your local file to GitHub repository;

## Summary: Workflow in GitHub and Local editors
- GitHub Workflow: Write code → Commit Changes → Make a Pull Request
- Local Git Workflow: Write code → Stage changes `git add` → Commit Changes `git commit` → Push Changes `git push` → Make a pull request

## 4. Git  Branching
how to use a git banching and.
