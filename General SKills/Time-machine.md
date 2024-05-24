# Time machine

**Description**

What was I last working on? I remember writing a note to help me remember...\
You can download the challenge files here:\
challenge.zip

**Hints**
1. The cat command will let you read a file, but that won't help you here
1. Read the chapter on Git from the picoPrimer here<https://primer.picoctf.org/#_git_version_control>.
1. When committing a file with git, a message can (and should) be included.

# Solution

* Firstoff ,I downloaded the zip file **challenge.zip**
* Then i unzipped using **unzip challenge.zip** command and found drop-in folder
* I then cd drop-in
* From the description,the author says he left a note to help remember
* After checking out the resource provided in the hint,I will use **git log** to see past commits
* Boom,found the flag

![Solution](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/71eab1d9-9f34-4302-b827-c082a2663760)
