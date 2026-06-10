# Fuzhou Metro Station Passenger Flow Simulation Model
## Simulation Design of Pedestrian and Train Operation Logic Based on AnyLogic

> Project Demo Video: [Click to Watch Video](https://drive.google.com/file/d/1GfVdwcJFdW1DahJy-TTblF2mRoxcHmjX/view?usp=drive_link)

---

## 1. Project Overview
This project takes Fuzhou University Metro Station as the simulation object. The whole-process modeling is completed on the AnyLogic platform to restore the physical layout of the station, and build complete operation logic for pedestrian flow, metro trains and escalators.

This is the final version of the model. On the basis of restoring the daily operation of the station, the passenger flow organization is optimized, and a switchable heat map function is added to quickly identify congestion levels and provide references for passenger flow guidance. Combined with field research and architectural drawings, a customized two-layer simulation model is built to conduct preliminary analysis on passenger flow behaviors and operational bottlenecks. Restricted by the positioning and design scope of the model, it cannot thoroughly solve deep problems such as transfer queuing and large-area congestion during peak hours.
1. **Project Background**
The selected station is an important passenger flow hub of Fuzhou Metro. Large crowds gather here during morning and evening rush hours, often causing transfer queues and passage congestion. It is a typical research scenario for rail transit passenger flow management.
2. **Project Objectives**
To build a simulation model that fits the actual situation and realize realistic simulation of pedestrian and train movements. By adjusting internal passage rules and streamline design, we can properly guide passenger flow and improve the overall operation of the station.

## 3. Technologies & Tool Stack
- Core Simulation Platform: **AnyLogic 8.9.8**
- Modeling Method: Multi-agent Modeling
- Auxiliary Tools: Screen recording software, video editing tools
- Data Source: Layout of Fuzhou Metro stations and regular operational rules summarized from public information

## 4. Overall Model Architecture
### 4.1 Physical Space Layout
The model fully replicates the physical areas of the target metro station, including security check areas, entry and exit fare gates, escalators, platforms and track lines.

### 4.2 Overall Operation Logic
Load spatial layout → Generate pedestrian agents and execute related behaviors → Run the logic of train arrival, stopping and departure → Display real-time operating status

### 4.3 Preset Monitoring Indicators
The model is equipped with data statistics functions to monitor indicators such as pedestrian travel time, train stopping time and platform passenger density.

## 5. Detailed Model Design
### 5.1 Pedestrian (Agent) Logic Design
1. Pedestrian Classification: Classify people by walking speed, including regular passengers and slow-moving pedestrians.
2. Basic Behavioral Rules: Realize autonomous route selection, normal walking, queuing, taking escalators or stairs and other basic actions.
3. Application Scenarios: Cover three core travel scenarios: entering the station, exiting the station and transferring within the station.

### 5.2 Train Operation Logic Design
1. Operating Rules: Set up the complete workflow of train arrival, passenger boarding and alighting, door closing and departure.
2. Time Parameters: Configure basic parameters such as regular train stopping duration and train departure intervals.
3. Linkage Logic: Connect the train stopping status with the boarding and alighting behaviors of pedestrians on the platform.

### 5.3 Scenario Settings
Current Simulation Scenario: Daily regular passenger flow scenario
Simulation Duration: Unlimited
Passenger Inflow Rate: 700 people per hour at Entrance B, 350 people per hour at Entrance A and Entrance C

## 6. Model Development Iteration
### 6.1 V1 Initial Version
1. Development Content: Completed the overall spatial layout of the metro station, including passages, fare gates, platforms and track lines. Built basic operation logic for pedestrians, trains and escalators.
2. Implemented Functions: Established the basic scene framework, restored the location and division of facilities, and ensured the normal operation of trains, escalators and pedestrians.
3. Existing Problems: The first and second floors were not integrated; there was no logic linkage between trains and pedestrians.


### 6.2 V2 Optimized Version (Current Final Version)
We upgraded the model based on V1, with core updates as follows:
1. Realized logic linkage between pedestrians and trains.
2. Added heat map function.
3. Debugged parameters to ensure smooth behaviors of pedestrians and trains, with no logical conflicts in all areas.
4. Added statistical chart for exit duration.

Current Status: The model runs stably, and pedestrians and trains operate in accordance with preset rules normally.



## 7. Simulation Operation Description & Effects
### 7.1 Operation Performance
The model can fully simulate the daily operation of the metro station. Pedestrians complete station entry, exit and transfer along designated routes, and trains arrive and depart on schedule to carry passengers. The whole system runs smoothly and all preset logic works properly.

### 7.2 Existing Problems
1. Only basic logic has been built, and targeted optimization for transfer queues and passage congestion has not been completed.
2. No comparative experiments have been carried out, so data such as congestion duration and crowd density have not been quantified.
3. Complex pedestrian behaviors such as congestion avoidance and temporary detours are not fully simulated.

### 7.3 Data Description
At present, we mainly focus on function debugging and logic verification, and no comparative data before and after optimization has been generated.

## 8. Operation Guide
### 8.1 Operating Environment
- Operating System: Windows
- Required Software: AnyLogic 8 or above

### 8.2 Operation Steps
1. Download the `.alp` project file and open it with AnyLogic.
2. Click the run button to start the simulation, and adjust the playback speed manually if needed.
3. Observe the overall status of pedestrian flow and train operation.
4. You can customize parameters such as passenger flow volume and train departure intervals. Rerun the model after modification.

### 8.3 Notes
- It is recommended to run the simulation at a low speed for easier observation of behavioral logic.
- Test step by step after modifying parameters to avoid logical errors.

## 9. Summary & Future Plans
### 9.1 Project Summary
In this phase, we have completed the core construction of the Fuzhou Metro Station simulation model, and realized three major functions: station space restoration, pedestrian behavior logic and train operation logic. The model runs stably and meets the basic simulation requirements.

The model has laid a foundation for passenger flow analysis, while optimization schemes for practical problems such as transfer queues and peak-hour congestion remain to be designed.

### 9.2 Deficiencies
1. Passenger flow diversion schemes for peak hours need to be improved.
2. The logic of multi-agent operation needs to be enriched.
3. Complex interaction between pedestrians and trains, as well as extreme passenger flow scenarios, need further improvement.
4. The function to adjust passenger flow or train schedules in real time is not available.

## 10. Team Information
Team Members: Feng Yibin, Huang Tianjing, Lin Yunlong, Pan Yueyue, Wang Yuchen, Wu Yuexian
Completion Date: June 9, 2026
