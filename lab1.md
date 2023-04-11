## Lab1: Markdown, URLs, Paths, and the Filesystem

This report gives instructions on remote access and the filesystem of a terminal.

### Step 1: Installing VSCODE

If your computer already has VScode installed, proceed to [Step 2](https://github.com/zoesolomon/cse15l-lab-reports/blob/main/lab1.md#step-2-remotely-connecting)).

I. Navigate to https://code.visualstudio.com/ and follow the instructions to download and install. (More information on starting VScode for Mac OSX here: https://code.visualstudio.com/docs/?dv=osx)

![Image](VSCODE_download.jpg)

II. Once fully installed, your window should look something like this:

![Image](VSCODE.jpg)

### Step 2: Remotely Connecting

I. Open terminal in VScode

II. Use the command format `$ ssh username@host` in this case, it would be `$ ssh cs15lsp23[your two letter code]@ieng6.ucsd.edu` 

III. Input password when prompted. Your window should look something like this:

![Image](ssh.jpg)

### Step 3: Trying Commands

I. Try running some commands in the terminal. Here are a few that may be useful:
```
cd ~
cd
ls -lat
ls -a
ls <directory> where <directory> is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, where the abc is one of the other group members’ username
cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/
cat /home/linux/ieng6/cs15lsp23/public/hello.txt
```
II. Here is an example of what some of these commands could look like:

![Image](commands.jpg)
