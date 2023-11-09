Cryptography

-------------------------------------

in this challenge we got zip file and its protected with a password and in challenge description there is password policy lets read it

Password Policy
The first character should be small\
The second character should be capital
The third character should be a symbol between (@&$)
The fourth character should be a number between (0-9)
The last thing you should put one of these names (feras,salem,basurrah)
Examples of a possible password: aA@0feras yS&4basurrah

so we have to generate a list of all possible combinations of letters that meet the password policy

so lets make python code that generate the list (u can use ChatGPT and it will help u to make this code)


![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/4e43cb4d-3705-42c8-ac94-6912c615c904)

lets run the code and save the output to txt file

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/c8031d13-0fc8-43a1-bb1f-341ac2b30f66)


now we got txt file the contain all possible combinations

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/e25236c9-a3c6-4e22-b77f-138ffb0208ce)


now we will use tool that cracked zip or rar files called john the ripper

we will use it by using the command : rar2john (filename) > (any output name) 

note: you can search more about john the ripper tool to learn more

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/599b4de5-5cc7-4ab9-bc4e-7c774a3229b5)


i got mm file output now i will use john command and the list of the passwords we did to crack it 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/4f2da1e5-9f67-40a0-830f-e133031c25c8)

We found the password:jY$2salem

now lets try to open the rar file using this password

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/60783666-9acf-40ed-ae8c-1d47a9927a7b)


we opend the rar and found txt file inside it and we open it and got the flag
