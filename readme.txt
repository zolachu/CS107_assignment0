File: readme.txt
Assignment: assign0
Author: Zolboo Chuluunbaatar
Preferred Gender Pronouns: Zola
----------------------

0. Tell us about yourself!  What do you do for fun?  Tell a quick anecdote about something that you feel makes you unique; a talent, experience, anything.

I binge watch k-dramas. Also, I guess the fact that I am from Mongolia makes me unique.

1. Please initial below to confirm your course enrollment.

[ZC] I have read and understood the CS107 collaboration policy at https://cs107.stanford.edu/collaboration.html. By adding my initials, I affirm my intention to abide by this policy.

INTRUDER DETECTION ACTIVITY
2a)

1.   touch new.txt
2.   touch newHome.txt
3.   echo |cat samples/server_files/users.list > new.txt
4.   ls ./samples/server_files/home/ > newHome.txt

These will copy all the directory names in ./server_files/home to newHome.txt
 and copy names in ./server_files/user.list to new.txt

5.   diff new.txt newHome.txt

command shows the following result

38a39
> mattv


Therefore the intruder's username was "mattv".



2b)
go to
   cd  ./samples/server_files/home/mattv

   ls -al

to print out all the hidden files

   emacs ./bash_history

will print out the activity history


2c)
go to
   cd  ./samples/server_files/home/mattv

   grep -R "sudo" .
   command will print out lines where the intruder used sudo command.

dmesg
emacs /etc/passwd
cp -r /etc /mnt/usb/etc
su


These 4 are the commands where the intruder executed using sudo.
