**Bash Scripting Commands**

This README.md file explains various bash scripting commands in a concise way.


**Commands**

**echo Hello, World**

_Prints "Hello, World" to the console._

**echo \"\(\Ôo\)\'**

_Prints a smiling face emoticon with the text "
\Ô
�
\Ôo" enclosed in single quotes._

**cat /etc/passwd**

_Displays the contents of the "/etc/passwd" file._

**cat /etc/passwd /etc/hosts**

_Displays the contents of both the "/etc/passwd" and "/etc/hosts" files._

**tail /etc/passwd**

_Displays the last 10 lines of the "/etc/passwd" file._

**head /etc/passwd**

_Displays the first 10 lines of the "/etc/passwd" file._

**head -3 iacta | tail -1**

_Displays the third line of the "iacta" file._

**`echo "Best School" > '*\'''"Best School"'''\*$?*****:)'**

_Creates a file named "'"Best School"''\$?*****:)" and writes "Best School" to it._

**ls -la > ls_cwd_content**

_Lists all files and directories in the current directory and saves the output to a file named "ls_cwd_content"._

**tail -1 iacta >> iacta**

_Appends the last line of the "iacta" file to the end of the "iacta" file._

**find . -name '*.js' -type f -delete**

_Finds all files with a ".js" extension and deletes them._

**find ./* -type d -print | wc -l**

_Counts the number of directories in the current directory._

**ls -t | head**

_Lists the files in the current directory sorted by modification time, and displays the first 10._

**sort | uniq -u**

_Sorts the input and removes any duplicate lines._

**grep "root" /etc/passwd**

_Finds and displays all lines containing the string "root" in the "/etc/passwd" file._

**grep bin /etc/passwd | wc -l**

_Finds and counts all lines containing the string "bin" in the "/etc/passwd" file._

**grep -A 3 root /etc/passwd**

_Finds all lines containing the string "root" in the "/etc/passwd" file and displays the 3 lines after each match._

**grep -v bin /etc/passwd**

_Finds and displays all lines that do not contain the string "bin" in the "/etc/passwd" file._

**grep "^[A-Za-z]" /etc/ssh/sshd_config**

_Finds and displays all lines in the "/etc/ssh/sshd_config" file that begin with a letter._

**tr "Ac" "Ze"**

_Translates all "A" and "c" characters in the input to "Z" and "e", respectively._

**tr -d [cC]**

_Deletes all "c" and "C" characters from the input._

**rev**

_Reverses the characters of each line of the input._

**cut -d":" -f 1,6 /etc/passwd | sort**

_Cuts the first and sixth fields of each line in the "/etc/passwd" file using ":" as the delimiter and sorts the output._

**find . -empty -printf "%f\n"**

_Finds all empty files in the current directory and displays their names._

**find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f**

_Finds all files with a ".gif" extension in the current directory and its subdirectories, extracts their filenames without the extension, sorts them alphabetically, ignoring case._

**cut -c 1 | paste -s -d ''**

_Takes the first character of each line of input, concatenates them into a single string, and displays the result._

**tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev**

_Processes the input, ignoring the first line, cuts the first field of each remaining line using a tab as a delimiter, sorts and counts the unique values, sorts them in reverse order, and displays the 10 most frequently occurring values with their counts._
