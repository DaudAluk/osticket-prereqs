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


<h3><strong> Install VC Redistributable </strong></h3>

<img src="https://github.com/user-attachments/assets/18f6c7a8-47e5-4c0a-962d-ad4145cba62a"/>
<img src="https://github.com/user-attachments/assets/55ed6ae3-e36b-4a42-ac28-9503afc43e3f"/>

* Open the "osTicket-Installation-Files" folder
* Locate "VC_redist.x86" and open
* Follow installation guidelines 


<h3><strong> Install My SQL </strong></h3>

<img src="https://github.com/user-attachments/assets/55db00d6-1dd6-4c53-87fa-e4314f50c709"/>
<img src="https://github.com/user-attachments/assets/691bf54a-8278-47b5-a70c-dc704a53a748"/>
<img src="https://github.com/user-attachments/assets/6ef2b65a-47da-4bf3-aa86-60d38a6421c2"/>
<img src="https://github.com/user-attachments/assets/06d3889b-720e-45af-8e3a-e17bf630af52"/>
<img src="https://github.com/user-attachments/assets/0c114972-8e7a-4147-ac4c-72c2e3bf52e5"/>
<img src="https://github.com/user-attachments/assets/8503fa57-84a9-4272-8994-78d9d8598576"/>
<img src="https://github.com/user-attachments/assets/da5dcb1f-7ab3-4a4f-9a3a-36e46c87e46a"/>
<img src="https://github.com/user-attachments/assets/b341243e-c0aa-4546-88ee-94abda98f96e"/>

* Open the "osTicket-Installation-Files" folder
* Locate "mysql-5.5.62-win32" and open
* Follow installation guidelines
* Once installed, check the "Launch the MySQL Instance Configuration Wizard"
* Click "Finish"
* Follow the Configuration Wizard guidelines (Selecting "Standard Configuration" > "Install as a Windows Service" > Create your own password)
* Execute


<h3><strong> Open IIS as Admin & Register PHP </strong></h3>

