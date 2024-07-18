# Training - Javascript, secure?
![image](https://github.com/user-attachments/assets/02eb0225-f67b-4b4d-b72f-b76fee9fed95)

Clicking the secret web page link, I find this page 

![image](https://github.com/user-attachments/assets/94883ea4-9e69-4b7f-a753-d2345848f148)

I try a random username and password and am denied access

![image](https://github.com/user-attachments/assets/025eb61c-c094-4a25-b48b-d2b55dea8de6)

I decide to check the source code

![VIEW-SOURCE](https://github.com/user-attachments/assets/8d58169a-dd2b-4e63-a59d-2f09d63687c8)

I try to understand what the code does.

This HTML and JavaScript code creates a simple authentication prompt on a webpage.\ 
When the page loads, it prompts the user for a username and password. \
A preset username value "kiddie" and password "javascript" are initialized.\
The username and password are checked to verify they match the preset values. \
If the username is incorrect, an "ACCESS DENIED!!!" alert is shown, and the page reloads. \
If the username is correct but the password is incorrect, the same alert is shown, and the page reloads. \
If both the username and password are correct, a success alert is displayed, and the user is redirected to a challenges page. \
The code uses `prompt()` for input and `alert()` for messages.

Now that I know the username and password to use, let's try logging.

Username: kiddie\
Password: javascript 

![username](https://github.com/user-attachments/assets/52eeb35b-0dc1-4a7d-97c5-4b230fcadfb2)\
![password](https://github.com/user-attachments/assets/1cee20ee-db93-4828-9785-9934d161f1a6)

After logging in using the credential, I get a message\
![image](https://github.com/user-attachments/assets/1fe4402d-5d40-4daa-a534-e36eb16a79c7)

I am redirected to the main page and use the password. Challenge solved!\
![image](https://github.com/user-attachments/assets/96c7ce97-b3a0-47e6-bea6-14d5c787476d)






