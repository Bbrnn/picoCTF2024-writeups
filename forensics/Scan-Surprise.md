# Scan surprise

**Description**

I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead?
You can download the challenge files here:
challenge.zip
Additional details will be available after launching your challenge instance.

**Hints**

1. If you don't have access to a phone, you can also use zbar-tools to convert an image to text
1. Mobile phones have included native QR code scanners in their cameras since version 8 (Oreo) and iOS 11
1. If you don't have access to a phone, you can also use zbar-tools to convert an image to text

## Solution

I donloaded the challenge zip file and unzipped it.I found a png file which turned out to be a qr code.\
![image](https://github.com/user-attachments/assets/8e284b65-93b1-44d8-8689-905cd5c4a40a)

![image](https://github.com/user-attachments/assets/737338b6-7758-4167-9214-76321e650fb1)


From the hints, I can use zbar tools to convert the image to text.\
I researched how to download and use zbar tools to scan the image\
You can use these commands to download zbar tools and scan the image file\
`sudo apt install zbar-tools`

`sudo zbarimg flag.png`

![image](https://github.com/user-attachments/assets/3c137bbf-a2f8-4764-a814-5442b17c3e17)\
I have found the flag. Yay


