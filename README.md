# Data-UCIDemo

## Welcome to the github and Jupyter Lab Workshop!
This repository will serve as a guide to what we will go over
in the workshop in the github portion! We will go through some
basic commits, pushes and reverts to help everyone get a basic
understanding of the benefits of git / github!

## Making a repository
By now you should have a github account (if you haven't done so already make one really quick and come back!),
now it is time to make our first repository. There are many ways to create a new one, but the simplest way 
is to go to the github home screen by clicking the logo in the top left corner (not the three horizontal lines)
and scroll down a little. There you should see a box that says "Start a new repository for [your username]". 
Be sure to name the repository and set it to public or private depending on what you want and click the
"Create a new repository button."

## Pushing our first commit
Once you hit the "Create a new repository button." You will prompted with a list of commands.
For now, we will use the set of commands that are under the "…or create a new repository on the command line."
Before we copy and paste those commands into our terminal, be sure to make sure that your current working
directory is the project folder you want to make into a git repo. Once you are in the right directory
copy and paste those commands into your terminal and press enter. Congratulations! you just made
your first commit to your repository. You can check this by refreshing the page and seeing a blank
repository that should just be your repository name displayed.


## Commiting and Pushing our notebook
Now that we made our first commit, lets commit our first notebook! 
Helpful tip: git status is your best friend at keeping track of files
that are in your project that might want to be pushed into the repository.
In this case, we're going to use git status to see which files we should / should
not add to the repo. Once called, you should be given some information about if your
branch is up-to-date, what branch you are on, and what are the untracked and staged files
in your current local project. For now, lets track all of our files by calling git add <file_name>.
This brings the untracked files to the staging area where they are ready to be committed. NOTE: If you
ever accidentally add something to the staging area and want to un-add it, just call git reset <file_name> if you want to un_add
a specific file or git reset if you want to un-add everything. Now that are files are added we can call git commit -m "[put message here]"
and then call git push your first notebook on your repo!

## Reverting a commit
Now that we have pushed something on to the repository; we are going to revert a commit.
Let's first make add and push a dummy notebook / file onto our repository (p.s this is great
practice for you to do what we just learned in the previous steps!) Once you added a dummy file,
lets revert it! First, we are going to call git log to see which commit we want to revert. Notice,
when you call git log, you get a list of the commits you have done throughout your project with the message
that you committed then with. Find the commit that you create, edited, and pushed your dummy file and copy the 
seed (it should be in yellow text where it says "commit [seed]." Once copied, we can call git revert seed and 
the command should bring you to a vim editor to write your commit message. Simply press i to go into insert mode
and when finished writing your message click the esc key and shift+zz to exit. Once, call git push to push the revert
and you have made your first revision. 
