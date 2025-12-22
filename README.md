<h2>This is a secure linux backup server that synchronizes data from client machine while defending against unauthorized access, data loss, disk theft and ransomeware file deletion.</h2>


This project demonstrates secure authentication, encryption in transit and at rest, least previledge, logging, monitoring and disaster recovery planning. here's how i did it,

<h2>Firstly, i installed the required package</h2>

<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/6cf9b78f-c060-4f82-8283-a47305d637ac" />


<h2>The next step was to create a dedicated backup user.</h2>
this prevents backups from running as root, limits damage if credentials are compromised and it also demonstrates the principle of least previledge.
i made it as simple as possible...



<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/e92a228c-0713-458d-b1d7-27b552567944" />



<h2>Then i added a secure SSH access (using a file editor). disabled root login and only allowed backuser access..</h2>

The use of SSH keys prevents password attacks and disabling root login to only backup user is a critical hardening step


<img width="1794" height="833" alt="image" src="https://github.com/user-attachments/assets/0d029c67-41e0-4590-be24-a4e0ba4af493" />


<img width="829" height="220" alt="image" src="https://github.com/user-attachments/assets/b8277ea7-067e-47c7-86ce-60caed712917" />



<h2>i went ahead to encrypt the backup vault incase if data is stolen it remains unreadable</h2>



<h2
