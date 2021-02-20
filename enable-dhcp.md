# Enable DHCP Server in Windows Server 2016

## Procedure

```
This guide assumes that you have already setup a static IP on the server. If you didn't, follow [this](static-ip.md) guide.
```

### **Adding through the Server Manager**

<img src="art/enabling-features/1-find-server-manager.png">

**Step 1**. Open the Start Menu then open `Server Manager`.

<img src="art/enabling-features/2-add-roles.png">

**Step 2**. In Server Manager, click `Add roles and features`.

<img src="art/enabling-features/3-next.png">

**Step 3**. Click `Next`

<img src="art/enabling-features/4-next.png">

**Step 4**. Leave everything as is, then click `Next` again.

<img src="art/enabling-features/5-destination.png">

**Step 5**. In the `Server Pool list`, click the only option below, then click `Next`.

<img src="art/enabling-features/6-dchp.png">

**Step 6**. Check the `DHCP Server` option. Then click `Next.

<img src="art/enable-dhcp/7-review.png">

**Step 7**. Click next.

<img src="art/enable-dhcp/8-confirm.png">

**Step 8**. Click next.

<img src="art/enable-dhcp/9-install.png">

**Step 9**. Wait for it to install.

<img src="art/enable-dhcp/10-configure.png">

**Step 10**. After installing click the yellow warning icon at the top then click `Configure DHCP Configuration`.

<img src="art/enable-dhcp/11-start-configure.png">

**Step 11**. Click next.

<img src="art/enable-dhcp/12-credentials.png">

**Step 12**. Click `Commit`.

<img src="art/enable-dhcp/13-commit.png">

**Step 13**. Click `Close`.

### **Configuration**

<img src="art/enable-dhcp/14-dhcp-man.png">

**Step 14**. Click `Tools` in the upper part of the interface then click `DHCP`.

<img src="art/enable-dhcp/15-new-scope.png">

**Step 15**. Expand the server then right click `IPv4`, then click `New Scope` in the context menu.

<img src="art/enable-dhcp/16-wizard.png">

**Step 16**. Type in a name for the scope.

<img src="art/enable-dhcp/17-range.png">

**Step 17**. Enter the range of addresses that the scope distributes. Then type the length then click `Next`.

<img src="art/enable-dhcp/18-exclusions.png">

**Step 18**. If there are any excluded address, add them here. If you are done, click `Next`.

<img src="art/enable-dhcp/19-lease.png">

**Step 19**. Click next.

<img src="art/enable-dhcp/20-gateway.png">

**Step 20**. Enter the IP Address of the router.

<img src="art/enable-dhcp/22-get-domain-name.png">
<img src="art/enable-dhcp/21-domain.png">

**Step 21**. Enter the domain name and its address.
```
Hint: The domain name is the PC name in the About section in the Settings app.
```
<img src="art/enable-dhcp/23-wins.png">

**Step 22**. Click next.

<img src="art/enable-dhcp/24-activate.png">

**Step 23**. Leave the current selection then click next.