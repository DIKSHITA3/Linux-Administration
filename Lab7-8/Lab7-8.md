<h1>
  🚀 LAB 7-8 🚀
</h1>

<h2>
  1. Create the /home/consultants directory.
    <br><br>
  2. Add write permission to the consultants group using the symbolic method for setting permissions.
    <br><br>
  3. Forbid others from accessing files in the /home/consultants directory using the octal method.
    <br><br>
  4. Change the default umask for the operator1 user to prohibit all access for users not in their group. Confirm the umask is changed.
</h2>

<hr>

<h3>
  Solution :
</h3>

<h5>
  Lab 7:
</h5>

<b>Step 1:</b> Open the terminal and type:
   <i>
     sudo mkdir /home/consultants
   </i>

  ![image](https://github.com/user-attachments/assets/a4f8e775-1102-4f22-a245-b0f5355278e1)


<b>Step 2:</b> To add write permission for the consultants group:
   <i>
     sudo chmod g+w /home/consultants
   </i>

   ![image](https://github.com/user-attachments/assets/d6851212-9a69-4203-b6f3-25f927dda579)


<b>Step 3:</b> To forbid others from accessing the directory (octal method):
   <i>
     sudo chmod 770 /home/consultants
   </i>

   ![image](https://github.com/user-attachments/assets/f69a6347-5a98-4a0e-a9aa-46dba9b6c169)


<h5>
  Lab 8:
</h5>

<b>Step 1:</b> To change the default umask for operator1:
   <i>
     sudo usermod -s "/bin/bash" operator1
   </i>

<b>Step 2:</b> Edit the profile file to update the umask:
   <i>
     sudo nano /home/operator1/.profile
   </i>
   
![image](https://github.com/user-attachments/assets/4e80531b-7eb3-467d-b2e0-496527714ba8)

<b>Step 3:</b> Add the following line to set umask:
   <i>
     umask 007
   </i>

   ![image](https://github.com/user-attachments/assets/7bdbc4eb-4a6f-4662-a4a7-5d444fc28d30)


<b>Step 4:</b> Save and exit, then verify using:
   <i>
     umask
   </i>

   ![image](https://github.com/user-attachments/assets/d9cc6010-ea58-4745-8fbc-a10a14339363)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
