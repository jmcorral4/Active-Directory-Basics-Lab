# 🖥️ GUI-Based Active Directory Setup

### ✅ Step 1: Open Server Manager
- Click the Windows Start icon
- Open **Server Manager**
- The lab required us to Deploy the ADDS

![image](https://github.com/user-attachments/assets/c1a2b3f1-2396-400e-9e47-6c5040ac90a5) <br>
![image](https://github.com/user-attachments/assets/69e58729-da44-4c71-9719-3dd6e90b2729) <br>
![image](https://github.com/user-attachments/assets/a0e22441-cf38-4ee7-a51c-18933b721310) <br>

### ✅ Step 2: Add Roles and Features
- Right click on domain `superfriends.local` and choose New> Organizational Unit (OU) <br>
  ![image](https://github.com/user-attachments/assets/855fc326-efc5-46e1-897b-765b7085efc5) <br>
- The OU was named Hall of Justice in order to separate Heroes and Villains between GUI and Powershell <br>
  ![image](https://github.com/user-attachments/assets/71d6148e-dc4a-453a-b7e3-3437669d42de) <br>
- Now Right click on the new OU in the Active Directory Users and Computers (ADUC) and choose New> User <br>
![image](https://github.com/user-attachments/assets/68976562-4faf-42db-ae16-6a886ec9c719)
- Add User information. In this example I used Bruce Wayne <br>
![image](https://github.com/user-attachments/assets/fcf6d4c2-a6ad-429b-94fa-344bee36c20d) <br>
- Now we can verify that the user is under the OU and within the domain of superfriends.local <br>
![image](https://github.com/user-attachments/assets/69150e28-d403-4091-956d-0f68403405ad) <br>
- Following Microsoft's recommended principle of AGDLP (Account, Global, Domain Local, Permission) I also set a group to have Bruce Wayne as a member. <br>
- Right click on the OU and choose New> Group <br>
![image](https://github.com/user-attachments/assets/ea7e398c-9179-4c10-b9da-df6eb254ff4f) <br>
- We simply name the group now and proceed with keeping it a Global group <br>
![image](https://github.com/user-attachments/assets/ae330b66-2cfa-45b0-a099-c86040e1ae71) <br>
- We can check to see if it was done correctly by seeing the security group under the OU, Hall of Justice. <br>
![image](https://github.com/user-attachments/assets/6f3bf117-a3ad-454d-8e0a-50275aa5a14a)
...

### 🧩 Domain Created: `superfriends.local`

### 👤 User Created: `Bruce Wayne`

### 👥 Group Created: `Heroes`
