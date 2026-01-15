# LAB-04 (Theory): Why VPNs Do Not Provide Anonymity

## Overview
Virtual Private Networks (VPNs) are commonly misunderstood as tools that provide complete anonymity. In reality, VPNs only address a limited part of online identification.

---

## What a VPN Actually Does

A VPN:
- Masks the user’s public IP address
- Encrypts traffic between the user and the VPN server
- Changes apparent geographic location

This affects **network-layer visibility only**.

---

## What a VPN Does NOT Hide

Even with a VPN enabled, websites can still identify users through:
- Browser fingerprinting
- Device characteristics
- Behavioral patterns
- Logged-in accounts
- Session correlation

As a result, the user may still be recognized as the same entity across visits.

---

## Security and Privacy Implications

From a security perspective:
- VPNs reduce exposure to ISP-level monitoring
- VPNs do not prevent platform-level identification
- VPN usage itself may be flagged as an anomaly

This is why VPNs are often combined with other controls in enterprise environments.

---

## Conclusion
VPNs are privacy-enhancing tools, not anonymity solutions. They reduce network-level exposure but do not prevent identification at higher layers of the web stack.
