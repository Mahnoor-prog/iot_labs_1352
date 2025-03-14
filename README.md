This project sets up an ESP32-based web server that allows users to monitor temperature and humidity while also controlling an RGB LED through a web interface.  

### Features:  
- Connects to Wi-Fi and starts a web server.  
- Reads temperature and humidity using a DHT11 sensor.  
- Displays the sensor data on an OLED screen.  
- Provides a web page where users can enter RGB values to control an LED.  
- Continuously updates sensor readings and responds to user input.  

### How It Works:  
1. The ESP32 connects to a Wi-Fi network and starts a web server.  
2. The DHT11 sensor takes temperature and humidity readings.  
3. The OLED display updates with the latest sensor data.  
4. The web page allows users to enter RGB values, which change the LED color.  
5. The system continuously updates and processes new inputs.  

This project integrates IoT, web development, and embedded systems to create an interactive and remote-controlled monitoring system.
