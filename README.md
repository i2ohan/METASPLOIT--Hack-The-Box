# METASPLOIT--Hack-The-Box

DEVELOPED BY - ROHAN MEHTA


PENETRATION TESTING – EXPLOITING VULNERABILITIES OF A TARGET MACHINE AND NOTIFYING IT AND THEN HOST DOES THE PATCHING OF THOSE BUGS FOR SECURITY OF THE CLIENT  

HOST : KALI LINUX 
IP ADDRESS: 10.0.2.15(LHOST) 
LPORT - 4444 

 ![image](https://user-images.githubusercontent.com/62021583/187677270-538c54e8-df2b-4979-8e24-85a345c625d9.png)

 
   
TO EXPLOIT: 
 
TARGET : BLUE MACHINE 
(WINDOWS MACHINE) 
IP ADDRESS: 10.0.2.5(RHOST) 
 
 ![image](https://user-images.githubusercontent.com/62021583/187677640-0d36b1fd-e4ae-4bcb-b6b6-853695996b57.png)

![image](https://user-images.githubusercontent.com/62021583/187677727-eaf0f62f-5580-49d8-8815-0e9924ac60bf.png)

![image](https://user-images.githubusercontent.com/62021583/187677768-1674d4e8-efe6-4723-a5ce-6236b4876039.png)

  
MSFCONSOLE- METASPLOIT: 
  
![image](https://user-images.githubusercontent.com/62021583/187677887-48579da9-5e33-4839-b3fd-47bc0e1865e4.png)

USING ETERNALBLUE : 
 
WE USE ETERNALBLUE EXPLOIT ON WINDOWS BINDING ON MHY SMB(SERVER MESSAGE BOX). 
SMB IS RUNNING ON PORT 445 WHICH WE OBTAINED DURING OR NMAP SCAN. 



ABOVE SCREENSHOT TELLS US THAT THE TARGET IS VULNERABLE AS IT IS USING WINDOWS 7 ULTIMATE SERVICE PACK x64 WHICH IS AN EXPIRED VERSION. 
 
![image](https://user-images.githubusercontent.com/62021583/187678835-5846abbc-51f9-4a51-865b-ccb34da331a5.png)


 
AFTER RUNNING THE EXPLOIT WE GET A METERPRETER SHELL AS WE SET THE PAYLOAD AS METERPRETER/REVERSE_SHELL  . 
IF WE TYPE HASHDUMP- WE WILL OBTAIN THE PASSWORD HASHES OF ADMIN AND USERS,WHICH CAN EASILY BE CRACKED BY SHA-256 OR MD-5 HASH DECRYPTER. 
HENCE,CREATING EASY ACCESS TO TARGET MACHINE. 

SINCE WE CREATE A REVERSE SHELL THE TARGET WONT KNOW THAT A REMOTE HOST CAN CONTROL IT AND HAS FULL ACCESS TO THEIR DEVICE. 





![image](https://user-images.githubusercontent.com/62021583/187678859-e0996d35-7603-434a-afbf-ff7f0002347c.png)

 
THIS CONSOLE WILL TELL IF THERE IS ANY FURTHER VULNERABILITY IN THE MACHINE AND IT IS PATCHED OR NOT. 
 

 
 ![image](https://user-images.githubusercontent.com/62021583/187678892-5e590316-34f3-4307-9248-9e5a7b45075d.png)

MACHINE HAS BEEN PATCHED. 
  
