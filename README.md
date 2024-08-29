# LabVIEW-DHT22-SubVI-StateMachine

In this extended LabVIEW-DHT22 project, I’ve introduced two key enhancements: the use of SubVIs and the State Machine architecture in LabVIEW.

**Key Enhancements:**

**1.	SubVIs:**

**o	Purpose:** SubVIs make it possible to encapsulate specific blocks of code into reusable modules. This modular approach makes the main VI (Virtual Instrument) more organized and manageable.

**o	Application:** I’ve wrapped the DHT11 or DHT22 sensor acquisition code into a SubVI named; DHT11_Sensor. This means that instead of cluttering the main VI with detailed code, I can call this SubVI wherever the sensor data is needed, making the overall program more readable and easier to debug.

**2.	State Machine Architecture:**

**o	Purpose:** The State Machine is a powerful programming structure in LabVIEW that allows for more dynamic and flexible code execution. It enables a program to transition between different states based on conditions or user inputs, improving code reusability and maintainability.

**o	Application:** I’ve employed a State Machine to handle the flow of the program. The states involve: Initialize DAQ Devices, Start, DTH11, and Stop. The flexibility of the State Machine allows you to easily modify or extend the program’s functionality without rewriting large sections of code.

**How These Enhancements Improve the Project:**

•	**Modularity:** By using SubVIs, the project is broken down into manageable, reusable components, making the codebase cleaner and more organized.

•	**Flexibility and Maintainability**: The State Machine architecture simplifies the addition of new features and improves the program’s robustness by making it easier to handle different states and transitions.

**Hardware Setup:**
•	The hardware setup remains unchanged from the original project, where you connect the DHT11/DHT22 sensor to the Arduino and link the Arduino to the computer via USB.
These improvements make the project more scalable and maintainable, providing a solid foundation for future enhancements or for adapting the project to new requirements.
