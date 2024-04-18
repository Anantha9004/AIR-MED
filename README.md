# AIR-MED

*In India approximately, 24,012 people die every day because of delays in getting medical assistance on time* - 2023 HSTP : Health Systems Transformation Platform Article.

This project tackles a critical challenge in emergency medicine: the race against time to save lives. With a staggering number of accidents happening worldwide, prompt medical attention is the ultimate difference between life and death.

Enter the innovative concept of the AIR-MED – a life-saving UAV (Unmanned Aerial Vehicle) designed to deliver immediate and face-to-face aid from medical experts directly to accident victims.

Traditional ambulances face limitations on the road. Traffic congestion and poor road conditions can significantly delay their arrival, jeopardizing the well-being of the injured and even cause fatality. VTOL (Vertical Take Off and Landing), however, bypasses these obstacles. Their agility and speed allow them to reach accident locations much faster, providing a crucial head start in critical situations.

AIR-MED proposes a versatile VTOL system capable of carrying medical supplies. Imagine a scenario where a victim requires immediate first aid. The medical module, equipped with a first-aid kit, can be dispatched instantly.

The AIR-MED can play a vital role by flying directly to the accident location, it can land near the victim, allowing medical personnel or bystanders to access the crucial medical supplies on board. This significantly reduces the time it takes to deliver these supplies, expediting treatment.

The impact of this technology extends beyond accident scenes. It has the potential to revolutionize emergency response in remote areas or disaster zones where traditional vehicles may struggle to access victims. By overcoming geographical barriers, AIR-MED can ensure timely medical intervention in even the most challenging situations.

The core technology behind this project lies in Vertical Take-off and Landing (VTOL) aircraft. These have the unique ability to take off and land vertically, eliminating the need for a runway. This frees them from the constraints of traditional airports, making them ideal for urban environments and confined spaces. Advancements in VTOL design and technology are constantly improving, making them a popular choice for diverse applications like emergency response, and even transportation.

## Team Members
- Flemin K Sony
- Jerrin Mathew
- Anantha Krishnan K P
- Deva Prakash

## How does it work?

The video showcases the project's real-time operation. The VTOL aircraft, equipped with VTOL functionality, carries a medical module attached to its undercarriage. Upon receiving an emergency notification, sent by a victim bystander of an accident via a user-friendly website, the VTOL transports the medical module to the patient's location. The website prompts the victim bystander to enter basic patient condition data and the GPS location of the victim.

Because of its VTOL capabilities, the aircraft utilizes four motors for vertical takeoff even in confined spaces. Once airborne, the propeller spins for efficient and high-speed flight, while the vertical take-off motors shut down.

After reaching the patient, the VTOL lands in close proximity, enabling the medical module to establish a connection with a doctor with the help of a bystander. The module is equipped with various sensors that transmit real-time vital signs data to the doctor through a live website interface. Additionally, the medical module includes a video call feature, facilitating face-to-face consultations and aiding the doctor in visually assessing the patient's condition. The doctor can illuminate a suitable medicine compartment available in the medical module. The medical compartment contains WHO-recommended emergency medicines.

## Libraries Used
- WiFi.h
- BlynkSimpleEsp32.h
- Wire.h
- I2S.h
- MAX30105.h
- heartRate.h
- esp_camera.h
- Adafruit_NeoPixel.h

## How to configure

1. Initializing and powering all the devices through the battery.
2. Checking the equipment and sensors are in working condition.
3. Calibrating the IMU (Inertial Measurement Unit) sensor.
4. Flash the firmware of the SpeedyBee in Mission planner program.
5. In the case of Mission Planner not working, the Code is directly injected into the STM32 chip with STM32CubeProgrammer.
6. Check the connectivity of AIRMED website.

## How to Run?

When an Emergency case occurs:
1. The bystander will open the user-friendly AIR-MED website and select the patient interface, and send the current location of the incident.
2. The VTOL AirCraft will get initialized and is navigated and lands in the patient's location with the help of the FPV Camera module.
3. The doctor will be able to see the medical module details. Then the video call feature gets started.
4. Vital monitoring is checked by the easy wearable devices which contain sensors for measuring, HeartRate, BP, SP02 and Breath Analysis, through the instruction of the doctor with the help of the bystander.
5. The doctor will get the live sensor data and analyze the current status of the patient though the doctor's interface.
6. Doctors can choose a suitable medicine which is available in the medical module, and the chosen medicines compartment will light-up using LED to indicate the corresponding medicine.
7. The Bystander can give further medical support through the instruction received from the doctor.
