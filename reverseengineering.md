# **PicoCTF**

## **(Reverse Engineering)**

**CHALLENGE NAME:**** Transformation**

**DESCRIPTION:**

I wonder what this really is... [enc](https://mercury.picoctf.net/static/77a2b202236aa741e988581e78d277a6/enc) &#39;&#39;.join([chr((ord(flag[i]) \&lt;\&lt; 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])

**APPROACH:**

After opening the file we find a text &quot;灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸強㕤㐸㤸扽&quot;.I encoded this with base64(54Gp5o2v5I2U5Jm744S25b2i5qW0542f5qWu542044y05pGf5r2m5by45by345Wk45C446S45om9) and converted base64 to octal.Octal was converted to hexadecimal.At the end hexadecimal is converted to text which gives the flag.

**FLAG:** picoCTF{16\_bits\_inst34d\_of\_8\_75d4898b}

**CHALLENGE NAME:**** vault-door-training**

**DESCRIPTION:**

Your mission is to enter Dr. Evil&#39;s laboratory and retrieve the blueprints for his Doomsday Project. The laboratory is protected by a series of locked vault doors. Each door is controlled by a computer and requires a password to open. Unfortunately, our undercover agents have not been able to obtain the secret passwords for the vault doors, but one of our junior agents obtained the source code for each vault&#39;s computer! You will need to read the source code for each level to figure out what the password is for that vault door. As a warmup, we have created a replica vault in our training facility. The source code for the training vault is here: [VaultDoorTraining.java](https://jupiter.challenges.picoctf.org/static/a4a1ca9c54d8fac9404f9cbc50d9751a/VaultDoorTraining.java)

**APPROACH:**

So after opening the java file we can see a part at the end wherein the password is mentioned.

**FLAG:** picoCTF{w4rm1ng\_Up\_w1tH\_jAv4\_be8d9806f18}

**CHALLENGE NAME:**** vault-door-1**

**DESCRIPTION:**

This vault uses some complicated arrays! I hope you can make sense of it, special agent. The source code for this vault is here: [VaultDoor1.java](https://jupiter.challenges.picoctf.org/static/ff2585f7afd21b81f69d2fbe37c081ae/VaultDoor1.java)

**APPROACH:**

So after opening the java file we can see a part at the end wherein the password is mentioned.

**FLAG:** picoCTF{w4rm1ng\_Up\_w1tH\_jAv4\_be8d9806f18}
