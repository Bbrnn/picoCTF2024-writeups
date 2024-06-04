# Interencdec-Picoctf

**Description**

Can you get the real meaning from this file.
Download the file here.

**Hints**
1. Engaging in various decoding processes is of utmost importance

# Solution

* First,I downloaded the file,enc_flag
* I used the command cat enc_flag to display the contents of the file. The content seemed to be base64 encoded.
* Using this command `echo "base64_string' |base64 -d`,I was able to decode
* After decoding, I checked the contents again. It was still base64 encoded.
* So i decided to decode it again using the same command from 
* Well,The resulting string was still encoded, but the format resembled our flag.
* I visited this site <https://www.dcode.fr/caesar-cipher> to decode the string
* By using the Caesar Cipher tool on the website, I successfully decoded the string.
* Finally,I found the flag-It seemed to have been a caesar cipher.

However,you can  also use online base64 decoders

![base64_decoding](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/8374ef9d-7ed1-4ada-aff8-a3cfc07c684d)

![caesar_cipher](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/5900608f-7a6c-472a-bdff-42f9b4b644ca)



