# ECE445 Senior Design Journal - Household Water Monitoring System - Daniel Baker

---

## Project Overview
**Project Name**: Household Water Monitoring System  
**Team Member(s)**: Daniel Baker (drbaker5)
**Date Started**: [Insert Start Date]  
**Course**: ECE445 Senior Design  

---

## Table of Contents
1. [Week 1](#week-1)
2. [Week 2](#week-2)
3. [Week 3](#week-3)
4. [Week 4](#week-4)
5. [Additional Weeks...](#additional-weeks)
6. [Final Reflection](#final-reflection)

---

## Week 1: [9/9-9/13]  
**Objectives for the Week**:  
- Identify high-level design of the project  
- Start first draft of project proposal  
- Meet with Mentor TA  

**Tasks Completed**:  
- Met with Mentor TA  
- Brainstormed many ideas for the project, including Smart Roulette Wheel and IoT Alarm  
- Landed on Household Water Monitoring System due to budgeting, difficulty, and feasibility constraints  
- Created a high-level block diagram for the design of the project  
- Made three high-level requirements for the design  
- Started the first draft of the project proposal  

---

## Week 2: [9/16-9/20]  
**Objectives for the Week**:  
- Finalize all parts and design  
- Submit finished project proposal  

**Tasks Completed**:  
- Finalized first draft of the design  
- Submitted the project proposal  

---

## Week 3: [9/23-9/27]  
**Objectives for the Week**:  
- Meet with Mentor TA to finalize and correct the project proposal  
- Correct project proposal to reflect TA suggestions  

**Tasks Completed**:  
- Met with Mentor TA 
- Revised project proposal based on TA suggestions, including:
    - Created more specific subsystem requirements with detailed unit tests for each  
    - Created quantifiable high-level design requirements  

---

## Week 4: [9/30-10/4]  
**Objectives for the Week**:  
- Submit revised project proposal,  
- Finish and submit design document  

**Tasks Completed**:  
- Submitted project proposal revision
- Completed and submitted the design document
    - Created draft physical design
        - ie: ![physical_design error](physical_design.jpg)
    - researched and finalized more specified ideas for each subsystem, and created RV tables for each
        - ie: ![RV error](RV.jpg)
    - finalized flow rate formula for ultrasonic subsystem
        - ![formula error](formula.jpg)

---

## Week 5: [10/7-10/11]  
**Objectives for the Week**:  
- Practice for Design Review
- Start PCB

**Tasks Completed**:  
- Practiced and completed design review presentation
    - Learned of timing challenges for flow rate, thus the need for very presiced time meaurement ICs
        - landed on TDC1000 and TDC7200 for time to digital conversion
- Started Microcontroller Subsystem for PCB
    - ![MCU error](MCU.jpg) 

---

## Week 6: [10/14-10/18]  
**Objectives for the Week**:  
- Complete and order first draft of PCB
- complete teamwork evaluation 1

**Tasks Completed**:
- Completed Power and Programming Subsystem
    - ![power_programming_1 error](power_programming_1.jpg)
- Completed Ultrasonic Subsystem
    - ![ultrasonic_1 error](ultrasonic_1.jpg)
- Completed first draft of routed PCB 
    - ![PCB_1 error](PCB_1.jpg)
    

---

## Week 7: [10/21-10/25]  
**Objectives for the Week**:  
- Review hardware schematic  
- Plan integration of sensors with microcontroller  

**Tasks Completed**:  
- Reviewed and updated the hardware schematic with mentor feedback  
- Planned GPIO pin connections for sensor integration  

---

## Week 8: [10/28-11/1]  
**Objectives for the Week**:  
- Finalize PCB layout design  
- Start initial software testing on ESP32  

**Tasks Completed**:  
- Finalized PCB layout design  
- Set up basic I2C communication for OLED display  

---

## Week 9: [11/4-11/8]  
**Objectives for the Week**:  
- Begin software development for sensor data collection  
- Debug initial communication between components  

**Tasks Completed**:  
- Developed basic code for ultrasonic sensor data collection  
- Debugged communication between ESP32 and MAX3421E USB chip  

---

## Week 10: [11/11-11/15]  
**Objectives for the Week**:  
- Test subsystem functionality  
- Integrate power management system  

**Tasks Completed**:  
- Tested ultrasonic sensor data acquisition  
- Integrated and tested 5V and 3.3V power systems  

---

## Week 11: [11/18-11/22]  
**Objectives for the Week**:  
- Assemble and test PCB prototype  
- Continue software debugging  

**Tasks Completed**:  
- Assembled the first prototype PCB  
- Debugged power issues with the MAX660 voltage inverter  

---

## Week 12: [11/25-11/29]  
**Objectives for the Week**:  
- Test full system integration  
- Finalize software features  

**Tasks Completed**:  
- Tested integration of all subsystems on the PCB  
- Developed additional software features for data logging  

---

## Week 13: [12/2-12/6]  
**Objectives for the Week**:  
- Optimize hardware design based on testing feedback  
- Conduct performance tests on sensors and microcontroller  

**Tasks Completed**:  
- Optimized PCB layout to reduce noise on sensor readings  
- Conducted performance tests for the ultrasonic sensor and ESP32  

---

## Week 14: [12/9-12/13]  
**Objectives for the Week**:  
- Prepare for final project presentation  
- Finalize all documentation  

**Tasks Completed**:  
- Created final project presentation slides  
- Completed and reviewed all project documentation  

---

## Final Reflection
**Project Summary**:

**Biggest Takeaways**:

**Next Steps**:

**Final Grade (Self-Assessment)**:
