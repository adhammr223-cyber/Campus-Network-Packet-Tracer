# Campus Network — Cisco Packet Tracer

I built this campus network as a networking course project. It connects five buildings and brings together subnetting, static routing, central network services and wireless access.

## Campus layout

- Administration and server room.
- Library.
- Engineering.
- Business.
- Health.

Each building has two floor networks. The five main building routers use a full mesh with 10 links, and each building connects to its floor routers.

## What I practiced

- IPv4 addressing with `/24` LANs and `/30` router links.
- Static routes and default routes.
- Central DHCP and DHCP relay.
- DNS records and web, email and LMS services.
- Wireless access with WPA2 Personal and an Enterprise lab configuration.
- Connectivity checks using ping, name resolution, web and email services.

## Addressing overview

| Building | Floor 1 LAN | Floor 2 LAN |
| --- | --- | --- |
| Administration | `192.168.4.0/24` | `192.168.5.0/24` |
| Library | `192.168.10.0/24` | `192.168.11.0/24` |
| Engineering | `192.168.20.0/24` | `192.168.21.0/24` |
| Business | `192.168.30.0/24` | `192.168.31.0/24` |
| Health | `192.168.40.0/24` | `192.168.41.0/24` |

LAN gateways use the `.1` address. Main router links use `/30` subnets from `10.0.0.0`, and building-to-floor links use `/30` subnets from `172.16.0.0`.

| Service | Address |
| --- | --- |
| DHCP | `192.168.4.2` |
| DNS | `192.168.4.3` |
| LMS | `192.168.4.4` |
| Email | `192.168.4.5` |
| Web | `192.168.4.6` |

## Open the project

1. Download or clone this repository.
2. Open `packet-tracer/campus-network.pkt` in Cisco Packet Tracer.
3. Allow the links to come up, then inspect the routers, switches, clients and servers.
4. Follow the addressing tables and test plan in the [project report](docs/network-project.pdf).

The Packet Tracer file and the original project documents are included as submitted.

## Documentation and walkthrough

- [Network project report](docs/network-project.pdf) — topology, subnet tables, routing, services, wireless setup and test plan.
- [Watch my project explanation](https://youtu.be/CXXiTfmGGpQ).
- [Video submission document](docs/video-explanation.docx).

Wireless values and service domain names in the report belong to the Packet Tracer lab.

## Author

Adham Muayad Hashem
