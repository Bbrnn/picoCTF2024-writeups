# Commit issues
<https://play.picoctf.org/practice/challenge/411?category=5&originalEvent=73&page=1>

**Description**\
I accidentally wrote the flag down. Good thing I deleted it!
You download the challenge files here:\
* challenge.zip

# Solution

First I checked out the hints we have been given.It seems we will need github commands.<br>
Luckily, we have been provided a link to understand github commands.<br>
Check it out here:\
<https://primer.picoctf.org/#_git_version_control>

Now,download the zip file,challenge.zip.Then unzip it using unzip challenge.zip command.\
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/c986570c-9697-4c80-82d8-2b71f1bd9cdb)
After unzipping ,I found drop-in folder

Next step is to **cd drop-in**\
Then **ls** to display the contents of drop-in folder\
After you will find a file called *message.txt*\
To display content of the file run **cat message.txt**\

You can use ** git log ** to checkout prior commits.\
I found one of the commits that says **create a flag** with commit ID 6603cb4ff0c4ea293798c03a32e0d78d5ab12ca2


![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/be72e1aa-7568-4e8b-844a-d4713656b470)









