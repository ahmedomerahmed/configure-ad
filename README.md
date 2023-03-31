<p align="center">
<img src="https://i.imgur.com/WQLWxYw.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>How to create virtual machice through Azure </h1>
This tutorial outlines the step by step to create Virtual Machines.<br />




<h2>Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)


<h2>Configuration Steps</h2>
Step 1 : Go to https://portal.azure.com/


Step 2 : Set up $200 free credit account

Step 3: Create a new resourse Group within the Azure portal

<p>
<img src="https://i.imgur.com/VzZPMxG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Use the search bar in the Azure Portal to find "Resource Groups", and then create a new Resource Group. Choose the region that is geographically closest to your location during setup. Review the settings, and once you're done, click "Create". On the next page, click "Create" again to complete the Resource Group setup.
</p>
<br />
Step 4: Create a Storage Account within the Resource Group created in Step 3
<p>
<img src="https://i.imgur.com/I250ucY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set up a Storage Account that will contain your Virtual Machine. Make sure that the Storage Account is in the same region as the Resource Group you created earlier..
</p>
<br />
Step 5: Set up a Windows 10 Virtual Machine (VM)
<p>
<img src="https://i.imgur.com/gfW5OIK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Provide a name for your Virtual Machine, and make sure to choose the same region used for your Resource Group. Select an operating system by clicking on "Image", and then choose the desired CPU specifications by selecting the appropriate size. Create a username and password for the administrator account. Check the box for licensing, and then click "Review + Create". Finally, click "Create" to complete the setup process.
</p>
<br />
Step 6: Go to the Azure portal's search bar and search for "Virtual Machines"
<p>
<img src="https://i.imgur.com/veSzNW2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Find your VM's overview page and locate its public IP address.Then, copy the IP address.
Step 7: Set up a Remote desktop
<p>
<img src="https://i.imgur.com/GWRi7KC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If you are using a Mac, go to the app store and download the Microsoft Remote Desktop app. Once downloaded, open the app and click on the "Add PC" button. Paste the public IP address of your VM into the "PC Name" field. Enter the username and password that you previously created for your VM. Click continue to complete the setup. If you are using a Windows, click on the Start menu and search for "Remote Desktop". Once you see the Remote Desktop app, open it and paste or type in the public IP address of your VM. Enter the username and password that you previously created for your VM. Click on "Connect" to proceed with the remote desktop connection.

Step 8: Delete the resourse Group after you complete virtual machice.
<p>
<img src="https://i.imgur.com/cFu8kPG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Return to the Azure portal website and navigate to your resource group. From there, you can delete the resource group and the NetworkWatcherRG folders that were created along with your VM. Copy and paste the Resourse group name (RG1) under "TYPE THE RESOURCE GROUP NAME" as well as same for NetworkWatcherRG.  Once you've deleted these resources, you're finished and your VM will no longer be available.

</p>
<br />
