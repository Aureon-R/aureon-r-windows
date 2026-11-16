<p align="center"><img src="https://aureonvpn.com/images/aureon-r-launcher.webp" width="96" height="96" alt="Aureon R"></p>
<h1 align="center">Aureon R for Windows</h1>

<p align="center">Your nodes. Your servers. Your control.</p>

<p align="center"><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>

<p align="center"><a href="https://github.com/Aureon-R/aureon-r-client">Android version</a> · <strong>Windows version</strong></p>

<p align="center"><strong><a href="https://github.com/Aureon-R/aureon-r-windows/releases/latest">Download latest Windows EXE (v0.1.35)</a></strong> · <a href="https://aureonvpn.com/en/aureon-r">Official website</a></p>

Aureon R is an independent proxy client that supports importing your own nodes and self-hosted VPS deployment. No official proxy nodes are provided.

## App screenshots

Windows v0.1.28 interface previews with example data. Select an image to view it at full size.

<table>
<tr>
<td align="center"><a href="home-en.png"><img src="home-en.png" width="190" alt="Connection"></a><br><strong>Connection</strong></td>
<td align="center"><a href="nodes-en.png"><img src="nodes-en.png" width="190" alt="Node management"></a><br><strong>Node management</strong></td>
<td align="center"><a href="deploy-en.png"><img src="deploy-en.png" width="190" alt="One-click VPS deployment"></a><br><strong>One-click VPS deployment</strong></td>
<td align="center"><a href="settings-en.png"><img src="settings-en.png" width="190" alt="Settings and import"></a><br><strong>Settings and import</strong></td>
</tr>
</table>

Actual connected Windows interface (Chinese UI; private connection information masked):

<a href="home-live-zh.png"><img src="home-live-zh.png" width="190" alt="Verified DNS and live connection"></a>


## Key Features

- **Multi-protocol support:** Dual sing-box and Xray cores supporting VLESS Reality Vision, VMess TLS, Trojan TLS, Hysteria 1/2, TUIC v5, WireGuard and AnyTLS.
- **Node management:** Import links, text, files, QR code images and subscriptions. Manage, update and switch nodes. No registration is required for ordinary node use.
- **Routing & security:** Global proxy, application/domain/IP split routing, LAN bypass, strict mode, encrypted DNS (DoH) and leak protection.
- **Connection monitoring:** Real-time traffic, one-click latency testing and ascending sorting, IP-based country and region flags, and DNS resolution verification.
- **Self-hosted deployment:** One-click Debian VPS deployment via SSH, automatic Docker and firewall configuration, and support for adding protocols, redeployment and removal.
- **Multiple VPS deployments:** Manage multiple independent VPS instances under one account, with up to eight supported protocols per server; adding servers preserves existing nodes.
- **Node sharing:** Share nodes via QR codes and links, with independent guest credentials, guest management and access revocation. Sharing access requires approval.
- **Backup & restore:** Encrypted backups and incremental restoration using the same account.
- **Desktop experience:** Chinese and English interface, system tray, account management, private support messaging and update checks.

## Multiple independent VPS deployments

Manage several Debian VPS instances under one account. Each server has its own Docker deployment and DNS settings and can host up to eight supported protocols. For example, three VPS instances in the US, Japan and Germany can host eight nodes each (24 nodes in total). To add another VPS, enter its own IP address and SSH credentials and deploy. Existing servers and their nodes remain unaffected. Manage, select and test all self-hosted nodes in the unified node list. Current local capacity is 20 saved VPS profiles and 100 total nodes (including imported, subscription and shared nodes), not a paid-plan quota.

## What's new in v0.1.35

- One-click latency testing for all nodes, including all eight supported protocols; sort from lowest to highest latency, with failed tests last.
- Test while the VPN is connected and strict network protection is active, without switching the current node.
- Probes bind to the physical network interface; temporary WFP rules are automatically removed after testing.
- TCP nodes use port-connect latency; UDP nodes use server ICMP round-trip latency, not UDP protocol handshake verification.

- Automatic and manual update checks, in-app downloads with progress and SHA-256 verification.
- Fixed update installation when the previous client was incorrectly detected as running. The independent update handoff waits for the old process to exit.

## Installation

Supports Windows 10/11 x64, with the .NET runtime included. In-place upgrades are supported. For a manual installation, exit the previous version from the system tray. In-app updates automatically shut down the client before starting installation. The EXE is not Authenticode-signed; Windows may show an unknown-publisher warning. Verify the SHA-256 checksum before running it.

---

## Links

- [Official website](https://aureonvpn.com/en/aureon-r)
- [User guide](https://aureonvpn.com/en/aureon-r/app-guide)
- [Support](https://aureonvpn.com/en/aureon-r/contact)

## Third-party components

- [sing-box 1.14.4 — GPL-3.0](https://github.com/SagerNet/sing-box/tree/v1.14.4)
- [Xray-core 26.10.31 — MPL-2.0](https://github.com/XTLS/Xray-core/tree/v26.10.31)
- IP Geolocation by DB-IP — CC BY 4.0.

See the accompanying third-party notices and SHA-256 checksum file.
