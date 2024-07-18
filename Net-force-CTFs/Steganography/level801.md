# Training - Can you see me?
![image](https://github.com/user-attachments/assets/307bafbb-750a-4b9b-b0d5-4505b147046d)

 The description is vague. It does not provide a clue on how to solve the challenge so I decide to view the source code.
 
 ![image](https://github.com/user-attachments/assets/cfa5295d-e10d-4346-8865-7a91fcf58547)

From the source code, we are given a hint. We should look for a password.gif file and mwe might be able to solve this challenge and go to the next one.\
Let's try. \
I had some problem finding the file, so I decided to change the url by appending the name of the file to the original url.\
Boom there we go, I found the file.\

![image](https://github.com/user-attachments/assets/b6ee8381-cf8c-48e0-b099-7d57446b9537)

I used this command\
`wget https://www.net-force.nl/challenge/level801/password.gif`

It seems this is a polygot file as it can be opened as a plain text file and contains readable ASCII text, which is unusual for a typical image file.

![image](https://github.com/user-attachments/assets/2eda2f89-dbc6-428d-a067-75db25bb5092)

Lets try opening the file using a text editor, nano

![image](https://github.com/user-attachments/assets/07d5107b-cbca-4710-a805-4889d19aaf75)



 
