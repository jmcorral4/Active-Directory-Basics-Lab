# 💻 PowerShell-Based Active Directory Setup

### ✅ Install AD DS Role
- Install-WindowsFeature -Name AD-Domain-Services -IncludeManagementTools <br>
  ![image](https://github.com/user-attachments/assets/f5394580-7796-43ef-9940-6abb5beebc51) <br>
- You'll then see it as a True statement if installed correctly <br>
  ![image](https://github.com/user-attachments/assets/d33eeb06-50d0-4b68-a8dc-1fcb71c5a209) <br>
- Now you can add a Forest domain for the villains. This one was aptly called `legionofdoom.local`
  ![image](https://github.com/user-attachments/assets/437bf7d7-52a4-449a-8201-e31cdcd96d66)
- By using the command Get-ADDomain we can pull the information of our newly created Domain.
  ![image](https://github.com/user-attachments/assets/782861d9-1503-42d9-b328-08402b7be555)
- Next step will be for us to add our Organizational User (OU) in the `legionofdoom.local` Domain
  ![image](https://github.com/user-attachments/assets/46007646-289d-498a-b7e1-c0b7478ea0bf)
- To verify we can use "Get-ADOrganizationalUnit -Filter ' Name -like "*" '| Format-table Name
- The script will then give us the name of our newly created OU
  ![image](https://github.com/user-attachments/assets/537268fa-e6b4-4122-9973-fd444799a428)
- Now we can add a User into the OU
  ![image](https://github.com/user-attachments/assets/307c5518-d62b-47f5-9d04-f4fc934f965d)
- The user information will now show to us like this.
  ![image](https://github.com/user-attachments/assets/23afd5b5-4c03-4951-af92-6fae691c0e23)
- The user's information would look like this in the Active Directory Users and Computers (ADUC)
  ![image](https://github.com/user-attachments/assets/9e88e52a-d6a4-43fc-afa7-51c94b2a989e)
- Lastly, we can right click on the windows start icon and choose the option 'run'. From there we can search dsa.msc bringing up our ADUC. Clicking on our OU, Hall of Doom, will allow us to see the user, Lex Luthor, within as a member.
# A tip I saw while working on the lab was that the Organizational Unit will have a different icon compared to the other containers within the Domain created in the Forest.



























































