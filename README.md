# Environmental Monitoring for Climate Resilience

## Project Overview

This project demonstrates the use of overloaded subprograms in Python to develop a tool for monitoring environmental parameters that contribute to climate resilience. The tool monitors three key variables: temperature, humidity, and soil moisture. It provides warnings when these parameters fall outside of acceptable ranges.

## Objectives

- To create a command-line tool that can assess environmental conditions.
- To utilize overloaded subprograms for flexible monitoring of different parameters.

## Features

- Monitors temperature, humidity, and soil moisture.
- Provides warnings for high temperature, low humidity, and low soil moisture.

Introduction :
            In an era where climate change significantly impacts our environment, developing tools that enhance climate resilience has become paramount. This report outlines a prototype submission designed to utilize overloaded subprograms in programming to create an effective environmental monitoring system. By focusing on parameters such as temperature, humidity, and soil moisture, we aim to provide a robust solution for monitoring environmental conditions that can affect agriculture, urban planning, and natural resource management.
Objectives

The primary objectives of this micro project are:
                                                To develop a user-friendly environmental monitoring tool that allows users to input various environmental parameters and receive real-time feedback.
                                                To implement overloaded subprograms that streamline the monitoring process, making the tool adaptable to different types of environmental data.
                                                To enhance climate resilience by providing stakeholders with valuable data that can inform decision-making and action plans.

Methodology :
1. Overloaded Subprograms
Overloaded subprograms, or method overloading, allow functions to have the same name but different parameters. This feature enhances code readability and usability. In our prototype, we developed a class called EnvironmentalMonitor, which includes overloaded methods for monitoring different environmental parameters. Each method is tailored to handle specific types of data, providing relevant feedback based on the input values.

2. Environmental Parameters
The prototype focuses on three key environmental parameters:
Temperature: High temperatures can lead to heat stress in crops and affect livestock health. Our system monitors temperature and raises warnings when thresholds are exceeded.
Humidity: Low humidity levels can lead to drought conditions, while high humidity can foster plant diseases. The tool assesses humidity levels and provides alerts when necessary.
Soil Moisture: Essential for healthy plant growth, soil moisture is critical for agricultural productivity. Our system monitors soil moisture and warns users of low levels.

3. Prototype Development
Using Python, we created the EnvironmentalMonitor class that includes methods for monitoring each of the three parameters. The user can input values through a simple command-line interface. The program processes the input and calls the appropriate overloaded method, which then provides feedback to the user.
Here is a simplified code snippet of the prototype:
python


class EnvironmentalMonitor:
    def monitor(self, temperature=None, humidity=None, soil_moisture=None):
        if temperature is not None:
            self.monitor_temperature(temperature)
        if humidity is not None:
            self.monitor_humidity(humidity)
        if soil_moisture is not None:
            self.monitor_soil_moisture(soil_moisture)

    def monitor_temperature(self, temperature):
        print(f"Monitoring temperature: {temperature}°C")
        if temperature > 35:
            print("Warning: High temperature detected!")

    def monitor_humidity(self, humidity):
        print(f"Monitoring humidity: {humidity}%")
        if humidity < 20:
            print("Warning: Low humidity detected!")

    def monitor_soil_moisture(self, soil_moisture):
        print(f"Monitoring soil moisture: {soil_moisture}%")
        if soil_moisture < 30:
            print("Warning: Low soil moisture detected!")

    def get_user_input(self):
        # Code to get user input...

4. Testing and Results

The prototype was tested under various simulated conditions to evaluate its functionality. Users were prompted to input environmental data, and the system successfully monitored and provided warnings when thresholds were exceeded. Feedback indicated that users found the interface intuitive and appreciated the immediate alerts that could help them take timely actions.

Conclusion
The prototype developed through this micro project demonstrates the potential of utilizing overloaded subprograms to create an effective environmental monitoring system. By focusing on critical parameters that influence climate resilience, we contribute to enhancing decision-making processes for stakeholders involved in agriculture, urban development, and natural resource management. The next steps involve refining the tool and exploring integrations that can further bolster its capabilities in the fight against climate change.
