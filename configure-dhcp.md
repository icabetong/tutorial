# Configuring DHCP and Connecting Local Devices to the Server

## Procedure

<img src="art/configure-dhcp/0-connect.png">

**Step 0**. Connect to a network, a mobile hostpot will suffice.

<img src="art/configure-dhcp/1-go-to-settings.png">

**Step 1**. Go to the Virtual Machine Settings by click the `Settings` button in the top. Note that the Virtual Machine needs to be powered off to change some settings.

<img src="art/configure-dhcp/2-change-adapter-type.png">

**Step 2**. Go to the Network page and change from `NAT` to `Bridged Adapter` assumming that you didn't change anything from this page. Click `OK`. Then start the VM.

<img src="art/configure-dhcp/3-note-ip-address.png">

**Step 3**. In the Virtual Machine, go to Command Prompt and take not of the current IP address and Gateway. The Gateway address is the most important here. Also, you'll need to be connected to a network it doesn't matter if there's no internet; your mobile hostpot network will do.

<img src="art/configure-dhcp/4-set-ip-address.png">

**Step 4**. Enter this information to the static IP addresses. You can change the IP Address of the Server itself but you'll need to enter the correct Gateway address from earlier.

```
If your Gateway address is 192.168.69.1 then your IP address must be 192.168.69.x

You can replace x with numbers from 2-255 assuming that Gateway is 192.168.69.1
```

<img src="art/configure-dhcp/5-server-manager.png">

**Step 5**. Open `DHCP Management Console` from Server Manager.

<img src="art/configure-dhcp/6-dhcp-console.png">

**Step 6**. Expand `IPv4` then delete the scope you created from other tutorials. Then create a new Scope.

<img src="art/configure-dhcp/7-add-scope.png">

**Step 7**. In the `IP Address Range`, enter an IP Scope, once again, if your gateway is `192.168.69.1` you'll need to enter `192.168.69.100` to `192.168.69.200`.

<img src="art/configure-dhcp/8-add-gateway.png">

**Step 8**. Enter the Gateway address here. Then finish the wizard.

<img src="art/configure-dhcp/9-connect-devices.png">

**Step 9**. Connect other devices through the same network as the Server. 

<img src="art/configure-dhcp/10-see-devices.png">

**Step 10**. If the IP Address of the device is in range on the scope of the IP Address you entered earlier, the device will see that it has been connected to the server. And the server will see the devices in the network.