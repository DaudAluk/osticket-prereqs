<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Creation of Resource Group and Virtual Machine using Azure
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<h3><strong> Create a Virtual Machine </strong></h3>
<img src="https://github.com/user-attachments/assets/df3235e7-a9f2-4e96-a626-51b4e476d843"/>

</p>
<p>
  
* Create a Resource Group, ensuring all corresponding resources are stored in one group
* Now start to create a [Windows 10, 4 vCPUs] Virtual Machine (VM) under the same Resource Group
* Set a desired VM Name, Username & Password
* Create VM

</p>
<br />

<h3><strong> Log into VM with Remote Desktop </strong></h3>
<img src="https://github.com/user-attachments/assets/b12420b6-5c32-4a78-9a3f-0cd7469eab6a"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/4c1d0045-f435-4d8f-9a89-16b781584125"/>

* Once VM has been deployed and created, copy the Public IP Address
* Open Remote Desktop
* Use the copied IP Address and VM login credentials created to log in
</p>
<br />

<h3><strong> Install osTicket on VM </strong></h3>
<img src="https://github.com/user-attachments/assets/9abd9d4f-f7e8-4656-a3c7-b03f9433c645"/>
<img src="https://github.com/user-attachments/assets/6a52b3da-84d3-4295-b623-0396de8b2876"/>

</p>
<p>
  
* When logged in to the VM, open the Internet Browser
* Open this link (https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)
* Download the osTicket Installation zip folder
* Extract the zip folder to reveal "osTicket-Installation-Files"
</p>
<br />

<h3><strong> Install / Enable IIS in Windows with CGI </strong></h3>
<img src="https://github.com/user-attachments/assets/c47b45f2-3009-4341-bbc7-2feb3009301a"/>

* Open Control Panel
* Programs > Programs and Features
* Click "Turn on Windows features on or off"
* On the list look for "Internet Informatiom Services" and check the box
* Once checked, expand "Internet Informatiom Services"

<img src="https://github.com/user-attachments/assets/03d2f03e-d697-47af-a992-f29e91356baa"/>

* Locate "World Wide Web Services" and expand
* Locate "Application Development Features" and expand
* Locate "CGI" and check the box
* Once checked, click "OK"
* Wait for the installation to finish 

<img src="https://github.com/user-attachments/assets/85e1eb40-a734-4c7f-a036-6556fa603ca5"/>
<img src="https://github.com/user-attachments/assets/05e8fdc5-a4ff-4dce-966a-397398a7aa98"/>

<h3><strong> Install PHP Manager for IIS </strong></h3>

<img src="https://github.com/user-attachments/assets/e943469e-61ae-4e13-9c61-b43d2742fce7"/>
<img src="https://github.com/user-attachments/assets/de97fb14-7fd5-4d00-80d4-8ac3c836aff1"/>

* Open the "osTicket-Installation-Files" folder
* Locate "PHPManagerForIIS_V1.5.0" and open
* Follow the installation guidelines 

<h3><strong> Install Rewrite Module </strong></h3>
<img src="https://github.com/user-attachments/assets/93aa3458-034f-4e6a-9fc2-389d1447ab72"/>
<img src="https://github.com/user-attachments/assets/b8ffa187-baba-44cf-b482-90c7b02521d3"/>

* Open the "osTicket-Installation-Files" folder 
* Locate "rewrite_amd64_en-US" and open 
* Follow the installation guidelines

<h3><strong> Create directory for PHP on C Drive </strong></h3>
<img src="https://github.com/user-attachments/assets/bf1a6eb1-1631-4072-b306-eaf74b6f4c9c"/>

* Open File Explorer
* Locate the C Drive "C:\" 
* Create a new folder and name it "PHP"


<h3><strong> Unzip PHP 7.3.8 into the PHP folder </strong></h3>

<img src="https://github.com/user-attachments/assets/a0375148-dc69-433b-9edb-294127bb0961"/>
<img src="https://github.com/user-attachments/assets/50e87d22-2b2d-4b11-b6d3-05e53fea2b37"/>
<img src="https://github.com/user-attachments/assets/3009019b-b084-4139-8a35-9dec9f9ccfdc"/>

* Open the "osTicket-Installation-Files" folder
* Locate "php-7.3.8-nts-Win32-VC15-x86"
* Extract all the contents into the "C:\PHP" folder 









