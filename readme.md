# Learning about Git

## Downloads
<details>
  <summary>Show all downloads</summary>

### Git/Git-bash

Mac users may already have Git installed. Check by typing `git --version` in the terminal. If it's not installdd, download it at: 

MacOS - https://git-scm.com/downloads

Windows users can download git bash which is an BASH (unix) emulator to run Git. It just makes it easier to run Git without any configuration.

Windows - https://gitforwindows.org/

### GitHub
To use Git properly, you will also need a GitHub account. When you first install Git, you will configure your username, email, and password to GitHub to work with Git that was just installed.

Link - https://www.github.com

### VSCode
Visual Studio Code is a very popular code editor used for development.  

Link - https://code.visualstudio.com/download

Students using windows can change the default terminal in VSCode shell by typing `ctrl + shift + p` to open the search bar. Once the search bar is opened, type `select default shell`. You will be able to select Bash as an option.

### Node/NPM
Link - https://nodejs.org/en/download/

Node allows you to run JavaScript outside the browser (uses the same <a href="https://v8.dev/">JavaScript engine</a>).  This will also install npm too. Npm is the tool you use to install packages to your app.  Yarn is an alternative to Npm, you just have to install it manually.

### Repl.it
Link - https://repl.it/

Repl is a popular live code editor. It is a good way to share and test code online.

</details>

## CLI

CLI (Command Line Interface): Also called the terminal, is the program we will use to interact with our computer's files and directories. It is helpful to become know how to use some of the various commands you can use in the terminal. On Apple computers you are able to use the built in terminal. On Windows machines you will need to download Bash for Windows which can be found [here](https://gitforwindows.org/)

## Common Terminal Commands (Same if you are using BASH for Windows)
<strong>Note:</strong> If you are a Windows user and not using BASH, then you are using the <a href="https://red-dot-geek.com/basic-windows-command-prompt-commands/#sec-basic">Windows Command Prompt</a> which have different commands.

- pwd: Stands for present working directory. Show's where you currently are in your file tree.

- ls: Stands for list. Lists available scripts(where you can navigate to in your file tree) from your current location.

- cd: Stands for change directory and is used to navigate the file tree. The command should be formatted like this: `cd [the name of the directory]`. You can also navigate up a level by typing `cd ..`.

- mkdir directory name: Stands for make directory. Creates a new directory at your current location.

- touch filename: Creates a new file at the current location. Should be called with the name and extension of the file to be created ie `touch index.html`.

- rm filename: Deletes a file. Cannot be undone.

- rm -rf directoryname - Deletes a folder and everything in it. Be VERY sure of what is being deleted before running this command, it cannot be undone.

## Git and GitHub

Git is a version control system used to track the progress of our projects. It allows us to commit changes at various points in the development process. A commit is like a milestone. You should get in the habit of committing your code often. GitHub is the website where our git repositories are stored. To store our code remotely, we can "push" our commits to github. Before pushing our code, there are three stages in which a file can exist in relation to git which are represented in this image:

![Git stages](git.png)

1. As we are working on our files, git does not automatically track any changes made. When we are ready to have git track these changes, we use the `git add` command and provide it with whatever files we want it to watch. By using the command `git add .` we can tell git to catalog all changes in all files in our current directory. This moves our files to the staging area.
2. The staging area is used by git to prepare any changes ready for saving. In this stage, git has cataloged any changes that we have told it to and is readying them for the next step. We commit our changes by using the `git commit` command. This will move our files from the staging area to the git repository. This is like pressing the save button. Our commit should always be accompanied a message describing what changes have been made and is formatted like this `git commit -m "message"`.
3. When we commit our code we create a snapshot of it at that moment. This allows us to revert back to that version at any time. Frequently committing our code will create different points in time that we can revert to if we ever need to.

Once our code has been committed, we can "push" it to GitHub which will create a remote version of our code. You will want to get in the habit of frequently "pushing" your code to github. This will protect against any work being lost. Below are the common git commands you will want to be familiar with:

### Git Init

`git init` initializes git in your current repository. This means that git will start watching all of the files and directories in that location.

### Git Add

`git add .` tells git to track any changes that have been made. This is the command you can run to start the process of pushing your code to github.

run:

```bash
git add .
```

### Git Commit

After staging your code using `git add .` we now need to commit our changes. This is the final step we will take before pushing our code to github. Think about commits as check points or save points in your code. You will need to provide a message about the commit using the `-m` flag.

run:

```bash
git commit -m 'message about your changes'
```

### Git Push

After staging and commiting your code, it is now ready to be pushed up to github. When your code is ready to be pushed, run:

```bash
git push origin master
```

### Git Status

`git status` is the command you can run to check what stage of the process you are on to push your code to github.

run:

```bash
git status
```

### Git Clone

We are able to easily make copies of existing repositories on GitHub, this is called cloning. First you need to copy the url for the github repo that you wish to clone down to your local machine then navigate to the directory that you want to clone the repo into. Once you are in the correct directory run:

```bash
git clone "url for github repo"
```

## Additional Resources

  * [Terminal Commands - Mac or GitBash](https://www.youtube.com/watch?v=5XgBd6rjuDQ&t=606s)
  * [Git: The Simple Guide](https://rogerdudler.github.io/git-guide/)
  * [Codecademy: Learn Git](https://www.codecademy.com/learn/learn-git)
  * [Git: Official tutorial](https://git-scm.com/docs/gittutorial)
  * [Colte Steele Git Tutorial](https://www.youtube.com/watch?v=USjZcfj8yxE)
  * [CS50 Git Lecture](https://www.youtube.com/watch?v=NcoBAfJ6l2Q)
  * [Git Branching Game](https://www.youtube.com/watch?v=lG90LZotrpo)
  * [CS50 Git Under the hood](https://www.youtube.com/watch?v=lG90LZotrpo)
  * [Show Hidden Folders/Files on Windows](https://support.microsoft.com/en-us/windows/view-hidden-files-and-folders-in-windows-97fbc472-c603-9d90-91d0-1166d1d9f4b5)