<h2>This project demonstrates how to build a secure linux backup server using SSH key authentication and least previledge principles.</h2>
i configured rsync backups over encrypted channels, disabled rooot access and applied filesystem protections to mitigate possible ransomeware attacks.

Here's how i did it, firstly i installed and updated the server


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/f8964b0c-d4e1-4f65-82ad-d81681153700" />


<h2>Then i enabled the SSH keys. which is very important for secure access..</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/060ad964-2d2c-4279-a6ce-50642a5f79ee" />



<h2>I created a dedicated backup user, created the backup directory,set the ownership and also the rights and permission</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/e89605f9-44e7-4757-8e74-0ba5a1a6b317" />


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/827b0117-0c34-4d20-9531-0fd8a8830748" />


<h2>The next step was to configure an SSH key, copy it to the server and test the login..</h2>



<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/5557aa8c-99b2-495d-ac84-16b4d45b9128" />


<h2>After i logged in and confirmed it using the "whoami" command. I hardend the SSH configuration using a file editor (nano). After which i restarted it and confirmed it was all set then i started the backup process...</h2>


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/aa8b6d2a-799a-4708-8e4b-feb3a4e208db" />


<h2>After backing it up and confirm it, i tested it using the "rsync" command and after getting the expected output from the backup which is "test.txt".</h2>

<img width="1771" height="421" alt="image" src="https://github.com/user-attachments/assets/0c209593-cc51-4428-93f6-dbc1cc0e7785" />



<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/47998e5e-7598-4a62-a655-c4487b184d09" />


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/5d7bfb0d-72a8-426c-ae8e-5b45df8b4ad4" />













