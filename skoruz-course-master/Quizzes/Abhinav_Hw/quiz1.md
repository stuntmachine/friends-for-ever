1. Suppose that the Current Working Directory is /lib/modules, give a single "CAT" command using a relative pathname
and a command using an absolute pathname, that would print out the contents of the regular file /lib/security/pam-access.
Command with Absolute Path:CAT /lib/security/pam-access

Command with Relative Path:CAT /security/pam-access

2. What is the standard command to determine the pathname/location  of the mv command/program.
ANS: "which" command to be used.

3. What is the purpose of the /sbin subdirectory? (I.e., what is normally stored there?)
ANS: Executable programs are stored(which are ready to run)

4. Explain the difference between “the root directory” and “root’s directory”.
ANS: The root directory is the directory which contains all other directories and files on the system and
     which is designated by a forward slash(/).
	 The root's directory  is the home for root users.
	 

5. Explain what the term “search path” means in the context of a shell (like Bash).
ANS: A search path is the sequence of directories where the shell looks for commands to execute.

6. What are two commands that could be used to display your current search path?
ANS: %echo $path , %printenv PATH

7. Suppose your current env PATH variable is set to /usr/bin:/bin:/usr/local/bin. Explain what
the shell does when you type the command “foo” at a prompt (and type return).
ANS: no command "foo" found.

8. Logged in as a non-root user, is /sbin in your search path? Explain why it is or is not
there.
ANS: Its not in search path. we need to root it.

9. Suppose you have created a shell script named foo and have made it executable, but
when you type it as a command (“foo”), Bash says: “command not found”. What is
wrong and what must you do to run the command?
ANS: We need to set the script permissions to executable:

chmod +x ./foo

10. Explain why the Linux does not have drive letters like Windows does.
ANS:Linux doesn’t have drive letters. Instead, it makes other file systems accessible at arbitrary directories.
    On Linux, everything is under / – the root directory. There are no files above the root directory, as there 
	are files outside of C: on Windows.

11. What is the contents of a file ~/song.mp3?

12. What command would show all lines containing the string “brace expansion” (ignoring
case) in the man pages for Bash? 
ANS: grep -i {brace expression}

13. What command would delete some files from the directory /tmp, where the relevant
filenames have this pattern: they begin with “A” or “B”, contain the string “406”, and
have a (final) extension of “.txt” or “.text”.

14. What are the commands that will reset the current working directory to your home directory, regardless of what directory you are currently in?
Ans: cd \home, cd ..

15. What are hidden files in Linux/UNIX, why are they called that, and what are they
commonly used for?
ANS:In Unix-like operating systems, any file or folder that starts with a dot character (for example, /home/user/.config), 
    commonly called a dot file or dotfile, is to be treated as hidden – that is, the ls command does not display them unless
	the -a flag (ls -a) is used.
	They are commonly used for storing user preferences or preserving the state of a utility, and are frequently created 
	implicitly by using various utilities.

