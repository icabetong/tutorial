# Enable DHCP Server in Windows Server 2016

## Procedure

This guide assumes that you have already setup a static IP on the server. If you didn't, follow [this](static-ip.md) guide.

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