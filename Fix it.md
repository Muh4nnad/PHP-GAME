Forensics challenge

----------------------------------------------------------

We have a jpeg file lets try to open it,

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/91e397cc-2fac-4ab9-b96f-7c02c0bdfdaf)

We can see that there is some error in the format so lets open HXD and check the file

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/a15a588f-033a-41e4-ac30-705aa3f2f678)

oh the jpeg Hex Signature is wrong it should start with FF D8 not 00 D8 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/6917dffd-cf0d-42c5-a4dd-8f07aa399df5)

here we can see the correct jpeg Hex Signature 

use this website to find all files signature https://www.garykessler.net/library/file_sigs.html

ok now we will change the signature using HXD  

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/a494d766-7b0c-4a77-ac17-fdf0c342598d)

now lets open the photo again

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/cf92fbf4-68a7-4d96-ab89-d2913eadf239)

We fixed the photo and now we got the flag
