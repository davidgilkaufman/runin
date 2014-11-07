Runin
=========

Overview
--------
This is a script designed to make it easier to manage files. Specifically, the script allows you to define groups of directories creates a simple syntax for running commands in these groups of directories.

Usage and Behavior
--------
runin <category> [<category> ...] [-- command [args]]
- <category> is defined by files in the $HOME/.config/runin/categories directory. Each file in that directory is the name of a category. Each line of the file is a directory in the category.
- if -- command is provided then that command is run on all directories in the specified categories
- if no command is specified the script will accept commands on standard input
- if the command results in some sort of output, the directory is printed in bold before the output

TODO
--------
- Support nested categories
- Parallelize running commands in categories


