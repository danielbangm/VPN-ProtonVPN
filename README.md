![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/5243893a-3691-4117-a385-a23f9910fce3)

<h2>VPN - Prerequisites and Installation</h2>

In this lab I will outline how VPN can securely link two computers(or networks) together across an insecure network such as the internet, allowing them to send encapsulated and encrypted data to each other.

<h2>Objectives</h2>

-  More Experience with Azure (I will Create the environment here)
-  Browse the internet without a VPN and with a VPN
-  Gain a better understanding of how VPN works.

<h2>Environments and Technologies Used</h2>

-  Microsoft Azure (Virtual Machines/Compute)
-  Remote Desktop Protocol
-  ProtonVPN

<h2>Operating Systems Used</h2>

-  Windows 10 pro

<h2>List of Prerequisites</h2>

-  All you need for this lab is the Azure Tenant and Subscription

<h2>Installation Steps</h2>

-  Step 1: Find the IP address of my Computer

To get my IP address I open a brwoser engine and go to www.whatismyipaddress.com and note that somewhere because I will compare different scenario in this lab to outline the benefit or importance of using a VPN. Mine are: IPv4 = 64.189.47.3
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/2d3ed712-99c0-4c40-a9f3-00ce8be17a46)

-  Step 2: Create a Virtual Machine (VM1) in Azure and access it via Remote Desktop Protocol

As usual I go to www.portal.azure.com and create a Virtual Machine VM1. For the sake of this lab I will choose an area different from my local area and in this case I chose Europe(UK south). I chose windows 10 pro as the OS for my VM1. My VM1 is created and automatically is assigned a virtual network and subnet.
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/bd65b04e-e7f6-460e-a0d6-a48ee8e4209d)

-  Step 3: Connect to VM1 via a Remote Desktop Protocol

Since I am on a windows machine I will use Remote Desktop Connection to connect to VM1 using its public IPv4 address(20.77.71.83). If you happen to be working on a Mac don't forget to download and install "Microsoft Remote Desktop". Just like that I am already connected to VM1
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/0ec1fabe-b5b6-40e7-8ed8-ee9205adc81e)

-  Step 4: Find the IP address of Virtual Machine VM1

To get VM1's IP address I open a brwoser engine and go to www.whatismyipaddress.com and note that somewhere because I will compare different scenario in this lab to outline the benefit or importance of using a VPN. IPv4 = 20.77.71.83 and the region is UK-London
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/50b6912e-ca4e-4dd8-a297-e22cef0ed3c8)

-  Step 5: Sign up for ProtonVPN and find my VM1 IP address again

I search for protonVPN and create a free account just for the sake of this lab. I prefer signing up for ProtonVPN from my personal computer, then getting the credetials before going to the Virtual Machine and connect to protonVPN as and end user with the same credential just to avoid messing up my location. I was able to create a free account and install it in my VM1
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/57160359-218d-472a-b0fc-fe7667cff459)

-  Step 6:  Connect the Virtual Machine VM1 to protonVPN and choose Japan as the Country

I do a quick connect inside protonVPN and chose Japan as the country and now I am protected on the internet and my traffic is from Japan
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/27940183-c2f3-4777-b163-59a4af703c96)

-  Step 7: Find the IP address of Virtual Machine VM1

Now that I am connected through protonVPN, I will go back into my browser and find my IP address at www.whatismyipaddress.com. Now my IP address is IPv4 = 37.19.205.154 and my location is Tokyo-Japan
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/17381a60-4cb0-4bbb-87b0-96e1c458578b)

<h2>Conclusion</h2>

Since my IPv4 address is different in each scenario I can conclude that VPN helps me appears on the internet with a different location and can help me protect my identity. This is a really cool lab that shows me how you can hide your address when browsing the internet. For example you can have access to some netflix content only reserved to Japan just by using a VPN. I tried to go to netflix.com from my Virtual Machine VM1 and here is the output:
![image](https://github.com/danielbangm/VPN-ProtonVPN/assets/22795502/519fd9be-04d9-4cdb-a150-99fdc6d83f64)

