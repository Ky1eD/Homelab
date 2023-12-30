# Homelab
Winows Server 2016 Home Lab
 
<h2>Description</h2>
Project consists of making my Home lab.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Windows Server 2016 </b> 
- <b>Virtual box </b>
- <b>Active Directory </b>

<h2>Environments Used </h2>

- <b>Windows Server 2016</b>

<h2>Walk-through:</h2>

<p align="center">
Firstly I downloaded the OSI File for Windows Server 2016. To get a copy of Windows Server you have to fill out some information that Microsoft requires: <br/>
<img src="https://i.imgur.com/XikGkT9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then I created a VM in VirtualBox which you can see my guide here:
 - (https://github.com/Ky1eD/Virtual-Box-VM-Guide) <br/>
<img src="https://i.imgur.com/BxY6j2T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now once you bootup to the VM and it loads the OS download. You can select the language, time, and keyboard you want:  <br/>
<img src="https://i.imgur.com/Z06dEPN.png)" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Next you need to click "Intall Now" then this page will appear after. After I chose the version of Windows Server 2016 I wanted(Standard Evaluation Desktop experience): <br/>
<img src="https://i.imgur.com/YtbBelG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then accept license terms and click next:  <br/>
<img src="https://i.imgur.com/5oVZNHG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now select custom install since this machine had no OS to begin with to upgrade:  <br/>
<img src="https://i.imgur.com/If7vFKM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then select the drive you made in vitrualbox:  <br/>
<img src="https://i.imgur.com/DWpRvEG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
It will now finally start installing and will restart after:  <br/>
<img src="https://i.imgur.com/tcWaXbb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now after it restarted and booted into it you need to make a password for the admin account so you can sign in:  <br/>
<img src="https://i.imgur.com/tmljDle.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then you have Windows Server 2016 installed on your VM:  <br/>
<img src="https://i.imgur.com/SFtpaVK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now that it is installed we can add Active Directory. First you need to go to Server Manager:  <br/>
<img src="https://i.imgur.com/mymIWue.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then in the top right go to manage and click "Add Roles and Features":  <br/>
<img src="https://i.imgur.com/TaPSLJH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next after reading this screen and for this use case don't need to change anything on the Server selection page either:  <br/>
<img src="https://i.imgur.com/C2hFsjM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now select "Role based or feature-based installation" and click next:  <br/>
<img src="https://i.imgur.com/MJTvnqA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Then on Server roles you need to select Active Directory Domain Services:  <br/>
<img src="https://i.imgur.com/sjonZj5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then that will take you to this screen and just need to press "Add Features":  <br/>
<img src="https://i.imgur.com/W4ixXOg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
It will take you to this screen where you just need to click install then it will start installing:  <br/>
<img src="https://i.imgur.com/S04EPcS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After the feature installation before you click close you need to Promote this server to a domain controller but clicking here:  <br/>
<img src="https://i.imgur.com/gK5EI7Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Next it will take you to this menu where you need to add a new forest because this a is new server and you don't have forest or domain:  <br/>
<img src="https://i.imgur.com/5WJdI8h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Then on this screen you need to make a DSRM password:  <br/>
<img src="https://i.imgur.com/eaHHXxj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After proceding to the prerequisites check(which will take some time) you just need to click install:  <br/>
<img src="https://i.imgur.com/MH9C8FT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once it gets installed you will be signed out and have to restart(The restart will take a lot of time to complete):  <br/>
<img src="https://i.imgur.com/5WJdI8h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now if you go to Active Directory Users and computers you can see it installed and see the domain:  <br/>
<img src="https://i.imgur.com/DVOi6Qz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
