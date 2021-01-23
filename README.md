# shell-data-processing

<br>
Some of the commands which might be useful.
Need to add more :smiley:

<br>
Command used to get the data : curl "http://www.eastoftheweb.com/short-stories/UBooks/ManCoug.shtml" -o try.txt
Command to sort the common words : tr ' ' '\12' < story.txt | sort | uniq -c | sort -nr > result.txt
##############################################################################
### BASH BASICS


env      &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;     &nbsp; &nbsp; &nbsp; &nbsp;    # displays all environment variables
<br>
echo $SHELL     &nbsp;    # displays the shell you're using
<br>
echo $BASH_VERSION  # displays bash version
<br>

bash                 # if you want to use bash (type exit to go back to your previously opened shell)
<br>
whereis bash        # locates the binary, source and manual-page for a command
<br>
which bash          # finds out which program is executed as 'bash' (default: /bin/bash, can change across environments)
<br>
clear               # clears content on window (hide displayed lines)
<br>

##############################################################################
### FILE COMMANDS

<br>


ls                            # lists your files in current directory, ls <dir> to print files in a specific directory
<br>
ls -l                         # lists your files in 'long format', which contains the exact size of the file, who owns the file and who has the right to look at it, and when it was last modified
<br>
ls -a                         # lists all files in 'long format', including hidden files (name beginning with '.')
  <br>
ln -s <filename> <link>       # creates symbolic link to file
  <br>
touch <filename>              # creates or updates (edit) your file
  <br>
cat <filename>                # prints file raw content (will not be interpreted)
<br>
any_command > <filename>      # '>' is used to perform redirections, it will set any_command's stdout to file instead of "real stdout" (generally /dev/stdout)

<br>
more <filename>               # shows the first part of a file (move with space and type q to quit)
<br>
head <filename>               # outputs the first lines of file (default: 10 lines)
<br>
tail <filename>               # outputs the last lines of file (useful with -f option) (default: 10 lines)
<br>
vim <filename>                # opens a file in VIM (VI iMproved) text editor, will create it if it doesn't exist
<br>
mv <filename1> <dest>         # moves a file to destination, behavior will change based on 'dest' type (dir: file is placed into dir; file: file will replace dest (tip: useful for renaming))
  <br>
cp <filename1> <dest>         # copies a file
  <br>
rm <filename>                 # removes a file
