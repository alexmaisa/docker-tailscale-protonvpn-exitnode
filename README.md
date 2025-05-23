# tailscale-protonvpn-exitnode
This repository provides a docker-compose setup for creating an encrypted VPN connection using Tailscale and ProtonVPN. The configuration allows your containerized applications to route traffic securely through Tailscale and uses ProtonVPN as an exit-node, enabling flexible and private networking across devices and environments.

## 🔧 Features

- 🔐 Secure outbound traffic via ProtonVPN (Wireguard-based connection).
- 🌐 Enable Tailscale exit-node from within a Docker container.
- 📦 Fully containerized setup using docker-compose.
- 🧩 Suitable for cloud instances, home labs, or headless environments.
- ⚙️ Easily customizable and extensible for other VPN providers*.
- 🛡️ Ideal for privacy-conscious developers and DevOps professionals.


## 📁 Contents

- compose.yaml: Multi-container setup for Gluetun (VPN) and Tailscale.
- README.md: Setup instructions, environment variables, and usage guide.


## 💡 Use Cases

- Remote development over Tailscale with ProtonVPN routing.
- Building self-hosted solutions with reliable encrypted traffic.
- Bypassing geo-restrictions while maintaining full privacy.

## 🚀 Installation

### 🧰 Prerequisites

Ensure you have the following installed:
- Docker
- Docker Compose or Portainer
- Active accounts for:
  - ProtonVPN
  - Tailscale

Directory structure

.</br>
├── gluetun/</br>
├── compose.yaml</br>
└── README.md

🔑 Step 1: Prepare Credentials and Update compose.yaml

🔐 ProtonVPN
1.  Create WireGuard configuration\
    Go to the ProtonVPN dashboard, go to “Downloads” menu, and select WireGuard configuration for your preferred server. Then copy the configuration.
2.  Update compose.yaml\
    Update compose.yaml variables with your WireGuard configuration.

🌐 Tailscale
1.  Generate an Auth Key\
    Visit https://login.tailscale.com/admin/settings/authkeys and create an auth key. You may turn on Reusable and Preauthorized options. Save your Auth Key.
2.  Update compose.yaml\
    Update - TS_AUTHKEY= with Auth Key that generated before.

▶️ Step 2: Start the Services
