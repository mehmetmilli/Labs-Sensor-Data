# Labs-Sensor-Data
Sensor data obtained in the laboratory environments
Relevant Paper:
The Design and Implementation of a Semantic-Based Proactive System for Raw Sensor Data: A Case Study for Laboratory Environments (not published yet)



sensor data collected in the
Scientific Industrial and Technological Research and Application (SITARC)
within the Bolu Abant Izzet Baysal University (BAIBU). Data collection was
carried out in 3 laboratories frequently used in BETUM. These laboratories
are MaldiTof, AoxMercury, and Chromatography laboratories. In these labora-
tories selected as Use Cases, microorganism identication, proteomic analysis,
bacteria count, fatty acid analysis, anion-cation determination, total halogen
determination, solid-phase extraction, etc. analyzes are done frequently.


The data collection process was started on 29.08.2019
The data collection process has been terminated on 12.10.2019
The measurement duration is totally 45 days.


Important Note: The data have float types values and in the Turkish system comma (,) represents floating numbers.



Data Set Features


FOI -> is the measurement environment (Labs) (There are three different environments: 1. MaldiTof, 2. AoxMercury, and 3. Chromatography

Platform -> shows which system (nodes) the measured value comes from.
	 -> There are 4 types of node in order to sense different feature and different environment
	 -> TYPE A Nodes --> 11, 41
	    TYPE B Nodes --> 12, 22, 32, 42, 52, 62, 72
	    TYPE C Nodes --> 13, 23, 33, 43, 53, 63, 73
	    TYPE D Nodes --> 34, 44

Property -> indicates which feature the nodes are measuring.
         -> There are 8 different fetures to measure (CO2 , TVOC, CO, PM2.5, PM10, Temperature, Humidity, Light)

Sensor 	 -> is the sensor name. There are five different sensor to measure 8 different feature.
	 -> Sensor names are (NovaSDS011, CCS811, DHT22, LDR, MQ7)

Result	 -> shows the hourly average for the measured value in an environment by the related sensor.

Date	 -> shows the time the measurement was made (actually it is the previous hour range)

Stimulus -> same as the property

Unit	 -> refers the unit of the measured value
