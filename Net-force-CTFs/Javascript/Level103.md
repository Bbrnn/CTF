# Is this safe...?!?

![image](https://github.com/user-attachments/assets/e66038dd-fbe7-4dfc-ba24-3e63a8b915e6)

I tried to login with a random password but I was directed to the home page

![image](https://github.com/user-attachments/assets/e989c193-cd5b-4932-955f-687217ef4932

I decide to view the source code

![image](https://github.com/user-attachments/assets/f6de983c-3ac8-4135-b510-297efd562970)

From the source code, I saw something that looks like the username and password

soulslayer:2aBl6E94IuUfo 

I try to login in with them but I am still directed to the home page

I inspect the source code again to see if I will find something interesting. I found something interesting in a javascript function.

![image](https://github.com/user-attachments/assets/d7d69556-b431-4c5f-930e-6a72257448e4)

From the function if the password is not null,visit the location whereby the location is:

location = user.toLowerCase() + "/" + pass.toLowerCase() + ".html";

user=soulslayer
pass=2aBl6E94IuUfo 

Location=soulslayer/2abl6e94iuufo.html

I concatente the location to the url of our challenge.\
The url still directs to the home page.\
I decided to move to the parent directory, /soulslayer

![image](https://github.com/user-attachments/assets/dedb7d72-22d1-422a-9258-41075cb5a534)

Clicking the blaat.html file ,I find the password

![image](https://github.com/user-attachments/assets/53966ccd-824a-4e08-ba9e-6c82013b12ea)


