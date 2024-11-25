<p align="center">
<img src="https://i.imgur.com/q2olSIK.png">
  </p>

<h1>Remote Desktop and Azure - How To</h1>
This guide will demonstrate how to connect to an Azure virtual machine with remote desktop.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection (RDP)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Prerequisites</h2>

- Azure Account
- Virtual Machine (Azure)

<h2>Setup Walkthrough</h2>

<p>
<img src="https://i.imgur.com/TnY6AyL.png" height="80%" width="80%" alt="Azure Account Creation"/>
</p>
<p>
The first thing you need to do is head to https://azure.microsoft.com, and sign up for a free account. Make sure to get your free 200$ of credit usable on the site.
</p>
<br />


<p>
<img src="https://i.imgur.com/hKmoYl5.png" height="80%" width="80%" alt="Resource Group Creation"/>
</p>
<p>
After you're signed into the portal, you need to create a Resource Group for the Virtual Machine to sit in. Click on Resource Groups, then create, and name it anything you like. 
</p>
<br />

<p>
<img src="https://i.imgur.com/1u6JXIB.png" height="80%" width="80%" alt="Virtual Machine Creation"/>
</p>
<p>
Now you will make a Virtual Machine, go back to the home portal and click on Virtual Machines, then create and select "Azure virtual machine".
  Set the resource group to the one you just created, select an appropriate name for the virtual machine, and pick a region where you want it to reside.
</p>
<br />

<p>
<img src="https://i.imgur.com/pBtM714.png" height="80%" width="80%" alt="Virtual Machine Config"/>
</p>
<p>
Scroll down and set the image to Windows 10. For the size I recommend anything with 2 vcpus so it's not too slow, whatever is cheapest as long as it has 2 vcpus. (Don't worry about the price, what is listed is only if you are running the machine 24/7)
</p>
<br />

<p>
<img src="https://i.imgur.com/dJlI7W6.png" height="80%" width="80%" alt="Don't miss the license!"/>
</p>
<p>
Continue down the page to make your username and password, and DON'T FORGET to select the easily missable licensing section where you need to confirm you have a Windows 10 license at the bottom.
</p>
<br />

<p>
<img src="https://i.imgur.com/yHcnBxc.png" height="80%" width="80%" alt="Create and validate"/>
</p>
<p>
Click review + create and wait for it to validate, create the machine and wait for it to deploy.
</p>
<br />

<p>
<img src="https://i.imgur.com/DSLTsiU.png" height="80%" width="80%" alt="Public IP for RDP"/>
</p>
<p>
Once deployed and running, it's time to connect using Remote Desktop. Navigate to the virtual machine and find its public IP address, copy it and open Remote desktop by searching "rdp" or "remote" in windows search and open up remote desktop connection.
</p>
<br />

<p>
<img src="https://i.imgur.com/O6IsXth.png" height="80%" width="80%" alt="Logging into RDP"/>
</p>
<p>
Paste the IP address you just copied and click connect, sign in using the account username and password you chose earlier and you should finally be logged into the virtual machine.

</p>
<br />

<p>
<img src="https://i.imgur.com/h5Bziq9.png" height="80%" width="80%" alt="Smile"/>
</p>
<p>
And you're done! This can now be used for whatever needs you require, but keep in mind the virtual machine will stay running (costs money) until you stop or delete it.
To "pause" the virtual machine to save money and continue to use it in the future, simply head to the Azure portal, select the virtual machine and select stop. Whenever you need to use it again all you need to do is start it.
  
  
  Thank you for reading, I hope this helped. :)
</p>
<br />
