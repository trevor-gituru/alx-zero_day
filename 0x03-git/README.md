# 0x03. Git 

![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Code Versioning](https://img.shields.io/badge/Code_Versioning-6f42c1?style=flat&logo=visualstudio&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)

## Concepts Learnt

- What is source code management
- What is Git
- What is GitHub
- What is the difference between Git and GitHub
- How to create a repository
- What is a README
- How to write good READMEs
- How to commit
- How to write helpful commit messages
- How to push code
- How to pull updates
- How to create a branch
- How to merge branches
- How to work as collaborators on a project
- Which files should and which files should not appear in your repo

## Tasks 
### 0. Create and setup your Git and GitHub account

#### **Step 0 - Create an account on GitHub [if you do not have one already]**

You will need a GitHub account for all your projects at ALX. If you do not already have a github.com account, you can create an account for free [ here ](https://github.com/)

#### **Step 1 - Create a Personal Access Token on Github**

To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow this tutorial to create a token.

Once it’s created, you should have a token that looks like this:
![ Token ](./i1.png)

#### **Step 2 - Update your profile on the Intranet**

Update your Intranet profile by adding your Github username here

If it’s not done the **Checker won’t be able to correct your work**

![ Intranet ](./i2.png)

#### **Step 3 - Create your first repository**

Using the graphic interface on the [ github website ](https://github.com/), create your first repository.

- Name: `alx-zero_day`
- Description: `I'm now a ALX Student, this is my first repository as a full-stack engineer`
- Public repo
- No `README`, `.gitignore`, or license

![Repo](./i3.png)

#### **Step 4 - Open the sandbox**

On the intranet, just under the task, click on the button <img src="./i4.png" width="100" height="40" /> and run to start the machine.

Once the container is started, click on <img src="./i5.png" width="100" height="40" /> to open a shell where you can start work from.

#### **Step 5 - Clone your repository**

On the webterm of the sandbox, do the following:

- Clone your repository
```bash
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-zero_day.git                  
Cloning into 'alx-zero_day'...
warning: You appear to have cloned an empty repository.       
```

**Replace {YOUR_PERSONAL_TOKEN} with your token from step 1**

**Replace {YOUR_USERNAME} with your username from step 0 and 1**

**Pro-Tip:** On windows, use CTRL + A + V to paste in the web terminal

#### **Step 6 - Create the README.md and push the modifications**

- Navigate to this new directory. Tips
```bash
root@896cf839cf9a:/# cd alx-zero_day/
root@896cf839cf9a:/alx-zero_day#
```
- Create the file `README.md` with the content `My first readme`. Tips
```bash
root@896cf839cf9a:/alx-zero_day# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/alx-zero_day# cat README.md                                                                                      
My first readme                                                                                                                       
```
- Update your git identity
```bash
root@896cf839cf9a:/alx-pre_course# git config --global user.email "you@example.com"
root@896cf839cf9a:/alx-pre_course# git config --global user.name "Your Name"
```
- Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
```bash
root@896cf839cf9a:/alx-zero_day# git add .
root@896cf839cf9a:/alx-zero_day# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/alx-zero_day# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/alx-zero_day.git                                                                                       
 * [new branch]      master -> master              
```

Good job!

You pushed your first file in your **first repository** of the **first task** of your **first ALX School project**.

You can now check your repository on GitHub to see if everything is good.
 
### 1. Repo-session

Create a new directory called `0x03-git` in your `alx-zero_day` repo.

Make sure you include a not empty `README.md` in your directory:

- at the root of your repository `alx-zero_day`
- AND in the directory `0x03-git`

**And important part:** Make sure your commit and push your code to Github - otherwise the Checker will always fail.

### 
### 
### 
### 
### 

## Resources
- [Source Code Management](./source_code_management.pdf)
- [ Git and Github cheat sheet - Everything in less than 30 seconds ](./git_github.pdf
)
- [ Authenticating Git ](./auth.pdf)
- [ Right-engineering, right-documenting ](./documentation.pdf)
- [ Resources to learn Git ](https://docs.github.com/en/get-started/git-basics/set-up-git)
- [ About READMEs ](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [ How to write a Git commit message ](https://cbea.ms/git-commit/)
- [ Learning branching ](https://learngitbranching.js.org/)
- [ Effective pull requests and other good practices for teams using GitHub ]()
