# Automated-Interactive-Campus-Cleaning-Robot
AICCR (Automated Interactive Campus Cleaning Robot) is an autonomous service robot that detects and sweeps debris from campus pathways. It combines smart navigation and motorized brushes with a touchscreen, voice interaction, and campus AI to help students and staff find places and access campus information.
-------------------------------------------------------------------------------------------------------------------------------
<img width="6000" height="4000" alt="DSC09080" src="https://github.com/user-attachments/assets/8bf7d789-a59e-4a0b-9bfe-d33972d3461a" />


<img width="6000" height="4000" alt="DSC09079" src="https://github.com/user-attachments/assets/c84c0e38-3fd7-445f-b278-b3b271d11584" />
<img width="6000" height="4000" alt="DSC09071" src="https://github.com/user-attachments/assets/0816162e-ba98-4e20-98bd-0207a6818e39" />


https://github.com/user-attachments/assets/27ed798f-1ab9-46e8-9268-d031ac257b2b

<img width="1280" height="960" alt="pic" src="https://github.com/user-attachments/assets/05eff735-ff9f-47ed-867c-e6802d4253b3" />
<img width="960" height="1280" alt="1" src="https://github.com/user-attachments/assets/25b77164-0462-4a80-9bc4-06d9e88a3f9d" />
<img width="960" height="1280" alt="3" src="https://github.com/user-attachments/assets/f51f40fb-972d-4d8d-96d0-bc469717ade7" />


https://github.com/user-attachments/assets/a5d6d6d6-3dee-4c07-8349-461972d18fc7


Automated Interactive Campus Cleaning Robot
The Automated Interactive Campus Cleaning Robot is a four-wheel-drive autonomous platform designed to clean campus pathways while providing information and assistance to students, staff, and visitors. It combines a Raspberry Pi 4, a camera module, ultrasonic sensors, and a 360-degree 2D LiDAR sensor with a multi-motor cleaning system. The robot’s electrical and embedded systems coordinate movement, obstacle detection, debris detection, brush operation, and user interaction.
Electrical power system
The robot is powered by a custom-built 12 V, 100 Ah, 4S LiFePO₄ battery pack. A Daly 100 A BMS manages and protects the battery pack within its configured operating limits. The battery supplies the robot’s electrical system through separate power branches for the motors and the lower-voltage electronics.

The high-current motor branch supplies the drive and cleaning motor systems. Relay modules switch power to the motor drivers, allowing the motor-driver supply to be turned on or off as required. The drive motors are controlled through SmartElex 15S motor drivers, which connect the robot’s control system to the four automotive wiper motors on the chassis. The roller brush and two side brushes each have their own motor channel, so the cleaning components can be operated independently.

A separate power branch uses a buck converter to step the battery voltage down to a regulated 5 V, 10 A supply. This 5 V rail powers the Raspberry Pi 4, sensors, and other devices designed to operate at 5 V. Keeping the motor supply and regulated electronics supply on separate branches helps the control computer and sensors receive a steady low-voltage supply while the motors draw the current needed for movement and cleaning.
Drive and cleaning system
The robot’s four automotive wiper motors provide drive power to its four-wheel-drive chassis. Motor drivers receive control commands from the Raspberry Pi and deliver the required power to the motors. This lets the embedded software control the robot’s movement and navigation through the campus.

The cleaning assembly has a central roller brush and two side brushes. The side brushes sweep debris inward toward the roller brush, helping collect material from a wider area. Each brush is driven independently, so the robot can control the brushes separately from the wheel motors. A brush-lifting mechanism raises and lowers the brushes as needed. Raising them when they are not required helps reduce unnecessary contact with the ground and limits brush wear.
Embedded control, sensing, and interaction
The Raspberry Pi 4 acts as the robot’s main embedded computer. Its software coordinates sensor readings, navigation decisions, motor commands, cleaning operations, and user-interface updates. The camera module detects debris, while the ultrasonic sensors measure nearby obstacles. The 360-degree 2D LiDAR scans the surrounding area to support mapping and autonomous navigation.

Based on the sensor data and navigation decisions, the software sends commands to the motor drivers and brush-control channels. It also monitors the robot’s operating state and presents cleaning and battery information on a 12-inch touchscreen. A microphone and speaker system allow users to interact with the robot by voice. The integrated small AI model can provide campus navigation guidance and answer questions about teachers, board members, important campus locations, and other relevant campus information.

The robot therefore combines autonomous cleaning with an interactive campus-assistance system. Renewable-energy integration is also being developed as a future addition to the power system.




