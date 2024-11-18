# iot-ti-ta-integration

Due to the size of the project, there is no drive for now: https://drive.google.com/drive/folders/1R-PCmGsQxgBLUHSn0TjFAI61nTSDnIVb?usp=sharing


⚙️ Learning Project: IoT Integration and IT/OT Connection ⚙️

I’d like to share a project I recently developed to enhance my skills in IoT and integration between IT and OT! This project involved visualizing temperature sensor variations, simulated using a potentiometer.

🔌 Overview:
The ESP32 captures data and sends it via MQTT to a broker, which logs it in the database whenever the temperature exceeds defined limits.
Applications are encapsulated in Docker, simplifying deployment.
I created a Flutter app for local system visualization and control, featuring physical and virtual LEDs to indicate temperature levels.
Additionally, I used Blynk to provide the same functionalities as the app, enabling remote access from anywhere.

🔧 Tools Used:

🐍 FastAPI + PostgreSQL + Pydantic: API to log and display date, time, and temperature records. The data is displayed on a web page generated by the ESP32, which also allows parameter configuration.

🦟 Mosquitto: Configured as the MQTT broker in the same Python script as the API to receive data from the ESP32.

🕒 FreeRTOS: Utilized to divide tasks on the ESP32, leveraging its cores for efficient and organized system operation.

🐳 Docker: Encapsulated applications for streamlined deployment and environment management.

🌐 Blynk: Used as a supervisory platform for its scalability, remote access, and ease of use.

🔄 OTA (Over The Air): Enabled firmware and parameter updates via a web interface.

📱 Flutter: Provided ESP32 parameterization and remote monitoring synchronized with Blynk.

This project offered me profound learning in essential IT, OT, and IoT concepts. It was a significant step toward exploring technologies that connect the physical and digital worlds! 🚀
