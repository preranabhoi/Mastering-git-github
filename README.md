    

### Introduction
    ## **What is VCS(Version Control System)?**
    
    Version control System is a system that records changes to files over time so that you can recall specific versions later. It is a fundamental tool in software development for managing code, tracking 
    changes, and enabling collaboration among team members.
    
    Version Control System provides Key Benefits like Collaboration, **History Tracking**, **Backup**, **Branching and Merging & Code Review.**
    
    Some Popular VCS Tools - Git, Subversion (SVN), Mercurial, Perforce, etc.
    
    ### Why Git is Preferred?
    
    Git is preferred because of its Distributed Nature, Powerful Branching, Community & Ecosystem and Speed.
    
    ### What is Git ?
    
    Git is a distributed version control system that lets developers track changes in their codebase. It allows multiple developers to work on a project simultaneously without interfering with each other's work.
    
    ### What is GitHub?
    
    GitHub is a cloud-based platform that hosts Git repositories, providing tools for collaborative development and code management.
    
    ## Why use Git and GitHub?
    
    ### Tracking Changes:
    
    * Git allows developers to track every modification made to the codebase, making it easy to see who made specific changes and when.
        
    * With Git, you can revert to previous versions if a new change introduces bugs or issues.
        
    
    ### Collaboration:
    
    * Git enables multiple developers to work on the same project without overwriting each other's work.
        
    * GitHub facilitates collaboration by providing tools for code reviews, pull requests, and discussions, improving team productivity and communication.
        
    
    ### Branching and Merging:
    
    * Developers can work on new features or bug fixes in isolated branches and merge them into the main codebase once they are tested and complete.
        
    * This workflow allows teams to manage multiple streams of development simultaneously.
        
    
    ### Backup and Recovery:
    
    * By pushing code to remote repositories on GitHub, teams have a secure backup of their projects, protecting against data loss.
        
    
    ## Difference between Git & GitHub
    
    ### Git
    
    * Git is a distributed version control system that runs locally on your machine. It is used to manage and keep track of your source code history.
        
    * It provides commands for adding, committing, branching, merging, and more, to manage code changes effectively.
        
    * Git operates offline, allowing you to manage your code without an internet connection.
        
    
    ### GitHub
    
    * GitHub is a cloud-based platform that hosts Git repositories. It provides a web interface and additional features that make Git easier to use, especially for teams.
        
    * GitHub enhances Git’s functionality by offering tools for collaboration, such as pull requests, code reviews, issue tracking, and project management.
        
    * While Git is the version control tool, GitHub is the platform that helps manage Git repositories and facilitates teamwork.
        
    
    ## Section 1 - Git
    
    ### **Setting Up Git**
    
    #### **Installing Git**
    
    Instructions for Windows, MacOS & Linux
    
    ##### **For Windows:**
    
    1. **Download Git**:
        
        * Visit [https://git-scm.com/downloads](https://git-scm.com/downloads). and click on “Download for Windows“.
            
            ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736427107224/58eab5a7-9647-4e53-ae96-374eca9ab23c.png align="center")
            
            ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736427432489/599e12da-523f-41b9-9257-59d9c646e7e8.png align="center")
            
            ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736427566825/38e2dc81-40a2-45d0-aba5-9e8ceeb2ba7c.png align="center")
            
    2. **Run the Installer**:
        
        * Locate the downloaded `.exe` file and double-click it to start the installation.
            
        * Follow the prompts in the setup wizard, selecting the default options unless specific customization is needed.
            
        * Choose your preferred text editor and other settings as you proceed.
            
    3. **Finish Installation**:
        
        * Complete the installation and open **Git Bash** or **Command Prompt** to verify the installation
            
        * ```bash
            git --version
            ```
            
            ##### **For macOS:**
            
            1. **Using Homebrew**:
                
                * If Homebrew is installed, open **Terminal** and run:
                    
                    ```bash
                    brew install git
                    ```
                    
            2. **Or Download the Installer**:
                
                * Download the Git installer from [https://git-scm.com](https://git-scm.com/).
                    
                * Open the `.dmg` file and follow the installation instructions.
                    
            3. **Verify Installation**:
                
                * In Terminal, run:
                    
                    ```bash
                    git --version
                    ```
                    
            
            ##### **For Linux:**
            
            1. **Install Git using Package Manager**:
                
                * Open **Terminal** and run the appropriate command for your distribution:
                    
                    * **Ubuntu/Debian**:
                        
                        ```bash
                        sudo apt update
                        sudo apt install git
                        ```
                        
                    * **Fedora**:
                        
                        ```bash
                        sudo dnf install git
                        ```
                        
                    * **Arch Linux**:
                        
                        ```bash
                        sudo pacman -S git
                        ```
                        
            2. **Verify Installation**:
                
                * Run:
                    
                    ```bash
                    git --version
                    ```
                    
            
            ---
            
            #### **Configuring Git**
            
            After installing Git, you need to configure your user information to associate your commits with your identity.
            
            1. **Set Your Username**:
                
                ```bash
                git config --global user.name "Your Name"
                ```
                
            2. **Set Your Email**:
                
                ```bash
                git config --global user.email "youremail@example.com"
                ```
                
            3. **Verify Configuration**:
                
                * To check your configuration, run:
                    
                    ```bash
                    git config --global --list
                    ```
                    
                * This will display your username and email along with other configurations.
                    
            
            To check if Git is already installed on your system, you can use the command line on Windows, macOS, and Linux. Here’s how you can do it for each platform:
            
            ### **1\. Checking Git Installation on Windows**
            
            **Step 1: Open Command Prompt or Git Bash**
            
            * Press `Win + R`, type `cmd`, and hit Enter to open Command Prompt.
                
            * Alternatively, you can open **Git Bash** if it’s already installed.
                
            
            **Step 2: Check Git Version**
            
            * Run the following command:
                
                ```bash
                git --version
                ```
                
            * If Git is installed, it will return a version number like `git version 2.x.x`.
                
            * If Git is not installed, you will see an error message or the command will not be recognized.
                
            
            ### **2\. Checking Git Installation on macOS**
            
            **Step 1: Open Terminal**
            
            * You can open Terminal by pressing `Cmd + Space`, typing `Terminal`, and hitting Enter.
                
            
            **Step 2: Check Git Version**
            
            * Run the following command:
                
                ```bash
                git --version
                ```
                
            * If Git is installed, it will return the version number.
                
            * If Git is not installed, macOS may prompt you to install Git or Xcode Command Line Tools.
                
            
            ### **3\. Checking Git Installation on Linux**
            
            **Step 1: Open Terminal**
            
            * Depending on your distribution, you can open Terminal from the applications menu or by pressing `Ctrl + Alt + T`.
                
            
            **Step 2: Check Git Version**
            
            * Run the following command:
                
                ```bash
                git --version
                ```
                
            * If Git is installed, it will display the version number.
                
            * If not installed, you may get a "command not found" error.
                
            
            ### **Basic Git Commands**
            
            Here’s a list of essential Git commands that are commonly used in everyday development:
            
            #### **1\. Initializing a Repository**
            
            * **Command**:
                
                ```bash
                git init
                ```
                
            * **Description**: Initializes a new Git repository in the current directory.
                
            
            #### **2\. Cloning a Repository**
            
            * **Command**:
                
                ```bash
                git clone <repository-url>
                ```
                
            * **Description**: Creates a copy of an existing repository from a remote source.
                
            
            #### **3\. Checking the Status**
            
            * **Command**:
                
                ```bash
                git status
                ```
                
            * **Description**: Displays the state of the working directory and staging area, showing changes to be committed, staged, or not tracked.
                
            
            #### **4\. Adding Changes**
            
            * **Command**:
                
                ```bash
                git add <file>
                ```
                
                or to add all changes:
                
                ```bash
                git add .
                ```
                
            * **Description**: Stages the specified files or all changes for the next commit.
                
            
            #### **5\. Committing Changes**
            
            * **Command**:
                
                ```bash
                git commit -m "Commit message"
                ```
                
            * **Description**: Records the changes in the repository with a descriptive message.
                
            
            #### **6\. Viewing Commit History**
            
            * **Command**:
                
                ```bash
                git log
                ```
                
            * **Description**: Displays the commit history for the repository.
                
            
            #### **7\. Creating a New Branch**
            
            * **Command**:
                
                ```bash
                git branch <branch-name>
                ```
                
            * **Description**: Creates a new branch.
                
            
            #### **8\. Switching Branches**
            
            * **Command**:
                
                ```bash
                git checkout <branch-name>
                ```
                
            * **Description**: Switches to the specified branch.
                
            
            #### **9\. Merging Branches**
            
            * **Command**:
                
                ```bash
                git merge <branch-name>
                ```
                
            * **Description**: Merges the specified branch into the current branch.
                
            
            #### **10\. Pushing Changes to Remote**
            
            * **Command**:
                
                ```bash
                git push origin <branch-name>
                ```
                
            * **Description**: Pushes the committed changes to the remote repository.
                
            
            #### **11\. Pulling Changes from Remote**
            
            * **Command**:
                
                ```bash
                git pull
                ```
                
            * **Description**: Fetches and merges changes from the remote repository into the current branch.
                
            
            #### **12\. Viewing Differences**
            
            * **Command**:
                
                ```bash
                git diff
                ```
                
            * **Description**: Shows the changes between the working directory and the staging area, or between commits.
                
            
            #### **13\. Discarding Local Changes**
            
            * **Command**:
                
                ```bash
                git checkout -- <file>
                ```
                
            * **Description**: Discards changes in the working directory, reverting to the last committed state of the file.
                
            
            #### **14\. Stashing Changes**
            
            * **Command**:
                
                ```bash
                git stash
                ```
                
            * **Description**: Temporarily saves changes that are not ready to be committed.
                
            
            #### **15\. Applying Stashed Changes**
            
            * **Command**:
                
                ```bash
                git stash apply
                ```
                
            * **Description**: Applies stashed changes back to the working directory.
                
            
            These commands form the foundation of working with Git. Each plays a crucial role in managing a project’s history and collaborating effectively with others.
            
            ### **Common Git Scenarios & Troubleshooting**
            
            #### **1\. Untracked Files**
            
            **Scenario**: You have created new files, but they are not tracked by Git.
            
            **Solution**:
            
            * Run:
                
                ```bash
                git add <file>
                ```
                
                or
                
                ```bash
                git add .
                ```
                
            * Commit the changes:
                
                ```bash
                git commit -m "Add new files"
                ```
                
            
            #### **2\. Undoing Changes in the Working Directory**
            
            **Scenario**: You made changes to a file but want to discard them.
            
            **Solution**:
            
            * Discard changes to a specific file:
                
                ```bash
                git checkout -- <file>
                ```
                
            
            #### **3\. Forgot to Add a File to the Last Commit**
            
            **Scenario**: You forgot to include a file in your last commit.
            
            **Solution**:
            
            * Stage the missing file:
                
                ```bash
                git add <file>
                ```
                
            * Amend the last commit:
                
                ```bash
                git commit --amend
                ```
                
                (This will open the commit message editor. Save and close it to update the commit.)
                
            
            #### **4\. Reverting a Commit**
            
            **Scenario**: You need to undo a commit that has already been pushed.
            
            **Solution**:
            
            * Revert the commit:
                
                ```bash
                git revert <commit-hash>
                ```
                
            * This will create a new commit that undoes the changes.
                
            
            #### **5\. Resolving Merge Conflicts**
            
            **Scenario**: You encounter merge conflicts when merging branches.
            
            **Solution**:
            
            1. Git will mark conflicts in the affected files.
                
            2. Open the files and look for conflict markers like:
                
                ```bash
                <<<<<<< HEAD
                Your changes
                =======
                Incoming changes
                >>>>>>> branch-name
                ```
                
            3. Manually resolve the conflicts.
                
            4. After resolving, stage the files:
                
                ```bash
                git add <file>
                ```
                
            5. Complete the merge:
                
                ```bash
                git commit
                ```
                
            
            #### **6\. Detached HEAD State**
            
            **Scenario**: You checked out a specific commit and are now in a detached HEAD state.
            
            **Solution**:
            
            * To return to a branch:
                
                ```bash
                git checkout <branch-name>
                ```
                
            
            #### **7\. Pulling Without Overwriting Local Changes**
            
            **Scenario**: You have local changes that you don’t want to lose when pulling the latest changes.
            
            **Solution**:
            
            * Stash your changes:
                
                ```bash
                git stash
                ```
                
            * Pull the latest changes:
                
                ```bash
                git pull
                ```
                
            * Reapply your stashed changes:
                
                ```bash
                git stash apply
                ```
                
            
            #### **8\. Resetting to a Previous Commit**
            
            **Scenario**: You want to undo all changes and reset your repository to a previous commit.
            
            **Solution**:
            
            * To reset the working directory to a previous commit (discarding all subsequent changes):
                
                ```bash
                git reset --hard <commit-hash>
                ```
                
            * Be cautious, as this will permanently delete all changes after the specified commit.
                
            
            #### **9\. Recovering a Deleted Branch**
            
            **Scenario**: You accidentally deleted a branch and need to recover it.
            
            **Solution**:
            
            * Check for the branch in the reflog:
                
                ```bash
                git reflog
                ```
                
            * Find the commit hash before the branch was deleted.
                
            * Create a new branch from that commit:
                
                ```bash
                git checkout -b <new-branch-name> <commit-hash>
                ```
                
            
            #### **10\. Pushing to the Wrong Branch**
            
            **Scenario**: You accidentally pushed changes to the wrong branch.
            
            **Solution**:
            
            * Revert the push by resetting the branch to the previous state:
                
                ```bash
                git reset --hard <commit-hash>
                ```
                
            * Force push the changes:
                
                ```bash
                git push origin <branch-name> --force
                ```
                
            * Then, push the correct changes to the intended branch.
                
            
            These scenarios cover common problems that developers face while using Git and provide practical solutions to resolve them effectively.
            
            Would you like to add more specific scenarios or deeper troubleshooting steps?
            
            ### **Section 2 - GitHub**
            
            ### Setting up GitHub
            
            1. **Create a GitHub Account:**
                
                * Go to **GitHub** and click on “Sign Up”.
                    
                * Fill in the required details such as username, email, and password.
                    
                * Follow the verification process to complete account creation.
                    
                    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1736481893521/1d0baa24-3506-47b3-bc35-174c917720cd.png align="center")
                    
            2. **Configure SSH Key (optional but Recommended)**:
                
                * Generate an SSH key:
                    
                    ```bash
                    ssh-keygen -t ed25519 -C "your.email@example.com"
                    ```
                    
                * Add the SSH key to your GitHub account. Go to **Settings &gt; SSH and GPG keys**, click **New SSH key**, and paste your public key.
                    
            
            ### GitHub Workflow
            
            1. **Forking a Repository:**
                
                * Go to the repository you [](https://github.com/)want to contribute to and click the **Fork** button.
                    
                * This creates a copy of the repository in your account.
                    
            2. **Cloning the Repository:**
                
                * Copy the repository URL from your GitHub account.
                    
                * Clone it to your local machine:
                    
                    ```bash
                    git clone <repository-url>
                    ```
                    
            3. **Creating a New Branch:**
                
                * Create a branch for your work:
                    
                    ```bash
                    git branch <branch-name>
                    ```
                    
                * Switch to the new branch:
                    
                    ```bash
                    git checkout <branch-name>
                    ```
                    
            4. **Making Changes**:
                
                * Make changes to the code and stage them:
                    
                    ```bash
                    git add <file>
                    ```
                    
                * Commit the changes:
                    
                    ```bash
                    git commit -m "Your commit message"
                    ```
                    
            5. **Pushing Changes**:
                
                Push the branch to your GitHub repository:
                
                * ```bash
                    git push origin <branch-name>
                    ```
                    
            6. **Creating a Pull Request:**
                
                * On GitHub, navigate to the original repository and click **New pull request**.
                    
                * Compare your branch with the main branch of the repository and submit the pull request for review.
                    
            
            ### Collaboration on GitHub
            
            1. **Reviewing Pull Request**:
                
                * Once a pull request is submitted, team members can review the changes.
                    
                * Add comments, suggest changes, or approve the pull request.
                    
            2. **Merging Pull Requests**:
                
                * After approval, the pull request can be merged into the main branch by clicking **Merge pull request**.
                    
            3. **Issues and Project** **Boards**:
                
                * **Issues**: Used to track tasks, enhancements, and bugs. You can create, assign, and comment on issues.
                    
                * **Project Boards**: Use project boards to manage workflows and organize tasks visually.
                    
            4. **Using GitHub Actions:**
                
                * Automate tasks such as testing, building, and deployment using **GitHub Actions**.
                    
                * Create workflows in the`github/workflows` directory of your repository.
