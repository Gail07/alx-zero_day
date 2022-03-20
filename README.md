# 0x03. Git

It is in this project to take in hand Git and GitHub.
And it will be done in the form of tasks.


## Tasks

#### 0. Create and setup your Git and GitHub account

##### Step 0 - Create an account on GitHub
You will need a GitHub account for all your projects at ALX. You can create an account for free [here](https://github.com/)

##### Step 1 - Create a Personal Access Token on GitHub 
To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow [this tutorial](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-tokento create a token.)

Once it’s created, you should have a token that looks like this:
![Create token](https://docs.github.com/assets/cb-33474/images/help/settings/personal_access_tokens.png)

##### Step 2 - Update your profile on the intranet
Update your Intranet profile by adding your Github username [here](https://alx-intranet.hbtn.io/users/my_profile)

If it’s not done **the Checker won’t be able to correct your work**
![username case image](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2022/2/6270480a0a982cd1846b877eda2ee405d2e8f575.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220320%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220320T142655Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ecbd4c2616d6cce76c3ad2edf01476d88ec7c5d8e5ea42148ef3511e5756b920)

##### Step 3 - Create your first repository
Using the graphic interface on the [github website](https://github.com/), create your first repository.

Name: alx-zero_day
Description: I'm now a ALX Student, this is my first repository as a full-stack engineer
Public repo
No README, .gitignore, or license
![new repository](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2022/2/2340a2d0f7c74b5dd6f8fc2aa58f94d13ea2c775.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220320%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220320T142655Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=07663bc3773a20c746c8d18ca351243fca933b981b044d3eaff1a6fd9782fb6f)

##### Step 4 - Open the sandbox
On the intranet, just under the task, click on the button ![Get a sandbox button](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2022/2/9db8eece71455dfddf4b7d8585c037c535f1d18d.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220320%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220320T142655Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e4448d8ad5750aade07b61e3950717d05661ce0f9366acc0d8a4f68b0fc2f13e) and run to start the machine.
Once the container is started, click on ![Webterm button](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2022/2/be9d1fbfb3d97e6924a4d2af7df9290ad7ae77df.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220320%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220320T142655Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ae184dd24eb26ff36a11b0c1cab8486e0c5171d04ee7ec9ae84b3932d5341246) to open a shell where you can start work from.

##### Step 5 - Clone your repository
On the webterm of the sandbox, do the following:
- Clone your repository

```

root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-zero_day.git                  
Cloning into 'alx-zero_day'...
warning: You appear to have cloned an empty repository.

```

**Replace {YOUR_PERSONAL_TOKEN} with your token from step 1**
**Replace {YOUR_USERNAME} with your username from step 1**

##### Step 6 - Create the README.md and push the modifications
- Navigaye to this new directory [tips](https://askubuntu.com/questions/232442/how-do-i-navigate-between-directories-in-terminal)
- Create the file README.md with the content My first readme. [Tips](https://www.howtoforge.com/community/threads/echo-into-a-file.115/)
- Update your git identity
```

root@896cf839cf9a:/alx-pre_course# git config --global user.email "you@example.com"
root@896cf839cf9a:/alx-pre_course# git config --global user.name "Your Name"

```
- Add this new file to git, commit the with this message “My first commit” and push to the remote server / origin
```

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

#### 1. Repo-session

Create a new directory called 0x03-git in your alx-zero_day repo.

Make sure you include a not empty README.md in your directory:

- at the root of your repository alx-zero_day
- AND in the directory 0x03-git
And important part: **Make sure your commit and push your code to Github - otherwise the Checker will always fail.**
**Repo:**
- GitHub repository: alx-zero_day

#### 2. Coding fury road

For the moment we have an empty project directory containing only a README.md. It’s time to code!

- Create these directories at the root of your project: bash, c, js
- Create these empty files:
 - c/c_is_fun.c
 - js/main.js
 - js/index.js
- Create a file bash/alx with these two lines inside: #!/bin/bash and echo "ALX"
- Create a file bash/school with these two lines inside: #!/bin/bash and echo "School"
- Add all these new files to git
- Commit your changes (message: “Starting to code today, so cool”) and push to the remote server


**Repo:**
    - GitHub repository: alx-zero_day
    - Directory: 0x03-git
    - File: bash/alx, bash/school, c/c_is_fun.c, js/main.js, js/index.js

#### 3. Collaboration is the base of a company

A branch is like a copy of your project. It’s used mainly for:

  - adding a feature in development
  - collaborating on the same project with other developers
  - not breaking your entire repository
  - not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch update_script and in this branch:

  - Create an empty file named bash/98
  - Update bash/alx by replacing echo "ALX" with echo "ALX School"
  - Update bash/school by replacing echo "School" with echo "The school is open!"
  - Add and commit these changes (message: “My personal work”)
  - Push this new branch [Tips] (https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository)
Perfect! You did an amazing update in your project and it’s isolated correctly from the **main** branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

  - Change branch to main
  - Update the file bash/alx by replacing echo "ALX" with echo "ALX School is so cool!"
  - Delete the directory js
  - Commit your changes (message: “Hot fix”) and push to the origin

Ouf, hot fix is done!

**Repo:**

  - GitHub repository: alx-zero_day
  - Directory: 0x03-git
  - File: bash/alx, bash/school, bash/98

#### 4. Collaboration: be up to date

Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – **and only for this task** – please update your file README.md in the main branch from GitHub.com. It’s the **only time** you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

  - Get all changes of the main branch locally (i.e. your README.md file will be updated)
  - Create a new file up_to_date at the root of your directory and in it, write the git command line used
  - Add up_to_date to git, commit (message: “How to be up to date in git”), and push to the origin

**Repo:**

  - GitHub repository: alx-zero_day
  - Directory: 0x03-git
  - File: README.md, up_to_date

#### 5. HAAA what did you do???

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch update_script to main: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

**HHHHHHHAAAAAAAA**

```

CONFLICT (content): Merge conflict in bash/alx

```
As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch update_script, and push the result to the origin.

At the end, you should have all your work from the branch update_script (new file and two updated files) and all latest main commits (new files, delete folder, etc.), *without* conflicts.

**Repo:**

  - GitHub repository: alx-zero_day
  - Directory: 0x03-git

#### 6. Never push too much

Create a .gitignore file and define a rule to never push ~ files (generated by Emacs). [Tips] (https://git-scm.com/docs/gitignore)

**Repo:**

  - GitHub repository: alx-zero_day
  - Directory: 0x03-git
  - File: .gitignore
