# ESP32-Radiation-Detection-Drone-Payload

Autonomous drone payload system for radiation monitoring, built using ESP32, Geiger counter, GPS, SD card logging, and real-time Wi-Fi data transmission.

## Subsystems Included
- [ESP32 code (.ino)](./ESP32_code.ino): Microcontroller code for interfacing Geiger counter, GPS module, SD card, and Wi-Fi.<br>
- [Live Processing (.m)](./live_processing.m): MATLAB scripts for real-time data acquisition via ESP32 Wi-Fi.<br>
- [Post Processing (.m)](./post_processing.m): MATLAB scripts for analyzing logged CSV data to generate radiation heatmaps.<br>
- [Final Project Report (.pdf)](./Project_Phase_III_Report.pdf): Full Phase III Systems Engineering report (Toronto Metropolitan University - Fall 2024).<br>

## Technologies Used
- **Microcontroller**: ESP32
- **Software**: Arduino IDE, MATLAB
- **Sensors**: Geiger-Müller counter, GPS (ATGM336H)
- **Storage**: SD Card (SPI interface)

## Features
- Real-time Wi-Fi streaming of radiation and GPS data
- Redundant SD card logging for post-flight data recovery
- MATLAB visualization of radiation intensity over geolocation
- Lightweight and low-cost design (under 300g and $50)

## Payload

The payload casing is designed to house the ESP32 microcontroller, Geiger–Müller counter, GPS module, SD card, battery, and internal wiring. 
It features a rotate-to-lock attachment mechanism, allowing quick and secure installation or removal from the drone. It was entirely 3D printed.

 ![Payload_Casing](Images_and_Plots/payload_casing.png)  
*Payload Casing and Attachment*

 ![Payload_Assembley](Images_and_Plots/payload_assembley.png)  
*Payload CAD Assembley View*

## Results / Testing

The results of the testing was highly successful. Not only was the payload able to accurately detect and measure radiation, but it was also able to livestream the live-
radiation data, along with its geographical positioning over a Wi-Fi connection, as it was being flown attached to the drone. All the important data was successively 
transmitted to the ground-station as it was being gathered. Below are some figures of these results.

 ![Radiation Map](Images_and_Plots/radiation_map.png)  
*Radiation Map of Drone Test Flight around school campus*

 ![Cs-137 Radiation Test](Images_and_Plots/radiation_test.png)  
*Radiation Detection and Measurement Test of Payload using Cs-137*

## Authors
- Elliott Arpino  
- Khadeeja Azizi  
- Maia Elizabeth Gorham  
- Abigail Marsella  
- Fadia Matti

## License
This project is for educational use and research demonstration only.
