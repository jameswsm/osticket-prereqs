<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
Tutorial for prerequisites and installation of the open-source help desk ticketing system osTicket.<br />
<br />
Part 1: Creating the virtual environment in Azure.<br />
Part 2: Installation of software dependencies and osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Active Subscription (Creation of Reasearch Group, VMs, Virtual Networks, Subnets)
- Enable Internet Information Services(IIS)
- Install Web platform installer?
- Item 4 Install MySQL set up username/pass
- Item 5 Install C++ redistributbal
- Item 6 Configure permissions / install osTicket






<h2>Installation Steps (Part 1) Steps: 1 - 12</h2>


![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/a00701b7-fa87-49f7-9808-097780c5c0e7)
<p>
Step 1: Navigate to "portal.azure.com/#home" to create a Resource Group. Search for Reasearh Groups. This group will house the Virtual Network and Subnet. 
</p>
<br />


![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/e924987f-8d09-4d24-be57-8eaf95e6456f)
<p>
Step 2: Click "Create" to create the Resource Group
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/88dae17e-6acc-4cda-84f5-26d115ff0d06)
<p>
Step 3: Name the resource group (ex: RGosTicket). Choose a region. Choose a region close to your primary user base to minimize latency. Also ensure that the region complies with local laws regarding data residency and privacy. Click Review + create.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/cb6d7724-bfed-41d2-910a-d8a0b3b97e29)
![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/01984bf3-2172-491c-9c26-5c1e969504ee)
<p>
Step 4: Search for Virtual Machines. Click Create. Select Azure virtual machine.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/2d704268-737a-468a-9f02-f2c7dc65e589)
<p>
Step 5: Select the Research Group we created (RGosTicket). Name the Virtual Machine (ex: vmOsTicket). Choose a Region (ex: (US) East US). Choose an image (ex: Windows 10 Pro, version 22H2 - x64 Gen2 (free services eligible)). 
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/8faa301e-1ca1-447f-966f-3d393adaa08c)
<p>
Step 6: Choose a size (ex: Standard_D4s_v3 - 4 vcpus, 16 GiB memory ($140.16/month)) note: limited subscriptions cannot use more than 4 vcpus. Choose a Username and Password (Username ex: jamesuser). Check the Licensing box, and click Next: 
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/c23a438e-7315-43ec-8017-9837fc8277db)
<p>
Step 7: Click Next again to navigate to Networking
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/a992ab4f-0500-42a1-b48d-c51701aa872c)
<p>
Step 8: Azure will create a new Virtual Network and Subnet automatically (ex: (new)vmOsTicket-vnet / ex: (new)default(10.0.0.0/24)). Click Review + Create
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/a3278296-1dc1-4253-8961-62604f8071f8)
<p>
Step 9: Once Validation is passed. Click Create.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/3155374b-544a-430a-b340-69a5dbb64009)
<p>
Step 10: When deployment is complete. Navigate to Virtual Machines. Click the Virtual Machine name (ex: vmOsTicket) to see VM information.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/5ba30669-0b74-4065-aadb-5e7231e63408)
<p>
Step 11: Copy the Public IP address(ex: 52.168.84.82). Open Remote Desktop Connection. Paste the Public IP address into bar. Click Connect.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/daa843e1-4251-4635-8924-ffd54c87b95d)
<p>
Step 12: Enter Username/Password we created in Step 6 (Username ex: jamesuser). Click Ok.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/c2d8fc54-2f24-44a2-9a91-653abb9bf360)
<p>
Screen should look similar to this.
</p>
<br />
<br />

<h2>Installation Steps (Part 2) Steps:  13 - somethingsomethingsomethingsomething</h2>


![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/2712a469-9053-4107-becd-4a8bf735d894)
![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/2ae77e51-192e-4378-b48b-68c2e413d227)
<p>
Step 13: Right click the start menu and select "Run". Type 'control' and hit enter to open the Control Panel.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/0f5ff643-63fa-464f-892f-5e0893dac3e3)
<p>
Step 14: Click "Programs"
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/5222a443-46e5-456e-a71a-a4c4319c3543)
<p>
Step 15: Click "Turn Windows features on or off"
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/c62f3b83-c862-45bc-b8df-2d37e9028d3c)
<p>
Step 16: Check the box for "Internet Information Services"
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/faa69f3b-afac-4720-8335-698abce825ef)
<p>
Step 17: Expand "Internet Information Services". Expand "World Wide Web Services". Expand "Application Development Features". Check the box for "CGI"
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/4976952a-085a-4359-ba6e-e844c528317c)
<p>
Step 18: Collapse "Application Development Features". Expand "Common HTTP Features". Select all boxes and hit ok.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/9c235930-66ba-4025-be8d-aaa63cfede7f)
<p>
Step 19: Ensure IIS enabling was successful by opening a browser. Enter 127.0.0.1 in the bar. Result should look like this. If unsucessful, see step 19.5, else go on to step 20.
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/187bcb23-4d34-4ed6-a94d-5000976107be)
![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/a08be245-8dc8-4e41-9228-96c7eae36ccb)
![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/9292168e-9100-4aac-ad35-83ba39e65b2a)
<p>
Step 19.5: If unsuccessful. Navigate back to "Programs". Click "Uninstall a program". Click "Turn Windows Features on or off". Uncheck Internet Information Services. Click Ok. Restart process from Step 13. 
</p>
<br />

![image](https://github.com/jameswsm/osticket-prereqs/assets/170709350/a00701b7-fa87-49f7-9808-097780c5c0e7)
<p>
Step 20: Download PHP manager https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link
</p>
<br />
