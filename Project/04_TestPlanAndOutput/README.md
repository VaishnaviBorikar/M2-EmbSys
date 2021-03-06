## High-Level test plan

| Test ID | Description |  Input |  Output | Test |
|---|---|---|---|---|
| HLTP01 | Servo-motor should ON and OFF  | Power Supply | Valve ON/OFF | Implemented |
|HLTP02 | Ultrasonic sensor sense the level of water | Level of water present | Continuous Signal | Implemented |
|HLTP03 | LED should glow red/green | Signal from sensor | LED will glow | Implemented |
|HLTP04 | Voltmeter should measure the voltage | Voltage from potentiometer | Display Voltage | Implemented |

## Low-Level test plan

|Test ID | Description | Input | Output | Test |
|--------|-------------|---------|---------|---------|
|LR_01    |Servo motor valve should be open when the water is less.            |Less water level        |  Servo Motor will ON      | Implemented       |
|LR_02    | Servo motor valve should close when water is full.       | Full water level       |Servo Motor will OFF     | Implemented  |
|LR_03    |  LED should glow Red when valve is open.          | Taking input from Arduino       |   Red LED will glow    |    Implemented    |
|LR_04    |         LED should glow green when valve is closed.|     Taking input from Arduino    |    Green LED will glow    |    Implemented     |
|LR_05   |      Potentiometer should regulate the voltage properly|     5V supply  |    Voltmeter will show the reading.    |    Implemented     |
