Steganography challenge

--------------------------------------------------------------------------------

in this we got a zip file so lets unzip it 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/53ae434c-20e8-4e44-9c39-c9c2579e4b0c)

we got a folder 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/2becce34-98ff-44d5-9a8a-4c156be05157)

so there is a 248 of same photo so we have to find if there is any photo seems different 

we used ls -l to list the file and see the time 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/fdfe275f-94e1-4135-9252-2729b67d00bf)

we found out that photo 248 and 2 has different time so lets try to stegcrack photo 248

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/ad9c61b7-6bf1-47f2-ba42-9dfa1ca0674d)

ok we found a password and its (orange) lets check the output file that we got from 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/cdf53ee4-dddd-434e-bb71-2404a0e4bf97)

unfortunately its fake flag , but luckily we have the password so lets make shell code or python code that steghide all the photos using password : orange  (u can ask ChatGPT it will do it for u)

we made this code because its best practice because if we have 100 fake flag we can't do it manually 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/6cb984bc-a70e-42c7-8b77-32ef4da5b034)

now we run the script

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/10098b59-a453-45b3-a96d-dabf0d85f4d2)

we got some output from some photos so now we will open all the txt files that we got from the photos using command : cat *.txt (*.txt means any .txt file in the folder)

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/9a9ee054-7f68-495f-98f8-de83cfc4eff9)

and thats how i got the flag
