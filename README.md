# ROverview: Lab 2 Renaming Windows Server 2022 and Installing Active Directory
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

![68747470733a2f2f692e696d6775722e636f6d2f354a66666939662e706e67](https://github.com/user-attachments/assets/86dd8148-a7b6-45a8-bddc-0e50d7b2e31b)

<br>
14. Click "Next," then choose "Role-based or feature-based installation" and click "Next" again to proceed.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f354a66666939662e706e67](https://github.com/user-attachments/assets/ab7da4d7-1f68-4ad5-9465-30e1e53e9349)

<br>

15.  Click "Next" again to proceed.

<br>

![68747470733a2f2f692e696d6775722e636f6d2f4c5565627538482e706e67 (1)](https://github.com/user-attachments/assets/16dfee87-d6a0-4f74-b44f-b535fdf1a6e1)


16. 



