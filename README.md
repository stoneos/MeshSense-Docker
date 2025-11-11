# MeshSense-Docker  
Docker Compose setup for MeshSense  

## Overview  
This repository provides a ready-to-use `docker-compose.yaml` configuration to deploy MeshSense in a containerised environment.  
MeshSense is an open-source tool that monitors, maps and visually presents the health of your Meshtastic mesh network (via Bluetooth or WiFi).  
👉 [MeshSense on GitHub](https://github.com/Affirmatech/MeshSense)

By using this Docker Compose setup, you can run MeshSense easily on a host system or within a server, without manual installation of all components.

## Features  
- Simple Docker Compose file to spin up all required services  
- Environment variables configurable via `.env` file (e.g., port mappings, volumes, data persistence)  
- Keeps the MeshSense application isolated and reproducible through containers  
- Integrates seamlessly with your Meshtastic node deployment  

## Quick Start  
1. Clone this repository:  
   ```bash
   git clone https://github.com/DN9KGB/MeshSense-Docker.git
   cd MeshSense-Docker
   ```
2. Copy and edit the .env file if needed (set ports, volumes, network settings)

3. Launch the services:
   ```bash
   docker-compose up -d
   ```

4. Access the MeshSense UI (via the port defined in your .env or docker-compose.yaml)

5. For detailed usage of MeshSense itself, see the main project:
👉 https://github.com/Affirmatech/MeshSense

## About MeshSense
MeshSense connects to your Meshtastic node over Bluetooth or WiFi and continuously collects data to assess and visualise the network’s health — including connected nodes, signal reports, trace routes and more.
Repository: https://github.com/Affirmatech/MeshSense

## Licence
Please refer to the original MeshSense project’s licence (GPL-3.0) and ensure compliance.
This Docker Compose config inherits the same open-source nature.

## Contributing
Feel free to submit pull requests or file issues if you encounter any problems or would like enhancements (e.g., for ARM builds, additional services, monitoring setups).
