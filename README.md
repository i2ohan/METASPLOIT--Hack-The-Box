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
  
![MSF](https://user-images.githubusercontent.com/62021583/187682038-4e11289c-9974-47d7-a798-73b6ff06d200.jpg)


USING ETERNALBLUE : 
 
WE USE ETERNALBLUE EXPLOIT ON WINDOWS BINDING ON MHY SMB(SERVER MESSAGE BOX). 
SMB IS RUNNING ON PORT 445 WHICH WE OBTAINED DURING OR NMAP SCAN. 

![image](https://user-images.githubusercontent.com/62021583/187677887-48579da9-5e33-4839-b3fd-47bc0e1865e4.png)

![MSR](https://user-images.githubusercontent.com/62021583/187682063-4296c7b9-928d-44fc-b30a-f48e256aa3bf.jpg)


ABOVE SCREENSHOT TELLS US THAT THE TARGET IS VULNERABLE AS IT IS USING WINDOWS 7 ULTIMATE SERVICE PACK x64 WHICH IS AN EXPIRED VERSION. 

![S1](https://user-images.githubusercontent.com/62021583/187684886-d1fb6317-5c55-4595-8f09-c2a875668f39.jpg)


![K2](https://user-images.githubusercontent.com/62021583/187683249-45fc337b-6808-49d8-854b-3d416a779a70.jpg)

 
AFTER RUNNING THE EXPLOIT WE GET A METERPRETER SHELL AS WE SET THE PAYLOAD AS METERPRETER/REVERSE_SHELL  . 
IF WE TYPE HASHDUMP- WE WILL OBTAIN THE PASSWORD HASHES OF ADMIN AND USERS,WHICH CAN EASILY BE CRACKED BY SHA-256 OR MD-5 HASH DECRYPTER. 
HENCE,CREATING EASY ACCESS TO TARGET MACHINE. 

SINCE WE CREATE A REVERSE SHELL THE TARGET WONT KNOW THAT A REMOTE HOST CAN CONTROL IT AND HAS FULL ACCESS TO THEIR DEVICE. 

 ![K3](https://user-images.githubusercontent.com/62021583/187683381-96c1ed8e-c583-458f-a37c-a83efcc41fed.jpg)

THIS CONSOLE WILL TELL IF THERE IS ANY FURTHER VULNERABILITY IN THE MACHINE AND IT IS PATCHED OR NOT. 

 ![R2](https://user-images.githubusercontent.com/62021583/187685903-7acec769-8d13-43f0-911e-c2fe3add592e.png)


 ![K1](https://user-images.githubusercontent.com/62021583/187682142-3807860f-44e4-4a66-85a1-d647ebcec4bc.png)
 
![image](https://user-images.githubusercontent.com/62021583/187678835-5846abbc-51f9-4a51-865b-ccb34da331a5.png)

![image](https://user-images.githubusercontent.com/62021583/187678859-e0996d35-7603-434a-afbf-ff7f0002347c.png)

MACHINE HAS BEEN PATCHED.

 ![image](https://user-images.githubusercontent.com/62021583/187678892-5e590316-34f3-4307-9248-9e5a7b45075d.png)

  
