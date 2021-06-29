Sensor Data Obtained in The Laboratory Environments

Relevant Paper:
		The Design and Implementation of a Semantic-Based Proactive System for Raw Sensor Data: A Case Study for Laboratory Environments (not published 		yet)

Environments:
		Sensor data collected in the Scientific Industrial and Technological Research and Application (SITARC) within the Bolu Abant Izzet Baysal 			University (BAIBU). Data collection was carried out in 3 laboratories frequently used in BETUM. These laboratories are MaldiTof, AoxMercury, and 		 Chromatography laboratories. In these laborataries selected as use cases, microorganism identication, proteomic analysis, bacteria count, fatty 		 acid analysis, anion-cation determination, total halogen determination, solid-phase extraction, etc. analyzes are done frequently.

Duation:
		The data collection process was started on 29.08.2019-16:00 The data collection process has been terminated on 12.10.2019-15:00The measurement 			duration is totally 45 days.

Notes
Important Note 1: 
		The data have float types values and in the Turkish system comma (,) represents floating numbers.
		
Important Note 2:
		The collected data is presented to data consumers in 2 different formats to expand the range of uses. In the first format, it is structured in an 		  ontological framework as used in the original work. In the second format, the collected data is presented as an excel sheet.
		
Important Note 3:
		Some of the important expressions in the Ontological Sensor Dataset are explained below. For more detailed information, see (Haller, Janowicz, Cox, 		    Lefrançois, & Taylor, 2018; Haller, Janowicz, Cox, Lefrançois, Taylor, et al., 2018; World Wide Web Consortium, n.d.).



Data Set Features

Observation -> 
		Shows the characteristics (Result, Date, Time, etc.) of a measurement associated with a FeatureOfInterest. A unique id is defined for each 			measurement value in the data file.
		
FeatureOfInteres ->
		is the measurement environment (Labs) ın this proposed study there are three different FeatureOfInteres. These are 1. MaldiTof, 2. AoxMercury, and 		   3. Chromatography.
		
Platform -> 
		shows which system (nodes) the measured value comes from. It hosts sensors, actuators, and other electronic devices In this study,  4 types of node 		    are used in order to observe different feature in different environment. These platforms are following;
		
1)	TYPE A Nodes --> SN_11 
2)	TYPE B Nodes --> SN_12, SN_22, SN_32
3)	TYPE C Nodes --> SN_13, SN_23, SN_33
4)	TYPE D Nodes --> SN_34

Property -> 
	indicates which feature the nodes are measuring. In this study, 8 different environmental parameters were measured. These parameters are CO2, TVOC, 	 	 CO, PM2.5, PM10, Temperature, Humidity, Light.
	
Sensor ->
	are the systems that perform the measurements. In this study, five different sensors are used to measure 8 different features. These sensors are Nova 		SDS011, CCS811, DHT22, LDR, MQ7.
	
Result ->
	shows the hourly average for the observation value in FeatureOfInterest by the related sensor.
	
Date ->
	shows the time the measurement was made (actually it is the previous hour range). For example, data labeled 17:00 actually shows the average value of that 	   parameter between 16:00 and 16:59.
	
Stimulus ->
	shows events that trigger the sensor. It is events, not objects or concepts, that trigger the sensor in the real world. For example, it is not the presence   	    of the feature of interest that triggers a sensor, but the change in the intensity or value of the feature in the environment.
	
MeasurementUnit ->
		The ‘MeasurementUnit’ class was created to avoid unit complexity at the proposed ontology. This class is not included in the core SOSA/SSN ontology 		    This class specifies the unit of the ‘sosa:hasSimpleResult’ value of the individuals of the measured ’sosa:Observation’ class. Within the scope of 		       the proposed project, the units of the parameters measured in laboratories were added as individuals of the ’MeasurementUnit’ class. Parts per 			million (ppm) was used as the unit of measurement for PM2.5, PM10, CO2, and CO. While Celsius was used as the measurement unit for temperature, 		parts per billion (ppb) was used as the measurement unit for TVOC. Finally, percent was used as the unit of measurement light and humidity. If 			other units will be used in different projects, it is enough to add them to the ’MeasurementUnit’ class. For example, if the temperature is to be 		  measured in Kelvin, it should be added to the ‘MeasurementUnit’ class of the Kelvin unit. Thus, it is considered that there will be no unit 			confusion between the values to be measured in different projects to be managed under the same framework. Since ‘MeasurementUnit’ is the unit of 		the observed property, ’hasMeasurementUnit’ object property has been created between the ’sosa:Observation’ class.




REFERENCES

Haller, A., Janowicz, K., Cox, S. J. D., Lefrançois, M., & Taylor, K. (2018). The SOSA / SSN Ontology : A Joint W3C and OGC Standard Specifying the Semantics of Sensors , Observations , Actuation , and Sampling, 1–19.

Haller, A., Janowicz, K., Cox, S. J. D., Lefrançois, M., Taylor, K., Le Phuoc, D., … Stadler, C. (2018). The modular SSN ontology: A joint W3C and OGC standard specifying the semantics of sensors, observations, sampling, and actuation. Journal of Semantic Web, 10(1), 9–32. https://doi.org/10.3233/sw-180320

World Wide Web Consortium. (n.d.). Core SSN Ontology. Retrieved November 20, 2018, from https://www.w3.org/ns/sosa/


