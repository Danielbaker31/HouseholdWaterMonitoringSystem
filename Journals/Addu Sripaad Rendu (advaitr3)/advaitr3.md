# ECE445 Senior Design Journal - Household Water Monitoring System - Advait Renduchintala

---

## Project Overview
**Project Name**: Household Water Monitoring System  
**Team Member(s)**: Advait Renduchintala (advaitr3)  
**Date Started**: 09/16/2024  
**Course**: ECE445 Senior Design  

---

## Table of Contents
1. [Week 1](#week-1)  
2. [Week 2](#week-2)  
3. [Week 3](#week-3)  
4. [Week 4](#week-4)  
5. [Week 5](#week-5)  
6. [Week 6](#week-6)  
7. [Week 7](#week-7)  
8. [Week 8](#week-8)  
9. [Week 9](#week-9)  
10. [Week 10](#week-10)  
11. [Week 11](#week-11) 
12. [Week 12](#week-12)   

---

## Week 1
**Dates**: [9/16-9/21]  
**Goals for the Week**:  
- Started first draft of project proposal  
- Meet with TA to discuss design and get project approved  

**Tasks Completed**:  
During the first week of the project, I focused on creating a high-level block diagram to outline the design of our Household Water Monitoring System. This involved dividing the system into key subsystems: the frontend for user interaction, API endpoints for data communication, and a database to store water usage data. For the database, we explored using AWS DynamoDB, a scalable NoSQL database designed for real-time data handling [1]. To facilitate seamless communication between the frontend and the database, I also began planning the implementation of AWS Lambda functions, which enable serverless API endpoints for data processing [2].

In collaboration with my project partners, I spent significant time understanding the capabilities and limitations of the ESP32 microcontroller. We reviewed its datasheet and referred to online tutorials to understand its GPIO pin configurations and communication protocols [3]. Initially, we planned to integrate the ESP32 as the central device for data collection, using its Wi-Fi capabilities to send sensor data to AWS DynamoDB via the Lambda functions. This integration aimed to ensure real-time monitoring and minimal latency between the hardware and cloud components.

Additionally, I worked on defining three high-level requirements for our system, focusing on functionality, scalability, and usability. I also started drafting the project proposal, which detailed the system’s architecture and the roles of each subsystem. By the end of the week, I completed and submitted the finalized project proposal, ensuring it encompassed all necessary technical and design details.

**Challenges**:  
- Understanding ultrasonic sensor's datasheet and how to integrate it into the project. There is not much description in this picture

**Next Steps**:  
- Drill down design and finish first draft of project proposal  

**Bibliography**:
1. AWS. "Amazon DynamoDB Documentation." AWS Documentation. Available at: https://docs.aws.amazon.com/amazondynamodb/
2. AWS. "AWS Lambda Documentation." AWS Documentation. Available at: https://docs.aws.amazon.com/lambda/
3. Espressif Systems. "ESP32 Technical Reference Manual." Espressif Systems. Available at: https://www.espressif.com/en/products/socs/esp32/resources

---

## Week 2
**Dates**: [9/23-9/28]  
**Goals for the Week**:  
- Start Design Review  

**Tasks Completed**:  
- Rough Draft of design review completed  
- Started researching parts that we need to order  

**Challenges**:  
- Our project requires many systems that we have little experience with, so we needed to research a lot to figure out our design review  

**Next Steps**:  
- Finalize Design Review  

---

## Week 3
**Dates**: [9/30-10/4]  
**Goals for the Week**:  
- Meet with Mentor TA to finalize and correct project proposal  
- Correct project proposal to reflect changes TA suggests  
- Finish design review  

**Tasks Completed**:  
- Met with Mentor TA  
- Created more specific subsystem requirements with detailed unit tests for each  
- Created quantifiable high-level design requirements  
- Finished design review and added new subsystems  
- Did more calculations to ensure our subsystems would succeed  

**Challenges**:  
- We needed to develop unit tests for high-level software components when we haven’t made them yet  

**Next Steps**:  
- Start order parts  
- Set up AWS  
- Begin PCB design  

---

## Week 4
**Dates**: [10/7-10/12]  
**Goals for the Week**:  
- Start order parts  
- Set up AWS  
- Begin PCB design  

**Tasks Completed**:  
- Researched sensors to fit within budget constraints  

**Challenges**:  
- Finding sensors that fit within budget constraints  

**Next Steps**:  
- Finalize part orders  
- Begin ESP32 programming  

---

## Week 5
**Dates**: [10/14-10/19]  
**Goals for the Week**:  
- Constuct Front End
- Breaboard ESP 32 to integrate with WiFi

**Tasks Completed**:  
- Ordered ultrasonic sensors and ESP32 boards  
- Set up initial AWS DynamoDB tables  
- Started basic ESP32 connectivity tests  

**Challenges**:  
- AWS configuration issues and access permissions  

**Next Steps**:  
- Troubleshoot AWS setup  
- Test ESP32 communication with AWS  

---

## Week 6
**Dates**: [10/21-10/26]  
**Goals for the Week**:  
- 3D Prints
- User Interface for Device Registration

**Tasks Completed**:  
- Established working connection between ESP32 and DynamoDB  
- Tested ultrasonic sensor’s basic functionality  
- Sketched preliminary PCB design  

**Challenges**:  
- Interfacing with the ultrasonic sensor using ESP32 GPIO pins  

**Next Steps**:  
- Refine ESP32 code for real-time data logging  
- Start building a breadboard prototype  

---

## Week 7
**Dates**: [10/28-11/2]  
**Goals for the Week**:  
- Test Transducers with ultrasonic sensor + code
- Integrate Database and API Protocols with ESP 32 and PCB

**Tasks Completed**:  
- Built breadboard prototype with ESP32 and sensors  
- Successfully sent mock data to DynamoDB  
- Began debugging timing issues with the sensor  

**Challenges**:  
- Ensuring accurate sensor readings under various flow conditions  

**Next Steps**:  
- Debug timing issues further  
- Start working on web dashboard  

---

## Week 8
**Dates**: [11/4-11/9]  
**Goals for the Week**:  
- Modify Device mount and prints
- Discuss Design changes

**Tasks Completed**:  
- Improved accuracy of ultrasonic sensor measurements  
- Created basic web dashboard framework using React  
- Integrated dashboard with DynamoDB to fetch water usage data  

**Challenges**:  
- React routing and API integration issues  

**Next Steps**:  
- Enhance dashboard design  
- Add real-time updates to the dashboard  

---

## Week 9
**Dates**: [11/11-11/16]  
**Goals for the Week**:  
- Run test cases and verifications for software + 
- fix ultrasonic sensors

**Tasks Completed**:  
- Successfully integrated ESP32, sensors, AWS, and dashboard  
- Verified end-to-end functionality for data logging and visualization  
- Began PCB schematic design  

**Challenges**:  
- Debugging intermittent connectivity issues  

**Next Steps**:  
- Refine PCB design  
- Test system stability under prolonged usage  

---

## Week 10
**Dates**: [11/18-11/23]  
**Goals for the Week**:  
- Tweak bugs find a fix for ultrasonic sensors  

**Tasks Completed**:  
- Completed PCB schematic design  
- Ordered custom PCB for testing  
- Conducted stress tests on system stability  

**Challenges**:  
- Ensuring proper trace routing for the TDC chips  

**Next Steps**:  
- Assemble PCB when it arrives  
- Test full system with PCB  

---

## Week 11
**Dates**: [11/25-11/30]  
**Goals for the Week**:  
- Work on assembly of testing device
- Integrate new ultrasonic sensor and new LCD

**Tasks Completed**:  
- Received and assembled PCB  
- Conducted full system test, including water usage monitoring  
- Debugged minor hardware issues with soldering connections  

**Challenges**:  
- PCB assembly errors leading to intermittent signal loss  

**Next Steps**:  
- Refine soldering technique  
- Begin final report preparation  

---

## Week 12
**Dates**: [12/2-12/06]  
**Goals for the Week**:  
- Final Demo
- Work on final presentation

**Tasks Completed**:  
- Received and assembled PCB  
- Conducted full system test, including water usage monitoring  
- Debugged minor hardware issues with soldering connections  

**Challenges**:  
- PCB assembly errors leading to intermittent signal loss  

**Next Steps**:  
- Refine soldering technique  
- Begin final report preparation  

---

## Final Reflection
**Project Summary**:  
The Household Water Monitoring System successfully integrates hardware and software to measure and display water usage data in real-time. The system uses ultrasonic sensors, an ESP32 microcontroller, AWS cloud infrastructure, and a React-based dashboard to provide transparency in household water consumption.  

**Biggest Takeaways**:  
- Importance of iterative design and testing for hardware-software integration  
- Value of planning and documenting every stage of the process  

**Next Steps**:  
- Continue optimizing system design for cost and performance  
- Explore commercialization opportunities  

**Final Grade (Self-Assessment)**: A  
