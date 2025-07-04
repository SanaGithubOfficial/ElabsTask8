# Working with VPNs
## Objective:
 Understand the role of VPNs in protecting privacy and secure communication.

## 1. Why VPN?
VPNs (Virtual Private Networks) encrypt your internet traffic and mask your IP address, giving you:
Privacy: Hide your real location/IP
Security: Encrypts data, especially on public Wi-Fi
Freedom: Access blocked or restricted content

## 2. Setup Steps Recap (ProtonVPN)
### Required Steps You Likely Did:
1. Created a free ProtonVPN account: https://account.protonvpn.com
2. Downloaded OpenVPN configuration files from: https://account.protonvpn.com/downloads
3. Placed .ovpn files into:
C:\Program Files\OpenVPN\config
4. Ran OpenVPN as Admin, right-clicked tray icon → Connected to server.

## 3. Screenshots 
### Take the following screenshots:
1.	protonVPN  showing “Connected” (bottom-right taskbar icon green)

2.	https://whatismyipaddress.com with new ProtonVPN-assigned IP
 
3.  Wireshark with TLS filter applied: tls
 Confirms encrypted HTTPS traffic
 
4.  Disconnected state – show original IP and/or speed comparison (optional: speedtest.net)
 

## 4. Verify VPN Effectiveness
Visit: https://whatismyipaddress.com
Before VPN: Take note of your IP & location.
After VPN: Confirm IP has changed to ProtonVPN server location.
Run Wireshark:
Filter: tls
You should see encrypted traffic when browsing HTTPS websites.

## 5. VPN Encryption & Privacy Features (ProtonVPN)
Protocols: OpenVPN (UDP/TCP), IKEv2, and WireGuard
Encryption: AES-256, perfect forward secrecy (PFS)
DNS Leak Protection: Enabled
Kill Switch: Prevents traffic leaks if VPN disconnects
No Logs Policy: No personal data stored or sold
Secure Core: (Paid only) routes traffic through multiple servers

## 6. Summary: VPN Benefits & Limitations
### Benefits:
Strong traffic encryption
 Masks IP and protects against ISP/government surveillance
 Secures public Wi-Fi use
 Access geo-blocked content (limited in free plan)

### Limitations:
 Free plan only has a few servers (can affect speed)
 No P2P or Secure Core on free accounts
 Slight latency increase due to encryption
 Trust still required in VPN provider
