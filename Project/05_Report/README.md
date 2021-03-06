## Water Supply Control
- water tank overflow is a common problem which leads to the wastage of water. A circuit which will detect the water level and will glow a led upon getting the water tank full or a preset level. Water level indicator is a modern way of measuring the water level using latest technologies like sensors,arduino.The main aim of the project is to calculate the water level at any instant of time. We use arduino and ultrasonic sensor to make it possible. This may be useful to conserve water and helps us.

### Requirements
- High-Level Requirements
| ID | Description |
  |---|---|
  |HLR01| Servo Motor Should ON/OFF |
  |HLR02 | Ultrasonic Sensor should sense the level of water |
  |HLR03 | LED should glow RED/GREEN |
  |HLR04 | Voltmeter should measure the voltage |
  
 - Low-Level Requirements
   | ID | Description |
    |---|---|
    |LLR01| Servo motor valve should be open when the water is less |
    |LLR02 | Servo motor valve should close when water is full |
    |LLR03 | LED should glow Red when valve is open |
    |LLR04 | LED should glow green when valve is closed |
    |LLR05 | Potentiometer should regulate the voltage properly |
  
### Block Diagram
![water supply control](https://user-images.githubusercontent.com/98817420/155746157-e282c0cd-1574-42bb-8356-e648e0c306d2.png)
#### Arduino
- Arduino UNO is a low-cost, flexible, and easy-to-use programmable open-source microcontroller board that can be integrated into a variety of electronic projects. This board can be interfaced with other Arduino boards ,and can control relays, LEDs, servos, and motors as an output.
#### Servo Motor
- The function of the servo motor is to convert the control signal of the controller into the rotational angular displacement or angular velocity of the motor output shaft. Servo motor is used to drive the joints.
#### Ultrasonic Sensor (HC-SR01)
- To determine the distance to the water, it transmits a sound pulse that reflects from the surface of the water and measures the time it takes for the echo to return. To automatically control open and close the water gate, we use Ultrasonic sensors as input values
#### Potentiometer
- The mechanical system of sensor is destined to convert linearly the value of potentiometer resistance to the water level variation. The signal conditioning consists of analog and digital system especially microcontroller circuit.
#### Voltmeter
- Voltmeters can also be used to measure DC voltage as well as sinusoidal AC voltages but the introduction of a voltmeter as a measuring instrument into a circuit can interfere with its steady state conditions.
#### LED
-  LED is a semiconductor device used in many electronic devices, mostly used for indication purposes. It is used widely as indicator during test for checking the validity of results at different stages.It is very cheap and easily available in variety of shape, color and size. The LEDs are also used in designing of message display boards and traffic control signal lights etc.

### SWOT Analysis
![SWOT_WATER](https://user-images.githubusercontent.com/98817420/157003795-3924ef1f-5616-44f6-ad7e-c627c219cac9.jpg)

### 4W's and 1H
#### Who
- Anyone, this system can be used for industrial and domestic purpose.
#### What
- This system will turn ON/OFF the motor depending upon the level of water in the tank.
#### When
- Depending upon the water level it will turn ON/OFF the motor.
#### Where
- In industries as well as for domestic purpose.
#### How
- System controls the motor depending upon the water level in the tank.

### Applications
- Can be used in water tanks to control water levels.
- Automatically turn ON/OFF pumps.
- Can be used in factories, commercial complexes, apartments, home.
- Oil tank level control.
- Pool water level control.

### Simulation
![water_1](https://user-images.githubusercontent.com/98817420/157006791-64a12912-f4cf-4ed1-88b8-61314967d558.png)
![water_3](https://user-images.githubusercontent.com/98817420/157179565-56b2ac42-110d-473f-abdc-ed737d3da17a.png)

### Test Plan
#### High-Level test plan

| Test ID | Description |  Input |  Output | Test |
|---|---|---|---|---|
| HLTP01 | Servo-motor should ON and OFF  | Power Supply | Valve ON/OFF | Implemented |
|HLTP02 | Ultrasonic sensor sense the level of water | Level of water present | Continuous Signal | Implemented |
|HLTP03 | LED should glow red/green | Signal from sensor | LED will glow | Implemented |
|HLTP04 | Voltmeter should measure the voltage | Voltage from potentiometer | Display Voltage | Implemented |

#### Low-Level test plan

|Test ID | Description | Input | Output | Test |
|--------|-------------|---------|---------|---------|
|LR_01    |Servo motor valve should be open when the water is less.            |Less water level        |  Servo Motor will ON      | Implemented       |
|LR_02    | Servo motor valve should close when water is full.       | Full water level       |Servo Motor will OFF     | Implemented  |
|LR_03    |  LED should glow Red when valve is open.          | Taking input from Arduino       |   Red LED will glow    |    Implemented    |
|LR_04    |         LED should glow green when valve is closed.|     Taking input from Arduino    |    Green LED will glow    |    Implemented     |
|LR_05   |      Potentiometer should regulate the voltage properly|     5V supply  |    Voltmeter will show the reading.    |    Implemented     |
