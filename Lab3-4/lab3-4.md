<h1>
  🚀 Experiment 3 - 4 🚀
</h1>

<h3>
  1. View the gedit man page.<br><br>
  2. Use the man -k ext4 command to find the command to tune ext4 file-system parameters.<br><br>
  3. Understand and demonstrate the use of brace expansion.
</h3>

<hr>

<h1>
  Solution : 
</h1>

<h5>
  Lab 3: 
</h5>

  1. Open the terminal and type:
     <i>
       man gedit
     </i>
     
     ![image](https://github.com/user-attachments/assets/01232dbf-01cf-49cc-b3fa-bbb4d358476f)


  2. If the manual page is not available, try installing `gedit` first:
     <i>
       sudo apt update && sudo apt install gedit
     </i>
     
     ![image](https://github.com/user-attachments/assets/05a1bbd1-fc49-4985-8c1e-31eb7704feee)


<h5>
  Lab 4:
</h5>

  1. To search for commands related to ext4, type: <br>
     <i>man -k ext4</i>
     
     ![image](https://github.com/user-attachments/assets/52092925-77fb-43fd-b653-d29c9a67c679)


  2. To find the command to tune ext4 file systems, look for `tune2fs` in the output and check its manual page:
     <i>man tune2fs</i>
     
     ![image](https://github.com/user-attachments/assets/3d1bdedb-f6fe-4f80-b77c-b33744b1092e)


  3. Understanding Brace Expansion: <br>
     <i>echo file{1,2,3}.txt</i><br>
     Output:
     <pre>file1.txt file2.txt file3.txt</pre>

     ![image](https://github.com/user-attachments/assets/2b3b7aee-5349-43e7-b0e0-dd966ab8bdd2)


  4. Using a sequence expression:
     <i>echo file{1..5}.txt</i>

     ![image](https://github.com/user-attachments/assets/04f9a880-3172-4e85-afe6-ede3e290f1e3)

     
