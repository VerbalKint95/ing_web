---
title: PQC Data Signing API
publishDate: 2023-02-27 00:00:00
img: /assets/thales_project_image.jpeg
img_alt: THALES DIS Project
description: |
  Designed and implemented an API during my internship at THALES DIS, providing a data signing service using the Crystal Dilithium algorithm—a Post Quantum Cryptographic (PQC) algorithm designed to resist attacks by quantum computers. This project served as a demonstration within the scope of the European Electron project.

tags:
  - API
  - Cryptography
  - PQC
  - C++
  - SpringBoot
---

## Overview

Embarked on a project at <a href="https://www.thalesgroup.com/en/markets/digital-identity-and-security">THALES DIS</a> to design and implement an API delivering a data signing service utilizing the <a href="https://pq-crystals.org/dilithium/">Crystal Dilithium algorithm</a>. Crystal Dilithium is a Post Quantum Cryptographic algorithm specifically crafted to withstand potential attacks by quantum computers. The project played a pivotal role in the European <a href="https://electron-project.eu">Electron</a> project, serving as a demonstration of the practical application of advanced cryptographic techniques.

### Implementation Details

The implementation involved a client-server architecture, with a C++ client communicating with a SpringBoot service. The client submitted a request containing the data to be signed. The SpringBoot server, in turn, transmitted this data to an executable via a file system. The C++ executable utilized the PKCS#11 library to facilitate data signing through a smart card containing the Dilithium implementation.

### Key Components

- **Crystal Dilithium Algorithm:** Employed as the core cryptographic algorithm for data signing, providing a robust defense against potential quantum attacks.
- **C++ Client:** Responsible for initiating the signing process by sending data signing requests to the SpringBoot server.
- **SpringBoot Server:** Acted as the intermediary between the client and the executable, facilitating seamless communication and data transmission.
- **PKCS#11 Library:** Utilized by the C++ executable to interact with the smart card, ensuring secure and standardized cryptographic operations.

### Project Significance

This project showcased the practical integration of post-quantum cryptographic techniques into real-world applications. As part of the European Electron project, it contributed to the exploration and validation of advanced cryptographic methods for securing sensitive data in the face of evolving technological landscapes.

---