---
layout: default
title: Skynet, the local network tyrant
---

# Skynet, the local network tyrant
![interface](https://github.com/n4s3r/n4s3r.github.io/assets/145504084/fc4dafcc-ff18-4475-9eab-80dadff6b42b)
This was my end of ASIX project. It's a network privilege scaling tool. [Link](https://github.com/n4s3r/skynet "Go to Skynet")

It uses a layered attack:
1. DoS of network's DHCP server
2. Run a rogue DHCP server (automated with templates)
3. Run a rogue DNS server (automated with templates)
4. Run a rogue HTTP server (automated with templates)
5. Infect clients with malware templates hosted on the HTTP server.
