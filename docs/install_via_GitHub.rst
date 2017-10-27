Install pyspeckit via GitHub
============================

Logged into your github account, go to https://github.com/pyspeckit/pyspeckit
and click “Fork” in upper right.

Copy the URL of your pyspeckit fork https://github.com/*yourusername*/pyspeckit

On the command line type

  ``git clone https://github.com/yourusername/pyspeckit``

(it will put it in a directory called pyspeckit in your working directory)

  ``cd pyspeckit``

  ``git remote add upstream https://github.com/pyspeckit/pyspeckit``

To get the most up to date version, type

  ``git pull upstream master``

Update your personal "fork" to match ``upstream/master``

  ``git push origin master``

and enter your username and password if it asks.

Still in the ``pyspeckit/`` directory, type

  ``python setup.py develop``

You're good to go!

To make changes and generate a Pull request:
--------------------------------------------

Create a new branch: ``git checkout -b name_of_your_new_branch`` This will
automatically switch you to this new branch.  Type ``git branch`` to see all
the branches.  The active one will be highlighted and have an asterisk next to
it.  To switch to an existing branch, type ``git checkout name_of_branch``

After you make a change inside your local fork on your machine, type ``git add
changed_file`` where changed_file is the name of the file(s) you edited.

Time to commit your change and add a little note about your change ``git commit
-m details`` ``details`` should be a description of the changes you made,
inside quotes

Push the change to GitHub: ``git push origin name_of_branch`` where
name_of_branch is the branch you’ve been active in during this process.

If you want to contribute your changes to
https://github.com/pyspeckit/pyspeckit, create a “pull request”.  In
https://github.com/yourusername/pyspeckit, navigate to your branch where you
pushed you want to merge with https://github.com/pyspeckit/pyspeckit and click
"Pull request"
