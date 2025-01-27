A comprehensive IoT-based weather monitoring system that combines Arduino hardware with a web interface to track and display environmental conditions in real-time.

Hardware Components
Arduino UNO R3 (Main controller)
DHT11 Temperature & Humidity Sensor
MQ135 Gas Sensor (Air Quality)
BMP180 Barometric Pressure Sensor
ESP8266 Wi-Fi Module
Breadboard and connecting wires

Hardware Setup
The system uses the following pin connections:

DHT11 Temperature & Humidity Sensor:

VCC to 5V
GND to Ground
Data to Digital Pin

MQ135 Gas Sensor:

VCC to 5V
GND to Ground
Analog output to A0

BMP180 Barometric Pressure Sensor:

VCC to 5V
GND to Ground
SDA/SCL to Arduino I2C pins

ESP8266 Wi-Fi Module:

VCC to 3.3V
GND to Ground
RX/TX for serial communication

Features
1. Temperature Monitoring

Primary display in Celsius (°C)
Automatic conversion to:

Kelvin (K)
Fahrenheit (°F)

Temperature status indicators:

Unearthly Cold (-46°C or lower)
Extremely Cold (-45°C to -31°C)
Severe Cold (-30°C to -16°C)
Cold (-15°C to 5°C)
Moderate (6°C to 15°C)
Warm (16°C to 30°C)
Hot (31°C to 40°C)
Severe Hot (41°C to 60°C)
Extreme Heat (61°C to 80°C)
Unearthly Heat (81°C to 100°C)

2. Humidity Monitoring

Display in percentage (%)
Status classifications:

Dry (0-39%)
Optimum (40-60%)
Moist (>60%)

Health impact analysis chart showing effects on:

Bacteria growth
Virus survival
Fungi development
Mites
Respiratory infections
Allergic reactions
Chemical interactions
Ozone production

3. Air Quality Monitoring

Primary measurement in PPM (Parts Per Million)
Secondary conversion to PPB (Parts Per Billion)
Real-time air quality status updates

4. Barometric Pressure

Measurement in kPa (kilopascals)
Continuous pressure trend monitoring

Main Overview Panel:

Four main measurement cards showing current readings
Clear icons for each environmental parameter
Real-time value updates

Detailed Analysis Pages:

Individual pages for each parameter
Historical trend graphs
Unit conversions
Status indicators with color coding
Reference charts and guidelines

Graph Features:

Dynamic updating
Time-based tracking
ThingSpeak integration
Customizable timeframes

Technical Specifications

Operating Temperature: -46°C to 100°C
Humidity Range: 0-100%
Pressure Range: Atmospheric
Air Quality Resolution: 1 PPM
Update Frequency: 15 seconds
Data Storage: ThingSpeak Cloud Platform

Installation
Hardware Assembly:

Connect sensors according to the circuit diagram
Verify power connections
Check communication pins

Software Setup:

Install required Arduino libraries
Configure Wi-Fi credentials
Set up ThingSpeak integration
Deploy web interface files

Usage

Power up the Arduino system
Connect to the local network
Access the web interface
Monitor real-time environmental data
View detailed analysis by clicking on individual parameters

Dependencies

Arduino IDE
ThingSpeak account
Web browser with JavaScript enabled
Internet connection
