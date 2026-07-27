<h1>ExpNo 1 :Developing AI Agent with PEAS Description</h1>
<h3>Name: Samyuktha S</h3>
<h3>Register Number: 212225040363</h3>


<h3>AIM:</h3>
<br>
<p>To find the PEAS description for the given AI problem and develop an AI agent.</p>
<br>
<h3>Theory</h3>
<h3>Smart Irrigation Agent:</h3>
<p>

This agent provides irrigation to crops based on temperature and climate conditions. The agent monitors the temperature, soil moisture, humidity, and rainfall. If the temperature is high, the soil is dry, and there is no rainfall, the agent automatically turns on the irrigation system to supply water. If the soil has enough moisture or rain is detected, the agent turns off the irrigation system to conserve water. The environment consists of different agricultural field sections. The agent moves between these sections, checks the environmental conditions, and irrigates only the areas that require water. The performance of the agent is measured by minimizing water wastage, maintaining optimal soil moisture, and ensuring healthy crop growth while reducing unnecessary irrigation..</p>
<hr>
<h3>PEAS DESCRIPTION:</h3>
<table>
  <tr>
    <td><strong>Agent Type</strong></td>
    <td><strong>Performance</strong></td>
     <td><strong>Environment</strong></td>
    <td><strong>Actuators</strong></td>
    <td><strong>Sensors</strong></td>
  </tr>
    <tr>
    <td><strong>smart irrigation agent</strong></td>
    <td><strong>Efficient water usage, healthy crop growth, reduced water wastage</strong></td>
     <td><strong>Agricultural field, crops, weather conditions, climate changes</strong></td>
    <td><strong>Water pump, irrigation valves, sprinkler/drip system</strong></td>
    <td><strong>Temperature sensor, soil moisture sensor, humidity sensor, rainfall sensor</strong></td>
  </tr>
</table>
<hr>
<H3>DESIGN STEPS</H3>
<h3>STEP 1:Identifying the input:</h3>
<p>Temperature from patients, Location.</p>
<h3>STEP 2:Identifying the output:</h3>
<p>Prescribe medicine if the patient in a random has a fever.</p>
<h3>STEP 3:Developing the PEAS description:</h3>
<p>PEAS description is developed by the performance, environment, actuators, and sensors in an agent.</p>
<h3>STEP 4:Implementing the AI agent:</h3>
<p>Treat unhealthy patients in each room. And check for the unhealthy patients in random room</p>
<h3>STEP 5:</h3>
<p>Measure the performance parameters: For each treatment performance incremented, for each movement performance decremented</p>

## CODE

class SmartIrrigationAgent:

    def choose_action(self, temperature, humidity, moisture, pest):

        print("\n------ Sensor Readings ------")
        print("Temperature :", temperature, "°C")
        print("Humidity    :", humidity, "%")
        print("Soil Moisture:", moisture, "%")
        print("Pest Detected:", pest)

        print("\n------ AI Decisions ------")

        # Temperature
        if temperature >= 35:
            print("✓ High temperature detected")
            print("→ Supply MORE water")
            print("→ Add nutrients to irrigation water")

        elif temperature <= 20:
            print("✓ Low temperature detected")
            print("→ Reduce water supply")

        else:
            print("✓ Normal temperature")
            print("→ Normal irrigation")

        # Humidity
        if humidity >= 80:
            print("✓ High humidity detected")
            print("→ Less water is enough")

        elif humidity <= 40:
            print("✓ Low humidity detected")
            print("→ Increase water supply")

        # Soil Moisture
        if moisture <= 30:
            print("✓ Soil is dry")
            print("→ Turn ON water pump")

        elif moisture >= 70:
            print("✓ Soil is already wet")
            print("→ Turn OFF water pump")

        else:
            print("✓ Soil moisture is adequate")

        # Pest Detection
        if pest.lower() == "yes":
            print("✓ Pest detected")
            print("→ Spray pesticides")

        else:
            print("✓ No pests detected")

        print("-----------------------------")


print("===================================")
print(" SMART AI IRRIGATION SYSTEM ")
print("24/7 FARM MONITORING AGENT")
print("===================================")

agent = SmartIrrigationAgent()

while True:

    print("\nEnter Sensor Values")

    temperature = float(input("Temperature (°C): "))
    humidity = float(input("Humidity (%): "))
    moisture = float(input("Soil Moisture (%): "))
    pest = input("Pest Detected? (Yes/No): ")

    agent.choose_action(temperature, humidity, moisture, pest)

    choice = input("\nContinue Monitoring? (Yes/No): ")

    if choice.lower() != "yes":
        print("\nSystem Monitoring Stopped.")
        break
        

##OUTPUT

<img width="1883" height="912" alt="image" src="https://github.com/user-attachments/assets/ab8834ef-c63b-48f0-9ff2-00269b77e758" />

## result
thus the program executed successfully using irrigation management peas discription

        
