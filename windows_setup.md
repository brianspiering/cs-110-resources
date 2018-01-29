Setting up Cygwin and Python on windows
=======

__Before installing [Python](https://www.python.org/), install [cygwin](http://www.cygwin.com/)__

Cygwin creates a new file tree on your computer in which Python must be installed in, so it is much easier to install cygwin first. 

When installing cygwin, it asks quite a few questions, you can keep pressing next and leave everything default.

It will then show a page asking what site you want to download cygwin from. You can pick any of them but I chose the first.

Keep pressing next untill cygwin starts to install.

----

Once cygwin is installed, open it and navigate to `$ cd /cygdrive/c`. 

This is where you want to install Python.

Now you can install python. If you are using [Anaconda](https://www.anaconda.com/download/), install Anaconda in the same place.

Once it is installed in `/cygdrive/c`, go to the folder and type `$ ls`

You should see that there is now a directory that looks like `/Python32` (for 32 bit python) or `/Python64` (64 bit python).

Remember what the directory is called and then navigate back to your home directory (/~)  with `$ cd ../..`

Once you do this, type the command echo `$ "PATH=\$PATH:/cygdrive/c/Python32" >> .bash_profile`

Now you can try to open the python interpreter from within cygwin with the command `$ python3`

If you enter the interpreter and see `>>> ` then everything was installed successfully!

If you get an error message, check with a professor or TA either during a break or office hours.
