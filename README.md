<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/80cf4aa2-c45f-4a0b-bc18-0d706152188b" /># Smart India Hackathon Workshop
# Date:21-09-2025
## Register Number:25006694
## Name:Minhaj Ahamed.J
## Problem Title
SIH 25010: Smart Crop Advisory System for Small and Marginal Farmers
## Problem Description:
A majority of small and marginal farmers in India rely on traditional knowledge, local shopkeepers, or guesswork for crop selection, pest control, and fertilizer use. They lack access to personalized, real-time advisory services that account for soil type, weather conditions, and crop history. This often leads to poor yield, excessive input costs, and environmental degradation due to overuse of chemicals. Language barriers, low digital literacy, and absence of localized tools further limit their access to modern agri-tech resources.

Impact / Why this problem needs to be solved

Helping small farmers make informed decisions can significantly increase productivity, reduce costs, and improve livelihoods. It also contributes to sustainable farming practices, food security, and environmental conservation. A smart advisory solution can empower farmers with scientific insights in their native language and reduce dependency on unreliable third-party advice.

Expected Outcomes

• A multilingual, AI-based mobile app or chatbot that provides real-time, location-specific crop advisory.
• Soil health recommendations and fertilizer guidance.
• Weather-based alerts and predictive insights.
• Pest/disease detection via image uploads.
• Market price tracking.
• Voice support for low-literate users.
• Feedback and usage data collection for continuous improvement.

Relevant Stakeholders / Beneficiaries

• Small and marginal farmers
• Agricultural extension officers
• Government agriculture departments
• NGOs and cooperatives
• Agri-tech startups

Supporting Data

• 86% of Indian farmers are small or marginal (NABARD Report, 2022).
• Studies show ICT-based advisories can increase crop yield by 20–30%.

## Problem Creater's Organization:
Government of Punjab

## Theme:
Agriculture, FoodTech & Rural Development

## Proposed Solution:
Farmers face many challenges in irrigation, such as overflowing or empty tanks, pumps getting damaged due to dry runs, and pipes getting blocked or leaking. Since most of these issues are usually checked manually, it consumes a lot of time and effort. Improper irrigation also affects crop growth, either by overwatering or underwatering, which reduces yield. To solve these problems, a smart irrigation system using sensors can be introduced.

In this system, three sensors play an important role. A float sensor inside the water tank acts like a guard, indicating whether the tank is empty or full and preventing the pump from running dry or causing overflow. An ultrasonic sensor is used to measure the exact water level in the tank without touching the water, giving a clear idea of how much water is available at any time. A pressure sensor is connected to the pipeline to check the water pressure. If the pressure is too low, it means there may be a leak or the pump is not pulling water. If the pressure is too high, it indicates a blockage in the pipe.

Together, these sensors make the irrigation process automatic and safe. The pump can switch on and off automatically based on water level, and the system can stop itself if any problem is detected, preventing damage. This setup helps save water, protects pumps and pipes, reduces the farmer’s manual work, and ensures that crops receive the right amount of water, leading to better yield and efficiency in agriculture.

## Technical Approach:
The proposed solution makes use of ESP32 as the central controller, along with a float sensor, ultrasonic sensor, and pressure sensor to address common irrigation issues faced by farmers. The methodology starts with identifying the key problems such as irregular monitoring of tank water levels, pump damage due to dry running, and undetected leakages or blockages in pipelines. The system is then designed to continuously sense these parameters and automatically control the pump to ensure safe and efficient irrigation.

In the implementation process, the float sensor is placed inside the tank to act as a simple switch, indicating whether the tank is full or empty. This prevents the pump from running without water or causing overflow. The ultrasonic sensor is mounted at the top of the tank to measure the exact water level by calculating the distance between the sensor and the water surface. This data helps in knowing the percentage of water available at any time. The pressure sensor is connected to the irrigation pipeline and monitors the water pressure while the pump is running. Abnormally low pressure signals a leakage or suction issue, while very high pressure indicates blockages.

All three sensors send their readings to the ESP32, which processes the data and makes decisions. The ESP32 can automatically switch the pump ON or OFF through a relay module depending on the water level and pressure conditions. It can also send alerts to the farmer via Wi-Fi or GSM module when faults are detected, such as “tank empty,” “pump stopped due to low pressure,” or “pipeline blockage.” The system can be powered using mains electricity or a solar panel with a battery for field deployment.

