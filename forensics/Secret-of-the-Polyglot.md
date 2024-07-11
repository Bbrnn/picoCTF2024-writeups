# Secret of the polygot

**Description**

The Network Operations Center (NOC) of your local institution picked up a suspicious file, \
they're getting conflicting information on what type of file it is. \
They've brought you in as an external expert to examine the file. \
Can you extract all the information from this strange file?\
Download the suspicious file here.

**Hints**
1. This problem can be solved by just opening the file in different ways

   
## Solution

I downloaded the file, and it happens to be a PDF file. Based on the hint, I can solve the problem by opening the file in various ways. I opened the PDF file first before analyzing it.

![pdf](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/922023b5-ea4f-4ba0-8065-55e2b6930a18)

It looks like a piece of our flag.

After opening the PDF file, I continued with my analysis. I researched different ways to open a PDF file and found this helpful article:<https://developnsolve.com/how-to-open-pdfs-in-linux-simple-guide>

From the article,I decided to use the pdftotext tool.I found the same flag I found at the beginning.

![pdftotext](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/c81a29c3-ebf2-4eae-b28b-c2c1ea9ca24f)


Next, I checked the metadata of the downloaded file using the command:

`pdfinfo  name_file`

![pdfinfo](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/2cfaa2f7-097a-492d-a580-911facb52ced)
I did not find anything interesting.

I decided to check what type of file it is\
![file](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/aa89cf8c-3e9d-448b-ae79-6350e526be98)

Interestingly, it seemed to be a PNG image file. This was odd. I researched the meaning of polyglot, and now it makes sense how the file is a PDF but its signature identifies it as a PNG image file.

**Polyglot**

A polyglot file in cybersecurity is a type of file that is designed to be interpreted in multiple ways, depending on the software used to open it. This can be used as a technique to evade antivirus software or as a way to create malicious files that can exploit different applications.


I renamed the file using png extension
![rename_png](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/39a5b754-61ec-4ac0-934c-b9b4ece03185)

Opening the renamed PNG file, I found this. It looks like another part of our flag.
![flag](https://github.com/Bbrnn/picoCTF2024-writeups/assets/113863725/eba6eb2c-01e7-4ce6-854e-a66010464c5f)

Now,I have two parts of the flag.\
As you can remember,when I opened the pdf file ,I found a part of our flag which also happens to be the same flag as the one I found using the pdftotext command:\
1n_pn9_&_pdf_7f9bccd1}

I also found another part of the flag after renaming the pdf file to png :\
picoCTF{f1u3n7_

Combining both parts of the flag makes it whole, and Bingo! \
I found the flag: picoCTF{f1u3n7_1n_pn9_&_pdf_7f9bccd1}.







