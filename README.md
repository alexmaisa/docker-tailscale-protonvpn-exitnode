# docker-tailscale-protonvpn-exitnode
This repository provides a docker-compose setup for creating an encrypted VPN connection using Tailscale and ProtonVPN. The configuration allows your containerized applications to route traffic securely through Tailscale and uses ProtonVPN as an exit-node, enabling flexible and private networking across devices and environments.

🔧 Features

🔐 Secure outbound traffic via ProtonVPN (OpenVPN-based or Wireguard-based connection).

🌐 Enable Tailscale exit-node from within a Docker container.

📦 Fully containerized setup using docker-compose.

🧩 Suitable for cloud instances, home labs, or headless environments.

⚙️ Easily customizable and extensible for other VPN providers*.

🛡️ Ideal for privacy-conscious developers and DevOps professionals.


📁 Contents

docker-compose.yml: Multi-container setup for Gluetun (VPN) and Tailscale.

tailscale/: Configuration for setting up Tailscale within a container.

protonvpn/: OpenVPN or WireGuard credentials and integration scripts for ProtonVPN.

README.md: Setup instructions, environment variables, and usage guide.


💡 Use Cases

Remote development over Tailscale with ProtonVPN routing.

Building self-hosted solutions with reliable encrypted traffic.

Bypassing geo-restrictions while maintaining full privacy.
