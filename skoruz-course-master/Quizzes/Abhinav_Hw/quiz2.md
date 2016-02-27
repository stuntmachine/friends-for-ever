
QUIZ2        

1. What command would list all the files in the current working directory?
Ans: Command - ls 

2. What is the simplest command for adding execute permission to file ~/foo, for all users
(without changing any other permissions)?

Ans:   chmod +777 foo
          chown +755 foo


3. Explain what execute permission means/allows when it is associated with a directory.
Ans: Basically it means you can tell the operating system to run the code in the file. For example, if the file was a binary executable, write access would allow you to modify it, read access would allow you to view it, but without execute permissions you would not be able to run the program. In the case of a script, its a little more complicted, because you don't necessarily need to 'run' the program, you can just read its contents into an interpreter, which itself has the execute privelige, but you do not need execute permissions on the script itself.




4. Suppose that you wanted all users on the machine to be able to see the contents
of the file ~/public/software/instructions.text. Explain the minimum set of
permissions for files and directories needed to allow this, and any security issues that
arise.




5. Suppose that you want to allow (only) other users bob and chuck to be able to access
the above file. Explain what you would have to do differently from what you described
above. (You are not allowed to consider the use of ACLs.)
Ans: -rwxr--rwx ,  chmod 747 filename



6. How would your answer to the previous problem change if you were to use ACLs (access
control lists)?




7. What are set UID (SUID) files, and when are they typically used?
Ans: SUID (set  user ID) is the special type of file permissions given to the file. When the programs run, it inherits the access permission from the logged in users. SUID gives temporary permission to the user to run the program with the permission of the file owner rather than the user. It allows anyone to become the temporary files owner while being executed in the memory.


8. Find one SUID file on a Linux system, and show its “long listing” (permissions, owner,
etc.).
Ans: -rwsr-xr-x. 1 root root 30768 Feb 22  2012 /usr/bin/passwd
 



9. Why are SUID root files considered a security issue?
Ans: They are managing dangerous filesystem permissions. Executable files with SUID OR SGID are favourite malicious users. The executable permission allow anyone to become files owner while its being executed in the memory. The riskiest case is if the file's owner is root. 


10. What command would be used to set a file foo to be SUID, and how exactly would it
be done?
Ans: chmod u+s foo
        chmod 4750 foo


11. What command could determine the process ID (PID) of a running SSH server (sshd)?
Ans: Ps -ef | grep sshd	



12. What command would best identify which process is using excessive CPU resources?
Ans: Command-Top


13. What command that should definitely terminate the process identified above?
Ans: Command-Kill


14. What file contains the list of valid user ID’s (UID’s) and their associated usernames?
Ans; /etc/passwd


15. What file contains passwords on a Linux system (if that system is using local authen-
tication rather than NIS, etc.)?
Ans: /etc/shadow



16. What is difference between telnet and ssh. When will you use each command. give examples.
Ans: Telnet:
Telnet is the joint abbreviation of Telecommunications and Networks and it is a networking protocol best known for UNIX platform.Telnet uses the port 23 and it was designed specifically for local area networks.Telnet is not a secure communication protocol because it does not use any security mechanism and transfers the data over network/internet in a plain-text form including the passwords and so any one can sniff the packets to get that important information.
SSH:
SSH stands for Secure Shell and it is now only major protocol to access the network devices and servers over the internet.SSH runs on port 22 by default; however it can be easily changed.SSH is a very secure protocol because it shares and sends the information in encrypted form which provides confidentiality and security of the data over an un-secured network such as internet.

.

