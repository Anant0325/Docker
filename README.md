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
![image](https://github.com/Anant0325/Docker/assets/149093814/4f263925-b9a7-4448-b2bc-3c0470887e9d)


2. **Run Docker Containers:**  
   The containers ran successfully, and their installation and status information can be seen below:  
  ![image](https://github.com/Anant0325/Docker/assets/149093814/4e661d8c-325d-4709-a17a-231e297d7db9)


3. **Nginx Web Server:**  
   Set up an Nginx container running on port 8080 and customized the HTML to include group member names:  
![image](https://github.com/Anant0325/Docker/assets/149093814/b8fd03b2-37b4-4c54-81e1-e5720d439141)


4. **Ubuntu Container Customization:**  
   - Installed additional Linux packages inside the Ubuntu container.
   - Created a directory with the group name and added a text file listing all group members:  
![image](https://github.com/Anant0325/Docker/assets/149093814/391cdf25-8152-4a11-bbff-154f05f8ec06)


5. **Docker Hub Upload:**  
   The customized Ubuntu container was pushed to Docker Hub.
   ![image](https://github.com/Anant0325/Docker/assets/149093814/d7c30b62-96f2-471d-ba8e-46a6cd14c703)
 
   **Link:** [myubuntu_custom](https://hub.docker.com/repository/docker/shazam0325/myubuntu_custom/general)  
   Optional: [mission-possible](https://hub.docker.com/repository/docker/shazam0325/mission-possible/general)

### Task 2: Docker Networking
1. **Bridge Network:**  
   Connected three Alpine containers using the default bridge network. The connectivity between them was verified via ping commands.  
   - **Ping Results - Container 1:**  
    ![image](https://github.com/Anant0325/Docker/assets/149093814/85863432-62e6-4a1e-943d-5b1d0471ad1d)

   - **Ping Results - Container 2:**  
   ![image](https://github.com/Anant0325/Docker/assets/149093814/5ffed79c-94e6-42a3-86f7-68b15b59c6dd)

   - **Ping Results - Container 3:**  
    ![image](https://github.com/Anant0325/Docker/assets/149093814/1b55e4af-9e39-4534-8bd1-0ca32538766f)


2. **IPC Channel:**  
   Established an IPC channel between two Ubuntu containers using sockets.  
   - **Server Message:**  
   ![image](https://github.com/Anant0325/Docker/assets/149093814/aef75cf2-c7b4-44ae-9d0e-9a178a82dc58)

   - **Client Message:**  
    ![image](https://github.com/Anant0325/Docker/assets/149093814/3f91f969-2fa2-46d7-9fad-a80c0643d8df)


3. **Offloading Scenario:**  
   Transferred parametric values from container 1 to container 2, computing mean, median, and standard deviation:
   - **Mean:** 54.69
   - **Median:** 65.27
   - **Standard Deviation:** 32.15  
  ![image](https://github.com/Anant0325/Docker/assets/149093814/f06d635d-17a0-413d-888e-c8f88e6558f0)


4. **Second Offloading Scenario:**  
   Emulated another offloading scenario with server-client messages:
   - **Server-Side Message:**  
     ![image](https://github.com/Anant0325/Docker/assets/149093814/7bdbb1fc-9561-427d-a942-6d9eee3df8d4)

   - **Client-Side Message:**  
     ![image](https://github.com/Anant0325/Docker/assets/149093814/f9534e31-d6d6-4a0a-8bd2-3813e9a1af1a)


**Link:** [alpinecontainers](https://hub.docker.com/repository/docker/shazam0325/alpinecontainers/general)

## Conclusion
In this project, we demonstrated the successful use of Docker containers for edge computing. We used lightweight virtualization to simulate MEC and Fog computing paradigms while achieving networking and offloading scenarios through Docker networking.
