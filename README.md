<h2>This project involves setting up a Linux system to function as a backup server. The aim was to understand how backups are handled in a Linux environment and how data can be transferred securely between systems.</h2>


<h2>Tools used</h2>
Linux (ubuntu)

rsync

SSH keys

<h2>project description</h2>

In this lab, I configured a Linux server to act as a central location for storing backup files. A dedicated non root user was created on the server in order to apply the principle of least privilege, and secure access was configured using SSH.

Secure access to the server was configured using SSH. Backups were performed from a client system to the server using rsync, allowing files to be transferred efficiently and securely. The setup was tested to ensure that files were copied correctly and stored as expected on the backup server.



<h2>Lab set up and process<h2>
 
 firstly i installed and updated the server


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/f8964b0c-d4e1-4f65-82ad-d81681153700" />


<h2>Then i enabled the SSH keys. which is very important for secure access..</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/060ad964-2d2c-4279-a6ce-50642a5f79ee" />



<h2>I created a dedicated backup user, created the backup directory,set the ownership and also the rights and permission..</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/e89605f9-44e7-4757-8e74-0ba5a1a6b317" />


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/827b0117-0c34-4d20-9531-0fd8a8830748" />


<h2>The next step was to configure an SSH key, copy it to the server and test the login..</h2>



<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/5557aa8c-99b2-495d-ac84-16b4d45b9128" />


<h2>After i logged in and confirmed it using the "whoami" command. I hardend the SSH configuration using a file editor (nano). After which i restarted it and confirmed it was all set then i started the backup process...</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/47998e5e-7598-4a62-a655-c4487b184d09" />



<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/aa8b6d2a-799a-4708-8e4b-feb3a4e208db" />


<h2>After backing it up and confirming it. i tested it using the "rsync" command and i got the expected output from the backup which is "test.txt".</h2>




<h2>I went further to locate the directory in which the backed up file is located</h2>


<img width="1792" height="832" alt="image" src="https://github.com/user-attachments/assets/43c98d0c-c966-40c3-b7b5-1d951d184d0e" />


<h2>Results..</h2>

Files were successfully backed up from the client to the server

Data transfers were encrypted using SSH

Backup operations were performed using a non root user

The backup process worked reliably during testing

 <h2>what i learned</h2>
  
This project taught me how to secure a Linux server using SSH key-based authentication, apply least-privilege access with a non-root user, and perform secure backups with rsync. It also improved my understanding of Linux permissions, user management, and real-world troubleshooting of security and access issues.