This step-by-step methodology ensures that irrigation is automated and safe. The farmer does not need to check the tank and pipelines manually. Instead, the system continuously monitors the conditions, protects the pump and pipelines, and ensures crops get the right amount of water. This approach saves water, reduces labor, prevents equipment damage, and improves agricultural productivity

## Flow chart:
![block diagram](https://github.com/user-attachments/assets/2c0280cc-6aed-4ddf-a890-31d80f5677ee)



## Feasibility and Viability:
While the proposed system is practical, there are certain challenges that may arise during implementation. One major issue is the reliability of sensors. Float sensors may get stuck due to dirt or algae, ultrasonic sensors can be affected by external conditions such as foam or rainfall, and pressure sensors may provide inaccurate readings if not properly calibrated. Power supply is another concern, especially in rural areas where frequent power cuts can disrupt continuous operation. Connectivity problems may also occur if the farm is located in an area with weak Wi-Fi or GSM signals, leading to delays in sending alerts. Environmental conditions such as dust, heat, and moisture can damage electronic components if they are not properly protected. In addition, the system requires periodic maintenance, such as cleaning and calibration, which may be difficult for farmers who are not familiar with handling electronic devices.

To address these challenges, several strategies can be applied. For water level monitoring, both float and ultrasonic sensors can be used together, providing backup if one sensor fails. Protective enclosures such as waterproof and dust-proof casings can safeguard the ESP32 and other electronics from environmental damage. To ensure stable power, the system can include a solar panel and battery backup, allowing it to operate even during electricity cuts. The ESP32 can also be programmed with offline logic, so that it can continue to control the pump based on sensor readings even when internet connectivity is unavailable. Regular cleaning and calibration of sensors will help maintain accuracy, and farmers can be provided with simple guidelines for basic maintenance. Finally, starting with affordable sensors during prototyping and upgrading to industrial-grade sensors for large-scale deployment will balance both cost-effectiveness and reliability.

## Impact and Benefits:
 The proposed smart irrigation system has a direct and positive impact on farming practices. By automating water level monitoring and pump control, it reduces the dependency on manual checking, saving farmers both time and effort. The system helps prevent water wastage by avoiding overflows and ensures that pumps do not run dry, which lowers electricity consumption and maintenance costs. This contributes to better resource management, especially in areas where water scarcity is a major concern.

From an agricultural perspective, the system ensures that crops receive the right amount of water at the right time, which leads to improved plant growth and higher yields. The integration of alerts and monitoring also reduces the risk of sudden pump failures or irrigation breakdowns, giving farmers peace of mind and allowing them to focus on other farming activities. In the long term, adopting such technology supports sustainable farming by conserving water, protecting equipment, and reducing unnecessary expenses. Overall, the solution empowers farmers with a low-cost, reliable, and efficient tool that improves productivity, saves resources, and enhances the overall quality of agriculture.

## Research and References:
## Research:
The proposed system is inspired by ongoing research and real-world applications of sensor-based smart irrigation systems. Several studies highlight that the use of IoT-enabled devices and sensors in agriculture improves water efficiency, reduces labor, and increases crop productivity. Research on water management in farming confirms that improper irrigation is a major cause of reduced yield and resource wastage, and that automation can significantly reduce these issues. Sensors such as float sensors, ultrasonic sensors, and pressure sensors are already widely used in industries for monitoring liquid levels, detecting leaks, and protecting pumps. Adapting these technologies into agriculture ensures reliability and cost-effectiveness. The ESP32 microcontroller has been chosen due to its affordability, built-in Wi-Fi/Bluetooth capabilities, and compatibility with multiple sensors, making it a strong candidate for agricultural automation projects.

The literature also suggests that combining multiple sensors provides redundancy and improves system accuracy, which is important in real-world farm conditions where dust, moisture, and power cuts are common. Similar smart irrigation models have been tested in pilot projects across India and other countries, showing significant water savings and better yields. This research confirms that the proposed idea is feasible, scalable, and aligned with current trends in precision agriculture.

## Reference:
FAO — Agriculture Water Management overview
https://www.fao.org/land-water/water/water-management/agriculture-water-management/en/


