
![39](https://github.com/carlos-m-romero/Virtual_Private_Network_VPN_IP_Address_Observations/assets/148396073/b81a71d0-89d1-4b17-8141-d2f7c50f710c)


<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this project, I observed the impact of a virtual private network (VPN) on IP address, location, and web browsing.  <br />


  
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
-	Remote Desktop
-	ProtonVPN (free version)


<h2>Operating System Used </h2>

- Windows 10 (21H2)

# Lab Tutorial: Setting Up VPN in an Azure Virtual Machine

## Objective
Gain a better understanding of VPNs by setting up a Virtual Private Network inside an Azure virtual machine. This lab will explore the impact of VPNs on IP addresses and locations.

## Step-by-Step Guide

1. Start by accessing the website "whatismyipaddress.com" on your actual PC. Take note of your public IP address and the corresponding city.

2. Create a virtual machine in Azure and establish a connection to it using Remote Desktop Protocol (RDP). This connection bridges your PC and the Azure virtual machine.

3. Within the Azure virtual machine, visit the website "whatismyipaddress.com" once again. This time, note down the new IP address and location. It should differ from your actual PC's IP address.

4. Sign up for the free version of ProtonVPN on your PC. Download and install the ProtonVPN client.

5. Inside the Azure virtual machine, connect to a ProtonVPN server located in Japan (or another available country). This establishes a VPN connection between the virtual machine and the chosen ProtonVPN server.

6. Access the website "whatismyipaddress.com" again from within the Azure virtual machine, with the VPN active. Take note of the new IP address and location displayed. This IP address should reflect the location of the VPN server (e.g., Tokyo, Japan).

By following these steps, you will have three entries in your text file representing different IP addresses and locations:

1. IP address and location from your actual PC without using a VPN.


[Screenshot Here: PC IP Address]
![36](https://github.com/carlos-m-romero/Virtual_Private_Network_VPN_IP_Address_Observations/assets/148396073/f1c50e86-7f84-4423-8af8-ef0573ba81db)


4. IP address and location from the Azure virtual machine without using a VPN.


[Screenshot Here: Azure VM IP Address]

![37](https://github.com/carlos-m-romero/Virtual_Private_Network_VPN_IP_Address_Observations/assets/148396073/560ea571-b6b7-45d3-b107-2afaea9aa197)


5. IP address and location from the Azure virtual machine with the VPN connected to a ProtonVPN server in Japan.

[Screenshot Here: VPN IP Address]

![38](https://github.com/carlos-m-romero/Virtual_Private_Network_VPN_IP_Address_Observations/assets/148396073/4b420366-facd-491d-96dc-79cca8da9040)


## Understanding the Results

From this exercise, you can observe the following:

- When accessing the website from your actual PC without a VPN, it shows your original IP address and your city location.

- After connecting to the Azure virtual machine and accessing the website, a different IP address and the location of the virtual machine (e.g., Paris) are displayed.

- Finally, by connecting to the ProtonVPN server in Japan from within the virtual machine and accessing the website again, another IP address and the location of the VPN server (e.g., Tokyo, Japan) are shown.

This exercise demonstrates how VPNs work by encrypting and routing your internet traffic through remote servers, making it appear as if you are browsing from different locations. VPNs can enhance privacy, and security, and allow you to bypass geo-restrictions.
