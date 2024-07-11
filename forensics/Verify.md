# Verify

**Description**

People keep trying to trick my players with imitation \
flags. I want to make sure they get the real thing! I'm \
going to provide the SHA-256 hash and a decrypt \
script to help you know that my flags are legitimate.\
You can download the challenge files here:\
challenge.zip
Additional details will be available after launching your challenge instance.


**Hint**
1. Remember you can pipe the output of one command to another with |.\
Try practicing with the 'First Grep' challenge if you're stuck!
1. You can create a SHA checksum of a file with sha256sum <file> or\
all files in a directory with sha256sum <directory>/*.
1. Remember you can pipe the output of one command to another with |.\
Try practicing with the 'First Grep' challenge if you're stuck!

**I launched the instance and I found this addditional details.**

The same files are accessible via SSH here:\
ssh -p 63398 ctf-player@rhea.picoctf.net\
Using the password 84b12bae. Accept the fingerprint with yes, and ls once connected to begin. \
Remember, in a shell, passwords are hidden!\
Checksum: 3ad37ed6c5ab81d31e4c94ae611e0adf2e9e3e6bee55804ebc7f386283e366a4\
To decrypt the file once you've verified the hash, run ./decrypt.sh files/<file>.\

## Solution

I decided to solve the challenge using pico commandline. I ssh into the challenge and downloaded the file.
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/1cce5dec-111a-4eb6-81b1-a68bedcdd53c)

I went ahead and unzipped the zipped file and found this checksum text file\
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/5bc6ce0f-da67-4a72-9798-780675fadd05)

From the hint,I can check the checksum of files in a directory so I did that using the command given in the hint\
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/2f5f4e78-9797-4335-8fd5-26d174cb158a)

Next,I looked for a file with the same checksum value that matches the one in the description. To solve this I used grep command as hinted above
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/26a4c17d-acbe-4abd-bb48-be418ffe4131)

After finding the file with the same checksum value as the one that am looking for ,I display the type and contents of the file.It seemed the file had been encrypted.
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/ac022796-21a1-47a0-bc8f-b9c5cb422803)

I utilized the decrypt script to decrypt the file.\
![image](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/3e4fe365-75cc-4da2-91f9-0e87ba68a2ec)

Decrypting the file ,I find the file. Bingo








