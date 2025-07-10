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

### 2. Coding fury road

For the moment we have an empty project directory containing only a `README.md`. It’s time to code!

- Create these directories at the root of your project: `bash`, `c`, `js`
- Create these empty files:
    + `c/c_is_fun.c`
    + `js/main.js`
    + `js/index.js`
- Create a file `bash/alx` with these two lines inside: `#!/bin/bash` and echo "ALX"
- Create a file `bash/school` with these two lines inside: `#!/bin/bash` and `echo "School"`
- Add all these new files to git
- Commit your changes (message: “Starting to code today, so cool”) and push to the remote server
```bash
root@a710280214ff:~# cd ~/alx-zero_day/*03*
root@a710280214ff:~/alx-zero_day/0x03-git# mkdir bash c js
root@a710280214ff:~/alx-zero_day/0x03-git# touch c/c_is_fun.c js/index.js js/main.js
root@a710280214ff:~/alx-zero_day/0x03-git# echo -e '#!/bin/bash\necho "ALX"' > bash/alx
root@a710280214ff:~/alx-zero_day/0x03-git# echo -e '#!/bin/bash\necho "School"' > bash/school
root@a710280214ff:~/alx-zero_day/0x03-git# git add .
root@a710280214ff:~/alx-zero_day/0x03-git# git commit -m "Starting to code today, so cool"
[master a3aca55] Starting to code today, so cool
 5 files changed, 4 insertions(+)
 create mode 100644 0x03-git/bash/alx
 create mode 100644 0x03-git/bash/school
 create mode 100644 0x03-git/c/c_is_fun.c
 create mode 100644 0x03-git/js/index.js
 create mode 100644 0x03-git/js/main.js
root@a710280214ff:~/alx-zero_day/0x03-git# git push
Username for 'https://github.com': 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
Password for 'https://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@github.com': 
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 2 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (9/9), 652 bytes | 130.00 KiB/s, done.
Total 9 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/trevor-gituru/alx-zero_day.git
   fde2b38..a3aca55  master -> master
```
 
### 3. Collaboration is the base of a company

A branch is like a copy of your project. It’s used mainly for:

- adding a feature in development
- collaborating on the same project with other developers
- not breaking your entire repository
- not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch `update_script` and in this branch:

- Create an empty file named `bash/98`
- Update `bash/alx` by replacing `echo "ALX"` with `echo "ALX School"`
- Update `bash/school` by replacing `echo "School"` with `echo "The school is open!"`
- Add and commit these changes (message: “My personal work”)
- Push this new branch [ Tips ](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository)

Perfect! You did an amazing update in your project and it’s isolated correctly from the **main** branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

- Change branch to `main`
- Update the file `bash/alx` by replacing `echo "ALX"` with `echo "ALX School is so cool!"`
- Delete the directory `js`
- Commit your changes (message: “Hot fix”) and push to the origin

Ouf, hot fix is done
```bash
root@a710280214ff:~/alx-zero_day/0x03-git# git checkout -b update_script
Switched to a new branch 'update_script'
root@a710280214ff:~/alx-zero_day/0x03-git# touch bash/98
root@a710280214ff:~/alx-zero_day/0x03-git# sed -i 's/ALX/ALX School/' bash/alx 
root@a710280214ff:~/alx-zero_day/0x03-git# sed -i 's/School/The school is open!/' bash/school
root@a710280214ff:~/alx-zero_day/0x03-git# git add .
root@a710280214ff:~/alx-zero_day/0x03-git# git commit -m "My personal work"
[update_script d0d7924] My personal work
 3 files changed, 2 insertions(+), 2 deletions(-)
 create mode 100644 0x03-git/bash/98
root@a710280214ff:~/alx-zero_day/0x03-git# git push origin update_script
Username for 'https://github.com': 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
Password for 'https://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@github.com': 
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 504 bytes | 504.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'update_script' on GitHub by visiting:
remote:      https://github.com/trevor-gituru/alx-zero_day/pull/new/update_script
remote: 
To https://github.com/trevor-gituru/alx-zero_day.git
 * [new branch]      update_script -> update_script
root@a710280214ff:~/alx-zero_day/0x03-git# git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
root@a710280214ff:~/alx-zero_day/0x03-git# sed -i 's/ALX/ALX School is so cool!/' bash/alx 
root@a710280214ff:~/alx-zero_day/0x03-git# rm -r js/
root@a710280214ff:~/alx-zero_day/0x03-git# git add .
root@a710280214ff:~/alx-zero_day/0x03-git# git commit -m "Hot fix"
[master e82d469] Hot fix
 3 files changed, 1 insertion(+), 1 deletion(-)
 delete mode 100644 0x03-git/js/index.js
 delete mode 100644 0x03-git/js/main.js
root@a710280214ff:~/alx-zero_day/0x03-git# git push
Username for 'https://github.com': trevor-gituru
Password for 'https://trevor-gituru@github.com': 
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 439 bytes | 439.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/trevor-gituru/alx-zero_day.git
   a3aca55..e82d469  master -> master
root@a710280214ff:~/alx-zero_day/0x03-git#
```

### 4. Collaboration: be up to date

Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – `and only for this task` – please update your file `README.md` in the main branch from GitHub.com. It’s the `only time` you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

- Get all changes of the main branch locally (i.e. your `README.md` file will be updated)
- Create a new file `up_to_date` at the root of your directory and in it, write the git command line used
- Add `up_to_date` to git, commit (message: “How to be up to date in git”), and push to the origin
```bash

```
 
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
