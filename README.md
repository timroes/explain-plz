explain-plz
===========

This is a small python tool (required Python 2.7+), that explains you the Android
source code. To use it, just put the `explain-plz` file anywhere to your $PATH.

To explain the android source code manually created explanations are used.
These explanation can be found in the [explain-plz-data](https://github.com/timroes/explain-plz-data) project.
If you can add usefull data, please edit the data and send pull request to that 
project (more information can be found in its own README file).

To start the first time, you need to call `explain-plz --update` to update your
local database. From that on you can use the tool:


Usage
-----

To use the tool just call `explain-plz` while you are in any directory of your 
Android source code (see the [AOSP instuctions](http://source.android.com/source/initializing.html) for
information on how to get the Android source code).

The tool will then search the nearest parent directory, that it has an explanation
for and output that explanation. If you want another directory (than the current working
directory) explained, just add this as first parameter (e.g. `explain-plz tools/buils`).


Parameters
----------

Instead of just explaining a folder you have the following parameters:

**--help or -h** Shows a usage message with all the parameters.

**--update or -u** Updates the local database from the above mentioned project.

**--search <term> or -s <term>** Searches all explanation files for *<term>*.

**--list or -l** Prints out a list of all folder, that can be explained by the tool.


Bugs
----

If you find any bugs in the tool itself please report them via the GitHub issue tracker.
If you find any wrong information in the database or want to add some project or modify
explanation, please go to https://github.com/timroes/explain-plz-data
