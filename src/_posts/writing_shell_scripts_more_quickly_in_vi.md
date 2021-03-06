{
  "layout": "post",
  "title": "Writing shell scripts more quickly in vi",
  "date": "Mon Jul 20 2009 00:00:00 GMT+0100 (BST)",
  "description": "A couple of useful tips for writing shell scripts more quickly using the vi editor.",
  "tags": [
    "Linux"
  ]
}

## Shell scripts

If you are on a POSIX compliant machine (OSX or Linux) you can make use of Shell Scripts to do day-to-day donkey work. I use Shell Scripts for backups, cleaning out temporary folders, profiling and logging. Writing these scripts is pretty straightforward and if you are completely new to it I recommend getting a copy of [Classic Shell Scripting][1].

Recently I came across a couple of shortcuts that have greatly reduced the time it takes to write a script in the vi editor. 

## Run shell commands from within vi

Using :! from within vi you can run a shell command. This is great as you don't need to exit vi to test your code. Let's say for example your script is called myscript.sh. You can run your script from within the vi editor by using. 

    :!myscript.sh

Furthermore you can make more changes in vi, save the file and then run the script again by using 

    :!!

This is a shortcut to the last command issued to the shell, allowing you to retest your shell script without even typing the filename. 

## The % variable

Within vi the % variable refers to the file that you are currently editing. So to run the script you are editing from within vi you can also use: 

  :%

 [1]: http://oreilly.com/catalog/9780596005955/
