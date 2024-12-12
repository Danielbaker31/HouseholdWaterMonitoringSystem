# ECE445 Senior Design Journal - Household Water Monitoring System - Daniel Baker

---

## Project Overview
**Project Name**: Household Water Monitoring System  
**Team Member(s)**: Daniel Baker (drbaker5)
**Date Started**: [9/9/24]  
**Course**: ECE445 Senior Design  

---

## Table of Contents
1. [Week 1](#week-1-99-913)
2. [Week 2](#week-2-916-920)
3. [Week 3](#week-3-923-927)
4. [Week 4](#week-4-930-104)
5. [Week 5](#week-5-107-1011)
6. [Week 6](#week-6-1014-1018)
7. [Week 7](#week-7-1021-1025)
8. [Week 8](#week-8-1028-111)
9. [Week 9](#week-9-114-118)
10. [Week 10](#week-10-1111-1115)
11. [Week 11](#week-11-1118-1122)
12. [Week 12](#week-12-1125-1129)
13. [Week 13](#week-13-122-126)
14. [Week 14](#week-14-129-1213)


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
- Submit revised project proposal  
- Finish and submit design document  

**Tasks Completed**:  
- Submitted project proposal revision  
- Completed and submitted the design document
    - Created a draft physical design
        - e.g.: ![physical_design error](physical_design.jpg)
    - Researched and finalized more specific ideas for each subsystem, and created RV tables for each
        - e.g.: ![RV error](RV.jpg)
    - Finalized flow rate formula for the ultrasonic subsystem
        - ![formula error](formula.jpg)

---

## Week 5: [10/7-10/11]  
**Objectives for the Week**:  
- Practice for Design Review  
- Start PCB  

**Tasks Completed**:  
- Practiced and completed design review presentation
    - Learned about timing challenges for flow rate, necessitating very precise time measurement ICs
        - Decided on TDC1000 and TDC7200 for time-to-digital conversion
- Started Microcontroller Subsystem for PCB
    - ![MCU error](MCU.jpg)  

---

## Week 6: [10/14-10/18]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Complete and order first draft of PCB  
- Complete teamwork evaluation 1  

**Tasks Completed**:  
- Completed Power and Programming Subsystem
    - ![power_programming_1 error](power_programming_1.jpg)
- Completed Ultrasonic Subsystem
    - ![ultrasonic_1 error](ultrasonic_1.jpg)
- Completed the first draft of routed PCB  
    - ![PCB_1 error](PCB_1.jpg)

---

## Week 7: [10/21-10/25]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Order components for the PCB first draft  

**Tasks Completed**:  
- Met with TA Pusong Li
    - Recommended a breakout board for TDC chips for breadboard testing
- Ordered parts from the ECE parts shop for the first draft of the PCB
- Submitted order to DigiKey for the first draft of the PCB
- Created a test board with breakouts for TDC1000, TDC7200, OP Amps, and Ultrasonic Sensor Headers
    - ![breakout_SCH error](breakout_SCH.jpg)
    - ![breakout_PCB error](breakout_PCB.jpg)
    - ![breakout_3D error](breakout_3D.jpg)
- Submitted and ordered breakout board for the second round of orders  

---

## Week 8: [10/28-11/1]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Solder and test PCB if it arrives  

**Tasks Completed**:  
- Met with TA Pusong Li  
- PCB arrived  
    - ![real_PCB_1 error](real_PCB_1.jpg)
- Soldered PCB 1
    - ![soldered_PCB_1 error](soldered_PCB_1.jpg)
- Worked on powering and programming PCB, but too small of a diode footprint prevented us from programming. Scrapped PCB  

---

## Week 9: [11/4-11/8]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Make revisions to PCB based on errors from last PCB and findings from the breakout board (if it arrives)  
- Complete the individual progress report  

**Tasks Completed**:  
- Met with TA Pusong Li  
- Breakout board arrived
    - Attempted to program TDC1000 and TDC7200, no luck
    - Attempted to send and receive signals to/from ultrasonic sensors  
        - Thought we had success but found oscilloscope wires were acting as antennae
- Started final PCB with revisions:
    - Added two programming methods: automatic with CP2102 USB UART bridge and manual with buttons and headers for serial connection using an external bridge
    - Removed op amps
    - Added soft and hard reset buttons
    - Added indication LEDs
    - Changed protection diodes for power and programming subsystem to larger packages for easier soldering  

---

## Week 10: [11/11-11/15]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Complete and submit final PCB  
- Continue debugging breakout board and get ultrasonic sensors to send/receive  
- Sign up for presentation and demo  

**Tasks Completed**:  
- Met with TA Pusong Li  
- Completed and submitted final PCB  
    - ![MCU_final error](MCU_final.jpg)
    - ![power_programming_final error](power_programming_final.jpg)
    - ![ultrasonic_final error](ultrasonic_final.jpg)
    - ![PCB_final error](PCB_final.jpg)
- Continued debugging sensors and TDC chips, still no luck
    - Considered alternative solutions:
        - Using DAC and ADC to skip TDCs and use the internal 80 MHz clock to measure time differences (not viable due to clock mismatch)
        - Using ultrasonic sensors from the 110 lab kit (would work but lose ultrasonic subsystem points)
- Signed up for the presentation and demo  

---

## Week 11: [11/18-11/22]  
**Objectives for the Week**:  
- Meet with TA Pusong Li  
- Continue debugging  
- Mock demo  
- Solder final PCB if it arrives  

**Tasks Completed**:  
- Met with TA Pusong Li
    - Attempted to debug sensors with other TAs, but could not get them to work
    - Decided to focus on 110 lab kit ultrasonic sensors
- Final PCB arrived and soldered just before break:
    - Soldered headers to GPIOs and wires to the voltage regulator for 5V, GND, and GPIO signals to external LCD and ultrasonic sensing module
    - ![PCB_final_soldered error](PCB_final_soldered.jpg)
- Powered the PCB but could not program  

---

## Week 12: [11/25-11/29]  
**Objectives for the Week**:  
- Eat food on Thanksgiving  
- Continue to try to program  
- Make the demo setup  

**Tasks Completed**:  
- Ate food  
- Worked on programming with no success  
- Successfully created the demo setup  
    - ![demo_bucket error](demo_bucket.jpg)  

---

## Week 13: [12/2-12/6]  
**Objectives for the Week**:  
- Meet with TA Pusong Li to try to help program  
- Get everything working (uh oh)  
- Final demo  

**Tasks Completed**:  
- Met with TA Pusong Li and resolved programming issue by cutting traces. Successfully programmed!  
- Debugged software  
- 3D printed enclosure for demo
    - ![enclosure error](enclosure.jpg)
    - ![enclosure_2 error](enclosure_2.jpg)
- Set up for the final demo  
- Completed the final demo  

---

## Week 14: [12/9-12/13]  
**Objectives for the Week**:  
- Complete slides for final presentation  
- Deliver the final presentation  
- Complete demo video for extra credit  
- Complete final paper  

**Tasks Completed**:  
- Completed slides for the final presentation  
- Delivered the final presentation  
- Completed demo video for extra credit  
- Completed the final paper  
- Celebrated with Domino's pizza  

---

