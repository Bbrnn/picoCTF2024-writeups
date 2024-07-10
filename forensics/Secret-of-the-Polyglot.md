# Secret of the polygot

**Description**
The Network Operations Center (NOC) of your local institution picked up a suspicious file, 
they're getting conflicting information on what type of file it is. 
They've brought you in as an external expert to examine the file. 
Can you extract all the information from this strange file?
Download the suspicious file here.

**Hints**
1. This problem can be solved by just opening the file in different ways

   
## Solution

I download the file and it happens to be a pdf file\
From the hint I can solve the problem by opening the file in various ways\
I open the pdf file first befor analysing it
![pdf](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/922023b5-ea4f-4ba0-8065-55e2b6930a18)
It looks like a piece of our flag.

After opening the pdf file ,I continue with my analysis.\
I research on different ways to open a pdf file

I found this helpful article <https://developnsolve.com/how-to-open-pdfs-in-linux-simple-guide>

Now ,I will check the metadata of the downloaded file using the command\
`pdfinfo  name_file`

It seems to be a png image file .This is odd. 
I research on the meaning of polygot and now it makes sense how the file is a pdf but its signature identifies it as png image file

**Polygot**\
A polyglot file in cybersecurity is a type of file that is designed to be interpreted in multiple ways, depending on the software used to open it. 
This can be used as a technique to evade antivirus software or as a way to create malicious files that can exploit different applications.

I rename the file using png extension
![rename_png](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/39a5b754-61ec-4ac0-934c-b9b4ece03185)

Opening the rename png file, I find this. It looks like a part of our flag
![flag](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/eba6eb2c-01e7-4ce6-854e-a66010464c5f)

Now,I have two parts of the flag.As you can remember,when I opened the pdf file ,I found a part of our flag
1n_pn9_&_pdf_7f9bccd1}

I also found another part of the flag after renaming the pdf file to png 
picoCTF{f1u3n7_

Combining both parts of the flag makes it whole and Bingo I found the flag.








