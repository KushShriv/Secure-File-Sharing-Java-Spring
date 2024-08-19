# Secure File Sharing using Spring
<div align='center'>

![](https://img.shields.io/badge/Spring%20Boot-6DB33F.svg?style=for-the-badge&logo=Spring-Boot&logoColor=white)
![](https://img.shields.io/badge/Spring-6DB33F.svg?style=for-the-badge&logo=Spring&logoColor=white)
![](https://img.shields.io/badge/Apache%20Maven-C71A36.svg?style=for-the-badge&logo=Apache-Maven&logoColor=white)
</div>

## Problem Statement
The project is an end-to-end secure file sharing system, following the P2P architecture. It is developed using the Spring MVC framework and built with Maven.

### Overview
- The system allows secure file sharing through rooms created by clients. Each room has an invite link that peers use to join the network for sending or receiving files. 
- Files are encrypted using AES (Advanced Encryption Standard) encryption algorithm before transmission. The sender encrypts the file with a secret key before sending it, and the receiver decrypts it using the same key available in the room. 
- Additionally, checksums are used to verify file integrity, with SHA-256 as the checksum algorithm. Encrypted files are stored in MongoDB for future reference.


## Running the Project
1. Clone the Repository:
```
git clone https://github.com/KushShriv/Secure-File-Sharing-Java-Spring.git
```

2. Change to the Project Directory:
```
cd Safe-Send-Secure-File-Sharing-System
```

3. Install Maven Dependencies:
```
mvn install
mvn clean install
```

4. Execute the Code:
```
mvn spring-boot:run
```

5. Access the Application in a Browser:
> PEER-1 at Port 8001 and PEER-2 at Port 8002

```
http://localhost:8001
http://localhost:8002
```

### Note - Database Setup 
> Connect to MongoDB before running the project.
> 
> Create databases named `FileDB1` and `FileDB2`.

#### Software Versions used:
- Java - 17
- Spring Boot - 2.6.7
- Packaging - Jar
- Maven