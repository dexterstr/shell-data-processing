# shell-data-processing

<br>
Some of the commands which might be useful.
Need to add more :smiley:

<br>
Command used to get the data : curl "http://www.eastoftheweb.com/short-stories/UBooks/ManCoug.shtml" -o try.txt
<br>
Command to sort the common words : tr ' ' '\12' < story.txt | sort | uniq -c | sort -nr > result.txt
<br>
[Data File]()
[Result File]()
<br>
## BASH BASICS


env      &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;     &nbsp; &nbsp; &nbsp; &nbsp;    # displays all environment variables
<br>
echo $SHELL     &nbsp;    # displays the shell you're using
<br>
echo $BASH_VERSION  # displays bash version
<br>

bash              &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;   # if you want to use bash (type exit to go back to your previously opened shell)
<br>
whereis bash     &nbsp; &nbsp; &nbsp; &nbsp;   &nbsp; &nbsp;  # locates the binary, source and manual-page for a command
<br>
which bash      &nbsp; &nbsp; &nbsp; &nbsp;   &nbsp; &nbsp;   # finds out which program is executed as 'bash' (default: /bin/bash, can change across environments)
<br>
clear           &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp;    # clears content on window (hide displayed lines)
<br>

z
### FILE COMMANDS

<br>


ls               &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;              # lists your files in current directory, ls <dir> to print files in a specific directory
<br>
ls -l             &nbsp; &nbsp; &nbsp; &nbsp;             # lists your files in 'long format', which contains the exact size of the file, who owns the file and who has the right to look at it, and when it was last modified
<br>
ls -a                 &nbsp; &nbsp; &nbsp; &nbsp;         # lists all files in 'long format', including hidden files (name beginning with '.')
  <br>
ln -s <filename> <link>   &nbsp; &nbsp; &nbsp;     # creates symbolic link to file
  <br>
touch <filename>        &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;       # creates or updates (edit) your file
  <br>
cat <filename>          &nbsp; &nbsp; &nbsp; &nbsp;       # prints file raw content (will not be interpreted)
<br>
any_command > <filename>    &nbsp; &nbsp; &nbsp; &nbsp;   # '>' is used to perform redirections, it will set any_command's stdout to file instead of "real stdout" (generally /dev/stdout)

<br>
more <filename>         &nbsp; &nbsp; &nbsp; &nbsp;       # shows the first part of a file (move with space and type q to quit)
<br>
head <filename>        &nbsp; &nbsp; &nbsp; &nbsp;        # outputs the first lines of file (default: 10 lines)
<br>
tail <filename>       &nbsp; &nbsp; &nbsp; &nbsp;         # outputs the last lines of file (useful with -f option) (default: 10 lines)
<br>
vim <filename>        &nbsp; &nbsp; &nbsp; &nbsp;         # opens a file in VIM (VI iMproved) text editor, will create it if it doesn't exist
<br>
mv <filename1> <dest>     &nbsp; &nbsp; &nbsp; &nbsp;     # moves a file to destination, behavior will change based on 'dest' type (dir: file is placed into dir; file: file will replace dest (tip: useful for renaming))
  <br>
cp <filename1> <dest>     &nbsp; &nbsp; &nbsp; &nbsp;     # copies a file
  <br>
rm <filename>         &nbsp; &nbsp; &nbsp; &nbsp;         # removes a file
