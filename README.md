# Overview: Lab 2 Renaming Windows Server 2022 and Installing Active Directory
In this home lab, I will be demonstrating the process of Renaming Server 2022 and Installing Active Directory in a home lab environment. I'll be using VirtualBox and be focusing on simulating a real-world IT setup. It serves as a practical demonstration of key IT administrative tasks, such as configuring server names, setting up Active Directory, and managing domain services.

## Objectives
- Rename a Windows Server 2022 instance to meet organizational standards.
- Install and configure Active Directory Domain Services (AD DS).
- Create and manage user accounts, groups, and security policies within Active Directory.

## Documentation
Now that we have Windows Server 2022 set up, we can proceed with installing Active Directory on our virtual machine home lab. Before that, let's rename our computer to keep things simple. 

<br>

1. 
![68747470733a2f2f692e696d6775722e636f6d2f5876656e6d42372e706e67](https://github.com/user-attachments/assets/6870e688-99a2-452e-ac1b-222367757f99)
<br>

2. To do so, open File Explorer from the taskbar, right-click on "This PC," and select "Properties."

![68747470733a2f2f692e696d6775722e636f6d2f75596c756a66342e706e67](https://github.com/user-attachments/assets/d969f7ba-ddcd-4b4a-8e36-76ab61ff7c34)

<br>

3. In the "About" section, scroll down until you see "Rename this PC (Advanced)" and click on it.
   <br>

![68747470733a2f2f692e696d6775722e636f6d2f565443326b384e2e706e67](https://github.com/user-attachments/assets/ffafe7c1-27fe-4757-b6df-525c5ca2ad8f)

<br>

4. Select “Change”.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f47634e544851442e706e67 (1)](https://github.com/user-attachments/assets/f2b11d17-ec95-4581-962e-85bf8913fec7)

<br>

5. We will rename the computer to "Server2022" and then click "OK." A prompt will appear asking you to restart your virtual machine, which is normal. Click "OK," then select "Restart Now" to apply the changes.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f59714f6f7632732e706e67](https://github.com/user-attachments/assets/76198685-b3e9-4672-a1a2-dca4ff75761b)

<br>
6. Click "OK," then select "Restart Now" to apply the changes.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f59714f6f7632732e706e67](https://github.com/user-attachments/assets/1be681c1-c607-4896-baa2-e42fa8209c55)

<br>

7. Proceed to log in the same way as before. Once you’ve logged into your administrator account, verify the renamed computer by following the same steps: open File Explorer, click on "This PC," then "Properties," and select "Rename this PC (Advanced)." Under "Full computer name," you should now see "Server2022.”

<br>

![68747470733a2f2f692e696d6775722e636f6d2f486252436f72612e706e67](https://github.com/user-attachments/assets/d19e83ca-76f5-4fac-8a4e-04b98fb0dbd0)

<br>

8. To optimize our performance for running virtual labs more efficiently, let's go to the search bar at the bottom left, type "About your PC," and search 

<br>

![68747470733a2f2f692e696d6775722e636f6d2f394f6848326f592e706e67](https://github.com/user-attachments/assets/48197a18-f9f7-4eab-9fef-71bc178bce7c)

<br>

9. Select "Advanced system settings."
    

    <br>

    ![68747470733a2f2f692e696d6775722e636f6d2f70764f4a5a70432e706e67](https://github.com/user-attachments/assets/922fb13a-ffc5-4d66-95d6-7d843257ff39)

<br>

10. In the "System Properties" window, click on the "Settings..." button under the "Performance" section.


<br>

![68747470733a2f2f692e696d6775722e636f6d2f345450394456542e706e67 (1)](https://github.com/user-attachments/assets/17aff466-a5aa-48eb-abae-41a3457f98eb)

<br>

11. In the "Performance Options" window, select "Adjust for best performance," then click "OK" to apply the changes.

    <br>
    
![68747470733a2f2f692e696d6775722e636f6d2f354a66666939662e706e67 (1)](https://github.com/user-attachments/assets/8457bbef-32f8-4f03-9f1b-53aeba85ec91)


<br>

12. Next, we will install Active Directory on our Server2022. Open Server Manager, click on "Manage" in the top right corner, then select "Add Roles and Features."

<br>

![68747470733a2f2f692e696d6775722e636f6d2f466f69587047372e706e67 (1)](https://github.com/user-attachments/assets/b60ac04c-b146-427d-80ec-3ba1a020205f)

<br>
13. Click "Next," then choose "Role-based or feature-based installation" and click "Next" again to proceed.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f474b686b5a434d2e706e67](https://github.com/user-attachments/assets/47a22314-b991-4833-b360-5b25e7e3c221)

<br>

14. Select "Active Directory Domain Services," then click "Add Features" when prompted and click next.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f4d4d435859627a2e706e67](https://github.com/user-attachments/assets/d4ea2f41-64ef-4e9a-983d-94c166575e96)


<br>

15. After that, click "Next" to continue.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f426749367441322e706e67](https://github.com/user-attachments/assets/c766a576-f8aa-4c27-805f-f184628ce8e8)

<br>

16. Finally select “Install”.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f4a5775443132562e706e67](https://github.com/user-attachments/assets/93e2be01-c09b-4c6d-959a-1bc1fd8f82bd)

<br> 

17. Select “Promote this server to a domain controller”.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f676964454449692e706e67](https://github.com/user-attachments/assets/dfb26ae2-c8c2-482d-9c6f-d466d4da4db6)

<br> 


18. Select "Add a new forest" and enter "tobifash.com" as the root domain name. Then click "Next" to proceed.


<br> 

<img width="542" alt="Screenshot 2025-02-14 at 12 02 51 AM" src="https://github.com/user-attachments/assets/607fab91-afc9-4db4-9f73-09e5ecb97eff" />

<br>

19. Create a password for our Directory Service Restore Mode (DSRM) then click “Next”.

<br>

<img width="542" alt="Screenshot 2025-02-14 at 12 03 41 AM" src="https://github.com/user-attachments/assets/2869f9c4-838d-4de6-ba10-f8f4aa4ed8f2" />

<br>

20. We can uncheck “Create DNS delegation” then click “Next” then “Install”.
<br>

![68747470733a2f2f692e696d6775722e636f6d2f627333337a524f2e706e67](https://github.com/user-attachments/assets/c38cdd0d-abae-4728-a5a2-37ab47bfa057)

<br>
21. Click “Install”.
<br>

![68747470733a2f2f692e696d6775722e636f6d2f437a45317554312e706e67 (1)](https://github.com/user-attachments/assets/585061b7-4b0f-447d-9197-1255f43b3de0)


<br>

22. After this process, the virtual machine will restart to install Active Directory Domain Services. Once the restart is complete, sign back in by selecting "Input" and clicking the "Ctrl + Alt + Del" button. You will notice that the domain controller is now listed as "Tobifash/Administrator." Go ahead and sign in to your account using the domain credentials.

<br>

<img width="633" alt="Screenshot 2025-02-17 at 2 04 20 AM" src="https://github.com/user-attachments/assets/a83d8f04-f41e-4738-ada4-d689daa7785b" />

<br>

23. Once signed in, with Server Manager open, click on "Tools" in the top right corner, then select "Active Directory Users and Computers" from the dropdown menu.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f61613237774a792e706e67](https://github.com/user-attachments/assets/85fd3ddc-355c-46b0-96e8-6231eb51957c)

<br> 

24. Congratulations we have successfully created a domain controller (SimoTech.com) with Active Directory installed!

<br> 

<img width="542" alt="Screenshot 2025-02-14 at 12 15 22 AM" src="https://github.com/user-attachments/assets/91d93516-9c22-491c-aed1-68724842fcdb" />

<br>


👉 Next Lab 3 : [Active Directory Account Creation, CMD Commands](https://github.com/tobifash0/Active-Directory-Account-Creation-CMD-Commands)









