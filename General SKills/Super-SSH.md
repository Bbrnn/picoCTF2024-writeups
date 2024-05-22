# Super ssh

## Description

Using a Secure Shell (SSH) is going to be pretty important.\
Can you ssh as ctf-player to titan.picoctf.net at port 56651 to get the flag?\
You'll also need the password 6dd28e9b. If asked, accept the fingerprint with yes.\
If your device doesn't have a shell, you can use: <https://webshell.picoctf.org>
If you're not sure what a shell is, check out our Primer: <https://primer.picoctf.com/#_the_shell>

### Solution
 
From the hints provided,the syntax to use is:\
**ssh user@hostname -p port_number**

To get the flag,I will ssh into the shell using this command

**ssh ctf-player@titan.picoctf.net -p 56561**\

If prompted this ,Are you sure you want to continue connecting (yes/no/[fingerprint])? \
Answer yes

Then enter the password 6dd28e9b\
Hooray,I have found the flag\

![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/65e58889-6ef6-45c4-a5b2-a11f55ec456c)



