<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project is a prerequisite for later projects showing how to set up osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a Resource Group in Azure
- Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs
- A new Virtual Network (Vnet)
- Install PHP Manager for IIs
- Install rewrite module
- create the directory c:\PHP
- install PHP 7.3.8
- install VC redist
- Install MySQL
- Install osTicket

 <h2> Installation files  
https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
<h2>Installation Steps</h2>
<p>
<img src="https://i.imgur.com/FDg5PGO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/9hVn1mU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/3Dkbu44.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First You want to make a resource group you can call Os-Ticket or whatever you want just remember what region you put it in. 

 Now you want to make a virtual machine, when you make the virtual machine make sure you put it in the resource group you just made and put it in the same region.

 After that use a Windows 10 image and for the size you can choose any size that has 4 CPUs.

 Then make a password and username and write it down for later. Then just click the box at the bottom of the page and click Review and Create.

 Now go to Your Virtual Machine and get the. IP address and copy and paste it on a remote Desktop if you have an Apple computer you'll need to download it from the Apple store.
 *use the pictures above to see what it should look like.
</p>
<br />

<p>
<img src="https://i.imgur.com/5c1aBjo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/EuaEyPA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now you want to install and enable IIS with CGI.

To do that you can go to the start menu search bar and search the control panel then select program, after that under programs and features select turn Windows features on or off then a page should pop up that looks like the pictures above.

Now just look through the list to find Internet information services, check its box and expand its list and find worldwide Web services and expand it to find application and development features, expand that to find CGI you can use the picture for help.   
  
Lastly, go under world wide web services and expand common HTTP Features and make sure all the boxes are checked and click ok and it should start installing IIS.
</p>
<br />

<p>
<img src="https://i.imgur.com/nMwWnuO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/3hyj8YO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/SeSKBKJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ofLJX2s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/PbzCO5y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/mZDDVjj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we are going to install PHP manager, rewrite module, and PHP 738 also we are going to create a directory C:\PHP and unzip PHP 738 contents in C:\PHP.

 First, copy the installation files link and open up internet explore on your virtual machine and download PHP Manager and install it, you can next through the setup.

 Then go back to the installation files and download and install the Rewrite module.

 Now we need to create PHP on the C drive in file explorer, go to the C drive and right click and press new folder and call it PHP.

 After that, go back to the Installation files and download PHP 738. This is an old version of PHP, so your computer might have trouble downloading it. But a yellow triangle will show up on the top right corner, just click on that downloads should pop up. Just click the three little dots and click keep and then keep anyways and it should download.
 *use the pictures for help

 Now in file Explore, go back to download a right click PHP 738, and select extract all and for the destination, you can type C:\PHP and press Extract.
 
</p>
<br />

<p>
  <img src="https://i.imgur.com/dK93fZ0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/SUALKL4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/pwQsDsP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now we are downloading and installing C++ and MYSQL

   First, go back to the install files and download and install Vc. 

Next, download MYSQL, and in the installation setup, do a typical install and install it then it's going to ask about the configuration, then make sure to install it as Windows service box is checked, then select next.

