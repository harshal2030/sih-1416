# AI-Based Automatic Alarm Generation and Payload Dropping via Drone

## Table of Contents
- [Project Description](#project-description)
- [Detailed Architecture](#detailed-architecture)
- [Use Cases](#use-cases)
- [Team Members](#team-members)
- [Timelines](#timelines)

## Project Description
This project aims to utilize AI and drone technology for disaster management by automatically generating alarms and deploying payloads to through drones. The solution employs infrared/thermal-camera-equipped drones, Nvidia Jetson for real-time AI processing, YOLOv5 for human detection, and more to effectively manage and respond to disaster scenarios.

## Detailed Architecture

### 1. Human Detection
- **Infrared/Thermal Camera:** FLIR Vue Pro R, for its radiometric data and excellent thermal sensitivity.
- **ML Algorithm:** YOLOv5, due to its impressive speed and accuracy in real-time object detection.
### 2. Drone Technology
- **Drone Model:** DJI Matrice 300 RTK, for its robust build, excellent payload capacity, and advanced AI capabilities.
- **Navigation:** Utilize the built-in GPS of DJI Matrice 300 RTK and integrate it with GIS for mapping and pathfinding.
- **Communication:** Utilize the OcuSync Enterprise transmission system for stable communication even in complex environments.
- **Payload Management:** Custom-built mechanical claws controlled via servo motors, designed to fit the drone’s payload mount.
### 3. Nvidia Jetson
- **Model:** Nvidia Jetson AGX Xavier, for its high-performance compute capabilities in AI processing and robotics, while maintaining a compact form factor suitable for drone integration.
### 4. GIS and Navigation
- **Mapping:** Utilize high-resolution satellite imagery, possibly from a provider like Mapbox.
- **Pathfinding Algorithm:** A* algorithm, for its effectiveness in finding the shortest path while considering various constraints.
- **Dynamic Re-routing:** Implement a dynamic re-routing algorithm that adjusts the path based on real-time obstacle data and mission updates.
### 5. Communication Hub
- Data Transmission: Utilize a 4G/LTE module for communication between the drone and the control center.
Data Security: Implement end-to-end encryption using protocols like TLS for secure communication.
### 6. Scalable Swarm Intelligence
- **Swarm Coordination:** Utilize ROS (Robot Operating System) to manage and coordinate the swarm of drones.
- **Distributed Computing:** Utilize ROS 2’s DDS middleware to manage distributed computing across drones.
- **Swarm Communication:** Utilize a dedicated communication channel, possibly via a mesh network, to ensure reliable communication within the swarm.
### 7. Power Management
- **Battery:** Utilize TB60 Intelligent Flight Battery for DJI Matrice 300 RTK, considering its 55-minute max flight time.
- **Recharging:** Implement a manual battery replacement protocol for continuous operation.
- **Power Optimization:** Implement algorithms to optimize flight paths and operations for minimal power usage.

## Use Cases

- Aerial Lifeline : Drones form life-saving aerial bridges in inaccessible areas, expediting evacuations.

- Personalized Aid: AI-powered drones deliver tailored supplies, adapting to survivors' specific needs on the spot.

- Emergency Relays: Drones act as emergency communication relays, bridging communication gaps in remote disaster-stricken regions.

- Psychological Support: Utilize drones to broadcast messages of hope and reassurance to survivors, providing psychological support in distressing situations.

## Team Members

- [Harshal Sanghvi]()
- [Ashish Rathore]()
- [Keshav Joshi]()
- [Darshika Panwar]()
- [Palak Tiwari]()
- [Avdesh Kharadia]()

## Timelines

```// to be decided```
