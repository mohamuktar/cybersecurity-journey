# **LAB 8: Configure Secure Passwords and SSH**

**Purpose:** To secure the router (RTA) and switch (SW1) by configuring strong passwords, encrypting credentials, and enabling SSH for secure remote access.

## **Tasks Completed**

1\. **Configure Router RTA:** Set the hostname, configured the G0/0 IP address, enabled the interface, encrypted passwords, and created a strong enable secret.

2\. **Enable SSH on RTA:** Set the domain name, created a local user account, generated 1024-bit RSA keys, and configured VTY lines to allow SSH access.

3\. **Configure Login Security:** Set a minimum password length of 10 characters and configured login blocking after four failed attempts within two minutes.

4\. **Configure Switch SW1:** Set the hostname, configured the VLAN 1 management IP address and default gateway, and enabled the interface.

5\. **Secure Switch Ports:** Disabled unused switch ports using the `interface range` command and applied password encryption and SSH security settings.

6\. **Save Configurations:** Saved the router and switch configurations to NVRAM using `copy running-config startup-config`.

7\. **Test Connectivity:** Used PCA's command prompt to test SSH access to RTA and checked that all network links were green.

## **Additional Network Security Best Practices**

- **Access Control Lists (ACLs):** Restrict network traffic and prevent unauthorized access.
- **DHCP Snooping:** Protect against unauthorized DHCP servers.
- **Dynamic ARP Inspection (DAI):** Prevent ARP spoofing attacks by validating ARP packets.

**Conclusion:** This lab provided hands-on experience securing network devices through password protection, SSH configuration, login restrictions, and disabling unused switch ports.