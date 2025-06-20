# Smart Pharmacy 


## Introduction and state the problem:-
The smart pharmacy mainly provides accurate medication dispensing, reduces waiting times, the absence of medication errors, and an increased number of drugs dispensed daily. Nowadays, Hospitals and health institutions have been working on that by adopting specialized automation software.
This digital transformation contributed to changing advanced pharmacy management systems that are based on big data technologies, artificial intelligence, and cloud computing.
The smart pharmacy reflects the role of technology in medication dispensing without human intervention and without any errors. Also, it has achieved outstanding outcomes in terms of raising the level of effectiveness and operations efficiency, reducing the waiting time of patients to receive the service, and establishing a more efficient stock management while reducing medical errors using barcodes and keeping medicines in the best condition.

## Project description:-
Medications are dispensed in the smart pharmacy by a robot that picks up the medication and prints a label with patient and prescription information, then delivers it to the pharmacist’s window in a few seconds. The robotic pharmacy is also concerned with using advanced technological techniques through the design and operation of specialized software and the application of robots in pharmacies, as well as the computer systems necessary to manage them.    

![System Diagram](images/fig1.PNG)

Figure 1 shows an example of smart pharmacy.

The robot works with great capabilities and high technologies without any possibility of error, and therefore the smart pharmacy is the solution to protect the patient from medication dispensing errors. Not only that, the automation of work in the pharmacy has contributed to enhancing the effectiveness of operations using barcodes and artificial intelligence, in identifying the drug package through its dimensions as a tool to reduce medical errors, in addition to designing control and follow-up points and integrating them into the system to ensure the quality and continuity of service, such as monitoring the validity of medicines, and alerting when Near expiry dates, monitoring drug availability and near-expiration alerts, automating inventory and inventory management. 
Figure 2 shows the simple prototype which we are working on it.

![System Diagram](images/fig2.PNG)

Figure 2, Prototype


## Technical Aspect:-
The system is a two-axis system with a motor on each axis to support the movement. The motors which will be used are stepper motors if transistor output PLC (Programmable Logic Controller) that supports PTO (Pulse Train Out) signals is used. Otherwise, two dc motors will be used. A small motor will also be used for getting the medicine from its specified room. There will be 25 rooms for medicine in the prototype, each will have a specific number of medicines as a sample of the real project if it is applied. The whole system will have a SCADA (Supervisory Control And Data Acquisition) system to connect and collect data from and to outer resources and to simulate and show the necessary data to the user. The software that will be used for this is Ignition for easy connection between the PLC, Node-RED, databases, and finally the Arduino used in the system. The pharmacy will have its own database that will be written using MySQL language and that will contain the entities necessary for the system, such as the medicines, the admins and the users. It will contain the whole data for the medicine like the name, the date and the active substance of the medication. This database connection with SCADA will be done using a tool in the Ignition gateway. The PLC will also be connected to the database through Ignition. As said earlier in the description, the prescription that is written by the doctor will contain a barcode that will contain all the information about the medicines in that prescription. This barcode will be scanned using a camera module (in real project) or the mobile camera (in the prototype) and the camera module will be connected to the Node-RED to fetch the data in the prescription. The Node-RED then will be connected to the PLC using OPC-UA (Open Platform Communications United Architecture) protocol with the PLC is made as a client to receive the data in tags and then processing them through the code written to move the motors at the desired destination. After any process is done, tags related to the database will change according to the process and then these tags will be sent to the database through Ignition as described before. Finally, there will be an application for user-online use.Figure 3 shows an overview of the system.

![System Diagram](images/fig3.PNG)

Figure 3, Overview of the system


## Demo Video
▶ Watch Smart Pharmacy in Action

https://drive.google.com/file/d/1rrsA136CVRaQW-kxBiiirnZwwVgQCtyl/view?usp=drive_link



