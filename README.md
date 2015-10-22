# GitHub Tutorial

_by Kevin Orta_

---
## Git vs. GitHub
Git and Github can be used together, but git doesn't require you to use github, 
but github requires you to use git.. Both allow your to keep track of your 
progress, but offer different funcionalities that work well together


* Git
    * Runs locally
    * Allows you to take snapshot of your code

* GitHub
    *  Saves your commits in the cloud.
    * Allows collaboration on the same project.


---
## Initial Setup
Before using git and github you must first set up a few things.
####Creating A GitHub Account
1. Go to [GitHub](https://github.com)
2. Click the green **Sign Up** button in the top right corner.
3. Fill out the appropriate information.
4. Select the free account.
5. Click the **Finish Account** button    

####Adding an SSH Key
SSH Keys is the way you link your github to your cloud 9 so that it gives 
you access to your github account. 

1. Navigate to your cloud 9 settings.
2. Click on the **SSH Key** tab on the left.
3. Copy the **Default SSH Key** to your clipboard.
4. Head to your Github settings page.
5. Click the **SSH Keys** tab on the side.
6. Click **Add SSH Key**.
7. Make the title **Cloud 9** and paste the SSH Key you ahve copied into the provided box.



####Git Config
Git Config identifies the changes made to the repository as the name and email your input.    

* `git config --global user.name YOUR NAME` to set your name.
* `git config --global user.email YOUR EMAIL` to set up your email.
* Since you type it in --global you dont have to ever type this again.






---
## Repository Setup
1. First type `git init` in your main repository where you are working from.
    * If you initialize the wrong folder you can remove it by typing `rm -rf .git`
    * This tells cloud 9 that you will be using more git commands so it allows you to use them.
2. Once you make changes and save them you can use `git add`
    * a further explination of git add is below.
3. After adding you can make your first commit by using `git commit -m "MESSGE"`
    * Further explination below
4. On Github press the **+** button in the top right corner and select **New Repository**
5. Put in the same exact name for your local repository as your github repository.
6. **Create Repository**
7. Make sure you select SSH.
8. Copy the first line under **…or push an existing repository from the command line** : `git remote add origin git@github.com:USERNAME/REPOSITORY_NAME .git`
    * This connects your local repository to your github
9. Copy the line of code after that : `git push -u origin master`
    *This pushes your commits to github 
    *Further explination below





---
## Workflow & Commands
* To check what files need to by saved and commited:
    * `git status`
* To add files to the stage to get commited later on:
    * `git add FILENAME`
    * You can also use `--all` or `.` instead of the file name to add all files that have to be commited.
    * Multiple files can be added at the same time by putting a space between the file names.
* To commit files use:
    * `git commit -m "MESSAGE"`
    * `-m` means that the next thing you type will be your message
    * Your message should be in present tense and be a short explination of  
     the changes done by making the changes included in the commit.
    *Commiting files takes a snapshot of them so that you can review changes made.
* To send your commits to github use: 
    * `git push`
    * This sends all of your commits to github and changes your repository on github.
    
