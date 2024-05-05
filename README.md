# Edge Computing Project

## Overview
This project is part of the COMP 40660 course at University College Dublin. It focuses on understanding and implementing Multi-Access Edge Computing (MEC) and Fog Computing paradigms through Docker containers. These edge computing paradigms help 5G networks achieve low-latency and high-bandwidth goals.

## Objectives
- Understand lightweight virtualization for edge computing.
- Learn the basics of Docker virtualization.
- Develop a dockerized environment simulating an edge computing platform.
- Establish edge-to-edge connectivity between Docker containers.
- Emulate mobile offloading scenarios.

## Contributors
- Anant Singh (23200461)
- Subhranshu Swain (23202288)
- Sonia Srinivas (23200489)

## Tasks

### Task 1: Basic Docker Virtualization
1. **Pull Docker Images:**  
   Successfully pulled the following images:
   - hello-world
   - busybox
   - nginx  
   ![Pulled Docker Images](URL_TO_HELLO_WORLD_IMAGE)

2. **Run Docker Containers:**  
   The containers ran successfully, and their installation and status information can be seen below:  
   ![Docker Containers Running](URL_TO_RUNNING_CONTAINERS_IMAGE)

3. **Nginx Web Server:**  
   Set up an Nginx container running on port 8080 and customized the HTML to include group member names:  
   ![Nginx Web Server Custom HTML](URL_TO_NGINX_HTML_IMAGE)

4. **Ubuntu Container Customization:**  
   - Installed additional Linux packages inside the Ubuntu container.
   - Created a directory with the group name and added a text file listing all group members:  
   ![Customized Ubuntu Container](URL_TO_UBUNTU_CONTAINER_IMAGE)

5. **Docker Hub Upload:**  
   The customized Ubuntu container was pushed to Docker Hub.  
   **Link:** [shazam0325/mission-possible](https://hub.docker.com/r/shazam0325/mission-possible/tags)

### Task 2: Docker Networking
1. **Bridge Network:**  
   Connected three Alpine containers using the default bridge network. The connectivity between them was verified via ping commands.  
   - **Ping Results - Container 1:**  
     ![Ping Container 1](URL_TO_PING_1_IMAGE)
   - **Ping Results - Container 2:**  
     ![Ping Container 2](URL_TO_PING_2_IMAGE)
   - **Ping Results - Container 3:**  
     ![Ping Container 3](URL_TO_PING_3_IMAGE)

2. **IPC Channel:**  
   Established an IPC channel between two Ubuntu containers using sockets.  
   - **Server Message:**  
     ![IPC Server Message](URL_TO_IPC_SERVER_IMAGE)
   - **Client Message:**  
     ![IPC Client Message](URL_TO_IPC_CLIENT_IMAGE)

3. **Offloading Scenario:**  
   Transferred parametric values from container 1 to container 2, computing mean, median, and standard deviation:
   - **Mean:** 54.69
   - **Median:** 65.27
   - **Standard Deviation:** 32.15  
   ![Offloading Scenario Stats](URL_TO_OFFLOADING_STATS_IMAGE)

4. **Second Offloading Scenario:**  
   Emulated another offloading scenario with server-client messages:
   - **Server-Side Message:**  
     ![Second Offloading Server Message](URL_TO_SECOND_SERVER_MESSAGE_IMAGE)
   - **Client-Side Message:**  
     ![Second Offloading Client Message](URL_TO_SECOND_CLIENT_MESSAGE_IMAGE)

## Conclusion
In this project, we demonstrated the successful use of Docker containers for edge computing. We used lightweight virtualization to simulate MEC and Fog computing paradigms while achieving networking and offloading scenarios through Docker networking.

## Submission Instructions
Submit the design document, video, and README separately to Brightspace before the deadline: **11:59 PM on 28th April 2024**.
