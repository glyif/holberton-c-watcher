# Holberton C Watcher
### Description
Holberton C Watcher is a script built on top of [inotify-tools](https://github.com/rvoicilas/inotify-tools/) to watch for new and updated c files in a directory then runs the [Betty](https://github.com/holbertonschool/Betty) checker on those files. After checking the files, the output is the same as Betty.

### Installation
1) Install `inotify`
-   For Ubuntu 14.04 you can use the command `sudo apt-get install inotify-tools`

2) Clone the git repo to an accessible directory like your home directory.

3) Checkout the script to make sure you understand what's going on.

4) You can make an alias to the script so you can run it anywhere.
-   `alias hbtn-watch="bash /home/vagrant/holberton-c-watcher/watch`

5) Reload your bashrc or zshrc with the `source` command

6) Navigate to the folder you want to watch

7) Run the alias you just made.

### IMPORTANT
To keep the watcher running, you will need to open it in a different terminal buffer. If you exit out of the terminal buffer, the watcher will no longer run.

Also, this assumes you have Betty installed and you can run it using the command `betty`. If this isn't the case, this script won't work for you.

### Notes
In the script, the file path is defined by the variable $CURPATH which runs the command `pwd` which allows the watcher to run your current directory and it's child directories
