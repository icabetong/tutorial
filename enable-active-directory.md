# Enable and Configure Active Directory Services

## Procedure

### *This guide assumes that you have already setup a static IP on the server. If you didn't, follow [this](static-ip.md) guide.*

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

**Step 6**. Check `Active Directory Domain Services`

<img src="art/enabling-features/8-active-directory.png">

**Step 7**. Once again, click `Add Features`

<img src="art/enabling-features/6-dchp.png">

**Step 8**. Check `DNS Server`.

<img src="art/enabling-features/9-features.png">

**Step 9**. Leave everything as is, then click `Next`.

<img src="art/enabling-features/10-done-install.png">

**Step 10**. Wait for it to install. Then click `Close`.

<img src="art/enabling-features/11-configure.png">

**Step 11**. Click the yellow warning icon in the top, then click `Promote this server to a domain controller`

<img src="art/enabling-features/12-start-configure.png">

**Step 12**. Select `Add a new forest` then type a domain name. Then click `Next`

<img src="art/enabling-features/13-domain-controller.png">

**Step 13**. Leave everything as is, then type a password.

<img src="art/enabling-features/14-dns-options.png">

**Step 14**. Click `Next`.

<img src="art/enabling-features/15-netbios.png">

**Step 15**. Specify a NetBIOS name or leave the default, then click next.

<img src="art/enabling-features/16-review.png">

**Step 16**. Click next.

<img src="art/enabling-features/17-prereq.png">

**Step 17**. Click next again.

<img src="art/enabling-features/18-install.png">

**Step 18**. Wait for it to install.

<img src="art/enabling-features/19-check.png">

**Step 19**. From within Server Manager, click `Tools` then `Active Directory Users and Computers`.

<img src="art/enabling-features/20-check2.png">

**Step 20**. Expand the domain root (mine is `KASERWERKE.internal`) then click `Domain Controllers`. You should see your server being displayed. Close the window.

<img src="art/enabling-features/21-local.png">

**Step 21**. Go back to Server Manager then click `Local Server` at the left side then click `Remote Desktop`.

<img src="art/enabling-features/22-remote.png">

**Step 22**. Select `Allow remote connections to this computer`. Then uncheck the option `Allow connections only from computers running Remote Desktop with Network Level Authentication`.