Forensics challenge

------------------------------------------------

in this challenge we downloaded a file called CMD.pf 

We have to search about pf files first so lets search ....


after the search we find out that pf=Prefetch file and from the challenge description we knew that we have to analayze the file somehow so lets search about Prefetch Files cmd analyze

after we search we found out this https://www.socinvestigation.com/pecmd-windows-prefetch-analysis-for-incident-responders/ tool called PECmd and its related to the challenge name so lets download it and use it 



![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/c40c1208-bc6a-4fe6-a165-14f02a5f68b4)

we used this Command in cmd

 PECmd.exe -f CMD.pf 

![image](https://github.com/Muh4nnad/UJ-WRITEUP/assets/150369756/720499e8-ad63-4922-8a9b-eea1570434ee)

and from the output we can see the flag 

thats it..
