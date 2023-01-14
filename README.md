<h1>Capturing Image of a Virtual Machine in Azure Portal </h1>

<h2>Description</h2>

In this lab, I am capturing an image of a virtual machine on azure. I also created two folders into a folder named Test Folder on the VM's desktop to see if the folder will get restored when I try to restore the VM from the captured image. 

After the VM restores from the captured image. I will use Microsoft Remote Desktop to see if the VM runs without issues and ensure those folders are still there.
<br />

<h2>Utilities Used</h2>

- <b>Azure</b> 
- <b>Microsoft Remote Desktop</b>

<h2>Prerequisite </h2>

- <b>Virtual Machine Deployed on Azure Portal:</b> I am capturing the image of the VM I created in the past. During the capturing process, I had the option where VM deletes automatically once the image is captured. But I declined it and decided to delete the VM manually after the process was done.   

<h2>Program walk-through:</h2>

<p align="center">
Login in to Azure Portal. Go to All services-> Compute-> Virtual Machine. <br/>
Select the Virtual Machine that you want to capture. Go to Overview-> Capture <br/>
<img src="https://i.imgur.com/mGPNcRh.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Create an image: Instance details <br/>
I have named the image a: vm-captured-image. Once done click Review + create in bottom left
<img src="https://i.imgur.com/6qYRwCc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Create an image: Review + Create <br/>
Click Create <br/>
<img src="https://i.imgur.com/Hcc6aeb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
VM captured image successfully created <br/>
<img src="https://i.imgur.com/a0YlCWk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
VM captured image can accessed by going to All Services-> Other-> Images <br/>
<img src="https://i.imgur.com/kjjp2sR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
I am deleting my Virtual Machine and then i'll try to restore it from the captured image <br/>
<img src="https://i.imgur.com/UuxRsxN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
I will now restore my VM by going to All Services-> Other-> Images. Select the image and click Create VM <br/>
<img src="https://i.imgur.com/XkRIUHH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Create a Virtual Machine <br/>
I have named it vm-from-captured-image <br/>
<img src="https://i.imgur.com/OdBe3UD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Create a Virtual Machine: Administrator account & Inbound port rules <br/>
I have enabled RDP port for a remote access. Once Done click Review + create in bottom left <br/>
<img src="https://i.imgur.com/KwxTgz7.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Virtual Machine successfully restored from captured image. <br/>
I'll now access the VM remotely from my computer to see everything works fine. <br/>
<img src="https://i.imgur.com/GmMnUxH.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
VM is up and running & Test folders also restored <br/>
<img src="https://i.imgur.com/dOC12WA.png" alt="Disk Sanitization Steps"/>
<br />
<br />




<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
