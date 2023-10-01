<h1>Add Existing Data Disk to a VM in Azure</h2>

<h2>Overview</h2>
Our company has two virtual machines, but wants to delete one and attach the VM to the other virtual machine.
<br />
<img src="https://imgur.com/hVaiiIa.png" />
Opening Azure Portal, we can see our resource group in detail.
We have WinVM1 and WinVM2.
<img src="https://imgur.com/hRkZpgv.png" />
We can see an overview of the topology of our Resource Group.
<img src="https://imgur.com/KSumsAm.png" />
We'll start off by deleting the unneeded virtual machine.
<img src="https://imgur.com/nKr0EWD.png" />
WinVM2 and the corresponding NSG and PIP have been deleted, but the OS Disk remains.

Now if we open our winVM1 and go to > Disks. We can attach an existing disk. I can select the WinVM2 disk that remains and hit apply.
<img src="https://imgur.com/mZzmHMM.png" />
To connect to VM1, we can download the Native RDP file.
<img src="https://imgur.com/emvX0LD.png" />
If we log in via RDP to our VM, we can open it up. Looking at the file explorer you we can see that we have access to a Windows G drive.
<img src="https://imgur.com/DcI1OoO.png" />
We have successfully connected Disk2 with WinVM1.