# This won't take long...

![image](https://github.com/user-attachments/assets/12965408-dfab-420f-82ff-369fdf53bbef)

I try a random password but I get an error\
![image](https://github.com/user-attachments/assets/0fb161ec-6cfd-4dae-bd14-70b11c89beac)

I decide to check the source code

![image](https://github.com/user-attachments/assets/7f97bb6d-7680-4ed1-a6be-2d5da924ff65)

The javascript code seems interesting. Let's try to understand it.\
![image](https://github.com/user-attachments/assets/41c39247-d5ad-45d7-9035-040d11c88504)

This JavaScript code defines a function submitentry() that verifies a password entered by the user.\
It uses a string numletter that contains all digits, lowercase letters, and uppercase letters. \
The function constructs a password by extracting specific characters from this string using the substring() method.

Now that we have understood the code,lets try to extract each character and combining them to form  password\

var numletter="0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ";

Here are the index position of each character of the numletter variable\

| Index | Character |
|-------|-----------|
| 0     | 0         |
| 1     | 1         |
| 2     | 2         |
| 3     | 3         |
| 4     | 4         |
| 5     | 5         |
| 6     | 6         |
| 7     | 7         |
| 8     | 8         |
| 9     | 9         |
| 10    | a         |
| 11    | b         |
| 12    | c         |
| 13    | d         |
| 14    | e         |
| 15    | f         |
| 16    | g         |
| 17    | h         |
| 18    | i         |
| 19    | j         |
| 20    | k         |
| 21    | l         |
| 22    | m         |
| 23    | n         |
| 24    | o         |
| 25    | p         |
| 26    | q         |
| 27    | r         |
| 28    | s         |
| 29    | t         |
| 30    | u         |
| 31    | v         |
| 32    | w         |
| 33    | x         |
| 34    | y         |
| 35    | z         |
| 36    | A         |
| 37    | B         |
| 38    | C         |
| 39    | D         |
| 40    | E         |
| 41    | F         |
| 42    | G         |
| 43    | H         |
| 44    | I         |
| 45    | J         |
| 46    | K         |
| 47    | L         |
| 48    | M         |
| 49    | N         |
| 50    | O         |
| 51    | P         |
| 52    | Q         |
| 53    | R         |
| 54    | S         |
| 55    | T         |
| 56    | U         |
| 57    | V         |
| 58    | W         |
| 59    | X         |
| 60    | Y         |
| 61    | Z         |


We have to understand the substring fucntionality so as to extract the password\
The password is constructed by concatenating characters from the numletter string.\
The substring() method extracts characters at specified positions:
It extracts characters from a string between two specified indices. The first index is inclusive, and the second index is exclusive. This means that substring(23, 24) extracts the character at index 23, not 24.

let's reconstruct the password step by step:

*    numletter.substring(11, 12) is 'b' (index 11)
*    numletter.substring(18, 19) is 'i' (index 18)
*    numletter.substring(23, 24) is 'n' (index 23)
*    numletter.substring(16, 17) is 'g' (index 16)
*    numletter.substring(24, 25) is 'o' (index 24)
*    numletter.substring(1, 4) is '123' (indices 1, 2, 3)

Combining all the 7 characters,I get the passowrds as `bingo123`

Using the password, we complete the challenge. Hooray
![image](https://github.com/user-attachments/assets/daf0ca52-204d-439b-8b39-549b0c511c13)

