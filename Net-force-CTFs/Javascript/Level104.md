# Escape now

![image](https://github.com/user-attachments/assets/50689dee-c513-4316-918d-b71e5b4bc429)

I encounter a login form page and use random password but am denied access

![image](https://github.com/user-attachments/assets/4d44d6fc-ebd9-4242-98b2-3fcefc8734c5)

I decide to check the code

![image](https://github.com/user-attachments/assets/6aca583c-0f87-4ac7-a74d-b549a1f7d805)

Line 17 strikes my attention. It is a comment but it seems to be decoded

I start my research since I didn't know what unescape function is.

In MDN docs,\
The unescape() function replaces any escape sequence with the character that it represents.\ 
Specifically, it replaces any escape sequence of the form %XX or %uXXXX (where X represents one hexadecimal digit) with the character that has the hexadecimal value XX/XXXX. \
If the escape sequence is not a valid escape sequence (for example, if % is followed by one or no hex digit), it is left as-is.

This means that\
unescape decodes URL-encoded strings containing escape sequences.
Example: unescape("%3Cdiv%3E") returns <div>.

To decode the whole string I pasted it to **cyberchef** and used the URL decode to decodde the whole string

![image](https://github.com/user-attachments/assets/264b95b0-3a58-4910-b1dd-18881a3f2a0d)

THIS IS THE DECODED RESULT.It seems to be a html form. Now ,I think I understand how it is a javascript protection.

![image](https://github.com/user-attachments/assets/a163c73e-01d3-4fd1-b99a-fa2fcab7b11b)
![image](https://github.com/user-attachments/assets/9a59ada9-3992-404a-a558-b614c26c5f27)

Parameters:

    text1: The value entered in the username field.
    text2: The hardcoded string 'user'.
    text3: The value entered in the password field.
    text4: The hardcoded string 'member'.

Function validate checks if text1==text2 and text3==text4 are equal.

From this the \
Username is "user"
Password is "member"

I tested the username and password. They are correct. Hooray, another fun challenge

![image](https://github.com/user-attachments/assets/423062ad-74a3-43c0-8735-dca4d1a66d16)






