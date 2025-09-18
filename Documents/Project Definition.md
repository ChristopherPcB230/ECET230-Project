Project Definition: Bike-Powered Generator
Victor Cortes & Christopher D'Aloia
ECET 230 - 001 
9/14/2025



Table Of Contents

Table Of Contents	2
High-Level Description	3
Purpose	3
Client	4
Communication	4
Objectives	5
Scenario	5
User Interaction Stories	5
User Interface	5
User Acceptance	6
Parameters	6
Technical	6
Functions	6
Integration	6
Operational	7
Regulatory	7
Life Cycle	7
Environment	7
Starting Point	8
Key Concerns	8
Future	8
Glossary	9
Open Questions	9

High-Level Description
Name of the Project: Pedal-to-Power: Modular Bicycle Energy Harvesting System


Summary: A prototype system that converts cycling energy into usable electricity, stores it in batteries, and powers USB devices. The design can scale modularly—multiple bikes linked together to form microgeneration hubs that supply excess power to the grid.

Purpose
For the user: Provides renewable, on-demand energy while exercising, commuting, or during outages. If scaled large enough, users can sell excess power that was generated back to the grid.


Why we’re making this: To demonstrate sustainable energy harvesting, promote fitness, and explore a scalable alternative to grid power generation.



Top Usage Scenarios / User Stories:
Cyclists can charge their devices via USB.


Gym chains connect multiple bikes to offset facility energy usage.


Community micro-hubs sell surplus energy back to the grid, incentivizing participation.


Backup power source during emergencies.



Client
Contact: 
Victor Cortes    -    
Christopher D'Aloia    -    cd468@njit.edu


Roles: 
Project manager: Victor Cortes
Parts manager: Victor Cortes
Design Team: Victor Cortes & Christopher D’Aloia
Testing: Victor Cortes & Christopher D'Aloia
Electrical Engineering Lead: Christopher D'Aloia


Budget: $100


Communication

Repository: GitHub / Google Drive for schematics, code, BOM.


Logbook: Maintained digitally + hardcopy for changes, issues, milestones.




Objectives
High-level: Build a modular, pedal-powered energy harvesting prototype that stores energy in a battery and charges USB devices, with future expandability to grid-level integration.


Deliverables:
Proof-of-concept prototype (single bike).
Brochure explaining the grid-integration vision.
User demo model.


Scenario
User Interaction Stories
(INSERT)

User Interface
Displays: Small LCD or LED wattmeter showing generated power.
Buttons/Switches: On/off switch, reset button.
Indicators: Charging LED, error LED, grid-export status light.




User Acceptance
Criteria (Given-When-Then):
Given a user pedals steadily, when they generate ≥6W, then the USB port must charge a phone.
Given multiple bikes are linked, when combined power > threshold, then surplus should be export-ready.


Quantifiable Goals:
≥5V stable USB output.
≥80% energy conversion efficiency.

Parameters
Technical
Dimensions: Compact generator mount ( ≤ 24” x 30”).
Weight: Add-on module ≤15 lbs.
EMC/EMI: Must not interfere with nearby wireless devices.
Protection: Overcurrent and reverse polarity protection.


Functions
- Convert mechanical pedaling to DC electricity.
- Regulate and store energy in a rechargeable battery.
- Supply power to USB or grid (future).


Integration
Interfaces: USB, DC bus for bike-to-bike linking.
Protocols: Basic DC distribution, future smart-meter protocol.


Operational
Restrictions: Prototype for light loads (USB).
Duty Cycle: Short-to-medium term (30–90 min pedaling sessions).


Regulatory
Laws/Policies:


Consumer safety standards.


Future compliance with grid interconnection standards (IEEE 1547).



Life Cycle
Manufacturing: Simple 3D-printed mounts, off-the-shelf generator + controller.
Programming: Microcontroller for monitoring + grid sync (future).
Tracking: Energy logs stored locally or via app (future).
Service: Replaceable and interchangeable battery pack(s).
Associated Services: Community energy-sharing platform (future).





Environment
Temperature Range: 40–95°F (indoor use)
Hazards: Sweat/moisture → waterproof casing needed.
Ingress: IP-44 (dust/splash resistant).
Power: Human-powered; optional wall-charging for hybrid use.



Starting Point
Existing IP: Bicycle generator concepts, USB charging kits.
Existing Prototypes: Dynamo hubs, off-grid pedal power projects.



Key Concerns
Efficiency of conversion and storage.
Stability of modular connections.









Future
Expand prototype to multi-bike gym installations.
Develop grid-tied inverter module for power export.
Incentivize users with credit for supplying power back to grid.
Integrate with IoT dashboards for tracking and gamification.



Glossary
Microgeneration: Small-scale production of electricity.
Modular Design: System can expand by adding units.
Grid-tied: Connected and synchronized with local utility grid.
USB Output: Standard 5V DC charging.



Open Questions
How to safely synchronize multiple bikes for grid export?
What business model could sustain grid buy-back incentives?
What is the optimal battery type for modular scaling (Li-ion vs supercapacitors)?
How to ensure regulatory compliance for future commercialization?


