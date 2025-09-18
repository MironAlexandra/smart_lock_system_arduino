Smart Lock Project – Arduino
============================

About the Project
-----------------

This Arduino application was developed during **Integration 3** (Academic Year 2024–2025, KdG University). The goal was to build the **embedded device logic** for the Smart Lock system.

The Arduino scans RFID tags, connects to Wi-Fi, and communicates with the **Spring Boot backend** for validation. It can also process **remote unlock commands** sent from the backend.

Although developed as a **team project**, I contributed heavily to **backend integration, communication protocols, and testing with the Arduino device**.

My Contributions
----------------

*   Implemented **Wi-Fi communication logic** using Arduino libraries (WiFiS3, ArduinoHttpClient).
    
*   Developed the **REST client** to send RFID scans to the backend.
    
*   Handled **remote unlock commands** from backend to trigger lock status.
    
*   Contributed to **RFID registration workflow** (new tags sent to backend).
    
*   Debugged and tested data flow between Arduino and Spring backend.
    
*   Documented hardware setup and usage for my team.
    

Hardware & Libraries
--------------------

*   **Board:** Arduino UNO R4 WiFi
    
*   **RFID:** RDM6300 reader
    
*   **Indicators:** Green LED (unlock), Red LED (lock)
    
*   **Libraries:** ArduinoJson, WiFiS3, ArduinoHttpClient
    

Agile Process
-------------

We applied Scrum-inspired teamwork:

*   Pair programming on Arduino ↔ backend integration.
    
*   Frequent testing & sprint demos.
    
*   Issue tracking and peer reviews on GitLab.
    

Relation to Backend Repo
------------------------

This Arduino code is tightly coupled with the backend repository:

*   Sends **RFID data** → backend for validation.
    
*   Receives **unlock commands** ← backend.
    

👉 See the Backend repository for the server logic.

Setup & Run
-----------

1.  Flash this repo’s Arduino code to an **Arduino UNO R4 WiFi**.
    
2.  Connect to Wi-Fi (credentials in config.h).
    
3.  Ensure the backend is running and reachable.
    
4.  Scan an RFID tag – the Arduino will contact the backend for validation.
    

Contact
-------

📧 [mariaalexandra.mirongavril@student.kdg.be](mailto:mariaalexandra.mirongavril@student.kdg.be)

