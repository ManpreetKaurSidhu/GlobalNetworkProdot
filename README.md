# GlobalNetworkProdot
Global Network Setup for Prodot Company

## 🧠 Objective
Design, configure, and document a fully functional multi-office enterprise network for Prodot using Cisco Packet Tracer. The network supports all departments in the UK, USA, and Canada, and later extends to Australia with VoIP and smart IoT features.

---
## 🌍 Project Parts

- **Part 1** – UK, USA, Canada offices with shared infrastructure (DNS, DHCP, HTTP, Email)
- **Part 2** – Australia office with VoIP (IP phones) and Smart Office (IoT) integration

---
## 📍 Part 1 – Global Network (UK, USA, Canada)

### 📡 Topology Overview
- Offices: UK (HQ), USA, Canada
- Shared IT Support at UK HQ
- Devices used: 2911 Router, 3560 MLS, Access-Point PT, 2960 Switch, Server-PT, PC, Laptop, Smart Phone, Tablet
- Adding two HWIC-2T modules to enable serial connections in routers to enable redundant connections and power supply to MLS.
- Routers connected in mesh topology for redundancy
- [Topology Design document](https://github.com/ManpreetKaurSidhu/GlobalNetworkProdot/blob/main/Topology%20Design.docx)

### 🔧 Basic Device Configuration

- Created a **base configuration file** with:
  - Hostname setup
  - Banner message 
  - Console and VTY passwords
  - Disabled DNS lookup
  - SSH enabled (domain: `prodot.net`)
  - will enable port security after Vlan setups

- This base config was applied first on a one device, then
- The same configuration file was reused for other devices after making necessary changes

- Configurations were loaded into each device’s **startup-config**

- Devices were reloaded where necessary to apply the updated startup-configs
