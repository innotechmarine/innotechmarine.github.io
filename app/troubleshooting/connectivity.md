---
layout: page
title: Troubleshooting connectivity
parent: Troubleshooting
---

# Troubleshooting connectivity

The app connects to the devices (TCM, N2KWG) using Wi-Fi on the 2.4 GHz band and discovers them using mDNS. If you're having problems connecting to the devices, it is likely due to an issue in the Wi-Fi or mDNS.

## VPNs and Ad Blockers

VPNs are used to route network traffic elsewhere. Some ad blockers will also rely on using a local VPN to monitor and block traffic. However, since the app requires a direct connection to the devices, **you must disable the VPN** prior to using the app. If a VPN is enabled, some features (mDNS host resolution) may not function properly.

These apps are known to cause problems with connecting to a device:

- DuckDuckGo's ad blocker/privacy features
- Cisco AnyConnect

## External networks

If you're connecting your devices to an external network, you must enable:

- 2.4 GHz broadcast
    - Some newer routers may only provide a 5 GHz AP, however both the TCM and N2KWG require a 2.4 GHz access point
- Multicast
    - This is required to discover the devices on the network

