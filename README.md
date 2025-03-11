# Vitual Private Network (VPN)
<p>
  
![vpnlogo](images/vpnlogo.png)
</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of using a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating IP Through VM (France)
- STEP 4 - Connecting to VPN Through VM
- STEP 5 - Locating IP Through VPN (Japan)

<h2>Installation Steps</h2>

STEP 1 - Locate your own personal IP address by going to "www.whatismyipaddress.com" which will be able to show you your local IP address. We will use this later as well. See EXAMPLE 1A below.

EXAMPLE 1A
<p>

![img](images/img1.png)
</p>
<p>

Next we will set up a virtual machine on Azure. 
  
</p>
<br />

STEP 2 - Go to www.portal.azure.com and find Virtual Machines. (Create a free account with $200 if you need to). See Example 2A looking at the Virtual Machine set up page. 

EXAMPLE 2A
<p>
  
![img](images/img2.0.png)
</p>
<p>

Creating the Virtual Machine on Example 2B the VM as “VM-FranceCentral” and select that for the REGION as well. Ensure the other items are selected as shown in EXAMPLE 2B & 2C.

EXAMPLE 2B
<p>

![img](images/img2.png)
</p>
<p>

For the Username and Password you can create your custom information, just record it personally.
  
</p>
<br />

EXAMPLE 2C
<p>

![img](images/img3.png)
</p>
<p>

Select the “Networking” tab towards the top of the page and view EXAMPLE 2D inputs to match. 
  
</p>
<br />

EXAMPLE 2D
<p>

![img](images/img4.png)
</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

NEXT: At the Virtual Machine we find that the IP to the Virtual Machine is “4.233.217.28”. See EXAMPLE 2E

EXAMPLE 2E

<p>
  
![img](images/img5.png)
</p>
<p>


STEP 3 – Log Into the VM and Find IP Address
<p>
Now that we have set up the Virtual Machine we will connecting to it using the application “Remote Desktop Connection” (EXAMPLE 3A) and input the IP address for the VM that we located in EXAMPLE 2E and then input the set credentials we set when creating the VM (see EXAMPLE 3B). Once logged in, we will open the web browser and again look up www.whatismyipaddress.com (EXAMPLE 3C).

  
</p>
<br />
EXAMPLE 3A
<p>

![img](images/img5.5.png)
</p>
<p>

  
</p>
<br />

EXAMPLE 3B
<p>

![img](images/img6.png)
</p>
<p>

When we look up the IP address for this VM through www.whatismyipaddress.com we see that this VM is showing the location for France (EXAMPLE 3C).
  
</p>
<br />

EXAMPLE 3C
<p>

![img](images/img7.png)
</p>
<p>

STEP 4 – CONNECTING TO VPN (Free Version)

Using the local computer go to protonvpn.com and create a free account (if you use the VM then French will display on your browser, so use local computer desktop). Once you are logged into your account, copy the URL from the Proton VPN website (EXAMPLE 4A) and then paste the URL to the VM web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>

![img](images/img8.png)
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. See EXAMPLE 4B when this steps are completed.  
  
</p>
<br />


EXAMPLE 4B
<p>

![img](images/img9.png)
</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in Japan. See EXAMPLE 4C
  
</p>
<br />

EXAMPLE 4C
<p>

![img](images/img10.png)
</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to Japan. The website www.whatismyipaddress.com shows yet another IP address using the VPN from Japan. This is quite amazing.
  
</p>
<br />

EXAMPLE 4D
<p>

![img](images/img11.png)
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 76.170.202.220
Virtual Machin IP (France): 4.233.217.28
Virtual Machin IP VPN (Japan) 194.114.136.212

  
</p>
<br />
If you no longer need the VM, ensure to remove it from the Asure account for unwanted charges.

END OF TUTORIAL
