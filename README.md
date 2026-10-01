# Git_Github
"All commands for git and how all commands works on terminal"

Author: raikarpiyush
<br>
<h1>git config --global user.name "raikarpiyush" sets your Git username globally on your computer.</h1><br>
- git config → Configure Git settings<br>
- --global → Apply the setting to all Git repositories for your user<br>
- user.name → The name Git will attach to your commits<br>
- "raikarpiyush" → Your Git commit name<br>
Example: When you make a commit, Git records:<br>


<h1>git config --global user.email "raikarpiyush7@gmail.com" sets the email address Git uses for your commits.</h1><br>
- git config → Configure Git settings<br>
- --global → Apply to all repositories on your computer<br>
- user.email → Specifies the email associated with your <br>
In short: It tells Git, “Use this email address whenever I create a commit.”<br>

<h1>git status</h1>
Git checks your project and tells you:<br>
- 📁 Which branch you are currently on<br>
- ✏️ m - Modified files — files changed after the last commit<br>
- 🆕 u - Untracked files — new files Git isn't tracking yet<br>
- ✅ Staged files — files ready to be committed<br>
- 📌 Whether your working directory is clean<br>

<h1>Output</h1>
<P>On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean<P>

<h1>git clone <repository-url></h1><br>
Example<br>
git clone https://github.com/user/project.git // this link you will get in github repo <br>

How it works<br>
When you run git clone, Git:<br>
1. 🌐 Connects to the remote repository.<br>
2. 📥 Downloads the project's files.<br>
3. 📜 Downloads the Git history (commits, branches, etc.).<br>
4. 📁 Creates a new folder for the project.<br>
5. 🔗 Connects your local repository to the remote repository.<br>

How it works<br>
GitHub Repository
       ↓
   git clone
       ↓
Your Computer
       ↓
project/
 ├── .git/
 ├── src/
 └── README.md

 git clone is generally used when you don't have the project locally yet.<br>

<h1>ls</h1><br>
this command shows you all the files that are present in your directory<br>

Example<br>
project<br>
README.md<br> // md means markdown
Main.java<br>


<h1>git add filename</h1><br>
Git, add is used to move changes into the staging area, preparing them for the next commit.<br>

How it works<br>
Modify files
    ↓
git add .
    ↓
Staging Area
    ↓
git commit
    ↓
Repository


<h1>git add .</h1><br>
Is used to stage all changes in the current directory for the next commit.<br>


<h1>git commit -m "add a message"</h1><br>
Example<br>
git commit -m "Added login feature"<br>

How it works<br>
Modify files
     ↓
git add .
     ↓
Staging Area
     ↓
git commit -m "message"
     ↓
Git Repository

- git commit → Saves the staged changes<br>
- -m → Adds a message describing the changes<br>
- "Added login feature" → Your commit message<br>


<h1>git push -u origin main</h1> //For the first push, you may use:

<h1>git push</h1>

How it works<br>

Your Computer                  GitHub
     │                           │
     │  git commit               │
     │  (saved locally)          │
     │                           │
     │────── git push ──────────>│
     │                           │
     │                     Commit uploaded

git push → Sends your commits to the remote repository.<br>
origin → Usually the name of your GitHub remote.<br>
main → The branch you're pushing to.<br>
-u → Connects your local branch with the remote branch, so future git push commands can be shorter.<br>

