# Pre-HackRice Website Workshop
> This tutorial will help you create and publish a basic website, hosted on [Github Pages](https://pages.github.com/). We hope that this introduction helps you become acquainted with **Github** (a version control tool), **HTML & CSS** (the building blocks of basic websites), and **bash** (a way of interacting with your computer through your Terminal).

## Step 1: Setup

### Git

Git helps you maintain versions of your files online, enabling powerful revision history, enhanced collaboration for teams working on the same codebase. While there are graphical interfaces for interacting with `git`, we will use your command line so that you can simultaneously learn how to navigate your computer with your Terminal!

For more on how to use `git`, read this [simple guide](http://rogerdudler.github.io/git-guide/). 


#### Mac

Mac users should already have access to `git`. Open `Terminal.app` and type the following command to ensure it is installed:

```
git version
```

#### Windows

Download and install the latest version of Git from [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Once you have installed it, open your Command Prompt (`cmd.exe`) and type the following command to ensure it is installed:

```
git version
```

#### Linux

Installing `git` on your Linux installation may depend on the distribution ("distro") you have installed to your computer. Read [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) for more information on installing Git on Linux.

#### Settings

You can set a name and email associated with your Git installation using the following commands. If you do not already have an account on Github, you should create one first [here](https://github.com).

```
git config --global user.name "Your Name"
git config --global user.email your@email.com
```

### Text Editor

We will be walking through this demo using [Atom](https://atom.io), which is an open-sourced text editor built by a team at Github! Download it [here](https://atom.io).

Alternatively, you can also try [Visual Studio Code](https://code.visualstudio.com) built by Microsoft, or [Sublime Text 3](https://www.sublimetext.com/3), a popular but slightly outdated text editor.


## Step 2: Navigating Your Computer using Terminal

### Mac
Access Terminal by using the key combination `command + space` (which opens Spotlight), and searching for `Terminal`. For the purpose of simplicity, we will be creating a folder on your Desktop. Generally speaking, this is a **bad** practice, but we want you to be able to find these files easily! Type the following to **navigate** to your desktop:

```
cd ~/Desktop
```
The `~/` tells the computer to start at the root of your user's directory, and `cd` stands for `change directory`.

Now, let's create a folder on your desktop to store this project within, and move inside of it.

```
mkdir workshop
cd workshop
```

Now, we are in the `workshop` folder!

### Windows
On Windows, you can access your Command Prompt line by typing `cmd` into your search bar. If this doesn't work, you can also access the Command Prompt via `Shift + right-click` combination, and clicking the menu item **"Open Command Line Here"**. Once you have opened the app, type the following commands:

```
cd ~/Desktop
```
The `~/` tells the computer to start at the root of your user's directory, and `cd` stands for `change directory`.

Now, let's create a folder on your desktop to store this project within, and move inside of it.

```
mkdir workshop
cd workshop
```

Now, we are in the `workshop` folder!

## Aside: Maneuvering Around Terminal

A "directory" is a folder. It contains files or other folders. 

- To learn **where you are** on your computer right now, you can type `pwd` to resolve your current working directory. 
- To learn more **about a particular command**, you can type `man [command]` to view the manual for that file. This might look like `man cd` to understand how the `cd` (change directory) command works. This might be a little hard to read right now, but this is the fastest way to learn how your Terminal works!
- To see **all of the files** in your current directory, you can type `ls -a` (Mac, Linux) or `dir` (Windows).
- To move up a directory, try typing `cd ..`.
- To take advantage of the auto-complete feature of your Terminal, hit `[Tab]` when mid-way through a word to see the autocomplete suggestions.


## Step 3: Learning Git Commands

Git is a programmer's go-to tool. It helps maintain versions of your files, so that you don't lose changes if you lose a local copy of your files. It also helps teams collaborate on projects, so that they can share a unified codebase and merge edits to the same file (and resolve conflicts appropriately).

> If you are experiencing difficulties with using these commands, it's likely because you have set up authentication for Git incorrectly. Please let us know, and we can help you!

### Initializing a project.

```
git init
```

### Adding all files to version control.

```
git add .
```

### Adding individual files to version control.

```
git add file1.txt file2.md image1.png
```

### Stage these new files (or modifications of existing files).

```
git commit -m "your description of changes made go here"
```

> Remember to always make useful commit messages, for both your own sake and your collaborators!


### Push your changes onto a server online.
```
git push 
```

### Cloning a repository from online.
```
git clone [url].git
```

## Step 4: 
Create a new github account (you can link this to your student email later to get thousands of dollars worth of free developer tools/software). 

### Create a new repository.
Create a new repository first by clicking on the plus sign on the upper right hand corner of your screen.
<img src="https://i.imgur.com/ThwdbQY.png"/>

Name this repository `yourusername.github.io` and initialize it with a `README.md` (the type of file you're reading right now!). Github Pages enables each user to host a simple website. 
<img src="https://i.imgur.com/FeypG2U.png"/>

By naming this repository `username.github.io`, you are designating this repository to be your Github Pages site. You can add other projects on top of this later as well. 

### Why does this work?
Inside the `username.github.io` repository, Github will automatically look for an index.html file in the root (first-level) of the directory. This is the file we will create during this workshop!

### Clone this new repository into your deskop.
Copy the url Github provides you with in the repository. 
<img src="https://i.imgur.com/NZROsFs.png"/>

Go to your command line, and make sure you are in the `workshops` directory we created earlier. Type the following command.

```
git clone https://github.com/handsomericestudent/handsomericestudent.github.io.git
```
<img src="https://i.imgur.com/EL9ZEbX.png"/>

Now, inside `~/Desktop/workshop/`, you should find a new folder! Enter it using the `cd` command. 

### Initializing the index.html file 
For the sake of time, we will create a very simple website. Open up your sublime text editor and create a new file. Save this file as index.html inside the root (the main/first folder) of the repository you just cloned. 

Now open up that index.html file into your text editor.

Let's try something really simple. Write in 
```html
<!DOCTYPE html>
<html>
  <head>
    <title>[Name]'s Personal Website!</title>
  </head>
  <body>
    <img src="https://github.com/hackclub/dinosaurs/raw/master/smart_dinosaur_docs.png">
    <h1>Your name goes here.</h1>
    <p>Tell us a little bit about yourself below.</p>
    <ol>
      <li>Something goes here.</li>
      <li>Another thing goes here.</li>
      <li>Last thing! Make it special.</li>
    </ol>
  </body>
</html>
```

Modify the contents of this file to personalize this website. If you would like to learn more about the structure of an HTML document, visit the following link: [HTML Dog](http://htmldog.com). 

### Publishing your project.

Now let's use those commands we learned earlier. Navigate to the directory that should be username.github.io on your desktop using command line or terminal.

```
git add .
```

```
git commit -m "Added index.html file"
```

```
git push
```

Now go into your browser and go to `[username].github.io`. Congrats you've just made and deployed your first website!
