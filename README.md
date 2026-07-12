# MeshTik — WireGuard mesh config generator for MikroTik

MeshTik is a free tool that builds a full-mesh [WireGuard](https://www.wireguard.com/) configuration for MikroTik routers and any other device. You describe your sites once and get ready-to-paste RouterOS commands for each router, plus universal `wg-quick` files for Windows, macOS, Linux, iOS, and Android in the same mesh.

**Live tool: [meshtik.com](https://meshtik.com/)**

## What it does

Setting up WireGuard across several MikroTik sites by hand means writing peers, addresses, allowed IPs, routes, and firewall rules on every router, and keeping the public keys in sync. MeshTik does that part for you. Add your nodes, pick each device type, and it generates a complete configuration where every node can reach every other node.

For MikroTik you get RouterOS v7 commands you can paste straight into a terminal. For laptops and phones you get a standard `wg-quick` config that joins the same mesh, so a Windows machine and a MikroTik router end up on one network.

## Features

- Full-mesh topology: every node peers with every other node automatically.
- RouterOS v7 output for MikroTik, and universal `wg-quick` output for everything else.
- Keys are generated in your browser with Curve25519 and never sent anywhere. The page works offline.
- Download each config, grab them all as a single zip, or scan a QR code to import straight into the WireGuard mobile app.
- Available in several languages.

## How to use

1. Open [meshtik.com](https://meshtik.com/).
2. Set your network address range.
3. Add a node for each site or device and choose whether it is a MikroTik router or a plain WireGuard client.
4. Copy the generated commands to each MikroTik, or import the `wg-quick` files on your other devices.

No account, no server, no upload. Because the keys are generated locally, you can even run it with your network cable unplugged.

## Privacy

Every private and public key is created in your own browser using Curve25519, the same curve WireGuard uses. Nothing about your network leaves your device.

## Links

- Website: https://meshtik.com/
- WireGuard: https://www.wireguard.com/

---

Keywords: mikrotik wireguard, wireguard mesh generator, routeros wireguard config, wg-quick config, mikrotik site to site vpn.
