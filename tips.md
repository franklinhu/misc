# Helpful tips
## Navigation
* `ls` lists the files and directories in the current directory
* `ls -l` same as above but with more info
* `pwd` shows the path to the directory you're currently in
* `cd <some-directory>` takes you do that directory
* `cd ~` takes you back to your home directory (~ is shorthand for /home/<user>)
* You can change commands together with `&&`. Ex: `ls && cd <something>`
* `man <something>` brings up the help manual for a command. Insanely
useful. Press `q` to exit out of it. Ex:
```
man ls
man git
```

## Running some code
You can run python directory from the command line through the interpreter
```
$ python
Python 2.7.3 (default, Aug  1 2012, 05:14:39) 
[GCC 4.6.3] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

If you want to run a python file you've written, you can do so with
```
$ python myfile.py
```

## Version control
Once you start writing code you might find yourself in a position where
it works (yay!). Then you make some changes, it no longer works, and you
find that you can't undo. Version control systems make it super easy to 
avoid this. If you don't already have git
```
$ sudo apt-get install git
```

In a simple workflow, you have two main things you want to do
* add changes
* commit changes

Let's say you want to use git with some new project
```
~/code $
~/code $ mkdir cs61a-proj1
~/code $ cd cs61a-proj1
~/code/cs61a-proj1 $ git init
```

`git status` allows you to take a look at modifications or new files
Now, create a file
```
~/code/cs61a-proj1 $ touch myfile.py
~/code/cs61a-proj1 $ git add myfile.py
~/code/cs61a-proj1 $ git status
~/code/cs61a-proj1 $ git commit
```

At this point it'll bring up a text editor in which you can write a message
about what you're committing.

If you look at `git status` again, it should be clean.
`git log` gives you a view of the history of your repository



