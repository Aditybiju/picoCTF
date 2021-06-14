# **PicoCTF**

## **(Forensics)**

**CHALLENGE NAME: information**
--------------------------------

**DESCRIPTION:**

Files can always be changed in a secret way. Can you find the flag? cat.jpg

**APPROACH:**

They have provided a hint to look at the details of the file.The metadata provides all the text information in an image.So i used exiftool to extract the metadata.I found that in the details there is a part wherein the license is provided which seemed to be a base64 encoded.which upon decryption using the command : **echo&quot; &quot; | base64 -d** to get the flag.

**FLAG:** picoCTF{the\_m3tadata\_1s\_modified}

**CHALLENGE NAME: Matryoshka doll**
--------------------------------

**DESCRIPTION:**

Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What&#39;s the final one? Image: [this](https://mercury.picoctf.net/static/2978e1270538613cd8181c7b0dabe9bd/dolls.jpg)

**APPROACH:**

In the hints they have mentioned about hiding files inside file.So i tried unzipping the image file do get another folder having an image file in it.Move to the sub-folder and unzip the image file which results in similar sub-files having another image.Repeat the step 3 times until we get flag.txt. **Cat flag.txt** returns the flag

**FLAG:** picoCTF{the\_m3tadata\_1s\_modified}

**CHALLENGE NAME: MacroHard WeakEdge**
--------------------------------

**DESCRIPTION:**

I&#39;ve hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/d3dd8cd51524d9fafcccd1b7d55f85e7/Forensics%20is%20fun.pptm)

**APPROACH:**

Using binwalk we can see that the file type is zip.Upon unzipping the file using the command :&quot; **unzip Forensics\ is\ fun.pptm**&quot; we can see that there is a file named hidden in a folder ppt.By using the command we get a base64 encoded text. Which upon decryption gives the flag.

**FLAG:** picoCTF{D1d\_u\_kn0w\_ppts\_r\_z1p5}