![image](https://github.com/user-attachments/assets/66f81e23-fe9e-40ad-bb50-d8cf1d969ded)
![image](https://github.com/user-attachments/assets/343f63c2-4a29-47d5-bdd9-048813ccf48c)
![image](https://github.com/user-attachments/assets/67f9032a-59df-497b-9988-9e8d2e8dbd6d)
![image](https://github.com/user-attachments/assets/835979e5-9c68-4db0-aedd-c6621667af80)

* Open Start and Type "IIS"
* Once "IIS" is located, run as Administrator
* In "IIS", locate "PHP Manager" and open
* Under "PHP Set Up" locate "Register new PHP version" and open
* Locate the "C:\PHP" path and select "php-cgi"


<h3><strong> Reload IIS </strong></h3>

![image](https://github.com/user-attachments/assets/b1591215-637b-43c1-8e1f-9ff234e9cea4)
![image](https://github.com/user-attachments/assets/d849e9e0-7809-46a3-9dfc-71efe81d6618)
![image](https://github.com/user-attachments/assets/c464bd26-6844-42be-b9eb-fff16a58bd1f)

* Under "Connections", locate "osticket-vm" and open
* Under "Actions", locate "Manager Server"
* First, click "Stop"
* Once stopped, click "Start"


<h3><strong> Install osTicket </strong></h3>

![image](https://github.com/user-attachments/assets/6ab66d99-064e-4221-a346-ff352f10b319)
![image](https://github.com/user-attachments/assets/ba0c1e81-dd38-49c7-8eee-8f9d40175357)
![image](https://github.com/user-attachments/assets/5b6dd2de-5432-4656-952c-c377c351eb7c)
![image](https://github.com/user-attachments/assets/456acb89-aa59-4859-9ac3-c242285081f7)
![image](https://github.com/user-attachments/assets/013cf82e-cd01-43d8-bca4-75a81dc3f30b)
![image](https://github.com/user-attachments/assets/2fa9f4e7-6eeb-480c-961a-2c9a8dde5035)
![image](https://github.com/user-attachments/assets/6f01a628-b174-4f22-a285-29a5e5a041c4)

* Open the "osTicket-Installation-Files" folder
* Locate "osTicket-v1.15.8" zip folder, extract files
* Open the extracted "osTicket-v1.15.8" folder and leave the window open
* Open "C:\" in a new window
* Locate "inetpub" folder and open
* Locate "wwwroot" folder and open
* Locate "upload" folder and copy 
* Open the "osTicket-v1.15.8" window
* Paste the "upload" folder in "osTicket-v1.15.8" folder
* Rename "upload" folder and change to "osTicket"

<h3><strong> Reload IIS again </strong></h3>

![image](https://github.com/user-attachments/assets/66f81e23-fe9e-40ad-bb50-d8cf1d969ded)
![image](https://github.com/user-attachments/assets/d849e9e0-7809-46a3-9dfc-71efe81d6618)
![image](https://github.com/user-attachments/assets/c464bd26-6844-42be-b9eb-fff16a58bd1f)

* Open Start and Type "IIS"
* Once "IIS" is located, run as Administrator
* Under "Connections", locate "osticket-vm" and open
* Under "Actions", locate "Manager Server"
* First, click "Stop"
* Once stopped, click "Start"

<h3><strong> Observe osTicket Extensions </strong></h3>

![image](https://github.com/user-attachments/assets/0d8e163c-d075-4c5f-8ba7-e15b8b8a5639)
![image](https://github.com/user-attachments/assets/fbcfefd4-ad8a-4543-a9eb-8ba6e66c2422)

* Under "Connections", locate "osticket-vm" and expand
* Locate "Sites" and expand
* Locate "Default Web Site" and expand
* Locate "osTicket" and open
* Under "Actions", locate "Manager Folder", locate “Browse *:80 (http)" and open
* Once "http://localhost/osTicket/setup/" webpage opens, observe the extensions

<h3><strong> Enable osTicket Extensions </strong></h3>

![image](https://github.com/user-attachments/assets/536be792-a849-4f08-a602-a60469becb92)
![image](https://github.com/user-attachments/assets/1fcca1b0-c244-4edc-9cc7-28220c6ce78e)
![image](https://github.com/user-attachments/assets/7d7489cb-2fb6-4538-85b6-77cce4c92b55)
![image](https://github.com/user-attachments/assets/4efc3b78-d29b-4cd5-b30f-316a5ed4f26e)
![image](https://github.com/user-attachments/assets/44339924-ed5c-4be4-be50-08368fd73c4e)

* Open IIS and locate "Connections"
* Under "Connections", locate "osticket-vm" and expand
* Locate "Sites" and expand
* Locate "Default Web Site" and expand
* Locate "osTicket" and open
* Locate "PHP Manager" and open
* Locate "PHP Extensions" and click "Enable or disable an extension"
* On the list of PHP Extensions search for the following extensions: "php_imap.dll" "php_intl.dll" "php_opcache.dll" and enable them all
* Go back to "http://localhost/osTicket/setup/" webpage, refresh the page
* Observe the changes


<h3><strong> Rename ost-sampleconfig.ph </strong></h3>

![image](https://github.com/user-attachments/assets/5b6dd2de-5432-4656-952c-c377c351eb7c)
![image](https://github.com/user-attachments/assets/456acb89-aa59-4859-9ac3-c242285081f7)
![image](https://github.com/user-attachments/assets/013cf82e-cd01-43d8-bca4-75a81dc3f30b)
![image](https://github.com/user-attachments/assets/4e5be19a-d140-43fa-bf50-83a50adc3b52)
![image](https://github.com/user-attachments/assets/37e3e86f-8ad8-4334-bc01-b33724603a0a)
![image](https://github.com/user-attachments/assets/ed3cbef5-2f1f-4672-be7b-f617e1828956)
![image](https://github.com/user-attachments/assets/05c4e3e3-71b0-4de9-97a6-03dda7820d20)

* Open "C:\" in a new window
* Locate "inetpub" folder and open
* Locate "wwwroot" folder and open
* Locate "osTicket" folder and open
* Locate "include" folder and open
* Locate "ost-sampleconfig.ph" file
* Rename "ost-sampleconfig.ph" and change to "ost-config.php"

<h3><strong> Assign Permissions </strong></h3>

![image](https://github.com/user-attachments/assets/270fbd57-b7d6-4466-8d31-547b352036fe)
![image](https://github.com/user-attachments/assets/e50c9f17-13d9-424f-8278-4ccd50d09df3)
![image](https://github.com/user-attachments/assets/cf627fd3-dc7c-4e01-bd26-399994dbcbb9)
![image](https://github.com/user-attachments/assets/370bb3f0-75d2-475b-b178-cbf8208cb435)
![image](https://github.com/user-attachments/assets/8d2e33d6-4c1b-4207-b393-26cd67c6cb21)
![image](https://github.com/user-attachments/assets/382b17f7-b2ff-45b8-89ca-8f888a6b6b80)
![image](https://github.com/user-attachments/assets/ba1c7817-de8b-4bd4-a8c7-6930453270a0)
![image](https://github.com/user-attachments/assets/db181f35-34cd-4a7b-8999-d06d548b36b1)
![image](https://github.com/user-attachments/assets/28b5720a-fe74-44c7-9dbd-ff92204c811b)
![image](https://github.com/user-attachments/assets/35cd48bf-33aa-4510-b600-f3ed8fd23c5c)
![image](https://github.com/user-attachments/assets/b27e312f-eb73-498f-96d5-3db0ae690de2)

* Right click new "ost-config.php" file
* Click "Properties"
* Locate "Security" tab and open
* Locate "Disable inheritance" and click
* Click "Remove all inherited permissions from this object"
* Under "Permissions" tab, locate "Add" and open
* Locate "Select a principal" and open
* Type "everyone" and click "Check Names"
* Click "OK"
* Check "Full control" box
* Click "OK"
* Click "Apply"
* Click "OK"
* Click "OK"

  <h3><strong> Continue osTicket set up </strong></h3>

![image](https://github.com/user-attachments/assets/22efba72-3932-4609-a1e4-104ab31f85e7)
![image](https://github.com/user-attachments/assets/426dd10a-f807-40a5-b53c-cdbf5fab1dc6)
![image](https://github.com/user-attachments/assets/7f0ca11a-0c59-45cb-ac3a-63035389adf9)
![image](https://github.com/user-attachments/assets/81e3187a-ae26-4f46-b611-1a3620609d40)
![image](https://github.com/user-attachments/assets/cd3bca99-1455-46bb-b270-11e2bdc3d353)
![image](https://github.com/user-attachments/assets/270b0ef4-f4e1-4202-95bf-713e12783088)
![image](https://github.com/user-attachments/assets/1636dd11-0ea2-447c-90d4-a9aced5689a1)
![image](https://github.com/user-attachments/assets/dc575390-2ca7-4d36-afe4-fb5950e7935c)
![image](https://github.com/user-attachments/assets/2be8d592-a0f2-458a-90ba-e162693b0284)
![image](https://github.com/user-attachments/assets/04e259a9-7033-470f-a53e-425c377b1ab1)
![image](https://github.com/user-attachments/assets/41c07881-ab5a-4672-8fb1-8badf1bffa13)
![image](https://github.com/user-attachments/assets/06b53b7c-0856-45bc-9a11-f4a01b4467ca)
![image](https://github.com/user-attachments/assets/b4557122-eb77-45c8-9783-8828bba4ba0f)
![image](https://github.com/user-attachments/assets/965479fe-3789-44c7-a75c-09a294544c6e)
![image](https://github.com/user-attachments/assets/318aa994-c19b-4299-8598-1b9c0b987102)
![image](https://github.com/user-attachments/assets/cac81d46-e733-465b-90ea-54da1e766008)
![image](https://github.com/user-attachments/assets/24404ded-2451-4ced-8715-ecc35d7cd069)
![image](https://github.com/user-attachments/assets/40fbcf78-058a-4826-9d59-44baabe807ca)
![image](https://github.com/user-attachments/assets/bf136c12-ccaf-4b84-ba69-a24842399c88)

* Open the "osTicket" installer website in browser [localhost/osTicket/setup/install.php]
* Click "Continue"
* Fill both "System Settings" & "Admin User" sections of form with necessary details, ensuring the use of 2 different email addresses
* Leave the window open
* Open the "osTicket-Installation-Files" folder
* Locate "HeidiSQL_12.3.0.6589_Setup" and open
* Follow installation guidelines
* Once installed, launch program
* Once Heidi SQL has opened, locate "New" button and open
* Input password created and click "Open"
* Locate "Unnamed" and right click
* Locate "Create new" and follow flow to locate "Database"
* Click "Database"
















































