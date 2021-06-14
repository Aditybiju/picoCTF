# **PicoCTF**

## **(Cryptography)**

**CHALLENGE NAME: Mod 26**

**DESCRIPTION:**

Cryptography can be easy, do you know what ROT13 is? cvpbPGS{arkg\_gvzr\_V&#39;yy\_gel\_2\_ebhaqf\_bs\_ebg13\_jdJBFOXJ}

**APPROACH:**

It is ROT13 encrypted . Used the following command to decrypt it :

echo &#39;cvpbPGS{arkg\_gvzr\_V\&#39;yy\_gel\_2\_ebhaqf\_bs\_ebg13\_jdJBFOXJ}&#39; | tr &#39;A-Za-z&#39; &#39;N-ZA-Mn-za-m&#39;

**FLAG:** picoCTF{next\_time\_I&#39;ll\_try\_2\_rounds\_of\_rot13\_wqWOSBKW}

**CHALLENGE NAME: The Numbers**

**DESCRIPTION:**

The [numbers](https://jupiter.challenges.picoctf.org/static/f209a32253affb6f547a585649ba4fda/the_numbers.png)... what do they mean?

**APPROACH:**

We can easily understand that it is a1z26 cipher.So used a decoder and got the flag.

**FLAG:** PICOCTF{THENUMBERSMASON}

**CHALLENGE NAME: Easy1**

**DESCRIPTION:**

The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We&#39;ve given you the encrypted flag, key, and a table to help UFJKXQZQUNB with the key of SOLVECRYPTO. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.

**APPROACH:**

Use the table to decrypt the flag by using key(row) to intersect the corresponding ciphertext(column)

**FLAG:** picoCTF{CRYPTOISFUN}

**CHALLENGE NAME: 13**

**DESCRIPTION:**

Cryptography can be easy, do you know what ROT13 is? cvpbPGS{abg\_gbb\_onq\_bs\_n\_ceboyrz}

**APPROACH:**

This is ROT13 encrypted so can be decrypted by using the command:

echo &#39;cvpbPGS{abg\_gbb\_onq\_bs\_n\_ceboyrz}&#39; | tr &#39;A-Za-z&#39; &#39;N-ZA-Mn-za-m&#39;

**FLAG:** picoCTF{not\_too\_bad\_of\_a\_problem}