Now it should ask you to make a password you need to remember this so write it down if you need to then press next and execute then finish.
  </p>
  <br />
  
  <p>
  <img src="https://i.imgur.com/JnokTDH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/taU8mJF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/XQ3zV7x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/iy72Grx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/Q8IUK4h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now we are going to register PHP from within IIS

   First, click on start Type IIS and run as an administrator then double click PHP manager icon and click on register new PHP version and brows in the PHP folder you just made and click PHP-CGI.
   *Use the picture above for help

   Lastly, click VM-ticket on the left then restart on the right under the manager server.
  </p>
  <br />
  
  <p>
  <img src="https://i.imgur.com/Opx81nh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/C8WRnP9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/EuKXsI1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/iqpRDhi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/SJuAKMh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/b0T2BoV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/QHYGT6D.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/afFaVbd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/7G7gE0q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/knGt4z6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now we are going to install osTicket

  First download osTicket from the installation files

  Now we are going to extract and copy the upload folder from the osTicket download to C:\inetpud\wwwroot

  So open two file explorer pages and on one of them double click the osTicket download and there should be an upload folder inside.

  Now in the second one go to the C drive and click inetpud then click wwwroot.

  Then click the upload folder and drag it to wwwroot you can use the pictures for help.

  Once it's finished copying rename the upload file in wwwroot folder to osTicket.
  </P>
  <br />
  
  <p>
  <img src="https://i.imgur.com/TdTwoWr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/YnMSMWK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/5SGGBv9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/GJiOTjr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/2lP0OO3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/Zjnr118.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/rd0pwIR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now were are going to start setting up osTicket in the browser, first refresh IIS.

  Now click on sites then default website and osTicket on the left and on the right click browse 80. OsTicket should pop up on a browser with a couple of extensions disabled.

   So go back to IIS and click php manager and at the bottom click enable or disable an extension and enable PHP.Imap.dll, Intl.dll, and opcache.dll then refresh and they should become green on the osTicket site.
  </p>
  <br />
  
  <p>
    <img src="https://i.imgur.com/VzbxiPW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/5jR24Za.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/BEquvHX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/5YjgljM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/IxTwWOm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/0Ts5vUQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/yCl6J1H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/jKcDHcW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/dHy0VqS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/qfrUEn8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/4woyHyt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/RF5avU3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/9CT7bSJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Now we are going to rename ost-sample-config.php to ost-config.php.

   So open file explore go to the c: drive click inetpud then click wwwroot then osTicket then find include and click on it then in include scroll down until you find ost-config and right-click on rename it ost-config.

   Now we are going to change the Permissions so everyone has access to the file.

   So now right-click the file and go to properties, in properties go to security then go down to advanced in the advanced security settings disable inheritance. Then click Remove all inherited Permissions then you need to add permissions so press add then click Select a principal then type everyone and press ok, then check the full control box, press ok then click apply and ok.
  </p>
  <br />
  
  <p>
  <img src="https://i.imgur.com/qb6fGZd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/zLEaa00.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/31HOXsV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ub27uH6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/jgOZ2aR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/kVdid0h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ArByOqi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/Z0Y9L8s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now we are going to continue setting up osTicket in the browser.

  Press continue and just fill out the osTicket Basic installation page and write them down because you'll need them later, especially your username and password. Once you get to database settings stop because you need to download Heidi SQL.

  So go to your installation files to download Heidi SQL once it downloads go to your downloads folder and double-click it accept everything and install it and press finish.

  It should open up on the bottom left press new for the username make sure it's root and the password is the one you made for MY SQL and press open, name it osTicket then press ok.

  Now go back to Database settings and finish setting up osTicket and press install now.
  </P> 
  <br />
  
  <p>
   <img src="https://i.imgur.com/MAGQQdW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/bAvHtZT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/MZOWvAS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/txAO2w0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/5FCjv03.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/fdKGFkx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/FFqYgTe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/gVtKMS9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/dSPer9f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    </p>
    <p>
  Now we need to do a little cleanup.
   First, you need to delete the setup folder. So go to file explore and in the bar type C:\inetpud\wwwroot\osticket and scroll down to setup right click it and click delete.

   Now I want you to scroll up to include and click into the PHP folder and go to the ost-config so we can change it back to read-only. So right-click it and go to Properties then the security tab then go to Advance. Then click everyone and then click edit write then click ok apply and ok again.
  </p>
  <br />
  
  <p>
      <img src="https://i.imgur.com/JbrDW05.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/hCW1SeK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  <p>
  Now copy the URL into your virtual machine and log into osTicket with the username and password you made and you're done.
  http://localhost/osTicket/scp/login.php
  </p>
  <br />
