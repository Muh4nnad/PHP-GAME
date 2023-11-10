Cryptography challenge

---------------------------------------------------------------------

in this challenge we got txt file so lets open it first

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/6c1590be-7dca-47cd-afbb-d2fba5487721)

we got this base32 message so let put it on cyberchef

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/593e84a7-e9f1-4b26-b6c9-6479eb4f8559)

we can see that there is a encrypted message in the message 

so lets try decrypt this base message 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/cb482366-886d-4aec-8348-9d268142d34e)

ok we got half of the message using Base85 so i think the other half after { is encrypted with another Base so lets try

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/7008b545-83f8-40d1-9d56-ef119310ca99)

ok we found the other half and it was encrypted using Base58

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/fdf7eab8-c90f-4472-b2e8-78392a185375)


no we have a list of numbers and after i tried a lot of things i came back to ascii table again 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/d6e8f1a5-9a54-46cd-8298-b16d38e8ef87)

the problem is the ascii table is to 127 and we have numbers up to 753 so i got a plan 

we have this first char 513 447 405 537 405  and i think its flag format so thats mean
513= U  447= J 405= C 537= Y 405= C

now i have to find way to make 513 number = U and in ascii table we know that (U=85)

so i tried to divide 513 many times to get 85 and i found that 513/6 = 85

then i went to next number and divide 447/6 and i got 74 and 74=J in ascii table 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/39311b47-5803-42d5-b199-6d660163e7b2)


so i think we are in the right way and we need to divide every number by 6 to get the character in ascii table 

( you can do it manually but i made a python code that save ascii table and get input from the user and divide it by 6 then give the character result)

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/08063d3c-4c13-44aa-bc09-5dcc9d67884a)

after i divide all numbers by 6 i got the flag

sometimes you have to use your mind , tools will not solve everything




