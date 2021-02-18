# Installing Windows Server 2016 on VirtualBox

## Prerequisites
* [VirtualBox](https://download.virtualbox.org/virtualbox/6.1.18/VirtualBox-6.1.18-142142-Win.exe)
* Windows Server 2016 ISO

## Procedure

*This tutorial assumes you have already downloaded and installed the required materials.*

### Phase 1: Creating a Virtual Machine

<img src="art/creation/1-main.png">

**Step 1**. Open up VirtualBox then click the `New` button on the upper part of the interface.

<img src="art/creation/2-name.png">

**Step 2**. Then type the name of your Virtual Machine, although not required, you can use the name operating system that will be installed on the VM.

<img src="art/creation/3-ram.png">

**Step 3**. Specify how much RAM that will be allocated to the Virtual Machine. It is recommended that you do not put more than half of your host machine's memory.

<img src="art/creation/4-disk.png">

**Step 4**. Click Create.

<img src="art/creation/5-type.png">

**Step 5**. Click Next.

<img src="art/creation/6-allocation.png">

**Step 6**. Choose `Dynamically Allocated` then click `Next`.

<img src="art/creation/7-size.png">

**Step 7**. Specify the size of the virtual disk. The minimum recommended is 32GB but you can adjust it how much as your storage allows it.

<img src="art/creation/8-done.png">

**Step 8**. You are done. The Virtual Machine is created.

### Phase 2 - Installation

<img src="art/install/1-start.png">

**Step 1**. Start the Virtual Machine by click the `Start` button at the upper portion of the user interface. Click the little folder icon at the right side of the dialog at will eventually show up.

<img src="art/install/2-choose.png">

**Step 2**. A new dialog will show up. Click the `Add` button at the top.

<img src="art/install/3-browse.png">

**Step 3**. Browse for the ISO file you downloaded earlier.
```
The file with the name:
Windows_Server_2016_Datacenter_EVAL... .iso
```

<img src="art/install/4-boot.png">

**Step 4**. Click choose, then `Start` the Virtual Machine. You will be presented with the image above.

<img src="art/install/5-welcome.png">

**Step 5**. Eventually the installer will ask your language and keyboard preferences, leave everything as is then click `Next`.

<img src="art/install/6-start-install.png">

**Step 6**. Click `Install Now`

<img src="art/install/7-edition.png">

**Step 7**. Select `Windows Server 2016 Datacenter Evaluation (Desktop Experience)`. 

```diff
- If you do not select the correct edition, the one with the `Desktop Experience` you will have no GUI to work on!
```

<img src="art/install/8-license.png">

**Step 8**. Read and accept the license terms.

<img src="art/install/9-install-type.png">

**Step 9**. Select `Custom` as the Virtual Machine does not have any operating systems installed on it yet.

<img src="art/install/10-partitioning.png">

<img src="art/install/11-formatting.png">

**Step 10**. Click `New` to create a new partition. A warning appears which wants you to give the permission to system to create a drive for system files. Click on `Ok` button, if you want to add more drives do this process again. When finished hit Next.

<img src="art/install/12-wait.png">

**Step 11**. After clicking `Next`. Wait for the installation to finish. The virtual machine will restart itself a couple of times so be patient. ~~Especially users without SSDs~~.

<img src="art/install/13-password.png">

**Step 12**. After a couple of restarts, the installer will ask for an Administrative Password, enter it two times then click `Finish`.

<img src="art/install/14-ctrl.png">

**Step 13**. Press `CTRL + ALT + DEL` to login to the Virtual Machine, if Windows intercepts it, go to the Virtual Machine -> `Input` -> `Keyboard` -> `Insert CTRL + ALT + DEL`