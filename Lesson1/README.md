# Lesson 1: Week of June 19th

## Description
This week will be all about getting you started. You'll need to install a couple
development tools and make a push to GitHub. Let's get stared.

## Step 1: Bash Shell
The bash shell is arguably one of the most important tools in any programmer
toolkit. It's entirely text based so it can seem scary at first, but it'll soon
become second nature. Linux and macOS come with a native bash shell, but you're
on windows so we're going to have to install one ourselves.

To install bash just [ follow this installation guide](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide), if you get stuck feel free
to call me.

Now that it's install lets play around a bit. A lot of people get very intimidated
by the bash shell at first, but it's not nearly as bad as it looks. There's really
only a few commands you need to know and then from there you'll slowly learn more.

__Experiement with all the commands below. Simply type the command into the bash
shell and press enter.__

#### ls
The ls (that's an L not an I) will list everything in your current directory. A
directory is the formal name for a folder. You can add additional flags to the ls
command to show more information.

__Try the add a -a flag by writing the command below__
```
ls -a
```

-a will list all the files/directory in your directory including hidden ones
(any file/directory that begins with a "." is hidden).
__Try to add an -a and a -l flag__
```
ls -a -l
```

This will list (-l) all the files vertically with more information and display
all of the them (-a) including hidden ones.

#### cd
cd stands for change directory. In order to move around you need to be able to
change directories.

Simply write:
```
cd <insert directory name>
```

__Tip__: always use tab completion if you press tab it'll finish your file path
for you this will ensure that you don't misspell anything.

This will move into the directory that you give it. If you don't insert a
directory it'll move to your home directory.

___extra credit___

Play around with file paths, add (~ to start at your home directry or / to start
at the root directoy).

#### touch
Touch isn't that important of a command but what it does is create a file given
a name.

```
touch <filename>
```

Play around with adding a files use ls to confirm your work.

#### rm
rm will remove files, careful with rm though there's no trashcan. If you remove
a file it's essentially gone forever, there's no warning it's just gone, so make
sure your removing only what you want to remove.

#### sudo
Some times you need to elevate your permissions  and act as a super user to
execute a command. Simply preface any command with sudo and it'll ask you for
your password, but then you'll have root access. If you ever have issues with
permissions you should be able to sudo the away.


[__If you're still confused or want to dig deepers here's a code accademy
tutorial, I've never done it myself, but codeacademy has good tutorials I've
done several other ones myself__](https://www.codecademy.com/learn/learn-the-command-line)


## Step 2: Git

Now that you understand the basics of command line lets move on to git. Git is
a tool used to save your programming projects. It's the tool that's enabled all
of open source. It was started by Linus Torvald the creator of Linux so we can
thank Linus for Linux and Git and therefore basically all of modern software
development. Linux is arguably the most impactful software project ever. It runs
90% of the internet and all 2 billion Android phones among other devices. But I
digress.

#### Installation

##### Method 1
I don't have windows so I don't really have a way to play with this, but this
should work... From the bash shell try:

```
apt-get install git
```
if that doesn't work
```
sudo apt-get install git
```

_If the command `git -v` returns anything version 2.9 or greater then you're good_

##### Method 2
[Follow Atlassian's installation tutorial](https://www.atlassian.com/git/tutorials/install-git#windows)

#### Create a GitHub account
[GitHub](https://github.com/) is essentially the google drive of software development.
It's a website that allows you to store the all you software so you can work on it
anywhere.

#### Pull this project
Now open up your bash shell and navigate to a place you can remember. Maybe
your desktop folder, but it doesn't matter. Once there run the command

```
git pull https://github.com/adc613/PythonLessons.git
```

This will download this git repository.

__Let me know once you've gotten to this point and I'll give you permission to
add to the repo__

Once you have permission. Try adding a file using touch. Then you can add a
that file to the commit using:
```
git add .
```

Git add will add whatever you specify, the . is an abreviation for the current
directory so it'll add everything in the current directory.

Then you need to create a commit like so:
```
git commit -m "<insert commit message that describes what you're commiting>"
```

Finally push it to GitHub using the command:
```
git push
```

In your web browser navigate back to this repo and see if your file is there. If
it is you did everything right.


## Extra Credit

[We'll go over git more next week, but here's a link to a really fantastic git
tutorial.](http://learngitbranching.js.org/). I highly recommend going through it.

Next week we'll start writting python code. Python should still be installed on
your surface but if not simply run the command:
```
sudo apt-get install python
```
You might not need to add sudo I don't know how the windows command line handles
some things.

With Python installed you can open up a shell by using the command `python`
or you can run a python file by using the command `python <filename>`


As always feel free to call/text me if you have any questions.
