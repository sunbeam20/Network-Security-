# Network-Security-

A network design for CHIP TECH with a total number of 433 employees with larger IP
address block 192.168.1.0/ 25 will be assigned as its major IP address.


The Main office Petaling Jaya will be connected to other 5 branches Johor Bahru, Kuantan,
Kulim, Georgetown and Ipoh through a point to point leased line made of fiber optics. The
main office. The Main Office will have a server room with DHCP, Radius, Syslog, SSH,
Mail and web Server connecting with an encrypted router.



Topology Design

Network Protocol Used in this Network Design

1.Routing

OSPF- Router ospf 1

Dynamic routes are configured on each branch's office and in the main office, to route the
traffic from the inside network to another branch network.

2.DHCP

DHCP is configured in the DHCP server, which is in the server room in the Petaling Jaya
office 192.168.3.194 will be assigned to this server . Each of the hosts’ IP addresses in this
network system will be Allocated dynamically.

3.Network device security

Every router has been configured with password in the console line as well as the vty line.

4.Administrative access control for network device

User and admin has been created for access control for all network devices.

5.Secure Remote Connections (encrypted)

Secure remote connections have been configured with SSH server and scp protocol is
configured for securely transferring computer files between a local host and a remote host or
between two remote hosts.

6.NTP & event logging

For NTP , Petaling jaya’ s router has been made the master router, and all other routers have
been synchronized. And Syslog server is used for event logging , so that any event will be
captured by syslog server.

7.AAA (local, radius,)

Local aaa has been configured for VPN users and Remote aaa is configured in the radius
server.

8.ACL

ACL has been configured in the productive department of Petaling Jaya, Kulim, Kuantan and
Johor Bahru office, to restrict the workers from misuse of the internet for entertainment
purposes.
Extended access control list is also created for the zone firewall.

9.ZPF

Firewall has been configured in PJ router Gig0/0 and Gig0/1 is Trusted Zone mentioned in
the design and other areas are untrusted zones to block some users from accessing resources
which are not allowed.

10.DNS, FTP, SMTP

DNS, FTP and SMTP services have been configured to check whether ACL is working or
not.

11.Securing LAN configuration

CAM table attack:

Every Second layer switch has been configured so that no more than 3 Mac addresses for a
single port is allowed. And unused ports are down for 1st and 2nd layer switches to mitigate
the attacks.

DHCP attack:

All the trust ports are allowed for DHCP ip requests. And ip DHCP snooping limit rate is 6.

VPN

VPN is configured for remote hosts who are working from home due to covid-19 for
functional departments in PJ.

Wireless Security

3 Wireless lan Controllers have been configured for LAP in Petaling jaya, Ipoh, Kuantan so
that some users with wireless devices could use the company’s intranet.
