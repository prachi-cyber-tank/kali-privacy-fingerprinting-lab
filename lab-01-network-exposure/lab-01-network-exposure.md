# LAB-01: Network & IP Exposure (Kali Linux)

## 🎯 Objective
To understand what information about a user is exposed to websites when connecting to the internet, focusing on private IPs, public IPs, and ISP-based geolocation.

This lab is performed on the user’s **own Kali Linux system** for educational purposes.

---

## 🔹 Step 1: Identify Internal (Private) IP Address

### Command Used
```bash
ip
 a


##Example Output
inet 192.168.164.129/24 brd 192.168.164.255 scope global dynamic eth0

##Observation

The system is assigned a private IP address:

192.168.164.129

##Explanation

This IP address belongs to the private IP range:

192.168.0.0 – 192.168.255.255

##Key Point

Private IP addresses:

Are used only inside local networks (LAN)

Are not visible to the public internet

Cannot be directly tracked or geolocated by websites

🔹 Step 2: Identify Public IP Address
Tool Used

https://ipinfo.io

##Example Result (Public IP)
Public IP: 103.21.244.56
ISP: ExampleNet Broadband Services
Location: Hyderabad, Telangana, India

##Observation

The public IP address is different from the private IP

Location information (city/state) is derived from this public IP

##Explanation

Websites identify users using the public IP address, which is assigned by:

The Internet Service Provider (ISP)

The router or gateway connecting the network to the internet

🔹 Step 3: Private IP (Bogon) Lookup Test
##Action

The private IP address 192.168.164.129 was manually searched on ipinfo.io.

##Result
IP: 192.168.164.129
Type: Bogon / Private IP
Location: Not Available

##Explanation

Private IP addresses are marked as Bogon

They do not exist on the public internet

Geolocation is not possible for private IPs

##Important Clarification

Even when searching a private IP:

The website still detects the visitor’s public IP

Location is derived from the request source, not the searched IP

##Key Concepts Learned

NAT (Network Address Translation) separates private and public networks

Websites can only see public IP addresses

Private IPs never leave the local network

IP-based location is approximate, not exact

This behavior is normal internet operation, not hacking

##Conclusion

This lab demonstrates that online tracking at the network level relies on public IP addresses provided by ISPs. Understanding the difference between private and public IPs is fundamental for cybersecurity, ethical hacking, and privacy analysis.
