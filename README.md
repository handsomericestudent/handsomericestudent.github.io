# handsomericestudent.github.io
Throwaway website for Pre Hack Rice Workshop!

# You need to have set up
### Git 
Shashank please have your instructions here 

### Text Editor
We'll be using sublime 3 which some can argue to be deprecated but we still like it :)

Download here https://www.sublimetext.com/3

# Basic Git Interface in terminal/command line 

### Mac Users 
For mac users access terminal by command + space opens up a search bar --> type in terminal and open it. This defaults to the your user I believe. 

For the sake of clarity we will be working in the Desktop directory. Put the following line in terminal and press enter.
'''
cd Desktop
'''

### Windows Users
For windows users you can access command line by right clicking your desktop while holding down shift. There should be an option to "Open command line here". If that option doesn't appear you can also look for "Command Prompt" in your search bar on the bottom left corner of your screen.

If you had to search to find it for the sake of clarity we will be working in the Desktop directory put the following and press enter in command line.
'''
cd Desktop
'''

### Fundamental Commands to keep in mind

###### Maneuvuring 
A directory is essentially what you think of as a folder. It contains things. We aren't going too in depth on command line/terminal commands because linux and windows is different.

Enter in ls (mac) or dir (windows) if you want to see a list of the different directories/files within your current directory.

This command takes you into a directory you specify. 
'''
cd directoryname
'''

Go back out of the current directory
'''
cd .. 
'''

####### Git commands
*** If you do not have git set up with your user correctly when you try to push you will likely get rejected

Add everything in that directory
'''
git add . 
'''

Commit the changes you made 
'''
git commit -m "your message here"
'''

Push your code to the branch you are working in
'''
git push 
'''
# Github 
Create a new github account (you can link this to your student email later to get thousands of dollars worth of free developer tools/software). 

### Create a new repository
FYI. A repository is kind of like a place to store your code so multiple people can work with it. we won't go too in depth on this topic but github repositories enable us to have version control. This is VERY important and learning how to work with it is a must for working with multiple developers.


Create a new repository first by clicking on the plus sign on the upper right hand corner of your screen.

Name this repository yourusername.github.io and initialize it with a README (that's what you're reading right now). Github pages is a nifty little tool that github gives each user to host a static page (static meaning that it doesn't have things like a php engine for per say sending emails or otherwise anything that interacts with a database). 

By naming this repository username.github.io you are making this repository your gh pages site. You can add other projects on top of this later as well. 

### How does this even work?
username.github.io will automatically look for in its root (the very first directory) an index.html file. This is the file we will be trying to create.

### Clone this new repository into your deskop
Okay this is pretty simple. Copy the url github provides you with in the repository. 

Go to command line/terminal. You should be in the desktop directory still. Put in git clone and then paste in the url.
'''
git clone https://github.com/handsomericestudent/handsomericestudent.github.io.git
'''

Alright now if you check your desktop you should now have a folder named "username.github.io".

### Initializing the index.html file 
For now let's do something really simple. Open up your sublime text editor and create a new file. Save this file as index.html inside the root (the main/first folder) of the repository you just cloned. 

Now open up that index.html file into your text editor.

Let's try something really simple. 
'''html
<h1>Hello World!!!</h1>
'''

Now let's use those commands we learned earlier. Navigate to the directory that should be username.github.io on your desktop using command line or terminal.

'''
git add .
'''

'''
git commit -m "Added index.html file"
'''

'''
git push
'''

Now go into your browser and go to username.github.io. Congrats you've just made and deployed your first website!
