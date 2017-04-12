## Questions (in order of priority)

- how do we confirm things are working once the system is deployed? what is the "backend" the system is sending data to? 
- for each weather station memory card do I edit `FK.CFG` so `R6 ROCKBLOCK` -> `CT ROCKBLOCK`
- how do we confirm validity of data the sensors are collecting? Should we assume they are calibrated properly? 
A seperate field calibration procedure is only necessary on the water quality sensors, the validity of the other data is captured by past test experience and the outlined datasheets. The data will be reviewed upon uplink into the system, but the assumption that they are calibrated to acceptable standards is a safe one here. Once we transition to our FieldKit sensors, calibration certificates are part of the testing process before a unit enters the field. 
- for sonar / water depth sensor, how do we calibrate it? Should we record the height between the water surface level and the sensor? 
- does temperature sensor need any sort of calibration? 
No these do not need calibration. Previous testing shows that they are generally within +/- 0.1°C of each other across lots and fall closer in the ambient ranges that these will be measuring. These are not fake probes but come from the original manufacturer, which is some of the issues with cal on these in the past. Either way, the 3 sigma dispersion is within the accepted range for this data as told by the water scientists working on it. 
