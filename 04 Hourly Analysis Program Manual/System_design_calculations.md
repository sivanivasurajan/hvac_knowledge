29.0 System Design Calculations
29.1 Overview of System Design Calculations
29.0 System Design Calculations ››
Overview of System Design Calculations
29.0 System Design Calculations ›› 29.1 Overview of System Design Calculations ››
This chapter explains calculatin procedures for sizing components of HVAC air systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides overviews of system design procedures for different types of systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview of System Design Calculations
This is the first in a series of help topics describing calculation procedures used to size system components.
When performing calculations to determine required airflow rates, supply terminal characteristics and coil
capacities for HVAC systems, HAP uses the following general eight-step procedure:
1. Compute sensible and latent loads for all spaces in zones served by the HVAC system.
2. Sum space loads to obtain sensible and latent loads for all zones served by the HVAC system.
3. Determine required zone and space airflow rates.
4. Compute required sizes for zone equipment such as terminal reheat coils, supplemental zone heating units
and fan powered mixing boxes, as necessary.
5. Determine required system airflow rates. This includes sizing all fans and outdoor ventilation airflow rates.
6. Simulate HVAC system operation. Based on the required airflow rates determined in steps 3 thru 5,
operation of the HVAC system is mathematically simulated to produce profiles of loads on central cooling
and heating coils.
7. Identify peak coil loads. Cooling and heating coil load profiles from step 6 are inspected to identify maximum
loads.
8. Report results.
The use of this procedure varies between cooling and heating systems. The following three help topics discuss
how this procedure is applied:
Design Procedures for Cooling/Heating Systems
Design Procedures for Cooling-Only Systems
Design Procedures for Heating-Only Systems
Additional help topics discuss load and sizing calculations for the following:
Space and Zone Airflows
System Airflow
Supply Fan Airflow
Return Fan Airflow
Outdoor Ventilation Airflow
Terminal Reheat Coil Capacity
Page 1 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Design Procedures for Cooling/Heating Systems
29.0 System Design Calculations ›› 29.1 Overview of System Design Calculations ››
Zone Heating Unit Capacity
FPMBX Fan Airflow
4-Pipe Induction Systems
Cooling Coil Loads
Heating Coil Loads
Humidifier Loads
Outdoor Ventilation Loads
Plenum Loads
Fan Heat Gains
Duct Heat Gains or Losses
Duct Leakage
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Procedures for Cooling/Heating Systems
This help topic describes the 9-step procedure used to design systems which provide both cooling and
heating. Airflow rates for system terminals and fans will be based on worst case of cooling or heating
requirements. System airflow rates will then be used to simulate system operation for both design cooling and
design heating conditions to determine maximum coil loads. Each step in the sizing process is explained in the
following paragraphs.
1. Calculate Space Sensible and Latent Cooling Loads. First, sensible and latent cooling loads are
computed for each space served by the HVAC system. Hourly loads are computed for design cooling days
in each month included in the design analysis. Heat gains are first computed for each heat source in the
space and are then converted to loads using room transfer function equations . For these calculations it is
assumed cooling is provided 24 hours per day and each space is maintained exactly at the occupied
cooling thermostat setpoint for the zone in which it is included.
The assumptions of 24-hour cooling and a fixed zone temperature are required per ASHRAE procedures to
determine loads which will be used for sizing space and zone airflow rates. Once airflow rates have been
sized, air system operation will be simulated (see step 6). During system simulation, ASHRAE heat
extraction procedures will be used to correct the original space and zone sensible loads to account for
actual operating conditions including the following:
a. Availability of cooling for less than 24 hours per day.
b. Use of different occupied and unoccupied period thermostat setpoints.
c. Variation of the zone temperature within the thermostat throttling range.
This allows such phenomena as pulldown loads to be analyzed in the simulation calculations. Because the
correction of the original load data cannot be done until zone airflow rates have been calculated, pulldown
load considerations cannot be included in the original space and zone load calculations nor can they be
included in space and zone airflow calculations.
2. Calculate Space Sensible and Latent Heating Loads. Second, sensible and latent heating loads are
computed for the design heating condition for each space served by the HVAC system. The design heating
calculation differs from the design cooling calculation in that loads are calculated for one design heating
hour and heat gain from solar, lights, people, and electric and miscellaneous equipment are ignored to
provide a conservative heat loss estimate.
Page 2 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Design Procedures for Cooling-Only Systems
29.0 System Design Calculations ›› 29.1 Overview of System Design Calculations ››
3. Calculate Zone Sensible and Latent Loads. Next, zone loads are computed by summing loads for all
spaces included in each zone. This is done for both cooling and heating load conditions.
4. Calculate Required Zone and Space Supply Airflow Rates. Zone and space supply airflow rates are then
calculated for the worst case cooling condition and for the design heating condition. The larger airflow
requirement, whether from cooling or heating, will be chosen as the design airflow. Typically a design
cooling condition will set the design supply airflow due to the smaller delta-T’s involved. But this is not
always the case. In certain climates the design heating load will require larger airflow rates.
Zone and space supply airflow rates are computed using a sizing method specified by the user. These
calculations use required supply air temperatures or airflow rates specified by the user and the space and
zone sensible loads calculated in steps 1, 2 and 3 above.
5. Calculate Required Zone Equipment Sizes. Once zone airflow rates and design heating loads are known,
heating capacities for terminal reheat coils and supplemental zone heating units can be computed. The
required airflow rates for fan powered mixing box fans can also be computed.
6. Calculate System Airflow Rates. In this step, required airflow rates for the system , the central supply fan ,
the return fan , and for outdoor ventilation air are calculated.
7. Simulate Air System Operation. Once the airflow rates and zone equipment capacities for a system have
been determined, its operation is mathematically simulated to determine system coil loads. This produces
hourly profiles of cooling and heating coil loads. These simulations:
a. Are performed for the design cooling day in each month included in the analysis. A simulation is also
performed for the design heating condition.
b. Consider the specific configuration of system components.
c. Consider the specific operation of system controls.
d. Consider all components and controls specified in air system input.
e. Use the heat extraction procedures to correct the zone loads computed in steps 1 and 2 to determine the
actual zone conditioning requirements, how equipment responds to these loads and how the zone
temperatures vary within the thermostat throttling range.
f. Use zone loads with modified lighting and people load components if zone diversity factors were specified
by the user.
g. Compute the airflow rate, temperature and humidity at each point in the system.
h. Compute system coil loads using the airflow rate and entering and leaving conditions calculated for each
coil in the system.
Using this procedure, coil sizing results are specific to the type of system being analyzed. This is referred to
as "System Based Design".
8. Identify Peak Coil Loads. Coil load profiles generated by the air system simulations for design cooling
days are inspected to identify the maximum cooling coil loads . Maximum heating coil loads are obtained
from simulation results for the design heating condition. One exception is the peak load for a central reheat
coil which is part of an active dehumidification control system. This peak coil load is obtained from design
cooling days.
9. Report Results. Finally, space, zone and system loads, space and zone airflow rates, zone equipment
sizing data, and maximum cooling and heating coil loads are listed on the system design reports generated
by HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Procedures for Cooling-Only Systems
Page 3 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
This help topic describes the 8-step procedure used to design cooling-only systems. Peak cooling loads will be
used to determine airflow rates for system terminals and fans. System airflow rates will then be used to
simulate system operation for design cooling conditions to determine maximum coil loads. Each step in the
sizing process is explained in the following paragraphs.
1. Calculate Space Sensible and Latent Loads. First, sensible and latent cooling loads are computed for
each space served by the HVAC system. Hourly loads are computed for design cooling days in each month
included in the design analysis. Heat gains are first computed for each heat source in the space and are
then converted to loads using room transfer function equations . For these calculations it is assumed
cooling is provided 24 hours per day and each space is maintained exactly at the occupied cooling
thermostat setpoint for the zone in which it is included.
The assumptions of 24-hour cooling and a fixed zone temperature are required per ASHRAE procedures to
determine loads which will be used for sizing space and zone airflow rates. Once airflow rates have been
sized, air system operation will be simulated (see step 6). During system simulation, ASHRAE heat
extraction procedures will be used to correct the original space and zone sensible loads to account for
actual operating conditions including the following:
a. Availability of cooling for less than 24 hours per day.
b. Use of different occupied and unoccupied period thermostat setpoints.
c. Variation of the zone temperature within the thermostat throttling range.
This allows such phenomena as pulldown loads to be analyzed in the simulation calculations. Because the
correction of the original load data cannot be done until zone airflow rates have been calculated, pulldown
load considerations cannot be included in the original space and zone load calculations nor can they be
included in space and zone airflow calculations.
2. Calculate Zone Sensible and Latent Loads. Next, zone loads are computed by summing loads for all
spaces included in each zone.
3. Calculate Required Zone and Space Supply Airflow Rates. Zone and space supply airflow rates are
computed using a sizing method specified by the user. These calculations use required supply air
temperatures or airflow rates specified by the user and the space and zone sensible loads calculated in
steps 1 and 2 above.
4. Calculate Required Zone Equipment Sizes. Once zone airflow rates are known, heating capacities for
terminal reheat coils and supplemental zone heating units can be computed. The required airflow rates for
fan powered mixing box fans can also be computed.
5. Calculate System Airflow Rates. In this step, required airflow rates for the system , the central supply fan ,
the return fan , and for outdoor ventilation air are calculated.
6. Simulate Air System Operation. Once the airflow rates and zone equipment capacities for a system have
been determined, its operation is mathematically simulated to determine system coil loads. This produces
hourly profiles of cooling and heating coil loads. These simulations:
a. Are performed for the design cooling day in each month included in the analysis. A simulation is also
performed for the design heating condition.
b. Consider the specific configuration of system components.
c. Consider the specific operation of system controls.
d. Consider all components and controls specified in air system input.
e. Use the heat extraction procedures to correct the zone loads computed in steps 1 and 2 to determine the
actual zone conditioning requirements, how equipment responds to these loads and how the zone
temperatures vary within the thermostat throttling range.
f. Use zone loads with modified lighting and people load components if zone diversity factors were specified
by the user.
g. Compute the airflow rate, temperature and humidity at each point in the system.
h. Compute system coil loads using the airflow rate and entering and leaving conditions calculated for each
coil in the system.
Page 4 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Design Procedures for Heating-Only Systems
29.0 System Design Calculations ›› 29.1 Overview of System Design Calculations ››
29.2 Space and Zone Airflow Sizing Calculations
Using this procedure, coil sizing results are specific to the type of system being analyzed. This is referred to
as "System Based Design".
7. Identify Peak Coil Loads. Coil load profiles generated by the air system simulations for design cooling
days are inspected to identify the maximum cooling coil loads .
8. Report Results. Finally, space, zone and system loads, space and zone airflow rates, zone equipment
sizing data, and maximum cooling loads are listed on the system design reports generated by HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Procedures for Heating-Only Systems
This help topic describes the 8-step procedure used to design heating-only systems. Each step in the sizing
process is explained in the following paragraphs.
1. Calculate Design Heating Loads for Spaces. First, design heating loads are computed for all spaces
served by the HVAC system. Loads are computed as instantaneous heat losses using the winter design
temperature for outdoor air and the occupied heating thermostat setpoint for indoor air.
2. Calculate Zone Design Heating Loads. Next, zone loads are computed by summing loads for all spaces
included in each zone.
3. Calculate Required Zone and Space Supply Airflow Rates. Zone and space supply airflow rates are
computed using a sizing method specified by the user. These calculations use the required supply air
temperature specified by the user and the space and zone heating loads calculated in steps 1 and 2 above.
4. Calculate Required Zone Equipment Sizes. Once zone airflow rates and zone design heating loads are
known, heating capacities for terminal reheat coils and supplemental zone heating units can be computed.
5. Calculate System Airflow Rates. In this step, required airflow rates for the system , the central supply fan ,
the return fan , and for outdoor ventilation air are calculated.
6. Simulate Air System Operation. Once the airflow rates and zone equipment capacities for a system have
been determined, its operation is mathematically simulated to determine system coil loads. This simulation:
a. Is performed for the design heating condition.
b. Considers the specific configuration of system components.
c. Considers the specific operation of system controls.
d. Considers all components and controls specified in air system input.
e. Computes the airflow rate and dry-bulb temperature at each point in the system.
f. Computes system coil loads using the airflow rate and entering and leaving conditions calculated for each
coil in the system.
Using this procedure, coil sizing results are specific to the type of system being analyzed. This is referred to
as "System Based Design".
7. Identify Peak Coil Loads. Results from the air system simulations for the design heating condition are
assumed to represent the maximum heating coil loads .
8. Report Results. Finally, space, zone and system loads, space and zone airflow rates, zone equipment
sizing data, and maximum heating coil loads are listed on system design reports generated by HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 5 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
29.0 System Design Calculations ››
Space and Zone Airflow Sizing Calculations
29.0 System Design Calculations ›› 29.2 Space and Zone Airflow Sizing Calculations ››
This section explains procedures for sizing supply airflow to spaces and zones.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space and Zone Airflow Sizing Calculations
This help topic documents procedures used to calculate required space and zone airflow rates. Depending on
user specifications and the type of system involved any one of sixteen different sizing procedures could be
used to determine space and zone airflow rates. The large number of possible procedures is due to:
a. The choice of four different sizing methods offered by the program.
b. The ability to specify system sizing criteria in terms of supply air temperature, supply airflow (CFM or L/s)
and supply airflow per unit floor area (CFM/sqft or L/s/sqm).
c. Use of different load data when sizing cooling-only, cooling-and-heating, and heating-only HVAC systems.
Airflow sizing documentation will be provided in separate sections below. The first section will describe
procedures for cooling-and-heating systems, the second with cooling-only systems and the third with heating-
only systems. Within each section sizing calculations for the four sizing methods will be discussed. Within
each discussion, variations due to use of CFM (L/s), CFM/sqft (L/s/sqm) and supply air temperature sizing
criteria will be noted. A final section explains special sizing cases.
A. COOLING-AND-HEATING SYSTEMS
Space and zone airflow calculations for cooling-and-heating HVAC systems are explained below for each of
the four sizing methods offered by the program. Within each discussion an explanation of the method, a simple
example and the fundamental equations will be provided. Definitions of variables in these equations are
provided at the end of this help topic.
1. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Coincident Space Loads
Explanation: With this method, the zone airflow is calculated from either the maximum zone sensible
cooling load or the maximum zone heating load, whichever yields the larger airflow. The zone airflow is then
divided among spaces in the zone on the basis of space sensible loads which coincide with the time the
peak zone cooling or heating load occurs.
Example: A zone has a maximum sensible cooling load of 21600 BTU/h, the cooling setpoint is 75 F and
the supply air temperature is 55 F. Assuming sea level conditions, the required airflow rate for peak cooling
is 1000 CFM. The zone also has a maximum heating load of 38000 BTU/h, the heating setpoint is 70 F and
the supply air temperature is 110 F. The required airflow for heating is therefore 880 CFM. Because the
cooling condition yields the larger airflow rate, it is used as the design condition. This maximum zone
cooling load occurs at August 1600. Further, this zone contains two spaces. At August 1600, the spaces
have sensible cooling loads of 8000 BTU/h and 13600 BTU/h respectively.
The required airflow for the first space will be:
(1000 CFM) x (8000 BTU/h)/(21600 BTU/h) = 370 CFM.
The required airflow for the second space will be:
(1000 CFM) x (13600 BTU/h)/(21600 BTU/h) = 630 CFM.
Page 6 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
It is important to note that space loads at August 1600 are used in this example calculation even if larger
space loads exist at other times.
If the design heating load had yielded a larger zone airflow, then the space airflows would have been
calculated based on ratios using space heating loads instead of space cooling loads.
Zone Airflow Calculation:
Sizing Criteria is Supply Temperature:
Zone supply airflow is computed as the larger value for peak cooling and heating loads:
Vz = Qzc/[ρaCpaK(Tzc-Tsc)]
Vz = Qzh/[ρaCpaK(Tzh-Tsh)]
Sizing Criteria is Supply CFM or L/s:
The specified supply CFM or L/s is the airflow for the outlet of the air handling unit. Leakage is subtracted
first to determine the airflow available at zone terminals. This airflow is divided among the zones based
on maximum zone sensible cooling load ratios.
Vsys,adj = Vsys (1 - Fl/100)
Vz = (Qzc/Qzc,tot)Vsys,adj
Sizing Criteria is Supply CFM/sqft or L/s/sqm:
The airflow available at the outlet of the air handler is computed first. Duct leakage is then subtracted to
determine the airflow available at zone terminals. Finally, this airflow is divided among zones based on
the ratio of floor areas.
Vsys = (CFM/sqft or L/s/sqm) Asys
Vsys,adj = Vsys (1 - Fl/100)
Vz = Vsys,adj(Az / Asys)
Space Airflow Calculation:
Vs = (Qcsc/Qzc)Vz if peak cooling load dictates airflow.
Vs = (Qcsh/Qzh)Vz if peak heating load dictates airflow.
2. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Individual Peak Space Loads
Explanation: With this method, the required zone airflow rate is determined in the same manner as #1
above. Required airflow rates for spaces in the zone are calculated from the maximum sensible cooling load
for each individual space or the maximum heating load for the space, whichever yields the larger airflow.
Note that if peak loads for all the spaces in the zone occur at the time the peak zone load occurs, the sum
of the space airflow rates will equal the zone airflow rate. If the spaces experience peak loads at different
times, the sum of the space airflow rates will exceed the required zone airflow rate. In such a situation, the
ductwork between the zone terminal and the space diffusers will have excess airflow capacity. The example
below illustrates such a situation.
Example: A zone has a maximum sensible load occurring at August 1600 which requires an airflow of 1000
CFM. The zone contains two spaces. One space has a peak sensible load at August 1300 that requires an
airflow of 550 CFM. The second space has a peak sensible load at August 1700 that requires an airflow of
600 CFM.
Zone Airflow Calculation: (Same as Method #1)
Space Airflow Calculation:
For all sizing criteria cases, two space airflow rates are computed based on the peak space sensible
cooling load and the peak space heating load respectively. The airflow derived from the cooling load
uses the cooling setpoint and the cooling supply temperature. The airflow derived from the heating load
uses the heating setpoint and the heating supply temperature. If a supply temperature was not specified
Page 7 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
by the user, the program computes it using the maximum zone sensible cooling load and the required
zone airflow rate.
Vsc = Qmsc/ρaCpaK(Tzc-Tsc)
Vsh = Qsh/ρaCpaK(Tzh-Tsh)
The larger value of Vsc and Vsh is then used as the supply airflow rate for the space.
3. Zone Sizing Method: Sum of Space Airflow Rates
Space Sizing Method: Individual Peak Space Loads
Explanation: Design airflow rates for each space in a zone are calculated from the maximum sensible
cooling load or the maximum heating load for the space, whichever yields the larger airflow. The required
zone airflow rate is the sum of space airflows for all spaces in the zone.
Example: A zone contains two spaces. Both have airflows dictated by peak cooling loads. One has a peak
sensible load at August 1300 that requires an airflow of 550 CFM. The second space has a peak sensible
load at August 1700 that requires an airflow of 600 CFM. Therefore, the required zone airflow rate is:
(550 CFM) + (600 CFM) = 1150 CFM
Zone Airflow Calculation:
Vz = Sum of Vs, all spaces in zone.
Space Airflow Calculation:
Sizing Criteria is Supply Temperature:
Space supply airflow is computed for the peak sensible cooling load and the peak heating load. The
larger of the two airflows is used for the space:
Vs = Qmsc/[ρaCpaK(Tzc-Tsc)]
Vs = Qsh/[ρaCpaK(Tzh-Tsh)]
Sizing Criteria is Supply CFM or L/s:
The specified supply CFM or L/s is the airflow for the outlet of the air handling unit. Leakage is subtracted
first to determine the airflow available at zone terminals. This airflow is divided among the spaces based
on maximum space sensible cooling load ratios.
Vsys,adj = Vsys (1 - Fl/100)
Vs = (Qmsc/ Qmsc,tot) Vsys,adj
Sizing Criteria is Supply CFM/sqft or L/s/sqm:
The airflow available at the outlet of the air handler is computed first. Duct leakage is then subtracted to
determine the airflow available at zone terminals. Finally, this airflow is divided among spaces based on
the ratio of maximum space sensible cooling loads.
Vsys = (CFM/sqft or L/s/sqm) Asys
Vsys,adj = Vsys (1 - Fl/100)
Vs = (Qmsc/Qmsc,tot)Vsys,adj
4. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Zone CFM/sqft or L/s/sqm
Explanation: With this method, the zone airflow is calculated as described in #1 above. The zone airflow is
divided among spaces in the zone on the basis of zone CFM/sqft or L/s/sqm and space floor area.
Example: A zone has a required airflow rate of 1000 CFM. The zone contains two spaces of 600 sqft and
900 sqft floor area, respectively. Therefore, the overall zone CFM/sqft is 0.67 CFM/sqft.
The required airflow for the first space will be:
Page 8 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
(600 sqft) x (0.67 CFM/sqft) = 400 CFM.
The required airflow for the second space will be:
(900 sqft) x (0.67 CFM/sqft) = 600 CFM.
Zone Airflow Calculation: (Same as Method #1)
Space Airflow Calculation:
Vs = (Vz/Az) As
B. COOLING-ONLY SYSTEMS
Space and zone airflow calculations for cooling-only are explained below for each of the four sizing methods
offered by the program. Within each discussion an explanation of the method, a simple example and the
fundamental equations will be provided. Definitions of variables in these equations are provided at the end of
this help topic.
1. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Coincident Space Loads
Explanation: With this method, the zone airflow is calculated from the maximum zone sensible cooling
load. The zone airflow is then divided among spaces in the zone on the basis of space sensible cooling
loads which occur for the month and hour when the zone load peaks.
Example: A zone has a maximum sensible load of 21600 BTU/h and a required airflow rate of 1000 CFM.
This maximum zone load occurs at August 1600. Further, this zone contains two spaces. At August 1600,
the spaces have sensible cooling loads of 8000 BTU/h and 13600 BTU/h respectively.
The required airflow for the first space will be:
(1000 CFM) x (8000 BTU/h)/(21600 BTU/h) = 370 CFM.
The required airflow for the second space will be:
(1000 CFM) x (13600 BTU/h)/(21600 BTU/h) = 630 CFM.
It is important to note that space loads at August 1600 are used in this example calculation even if larger
space loads exist at other times.
Zone Airflow Calculation:
Sizing Criteria is Supply Temperature:
Zone supply airflow is computed using the supply temperature and the maximum zone sensible cooling
load.
Vz = Qzc/[ρaCpaK(Tzc-Tsc)]
Sizing Criteria is Supply CFM or L/s:
The specified supply CFM or L/s is the airflow for the outlet of the air handling unit. Leakage is subtracted
first to determine the airflow available at zone terminals. This airflow is divided among the zones based
on maximum zone sensible cooling load ratios.
Vsys,adj = Vsys (1 - Fl/100)
Vz = (Qzc/Qzc,tot)Vsys,adj
Sizing Criteria is Supply CFM/sqft or L/s/sqm:
The airflow available at the outlet of the air handler is computed first. Duct leakage is then subtracted to
determine the airflow available at zone terminals. Finally, this airflow is divided among zones based on
the ratio of floor areas.
Vsys = (CFM/sqft or L/s/sqm) Asys
Vsys,adj = Vsys (1 - Fl/100)
Page 9 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Vz = Vsys,adj(Az / Asys)
Space Airflow Calculation:
Vs = (Qcsc/Qzc)Vz
2. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Individual Peak Space Loads
Explanation: With this method, the required zone airflow rate is calculated from the maximum zone
sensible cooling load. Required airflow rates for spaces in the zone are calculated from the maximum
sensible cooling load for each individual space.
Note that if peak loads for all the spaces in the zone occur at the time the peak zone load occurs, the sum
of the space airflow rates will equal the zone airflow rate. If the spaces experience peak loads at different
times, the sum of the space airflow rates will exceed the required zone airflow rate. In such a situation, the
ductwork between the zone terminal and the space diffusers will have excess airflow capacity. The example
below illustrates such a situation.
Example: A zone has a maximum sensible load occurring at August 1600 which requires an airflow of 1000
CFM. The zone contains two spaces. One space has a peak sensible load at August 1300 that requires an
airflow of 550 CFM. The second space has a peak sensible load at August 1700 that requires an airflow of
600 CFM.
Zone Airflow Calculation: (Same as Method #1)
Space Airflow Calculation:
For all sizing criteria cases, space airflow rate is computed using the required zone supply temperature
and the maximum space cooling load. If a supply temperature was not specified by the user, the program
computes it using the maximum zone sensible cooling load and the required zone airflow rate.
Vs = Qmsc/ρaCpaK(Tzc-Tsc)
3. Zone Sizing Method: Sum of Space Airflow Rates
Space Sizing Method: Individual Peak Space Loads
Explanation: Design airflow rates for each space in a zone are calculated from the maximum sensible
cooling load for the space. The required zone airflow rate is the sum of space airflows for all spaces in the
zone.
Example: A zone contains two spaces. One has a peak sensible load at August 1300 that requires an
airflow of 550 CFM. The second space has a peak sensible load at August 1700 that requires an airflow of
600 CFM. Therefore, the required zone airflow rate is:
(550 CFM) + (600 CFM) = 1150 CFM
Zone Airflow Calculation:
Vz = Sum of Vs, all spaces in zone.
Space Airflow Calculation:
Sizing Criteria is Supply Temperature:
Space supply airflow is computed using the supply temperature and the maximum space sensible
cooling load.
Vs = Qmsc/[ρaCpaK(Tzc-Tsc)]
Sizing Criteria is Supply CFM or L/s:
The specified supply CFM or L/s is the airflow for the outlet of the air handling unit. Leakage is subtracted
first to determine the airflow available at zone terminals. This airflow is divided among the spaces based
on maximum space sensible cooling load ratios.
Vsys,adj = Vsys (1 - Fl/100)
Page 10 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Vs = (Qmsc/ Qmsc,tot) Vsys,adj
Sizing Criteria is Supply CFM/sqft or L/s/sqm:
The airflow available at the outlet of the air handler is computed first. Duct leakage is then subtracted to
determine the airflow available at zone terminals. Finally, this airflow is divided among spaces based on
the ratio of maximum space sensible cooling loads.
Vsys = (CFM/sqft or L/s/sqm) Asys
Vsys,adj = Vsys (1 - Fl/100)
Vs = (Qmsc/Qmsc,tot)Vsys,adj
4. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Zone CFM/sqft or L/s/sqm
Explanation: With this method, the zone airflow is calculated from the maximum zone sensible cooling
load. The zone airflow is divided among spaces in the zone on the basis of zone CFM/sqft or L/s/sqm and
space floor area.
Example: Based on the maximum zone sensible load, a zone has a required airflow rate of 1000 CFM. The
zone contains two spaces of 600 sqft and 900 sqft floor area, respectively. Therefore, the overall zone
CFM/sqft is 0.67 CFM/sqft.
The required airflow for the first space will be:
(600 sqft) x (0.67 CFM/sqft) = 400 CFM.
The required airflow for the second space will be:
(900 sqft) x (0.67 CFM/sqft) = 600 CFM.
Zone Airflow Calculation: (Same as Method #1)
Space Airflow Calculation:
Vs = (Vz/Az) As
C. HEATING-ONLY SYSTEMS
Space and zone airflow calculations for heating-only HVAC systems are explained below for each of the four
sizing methods offered by the program. Within each discussion an explanation of the method, a simple
example and the fundamental equations will be provided. Definitions of variables in these equations are
provided at the end of this help topic. Note that the sizing criteria for heating systems is always the heating
supply temperature.
1. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Coincident Space Loads
Explanation: With this method, the zone airflow is calculated from the zone sensible load at the design
heating condition. The zone airflow is then divided among spaces in the zone on the basis of space
sensible loads, also at the design heating condition.
Example: A zone has a heating sensible load of 21600 BTU/h and a required airflow rate of 1000 CFM.
Further, this zone contains two spaces whose design heating loads are 8000 BTU/h and 13600 BTU/h
respectively.
The required airflow for the first space will be:
(1000 CFM) x (8000 BTU/h)/(21600 BTU/h) = 370 CFM.
The required airflow for the second space will be:
(1000 CFM) x (13600 BTU/h)/(21600 BTU/h) = 630 CFM.
Zone Airflow Calculation:
Page 11 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Vz = Qzh/[ρaCpaK(Tsh-Tzh)]
Space Airflow Calculation:
Vs = (Qsh/Qzh)Vz
2. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Individual Peak Space Loads
Explanation: With this method, the required zone airflow rate is calculated from the zone sensible load at
the design heating condition. Required airflow rates for spaces in the zone are calculated from the heating
sensible load for each individual space, also calculated at the design heating condition.
Example: A zone has a design heating load which requires an airflow of 1000 CFM. The zone contains two
spaces. One space has a peak sensible heating load that requires an airflow of 400 CFM. The second
space has a peak sensible heating load that requires an airflow of 600 CFM.
Zone Airflow Calculation:
Vz = Qzh/ρaCpaK(Tsh-Tzh)
Space Airflow Calculation:
Vs = Qsh/ρaCpaK(Tsh-Tzh)
3. Zone Sizing Method: Sum of Space Airflow Rates
Space Sizing Method: Individual Peak Space Loads
Explanation: Design airflow rates for each space in a zone are calculated from the design heating load for
the space. The required zone airflow rate is the sum of space airflows for all spaces in the zone.
Example: A zone contains two spaces. One has a peak sensible heating load that requires an airflow of
550 CFM. The second space has a peak sensible heating load that requires an airflow of 600 CFM.
Therefore, the required zone airflow rate is:
(550 CFM) + (600 CFM) = 1150 CFM
Zone Airflow Calculation:
Vz = Sum of Vs, all spaces in zone.
Space Airflow Calculation:
Vs = Qsh/ρaCpaK(Tsh-Tzh)
4. Zone Sizing Method: Peak Zone Sensible Load
Space Sizing Method: Zone CFM/sqft or L/s/sqm
Explanation: With this method, the zone airflow is calculated from the zone sensible load calculated at the
design heating condition. The zone airflow is divided among spaces in the zone on the basis of zone
CFM/sqft or L/s/sqm and space floor area.
Example: Based on the sensible heating load for a zone, an airflow rate of 1000 CFM is required. The zone
contains two spaces of 600 sqft and 900 sqft floor area, respectively. Therefore, the overall zone CFM/sqft
is 0.67 CFM/sqft.
The required airflow for the first space will be:
(600 sqft) x (0.67 CFM/sqft) = 400 CFM.
The required airflow for the second space will be:
(900 sqft) x (0.67 CFM/sqft) = 600 CFM.
Zone Airflow Calculation:
Vz = Qzh/ρaCpaK(Tsh-Tzh)
Page 12 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Space Airflow Calculation:
Vs = (Vz/Az) As
D. SPECIAL SIZING CASES
This section describes how the program handles four special cases involving space and zone airflow sizing
calculations.
1. Minimum Supply Air Override. In addition to the sizing criteria for maximum zone airflow, users also
define the minimum required airflow rate for each zone. During sizing calculations HAP compares the zone
supply airflow rate calculated as described in sections A, B or C with the minimum required airflow rate. The
larger of the two values is assigned to the zone. This assures that the zone receives at least the minimum
zone airflow rate specified by the user.
Minimum supply airflow can be defined using five different units of measure. Procedures used to convert
each to minimum airflow in CFM or L/s are described below.
Vz,min = (CFM or L/s specified by user), or
Vz,min = (CFM/sqft or L/s/sqm) Az, or
Vz,min = (CFM/person or L/s/person) Omax, or
Vz,min = Fmin Vz / 100 when % of supply air specified
Vz,min =(Air Changes per Hour specified) x (air volume of spaces in zone) x (hr/60 min)
For VAV systems, Vz,min also serves to define the minimum airflow rate for the VAV terminal.
When a calculated zone airflow rate is overridden by the minimum airflow, airflow rates for the spaces in the
zone must be adjusted. All space airflow rates are increased by the same proportion. For example, if the
calculated zone airflow rate is overridden by a minimum airflow value which is 10% larger, then airflow rates
for all spaces in that zone are increased by 10% as well.
Readers should note that there are two cases in which the minimum zone airflow correction is not used.
Both cases involve the sizing method in which space airflow is calculated from individual peak space loads
and the zone airflow is the sum of the space airflow rates. If this sizing method is specified and the supply
air sizing criteria is CFM (L/s) or CFM/sqft (L/s/sqft), the minimum zone airflow correction is not made
because it would conflict with the supply air sizing criteria. For example, if supply air of 5000 CFM is
specified in conjunction with a minimum zone airflow rate of 5500 CFM, the two specifications are in direct
conflict with one another. Such conflicts must be corrected in the system input data by the user.
2. Reheat Terminal Airflow Override. When the zone air terminal includes a reheat coil, the supply airflow
required to meet the zone design heating load while supplying air at the specified heating supply air
temperature is calculated. If this reheat coil airflow is larger than the originally calculated zone supply
airflow, then the reheat supply airflow overrides the other flows and establishes the supply airflow for the
zone. When comparing airflows, the original zone supply airflow is the larger of the value from sections A,
B, or C above, and the minimum zone airflow.
The required reheat coil supply airflow rate is calculated as:
Vrh,z = Qzh/ρaCpaK(Trh,sat-Tzh)
3. Direct Exhaust Air Override. When direct exhaust air specified for a zone is larger than the required zone
airflow rate, the program overrides the calculated zone airflow rates and sets zone airflow equal to the direct
exhaust air. For example, if the direct exhaust for a zone is specified as 500 CFM and the calculated zone
airflow rate is 300 CFM, the program will override the calculated value and set zone airflow to 500 CFM.
Direct exhaust air is air exhausted from a zone before it flows through a return plenum or duct. Sample
applications include laboratory exhaust hoods, kitchen exhaust hoods and toilet exhausts. In order to
Page 13 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
maintain the specified direct exhaust airflow the zone airflow rate must be equal to or larger than direct
exhaust.
When the calculated zone airflow rate is overridden in this way, airflow rates for spaces in the zone must be
adjusted. This is done using the following equation:
Vs,new = Vs,old(Vz,new/Vz,old)
4. Outdoor Ventilation Air Override. When the design outdoor ventilation airflow rate is larger than the
required system supply airflow rate, the system supply airflow rate is set equal to the ventilation airflow rate.
The program assumes that ventilation airflow has higher priority since it is often mandated by codes and
therefore must be maintained.
Example: The calculated system supply airflow rate is 10000 CFM. The calculated outdoor ventilation
airflow rate is 12000 CFM. Therefore, the calculated system airflow rate will be overridden and set equal to
12000 CFM.
When the calculated system supply airflow rate is overridden, all other zone and space airflow rates in the
system must be adjusted. This is done using the following equations:
Vz,new = Vz,old (Vsys,new/Vsys,old)
Vs,new = Vs,old(Vz,new/Vz,old)
5. Series Fan Powered Mixing Boxes. When sizing airflow rates for zones containing series fan powered
mixing box terminals, and using a sizing method that considers peak zone sensible load, the required zone
airflow rate is based on the peak zone sensible load plus the heat gain for the terminal fan.
E. VARIABLE DEFINITIONS
A
=
Site altitude, ft or m above sea level.
As
=
Total floor area in space, sqft or sqm.
Asys
=
Total floor area for all zones in system sqft or sqm.
Az
=
Total floor area in zone, sqft or sqm.
Cpa
=
Heat capacity of air, 0.24 BTU/(lb-F) or 1004.8 J/(kg-K).
Fmin
=
Minimum supply airflow rate as a percentage of maximum
airflow rate, %.
Fl
=
Duct leakage rate, percent.
K
=
Unit conversion factor,
=
60 min/hr for English units and
=
cubic meter/(1000 L) for SI Metric units.
Omax
=
Maximum scheduled occupancy for zone, number of
people.
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
ρa
=
Air density corrected for altitude, lb/cuft or kg/(cubic meter)
Qcsc
=
Coincident space sensible cooling load, BTU/hr or W. This
space load is computed or the month and hour
when the maximum zone sensible cooling load
occurs.
Qmsc
=
Maximum space sensible cooling load, BTU/h or W.
Qmsc,tot
=
Sum of maximum space sensible cooling loads for all
spaces served by the air system, BTU/hr or W.
Qsh
=
Design space heating load, BTU/hr or W.
Qzc
=
Maximum zone sensible cooling load, BTU/h or W.
Page 14 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Air Density Calculations
29.0 System Design Calculations ›› 29.2 Space and Zone Airflow Sizing Calculations ››
Qzc,tot
=
Sum of maximum zone sensible cooling loads for all zones
served by system, BTU/hr or W.
Qzh
=
Design zone heating load, BTU/hr or W.
Trh,sat
=
Design heating supply air temperature for terminal reheat
coil, F or C.
Tzc
=
Zone occupied cooling thermostat setpoint, F or C.
Tzh
=
Zone occupied heating thermostat setpoint, F or C.
Tsc
=
Cooling design supply air temperature specified by user, F
or C.
Tsh
=
Heating design supply air temperature specified by user, F
or C.
Vrh,z
=
Zone supply airflow rate required for terminal reheat coil to
meet the design heating load, CFM or L/s
Vs
=
Required space airflow rate, CFM or L/s.
Vs,new
=
Adjusted space airflow rate, CFM or L/s.
Vs,old
=
Original calculated space airflow rate, CFM or L/s.
Vsys
=
System supply airflow specified by user, CFM or L/s.
Represents airflow at outlet of air handling
unit.
Vsys,adj
=
System supply airflow available after duct leakage is
subtracted, CFM or L/s.
Vsys,new
=
Adjusted system supply airflow rate, CFM or L/s.
Vsys,old
=
Original calculated or specified system supply airflow rate,
CFM or L/s.
Vz
=
Required zone airflow rate, CFM or L/s.
Vz,min
=
Minimum zone airflow rate, CFM or L/s.
Vz,new
=
Adjusted zone airflow rate, CFM or L/s.
Vz,old
=
Original calculated zone airflow rate, CFM or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air Density Calculations
The physical properties of air are involved in many of HAP’s load, airflow, fan performance and psychrometric
calculations. One of the key properties of air dealt with is the density of air. HAP adjusts the density of air for
altitude. Therefore, unless otherwise noted, all load, airflow, fan performance and psychrometric data reported
by the program is in terms of actual air properties rather than standard (sea level) properties.
Air density is adjusted for altitude effects using the following equation
ρa = ρsl Fa
where:
ρa
=
Air density corrected for altitude, lb/cuft or kg/(cubic meter)
ρsl
=
Standard air density at sea level, .075 lb/cuft or 1.201 kg/
(cubic meter)
Fa
=
Altitude correction factor for air density, dimensionless.
=
(1 - 6.87535 x 10^-6 A)^5.2561 for English units.
=
(1 - 2.25569 x 10^-5 A)^5.2561 for SI Metric units.
Note: ^ is an exponentiation symbol. Example: 10^-6 means
10 to the minus 6 power.
Page 15 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
29.3 Zone Equipment Sizing Calculations
29.0 System Design Calculations ››
Terminal Reheat Coil Sizing Calculations
29.0 System Design Calculations ›› 29.3 Zone Equipment Sizing Calculations ››
A common component in calculations involving airflow is the product of air density, specific heat and a
conversion factor. For standard air at sea level this product is 1.08 in English units and 1.207 in Metric units.
When adjusted for altitude, the product is:
ρaCpaK = 1.08 Fa for English Units
ρaCpaK = 1.207 Fa for SI Metric Units
where:
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor, adjusted for altitude.
Cpa
=
Heat capacity of air, 0.24 BTU/(lb-F) or 1004.8 J/(kg-K).
K
=
Unit conversion factor,
=
60 min/hr for English units and
=
cubic meter/(1000 L) for SI Metric units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains sizing procedures for zone equipment such as reheat coils, fan powered mixing boxes,
and zone baseboard or fan coil heating equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Reheat Coil Sizing Calculations
This help topic describes the procedure used to calculate the required heating capacity for zone terminal
reheat coils. Calculation procedures for each system application or terminal type are provided below.
1. CAV Single Zone Systems with Reheat Coil. .
Qrh = ρaCpaK Vz,max (Trh,sat - Tinlet)
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Tinlet = Temperature of supply duct air entering the reheat coil, F or C.
Vz,max = Design zone supply airflow rate, CFM or L/s.
If the CAV Single Zone system has a central heating coil and that coil is scheduled ON, then Tinlet is the
design heating supply temperature for the central heating coil. If that central heating supply temperature is
greater than the specified Trh,sat, then the reheat coil capacity is zero.
If the system does not have a central heating coil, or the coil is scheduled OFF, then the supply duct air has
not been cooled or heated and Tinlet is calculated as:
Tinlet = [ QSupplyFan / (ρaCpaK Vsys ) ] + [ (Treturn)(Vsys - Voa) + (ToaVoa) ] / Vsys
where:
Page 16 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
QSupplyFan = Supply fan heat gain, BTU/hr or W
Toa = Outdoor air dry-bulb temperature, F or C.
Treturn = Return air dry-bulb temperature, F or C.
Voa = Outdoor airflow rate, CFM or L/s
Vsys = System supply fan airflow rate at design, CFM or L/s
Reheat Terminal in a Single Zone CAV System
Commentary: The reheat coil capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load. If the system
does not have a central heating coil, the terminal receives air that is the result of mixing of outdoor air and
return air, with the addition of fan heat. If the system does have a central heating coil, then it is assumed
the terminal receives air at the design heating supply air temperature.
2. Reheat Coil in CAV Terminal Reheat System.
Qrh = ρaCpaK Vz,max (Trh,sat - Tinlet)
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Tinlet = Temperature of supply duct air entering the reheat coil, F or C. Set to design cooling supply air
temperature.
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Vz,max = Design zone supply airflow rate, CFM or L/s.
Constant Volume Reheat Terminal
Commentary: The reheat coil capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load. Air is assumed
to come to the terminal at the design cooling supply air temperature.
3. Reheat Coil in CAV Two-Deck Multizone, CAV Three-Deck Multizone and CAV Dual Duct Systems.
Qrh = ρaCpaK Vz,max (Trh,sat - Tinlet)
Page 17 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Tinlet = Temperature of supply duct air entering the reheat coil, F or C.
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Vz,max = Design zone supply airflow rate, CFM or L/s
If the hot deck for the system is scheduled ON, then Tinlet is set equal to the hot deck design supply
temperature. This involves a conservative assumption that 100% of supply air to the reheat coil is air from
the hot deck. If the hot deck design supply temperature is greater than Trh,sat, then the reheat coil capacity
is zero.
If the hot deck is scheduled OFF, then Tinlet then the supply duct air coming to the reheat coil has not been
cooled or heated and Tinlet is calculated as:
Tinlet = [ QSupplyFan / (ρaCpaK Vsys ) ] + [ (Treturn)(Vsys - Voa) + (ToaVoa) ] / Vsys
where:
QSupplyFan = Supply fan heat gain, BTU/hr or W
Toa = Outdoor air dry-bulb temperature, F or C.
Treturn = Return air dry-bulb temperature, F or C.
Voa = Outdoor airflow rate, CFM or L/s
Vsys = System supply fan airflow rate at design, CFM or L/s
Commentary: The reheat coil capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load. At heating
design air is delivered to the terminal from the hot deck. If the hot deck is scheduled off, this air is the
mixture of return air and outdoor air with supply fan heat added. If the hot deck is scheduled on, this air is
assumed to be at the hot desk design supply air temperature.
4. VAV Reheat Terminals
Qrh = ρaCpaK Vz,min (Trh,sat - Tinlet)
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Tinlet = Temperature of supply duct air entering the reheat coil, F or C. Set equal to the design cooling
supply air temperature.
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Vz,min = Minimum zone supply airflow rate, CFM or L/s.
VAV Reheat Terminal
Page 18 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Commentary: The reheat coil capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load. The terminal is
at minimum supply airflow. Air is delivered to the terminal at the design cooling supply air temperature.
5. VAV Series Fan Powered Mixing Box Terminals
Qrh = ρaCpaK Vz,max (Trh,sat - Tinlet)
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Tinlet = Temperature of air entering reheat coil, F or C.
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Vz,max = Design zone supply airflow rate, CFM or L/s
and:
Tinlet = [ QTermFan / (ρaCpaK Vz,max ) ] + [ (TprimaryVp,min) + (Th,occ(Vz,max - Vp,min) ] / Vz,max
where:
QTermFan = Mixing box terminal fan heat gain, BTU/hr or W
Th,occ = Zone occupied heating thermostat setpoint, F or C
Tprimary = Temperature of primary supply air delivered to the mixing box, F or C. Set equal to the design
cooling supply air temperature.
Vp,min = Minimum primary supply airflow delivered to the mixing box, CFM or L/s.
Series Fan Powered Mixing Box Terminal
Commentary: The reheat capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load, and the terminal
is receiving primary air (occupied hour). The coil flow rate is the design zone supply airflow rate, since a
series mixing box maintains this flow for all operating hours. The coil inlet air temperature is a mixture of
primary air and recirculated plenum air with fan terminal fan heat added. Primary air is at the minimum
primary airflow setting and design cooling supply air temperature. The recirculated air is at the occupied
heating thermostat setpoint for the zone. Because plenum load is not considered for design heating, no
consideration of plenum load is made.
6. VAV Parallel Fan Powered Mixing Box Terminals
Qrh = ρaCpaK Vcoil (Trh,sat - Tinlet)
where:
Qrh = Reheat coil capacity, BTU/hr or W
ρaCpaK = Product of air density times air specific heat x unit conversion factor, adjusted for altitude .
Page 19 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Sizing Calculations for Supplemental Zone Heating Units
29.0 System Design Calculations ›› 29.3 Zone Equipment Sizing Calculations ››
Tinlet = Temperature of air entering reheat coil, F or C.
Trh,sat = Design heating supply discharge temperature specified for reheat coil, F or C.
Vcoil = Airflow through coil, CFM or L/s.
and:
Tinlet = [ (Tprimary)(Vp,min) + (Tfan,out)(VTermFan) ] / Vcoil
Vcoil = Vp,min + VTermFan
Tfan,out = Th,occ + QTermFan / [ (ρaCpaK)(VTermFan) ]
where:
QTermFan = Parallel mixing box fan heat gain, BTU/hr or W.
Tfan,out = Temperature of air leaving the parallel mixing box fan, F or C.
Th,occ = Zone occupied heating thermostat setpoint, F or C
Tprimary = Temperature of primary supply air delivered to the mixing box, F or C. Set equal to the design
cooling supply air temperature.
Vp,min = Minimum primary supply airflow delivered to the mixing box, CFM or L/s..
VTermFan = Design airflow rate for parallel mixing box fan, CFM or L/s.
Parallel Fan Powered Mixing Box Terminal
Commentary: The reheat capacity is the heat necessary to raise the coil airflow from inlet to outlet
temperature. The worst case heating condition is when the zone has design heating load, and the terminal
is receiving primary air (occupied hour). Therefore, the coil flow rate is the sum of minimum primary airflow
and parallel mixing box design fan airflow. The coil inlet temperature is the mixture of primary air at the
design cooling supply temperature and recirculated plenum air. The temperature of air in the plenum
entering the mixing box fan is at the occupied heating thermostat setpoint for the zone. Because plenum
load is not considered for design heating, no consideration of plenum load is made.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Sizing Calculations for Supplemental Zone Heating Units
This help topic documents the procedures used to calculate required heating capacity for supplemental zone
heating units. These heating units can be baseboard heaters or fan coil heating units. They are controlled
either by the room thermostat, or an outdoor thermostat. Separate procedures are required for each type of
control. Procedures are discussed below. Definitions for variables used in these discussions appear at the end
of this help topic.
A. Room Thermostat Control
Page 20 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
When zone heating units are controlled by a room thermostat, the required heating capacity is determined in
three different ways depending on components used in the system:
1. Central Heat + Zone Heat Case. If the system contains a central heating coil, the zone heating unit
capacity equals the design heating load for the zone. It is assumed the primary air handling system does
not impose any additional load on the space heating unit.
Qzhu = Qzh
2. Zone Heat Only Case. If the system does not contain a central heating coil and the zone terminal does not
contain a reheat coil, the zone heating unit capacity is computed as the sum of the design heating load for
the zone plus the extra heating load caused by primary system air entering the zone. For example, for the
design heating condition in a VAV system, the central supply fan will deliver a minimum flow of air to the
zone. If this air is cooler than the zone heating setpoint, it will add to the demand on the zone heating unit.
Qzhu = Qzh + ρaCpaK Vz,htg (Tzh - Tsc)
The use of the design cooling supply temperature, Tsc, in this equation provides a conservative estimate of
the required zone heating unit capacity. If the actual primary air temperature is warmer than this design
value at the design heating condition, the heating unit will have excess capacity.
3. Zone Heat + Terminal Reheat Case. If the system does not contain a central heating coil, but the zone
contains both a terminal reheat coil and a zone heating unit, the zone heating unit capacity is equal to the
design heating load for the zone. It is assumed the terminal reheat coil supplies primary air reheat.
Therefore, the zone heating unit capacity is:
Qzhu = Qzh
B. Outdoor Thermostat Control
When the zone heating unit is controlled by an outdoor thermostat, the required heating capacity is equal to
the design heating load for the zone. Extra heating loads imposed by the primary air system are not
considered for this type of thermostat control.
Qzhu = Qzh
C. Water Flow Rate Sizing Calculation
For either type of control, the required hot water flow rate for a hydronic zone heating unit is calculated using
the following equation:
Vw = Qzhu / (ρwCpwKwVw ΔThw)
D. Variable Definitions
Cpw
=
Heat capacity of water, 1.0 BTU/(lbm-F) or 4186.8 J/
(kg-K).
ΔThw
=
Hot water delta-T for heating coil, F or K.
Kw
=
Unit conversion factor for water flow.
=
(60 min/hr)(0.13368 cuft/gal) = 8.02 for English Units.
=
(cubic meter/1000 L) = 0.001 for SI Metric Units
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
ρw
=
Density of water, 62.3 lb/cuft or 998.0 kg/cubic meter.
Qzhu
=
Required heating capacity for a supplemental zone heating
unit, BTU/hr or W.
Qzh
=
Zone design heating load, BTU/hr or W.
Tzh
=
Zone occupied heating thermostat setpoint, F or C.
Tsc
=
Design cooling supply air temperature, F or C.
Vz,htg
=
Zone supply airflow rate at the design heating condition,
CFM or L/s. For constant volume systems this
will be equal to the zone design supply airflow
rate, Vz. For VAV systems, it will be a
Page 21 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Fan Airflow Sizing Calculations for Fan Powered Mixing Boxes
29.0 System Design Calculations ›› 29.3 Zone Equipment Sizing Calculations ››
29.4 System and Fan Airflow Sizing Calculations
29.0 System Design Calculations ››
System Airflow Sizing Calculations
29.0 System Design Calculations ›› 29.4 System and Fan Airflow Sizing Calculations ››
minimum value based on the design supply
airflow rate and the minimum terminal damper
position specified by the user.
Vw
=
Required water flow rate, gpm or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Airflow Sizing Calculations for Fan Powered Mixing Boxes
This help topic describes the procedures used to calculate the required fan airflow rate for terminal fans
located in fan powered mixing box terminals. Separate procedures are used for series and parallel mixing
boxes.
A. Series Fan Powered Mixing Box Terminals
For a series fan powered mixing box, the mixing box fan receives the full zone airflow. Therefore, the fan in
this type of mixing box must be sized as:
Vmbf = Vz
B. Parallel Fan Powered Mixing Box Terminals
For a parallel fan powered mixing box, the mixing box fan is out of the zone air stream. According to common
industry practice it is sized for standalone heating operation in the unoccupied period when the primary portion
of the system is off. Therefore, the airflow at the specified heating supply temperature must be sufficient to
offset the design heat loss in the zone, assuming the zone is at the unoccupied heating setpoint:
Vmbf = Qzh / (ρaCpaK (Tsh,mbx - Tzh,unocc))
C. Variable Definitions
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qzh
=
Zone design heating load, BTU/hr or W.
Tzh,unocc
=
Zone unoccupied heating thermostat setpoint, F or C.
Tsh,mbx
=
Design heating supply air temperature for parallel fan
powered mixing box unit, F or C.
Vmbf
=
Mixing box fan required airflow, CFM or L/s.
Vz
=
Zone design supply airflow rate, CFM or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculation procedures for system-level airflow rates.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 22 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
System Airflow Sizing Calculations
This help topic documents procedures used to compute system supply airflow rates and supply temperatures.
Separate sections below discuss sizing calculations for:
1. Single-duct CAV systems.
2. Single-duct VAV systems.
3. Multizone and Dual Duct CAV systems.
4. Dual duct VAV systems.
Variables used in equations in the following discussions are defined at the end of this topic.
A. Supply Air Calculations for Single-Duct CAV Systems
This section describes supply air calculations for the following single-duct CAV systems: Single Zone CAV,
CAV Terminal Reheat, Packaged DX Fan Coil, Split DX Fan Coil, Water Source Heat Pump, 2-Pipe Fan Coil
and 4-Pipe Fan Coil systems. Calculations are described below.
Calculation of Supply Airflow Rate. When supply temperature is specified as the sizing criteria, the system
supply airflow rate is computed by summing required zone airflow rates for all zones in the system. Because
the airflow at the outlet of the air handling unit is needed, extra airflow capacity must be added to overcome
supply duct leakage, if leakage exists. The following equation is used:
Vsys = (Sum of Vz, all zones) / (1 - Fl/100)
When supply CFM/sqft or L/s/sqm is specified as the sizing criteria, the system airflow rate is computed as:
Vsys = (CFM/sqft or L/s/sqm) Asys
When supply CFM or L/s is specified as the sizing criteria no calculations are needed. The specified value is
used directly.
After calculating Vsys, it is compared with the required outdoor ventilation airflow rate. If Vsys is smaller than
the required ventilation airflow, it is increased to equal the ventilation airflow rate. Ventilation airflow is given
higher priority since it is often mandated by building codes.
Calculation of Supply Air Temperature. When CFM, L/s, CFM/sqft or L/s/sqm is specified as the supply air
sizing criteria, the program must calculate the design supply air temperature. This is done by first calculating
the required supply air temperature for each zone. The coldest zone supply temperature is chosen as the
required supply temperature at zone terminals. The required supply temperature for each zone is computed
using the following equation:
Tsc = Tzc - Qzc / (ρaCpaK Vz)
When the supply temperature is specified as the sizing criteria, no calculations are necessary. The specified
supply temperature is used directly. Note that all design heating systems fall into this category; heating supply
temperature must be specified for these systems.
B. Supply Air Calculations for Single-Duct VAV Systems
This section describes supply air calculations for single-duct VAV systems and VVT systems. Calculations are
described below.
Calculation of Supply Airflow Rate. For VAV systems a maximum diversified supply airflow rate is computed
using the following five step procedure:
1. The required airflow rate at each zone terminal is computed for each cooling design hour using the zone
sensible cooling load and the design supply air temperature. The following equation is used:
Vz,hr = Qzc,hr / [ ρaCpaK (Tzc – Tsc) ]
2. If necessary the calculated value of Vz,hr is adjusted when it is less than the minimum airflow for the VAV
terminal.
3. All zone airflow rates are then added together to obtain a system total.
4. The system total is adjusted to account for duct leakage, if necessary. The result is the system airflow rate
at the outlet of the central air handling unit. The following equation is used to make this adjustment:
Page 23 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Vsys,hr = (Sum of Vz,hr, all zones) / (1 - Fl/100)
5. Steps 1-4 are repeated for all hours for all months included in the design cooling analysis. Resulting hourly
system airflow rate values, Vsys,hr, are inspected to identify the maximum system airflow. This value is the
maximum diversified airflow for the system.
The following example illustrates this process for a simple case in which a VAV air system serves two zones,
and loads for only one design cooling month are considered in the analysis.
1. Figure 1 shows zone sensible cooling load profiles for the two zones served by the system. Zone 1 faces
east and therefore has a peak load early in the day. Zone 2 faces west and has a peak load later in the day.
Figure 2 shows the resulting hourly zone airflow rates calculated from these zone loads.
2. For several hours during the night, the airflow computed from the zone load drops below the minimum zone
airflow. Therefore, these zone airflow rates are adjusted upward to equal the minimum zone airflow.
3. Hourly zone airflow rates for the two zones are added together to determine a system total airflow rate, as
shown in Figure 3.
4. Hourly system airflow rates are adjusted for 5% duct leakage to determine the required system airflow rates
at the outlet of the air handling unit, as shown in Figure 3.
5. The maximum system airflow rate occurs at 5pm and is 2394 CFM.
In this example zone 1 has a peak airflow rate of 1198 CFM at 10am. Zone 2 has a peak airflow rate of 1446
CFM at 6pm. The overall system airflow (before duct leakage adjustments) peaks at 2274 CFM at 5pm. Thus
the diversified airflow requirement for the VAV system (2274 CFM) is about 14% less than the sum of the peak
zone airflow rates (2644 CFM) that would be required for a CAV system. Finally, duct leakage increases the
required system supply airflow to 2394 CFM.
Page 24 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Page 25 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Calculation of Supply Air Temperature. For all VAV air systems, supply temperature must be specified as
the sizing criteria. Therefore, calculation of the supply temperature is not required.
C. Supply Air Calculations for Multizone and Dual Duct CAV
This section discusses supply air calculations for the 2-Deck Multizone, 3-Deck Multizone and Dual Duct CAV
systems.
Calculation of Supply Airflow Rate. The required cold deck airflow rate is computed using the procedure
outlined section A for single duct CAV cooling-only and cooling-and-heating systems. The required hot deck
airflow rate is computed during simulation of system operation for the design heating condition.
Calculation of Supply Air Temperature. For these systems, the cold deck and hot deck supply temperatures
must be specified as the sizing criteria. Therefore, calculation of these supply temperatures is not required.
D. System Supply Calculations for Dual Duct VAV Systems
This section discusses supply air calculations for 1-Fan Dual Duct VAV and 2-Fan Dual Duct VAV systems.
Calculation of Supply Airflow Rate. For both systems, the required cold deck airflow rate is computed using
the procedure outlined section B for single duct VAV systems. For 1-Fan Dual Duct VAV systems, the required
hot deck supply airflow rate is determined from a simulation of system operation for the design heating
condition. For 2-Fan Dual Duct VAV systems, the required hot deck airflow rate is computed using the
following three step procedure:
1. The required hot deck supply airflow rate for a zone is computed using the equation below. This equation
accounts for the fact that sufficient hot deck air must be provided to meet both the design zone heating load
and the heating load due to the minimum flow of primary air into the zone.
Page 26 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Vz,hd = [ρaCpaK Vcd,min (Tzh - Tcd) + Qzh] / [ρaCpaK(Thd - Tzh)]
2. Step 1 is repeated for all zones. The resulting Vz,hd values are then added together for all zones in the
system to obtain the total hot deck airflow required.
3. Finally, the hot deck airflow is adjusted for supply duct leakage, if necessary. The following equation is
used:
Vhd = (Sum of Vz,hd, all zones) / (1 - Fl/100)
Calculation of Supply Air Temperature. For these systems, the cold deck and hot deck supply temperatures
must be specified as the sizing criteria. Therefore, calculation of these supply temperatures is not required.
E. Variable Definitions
Asys
=
Total floor area served by air system, sqft or sqm.
Fl
=
Supply duct leakage rate, percent.
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qzh
=
Design heating load for zone, BTU/h or W.
Qzc
=
Maximum zone sensible cooling load, BTU/h or W.
Qzc,hr
=
Zone sensible cooling load for a specific hour, BTU/hr or
W.
Tcd
=
Cold deck supply temperature, F or C.
Thd
=
Hot deck supply temperature, F or C.
Tsc
=
Required cooling supply temperature at zone terminal, F or
C. Note that if duct heat gain is considered, a
colder temperature will be required at the
outlet of the central air handling unit.
Tsh
=
Required heating supply temperature at zone terminal, F
or C. Note that if duct heat loss is considered,
a warmer temperature will be required at the
outlet of the central air handling unit.
Tzc
=
Occupied period cooling thermostat setpoint for zone, F or
C.
Tzh
=
Occupied period heating thermostat setpoint for zone, F or
C.
Vcd,min
=
Minimum cold deck supply airflow rate to zone, CFM or
L/s. Computed by multiplying the design zone
supply airflow rate, Vz, by the minimum
terminal damper position specified by the user.
Vhd
=
Required hot deck supply airflow rate, CFM or L/s.
Measured at the outlet of the hot deck.
Vsys
=
System supply airflow rate, CFM or L/s. For central
systems, this is the airflow rate at the outlet of
the air handling unit. For terminal systems
such as fan coils or water source heat pumps,
it is the supply airflow for the terminal unit.
Vsys,hr
=
Required system airflow rate for a specific hour, CFM or
L/s. Measured at the outlet of the central air
handling unit.
Vz
=
Required zone supply airflow rate, CFM or L/s. This is the
airflow at the zone terminal.
Vz,hr
=
Required zone supply airflow rate for a specific hour, CFM
or L/s. Measured at the zone terminal.
Vz,hd
=
Required hot deck airflow rate at the design heating
condition for a zone, CFM or L/s.
Page 27 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Supply Fan Sizing Calculations
29.0 System Design Calculations ›› 29.4 System and Fan Airflow Sizing Calculations ››
Return Fan Sizing Calculations
29.0 System Design Calculations ›› 29.4 System and Fan Airflow Sizing Calculations ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supply Fan Sizing Calculations
This help topic discusses procedures used to size the supply fan airflow rate. Procedures for the supply fan in
each type of system offered in HAP are listed below. Further details on each procedure are found in the
section of the help topic System Airflow Sizing Calculations indicated in the right-hand column of the table.
Procedures used to size the supply fan in a 4-Pipe Induction system are described in a separate help topic.
System Type
Required Supply Fan Airflow is
Equal To:
Details Provided in
System Airflow
Sizing Help Topic
Section:
CAV Single Zone
System supply airflow rate
A
CAV with Terminal Reheat
System supply airflow rate
A
CAV 2-Deck Multizone
Cold deck supply airflow rate
C
CAV 3-Deck Multizone
Cold deck supply airflow rate
C
CAV Dual Duct CAV
Cold deck supply airflow rate
C
CAV 4-Pipe Induction
User-defined ventilation airflow rate
VAV
Diversified supply airflow rate
B
VAV 1-Fan Dual Duct
Diversified supply airflow rate
B
VAV 2-Fan Dual Duct
Cold Deck: Supply airflow rate
D
VAV 2-Fan Dual Duct
Hot Deck: Supply airflow rate
D
VVT
Diversified supply airflow rate
B
Packaged DX Fan Coil
System supply airflow rate
A
Split DX Fan Coil
System supply airflow rate
A
Water Source Heat Pumps
System supply airflow rate
A
2-Pipe Fan Coil
System supply airflow rate
A
4-Pipe Fan Coil
System supply airflow rate
A
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Return Fan Sizing Calculations
The required airflow rate for a return fan is calculated using the system supply airflow rate:
Vrf = Vsys
This represents the worst case airflow for the return fan. In systems which directly exhaust air from zones a
lower airflow will exist for the return fan during occupied hours (supply airflow minus direct exhaust). But during
unoccupied hours when the ventilation dampers are closed, no air is directly exhausted and the return fan will
have to handle the full supply airflow rate.
Page 28 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Outdoor Ventilation Airflow Calculations
29.0 System Design Calculations ›› 29.4 System and Fan Airflow Sizing Calculations ››
where:
Vrf
=
Required return fan airflow rate, CFM or L/s.
Vsys
=
System supply airflow rate, CFM or L/s. For central
systems, this is the airflow rate at the outlet of
the air handling unit.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Outdoor Ventilation Airflow Calculations
This help topic documents how the required outdoor ventilation airflow rate is calculated. Control of outdoor
ventilation air during off-design times is described in a separate help topic.
Overview
The general procedure for calculating the outdoor ventilation airflow requirement for a system is as follows:
1. Calculate outdoor ventilation airflow for each space served by the system based on outdoor air
requirements defined by the user.
2. If the system uses the "Sum of Space OA Airflows" method for sizing ventilation air, sum the outdoor airflow
requirements for all spaces to obtain the system outdoor airflow rate.
3. If the system uses the "ASHRAE Std 62-2001" or the "ASHRAE Std 62-2001 (max only)" method, the
ASHRAE Standard 62-2001 Ventilation Rate Procedure (Section 6.1) is used to determine the outdoor
airflow requirements for all spaces and for the system. The Multiple Spaces portion of the Ventilation Rate
Procedure is designed to ensure that all spaces in a multiple-space system receive their required outdoor
airflow.
4. If the system uses the one of the ASHRAE Standard 62.1 methods (2004, 2007, 2010, 2013, or 2016), the
Ventilation Rate Procedure (Section 6.2 and Appendix A) from the Standard 62.1 is used to determine
outdoor airflow requirements for all spaces and the system.
These four steps are described in greater detail in separate sections below.
A. Calculating Space Ventilation Requirements
1. Define Space Requirements. One or two outdoor airflow requirements are defined by the user for each
space served by a system. The units of measure for these requirements can be CFM/person, CFM/sqft,
CFM or % of supply air. In SI Metric units the choices are L/s/person, L/s/sqm, L/s or % of supply air.
2. Calculate Uncorrected Space Outdoor Airflows. The specifications from step 1 are used to determine the
space outdoor airflow requirement in CFM or L/s. If only one requirement is defined for the space, it alone
establishes the outdoor airflow for the space. If two requirements are specified, then the sum of these
requirements establishes the outdoor airflow for the space. Calculations for the four different units of
measure options are as follows:
English Units
Outdoor CFM = (CFM/person) x (Maximum Occupants in Space)
Outdoor CFM = (CFM/sqft) x (Space Floor Area in sqft)
Outdoor CFM = (CFM specified by user)
Outdoor CFM = (% of Supply Air) x (Space Maximum Supply Airflow)
SI Metric Units
Page 29 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Outdoor L/s = (L/s /person) x (Maximum Occupants in Space)
Outdoor L/s = (L/s /sqm) x (Space Floor Area in sqm)
Outdoor L/s = (L/s specified by user)
Outdoor L/s = (% of Supply Air) x (Space Maximum Supply Airflow)
Note: For Standard 62.1 (2004, 2007, 2010, 2013, 2016 editions) uncorrected space outdoor airflow
calculation involves additional considerations not addressed here. Please see section D below for details.
B. Calculating System Ventilation Airflow by Summation Method
If the "Sum of Space OA Airflows" method is specified for a system, the total outdoor airflow rate for the
system is simply the sum of outdoor airflows for spaces served by the system. This "summation" method is
used in many jurisdictions not subject to ASHRAE Standard 62.1 and is also typically used in jurisdictions not
subject to any formal ventilation code.
Required Outdoor Airflow for System = (Sum of Required Outdoor Airflows for all Spaces)
C. Calculating System Ventilation Airflow by ASHRAE Std 62-2001
If the "ASHRAE Std 62-2001" or "ASHRAE Std 62-2001 (max only)" method is specified for sizing ventilation
airflow, the total outdoor airflow rate for the system is determined using the Ventilation Rate Procedure from
ASHRAE Standard 62-2001 Section 6.1. The Multiple Spaces portion of this procedure is designed to ensure
that all spaces in a multiple space system receive their required outdoor airflow rates. The discussion below
summarizes how the calculation is performed. The discussion assumes the reader has a basic familiarity with
Standard 62-2001 provisions and concepts.
VAV systems. Standard 62 requires the minimum outdoor airflow rates listed in Table 2 of the Standard be
provided to spaces in a system at all times. However, the Standard is not specific about procedures required
to ensure this for VAV systems. One formal request for interpretation of the Standard asked if ventilation
airflow requirements should be calculated at minimum VAV box position. The response from the Standard 62
committee indicated this was an acceptable approach, but other acceptable approaches also existed. For VAV
systems, HAP performs the Multiple Spaces portion of the Ventilation Rate Procedure for both "terminal boxes
full open" and "terminal boxes at minimum flow" conditions and then chooses the larger ventilation airflow rate
as the requirement for the system. HAP also gives users the option of choosing an "ASHRAE Std 62-2001
(max only)" sizing method which will only consider the "terminal boxes full open" condition for sizing
calculations. This extra option is to provide a designer with the flexibility to choose what he or she feels is the
most suitable approach to compliance. Because the Standard is not specific about VAV applications,
engineering judgement must be used to choose the most suitable approach.
For constant volume systems, and for VAV systems for the "terminal boxes full open" condition, the Ventilation
Rate Procedure is performed as follows:
1. Calculate Uncorrected Outdoor Airflow Fraction Z. Z is calculated for each space in the system as
follows:
Z = (Uncorrected Outdoor Airflow for Space) / (Maximum Supply Airflow for Space)
2. Identify Critical Space. Identify the space having the largest Z fraction among all spaces served by the
system. This is the "critical space".
3. Calculate Uncorrected Outdoor Airflow Fraction X.
Total Uncorrected Outdoor Airflow = Sum of Uncorrected Outdoor Airflow for all Spaces.
Total Maximum Supply Airflow = Sum of Maximum Supply Airflow for all Spaces
X = (Total Uncorrected Outdoor Airflow) / (Total Maximum Supply Airflow)
Page 30 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
4. Calculate Corrected Outdoor Airflow Fraction Y. Y is the ratio of corrected outdoor airflow for the system
divided by total supply airflow for the system. It is calculated using Equation 6-1 in the Standard:
Y = X / [1 + X – Z]
Discussion: All spaces receive supply air containing one uniform percentage of outdoor air. Therefore, the
critical space, which requires the highest percentage of outdoor air, influences the mixture of outdoor air
delivered to all other spaces. For example, if the critical space requires 50% outside air in its supply airflow,
and other spaces require 25%, a simplistic view is that all spaces must receive a 50% mixture of outdoor air
so that the critical space is satisfied. However, this oversupplies outdoor air to the non-critical spaces. The
Standard allows a credit for the fact that some outdoor air delivered to non-critical spaces is unused or
"unvitiated" and that some of this unvitiated air is recirculated. Therefore, the percentage of outdoor air in
supply air can be below that required by the critical space and still satisfy the critical space requirements.
Both the critical space and the unvitiated air considerations are incorporated in Equation 6-1 above. Thus,
using our simple example, it may be possible for a 38% mixture of outdoor air in supply air to satisfy both
the 50% critical space requirement (due to unvitiated recirculated air) and the non-critical space
requirements.
5. Calculate Corrected Outdoor Airflow for Spaces and System. Finally, use the Y factor to determine the
corrected outdoor airflow requirements for spaces and the system:
Corrected Outdoor Airflow For Space = Y x {Maximum Supply Airflow for Space}
Corrected Outdoor Airflow for System = Y x (Maximum Supply Airflow for System}
Or
Corrected Outdoor Airflow for System = {Sum of Corrected Outdoor Airflow Rates for Spaces}
For constant volume systems and for VAV systems using the "ASHRAE Std 62-2001 (max only)" sizing
method, the calculation stops at this point.
For VAV systems using the "ASHRAE Std 62-2001" sizing method, HAP repeats steps 1 thru 5 above using
the minimum space supply airflow rate in each place where the maximum space supply airflow is mentioned.
This represents a "terminal boxes at minimum flow" design condition. This yields a second corrected outdoor
airflow value for the system. The outdoor airflow results from "terminal boxes full open" and from "terminal
boxes at minimum position" are compared. The larger value is chosen as the outdoor airflow requirement for
the system.
Note: If the calculated outdoor ventilation airflow is less than the direct exhaust airflow total for all zones in the
system, the program overrides the calculated value and sets ventilation airflow equal to direct exhaust airflow.
Example: Based on a 25 CFM/person ventilation specification, the program calculates that 5000 CFM of
ventilation air is required. However, the total amount of direct exhaust air specified for zones in the system
is 6500 CFM. Therefore, the program overrides the ventilation calculation and uses 6500 as the required
ventilation airflow rate.
D. Calculating System Ventilation Airflow by ASHRAE Standard 62.1 (2004, 2007, 2010, 2013, 2016
editions)
If the one of the ASHRAE Standard 62.1 methods (2004, 2007, 2010, 2013, 2016) is specified for sizing
ventilation airflow, the total outdoor airflow rate for the system is determined using the Ventilation Rate
Procedure from section 6.2 and Appendix A of the named Standard. The discussion below summarizes how
the calculation is performed. This discussion assumes the reader has a basic familiarity with Standard 62.1
provisions and concepts.
Notes About Terminology:
1. The term "zone" is used throughout ASHRAE Standard 62.1 to refer to what HAP identifies as a "space". To
avoid confusion, the following discussion will adopt HAP's terminology. For example, what the Standard
refers to as a "zone ventilation efficiency" will be referred to here as "space ventilation efficiency" for clarity.
2. In Standard 62.1 the Ventilation Rate Procedure is performed separately for each "ventilation system". A
"ventilation system" is a fan system providing air to one or more spaces. Therefore one Standard 62.1
Page 31 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
sizing calculation is performed for each central system such as a CAV, VAV, VVT, dual duct or triple duct
system. In terminal systems such as fan coils, water source heat pumps, VRF, PTAC, induction beam or
active chilled beam systems, one Standard 62.1 calculation is performed separately for each terminal unit
zone, and a separate calculation is performed for the dedicated outdoor air system (DOAS), if applicable..
Overview. The Standard 62.1 procedure involves two fundamental calculation steps. First the required
breathing zone ventilation airflow rate (Vbz) is calculated for each space based on the CFM/sqft (L/s/sqm) and
CFM/person (L/s/person) requirements for that space. Second, the calculation determines how much outdoor
ventilation air is required at the central system outdoor air intake (Vot) to ensure that each space receives its
required breathing zone ventilation. Often the ventilation airflow required at intake is larger than the sum of the
breathing zone airflows. The amount of increase in airflow depends on critical space issues and the air
distribution effectiveness of the system and its air terminals.
a. The Critical Space concept existed in earlier editions of the Standard, but the mathematics for handling it
are different beginning in the 2004 edition. "Critical Space" involves a concept that meeting the ventilation
requirements of one space may require overventilating other spaces. Suppose space A has a supply airflow
of 800 CFM and requires 200 CFM of outside air, or 25% of supply. Suppose space B has a supply airflow
of 600 CFM and requires 300 CFM of outside air, or 50% of supply. Both spaces receive supply air from the
same AHU. If that supply air contains 25% ventilation air, the ventilation requirement of Space A will be met,
but the ventilation requirement of Space B will not be met. The common supply air must contain more than
25% outdoor air in order meet Space B requirements. This will overventilate Space A. However, once
Space A is overventilated, there is unused or "unvitiated" ventilation air that recirculates from Space A and
that moderates the need to increase supply air all the way to 50% ventilation. In this example Space B is
the critical space. The Standard 62.1 ventilation sizing calculation analyzes the requirements of all the
spaces to determine whether overventilation is necessary and if so, how much is needed to ensure that all
spaces receive their required ventilation airflow.
b. The Air Distribution Effectiveness is a also new concept in the 2004 edition. In the 2004 and later editions
it is not enough to simply deliver ventilation air to a space. That air must reach the breathing zone of its
occupants. Based on the location of supply outlets and return grilles, and on whether cold air or hot air is
being delivered, different applications are more or less effective at delivering ventilation air to the breathing
zone. Therefore, the effectiveness of the equipment is considered in calculating ventilation requirements.
Both the critical space and air distribution effectiveness considerations are built into a "space ventilation
efficiency" value calculated for each space. The critical space is the one having the lowest ventilation
efficiency. This critical space ventilation efficiency is used to correct the original uncorrected airflow
requirements to obtain the total ventilation airflow required at the system intake.
This entire calculation is performed twice - once for the design cooling condition and once for the design
heating condition. The results of the two calculations are compared and the larger value is used as the
required outdoor air intake flow (Vot) for the system. The worst case scenario is the one reported on the
Ventilation Sizing Summary Report.
Steps in the calculation process are summarized below. The first step calculates the breathing zone outdoor
airflow for each space. The remaining steps are needed to derive the system ventilation efficiency and
compute the total system ventilation airflow requirement.
1. Calculate "Breathing Zone Outdoor Air" for Each Space. (6.2.2.1 and 6.2.6.2).
Vbz = Rp Pz + Ra Az
or
Vbz = (CFM/person)(People) + (CFM/sqft)(Floor Area)
Vbz = (L/s/person)(People) + (L/s/sqm)(FloorArea)
where:
Vbz = Breathing zone outdoor airflow for space
Rp = Outdoor airflow per person requirement.
Pz = Space population.
Ra = Outdoor airflow per unit floor are requirement
Az = Floor area for space.
The space population, Pz, is calculated as:
Page 32 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Pz = (Maximum Occupants Specified) x (Time Averaging Factor).
If the number of people in the space fluctuates over time, the Standard allows the space population to be
estimated using an averaging procedure. First, the time averaging interval is calculated using equation 6-9a
in paragraph 6.2.6.2 of the standard. The interval is a function of the ventilation air change for the space.
Then average occupant schedule values are calculated for this interval and the largest average value is
used to determine the time averaging factor.
Example: A 2000 sqft space, with floor to ceiling height of 9 ft, has 10 occupants. The requirements for this
space are 5 CFM/person and 0.06 CFM/sqft. Using 10 occupants and 2000 sqft, the uncorrected outdoor
airflow (Vbz) is 170 CFM. The time averaging interval is 3 x Space Volume / Vbz which equals 318 minutes
or 5.3 hours. This is rounded to 5 hours. Next the program calculates an average schedule factor for each
group of 5 consecutive hours in the design day schedule. First hours 0000 thru 0400 are used, then 0100
thru 0500, then 0200 thru 0600, etc... For example, if the schedule values for five consecutive hours are
60%, 80%, 100%, 100% and 100%, the average for this block is 88%. Once averages are calculated for
each 5-hour block in the day, the largest average is used as the Time Averaging Factor.
Notes:
a. When demand controlled ventilation (DCV) control is used, ASHRAE Standard 62.1 does not permit time
averaging to be applied. This restriction is stated in the 62.1 User's Manual for Standard 62.1.
Therefore HAP does not calculate time averaging for that case.
b. If your occupant schedule uses 100% for all hours of the day, the Time Averaging factor will be 100%.
As a result, there is no reduction in the number of occupants used in the calculation of required
ventilation airflow.
c. Also note that only CFM/person (L/s/person) and CFM/sqft (L/s/sqm) airflow requirements are used in
this calculation. If you have specified a total airflow (CFM or L/s) or "% of supply airflow" ventilation
requirement for the space, these values will not be considered in the calculation as they are outside the
scope of the Standard 62.1-2004 Ventilation Rate procedure.
2. Determine Space Air Distribution Effectiveness (6.2.2.2)
The space air distribution effectiveness measures the ability of the air distribution system to deliver
ventilation air into the breathing zone of the space. Effectiveness values are provided in Table 6-2 in the
2004, 2007, and 2010 editions of the Standard, and in Table 6.2.2.2 in the 2013 and 2016 editions.
If the source of air distribution effectiveness for a zone is specified as Standard 62.1, HAP will assign a
value based on the specified locations of supply discharge and return grille, the cooling and heating
capabilityof the system, and the heating supply temperature and heating thermostat setpoint (as applicable)
using data from Table 6-2 / 6.2.2.2. The following table is a synthesis of air distribution effectiveness data
from Table 6-2 / 6.2.2.2.
Operating
Mode
Supply Air
Location
Return Grille
Location
Other
Conditions
Air
Distribution
Effectiveness
(Ez)
Cooling (1)
Ceiling (3)
Ceiling
-
1.0
Cooling
Ceiling
Floor
-
1.0
Cooling
Floor (4)
Floor
-
1.0 (5)
Cooling
Floor
Ceiling
Supply air
throw > 15
ft/min at 4.5 ft
height
1.0
Cooling
Floor
Ceiling
Low velocity
displacement
ventilation with
supply air
throw =< 15
ft/min at 4.5 ft
height
1.2
Page 33 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Heating (2)
Ceiling
Ceiling
Supply-to-room
delta-T < 15 F
1.0
Heating
Ceiling
Ceiling
Supply-to-room
delta-T >= 15 F
0.8
Heating
Ceiling
Floor
-
1.0
Heating
Floor
Floor
-
1.0
Heating
Floor
Ceiling
-
0.7
Notes:
(1) Cooling indicates air cooler than space air temperature is supplied.
(2) Heating indicates air warmer than space air temperature is supplied.
(3) Ceiling includes any point above the breathing zone which is from 3 in to 72 in above the floor.
(4) Floor includes any point below the breathing zone.
(5) Standard 62.1 does not specify any air distributiion effectiveness for this case with cooling operation, supply air at floor level, and
return grille at ceiling level. HAP applies an Ez value of 1.0 for this case on the principle that cool supply air is delivered into the
breathing zone and is returned from a location near the breathing zone. Therefore all delivered ventilation air reaches the breathing
zone.
Finally, if the source of air distribution effectiveness for a zone is specified as "user-defined", then the user-
specified air distribution effectiveness value for the zone is used without consideration of Table 6-2 /
6.2.2.2..
3. Calculate Space Outdoor Airflow (6.2.2.3)
The required outdoor air for the space is calculated by dividing the breathing zone outdoor air by the space
air distribution effectiveness.
Voz = Vbz / Ez
where
Voz = Space outdoor airflow..
Vbz = Breathing zone outdoor airflow.
Ez = Air distribution effectiveness for space.
4. Simple Cases
If the system serves a single space, the outdoor air intake flow equals Voz for that single space: Vot = Voz.
(6.2.3)
For a 100% outdoor air system serving one or more spaces, the outdoor air intake flow equals the sum of
Voz airflows for all spaces. (6.2.4)
For any system serving multiple spaces where outdoor is less than 100% of supply air, the additional
calculation steps below are required.
5. Calculate the Primary Outdoor Air Fraction for Each Space. (6.2.5.1)
The primary outdoor air fraction defines ventilation air as a percentage of supply air to the space. It is
calculated as:
Zp = Voz / Vpz
where
Zp = Primary outdoor air fraction.
Voz = Space outdoor airflow.
Vpz = Primary supply airflow for space.
For constant volume (CAV) systems the design supply airflow is used as Vpz. For variable volume (VAV)
systems, the Standard requires that minimum primary supply airflow be used.
6. Calculate System Ventilation Efficiency (6.2.5.2 and Appendix A)
As mentioned earlier in the Overview paragraph, the system ventilation efficiency accounts for critical space
issues.
Page 34 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Procedures in Appendix A of the Standard are used by HAP to calculate a space ventilation efficiency for
each space. The space having the lowest ventilation efficiency is identified as the critical space. The critical
space ventilation efficiency is used as the system ventilation efficiency. Calculation of space ventilation
efficiency uses a lengthy series of equations which will not be reproduced here. The reader is directed to
Appendix A of the Standard for full details.
The space ventilation efficiency represents the ratio of airflow at system intake required to ensure the
proper amount of ventilation air reaches the space divided outdoor airflow required at the space. For
example, if a space requires 200 CFM of outdoor air and has a ventilation efficiency of 0.75, 200/0.75 or
267 CFM of outdoor air must be introduced at the system intake to ensure that the space receives its 200
CFM of outdoor air. Therefore, the space with the lowest ventilation efficiency dictates the overall outdoor
airflow for the system since it will require the largest amount of over ventilation of other spaces to ensure it
receives its required airflow.
Note that the Standard provides two methods for determining System Ventilation Efficiency. The simplified
approach is to use efficiency values from Table 6-3 of the Standard. While this approach is simple, it tends
to result in a system ventilation airflow that is not optimized. The second approach is to use Appendix A.
While this approach is more computationally difficult, it tends to optimize the resulting system ventilation
airflow. Since a computer is performing the calculations, the Appendix A approach was selected for use
here.
7. Calculate System Uncorrected Outdoor Intake Airflow (6.2.5.3)
The total uncorrected outdoor air intake airflow for the system is the sum of uncorrected airflows for spaces
in the system, accounting for diversity, if necessary. The Standard refers to this as the "uncorrected outdoor
air intake", Vou. It is calculated as:
Vou = D (sum of RpPz all spaces) + (sum of RaAz all spaces)
where:
Vou = Uncorrected outdoor airflow rate for system.
D = Diversity factor.
Rp = Per person ventilation requirement for space.
Pz = Space population, calculated as described in item 1 above.
Ra = Per area ventilation requirement for space.
Az = Floor area of space.
If you specified the same diversity factor (or used the default of 100%) for all zones in your air system on
the Zone Components tab, Thermostats data view, then D equals the value you specified. If you specified
different diversity factors for individual zones in your air system then D is calculated as:
D = (sum of {diversity factor x Pz), all spaces) / (sum of Pz, all spaces)
where Pz is the space population whose calculation was discussed earlier in item 1.
8. Calculate Outdoor Air Intake Airflow Rate for System (6.2.5.4)
Finally the design ventilation rate for the system can be calculated. The standard refers to this value as
"outdoor air intake", Vot. It is calculated as:
Vot = Vou / Ev
where
Vot = Outdoor air intake flow rate for the system.
Vou = Uncorrected outdoor air intake flow rate for system (discussed in item 7)
Ev = System efficiency (discussed in item 6)
Note: If the required outdoor ventilation airflow for the system is less than the total direct exhaust airflow for
the system, the program overrides the calculated value and sets ventilation airflow equal to direct exhaust
airflow.
Example: Based on the Standard 62.1 calculation calculates that 5000 CFM of ventilation air is required for
the system. However, the total amount of direct exhaust air specified for zones in the system is 6500 CFM.
Therefore, the program overrides the ventilation calculation and uses 6500 as the required ventilation
airflow rate.
Page 35 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
29.5 Sizing Calculations for Induction Systems
29.0 System Design Calculations ››
Sizing Calculations for Induction Beams and Active Chilled Beams
29.0 System Design Calculations ›› 29.5 Sizing Calculations for Induction Systems ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains sizing procedures for induction and active chilled beam air systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Sizing Calculations for Induction Beams and Active Chilled Beams
The configuration of components and operating principles of Induction Beam and Active Chilled Beam systems
differ significantly from other types of HVAC systems. As a result special sizing procedures are required, as
described below. Definitions of variables used in equations are found at the end of this topic.
1. Primary Supply Airflow. During occupied period operating hours, primary supply airflow to the terminals is
100% outdoor air. Primary airflow is calculated as the larger of the outdoor ventilation airflow requirement
or the primary air required to achieve the supply airflow rate necessary to meet the peak zone sensible
load.
First the primary airflow is calculated as the outdoor ventilation airflow requirement for the zone.
Vpz1 = Voa
where Voa is computed based on the chosen ventilation sizing method:
a. Sum of Space OA Airflows. With this method the primary airflow for a zone is the sum of the outdoor
air ventilation requirements for spaces in the zone.
b. ASHRAE Standard 62-2001 or Standard 62.1 (2004, 2007, 2010, 2013 editions) With this method the
Standard 62 or 62.1 Ventilation Rate Procedure is applied to each zone in the system to determine its
primary airflow requirement. Because the zone terminal receives 100% outside air, the zone is
considered a "system" for Standard 62 or 62.1 ventilation calculation purposes.
Second, the primary airflow required for peak cooling is calculated:
Vsz = Qz,peak clg / [ ρa Cpa K (Tzc - Tzdcs) ]
Vpz2 = Vsz / Rair
Third, if the terminal provides heating, the primary airflow required for peak heating is calculated:
Vsz = Qzc,peak htg / [ ρa Cpa K (Tzdhs - Tzh) ]
Vpz3 = Vsz / Rair
Finally, the three primary airflow values, Vpz1 , Vpz2 , Vpz3 , calculated above are compared and the
largest value is chosen as the design value for the zone, Vpz.
2. Ventilation Fan. The required airflow rate for the ventilation AHU fan is calculated by summing the primary
supply airflows for all zones:
Vvf = (Sum of Vpz all zones)
Page 36 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
3. Exhaust Fan. The required airflow rate for the exhaust fan is set equal to the airflow for the ventilation fan.
4. Terminal Unit Cooling Coil Capacity. The required cooling coil capacity for each zone terminal is
determined from simulations of system operation for all hours on design cooling days. For each hour, the
simulation determines the zone cooling demand, the cooling contribution of primary air and the load on the
terminal cooling coil. The program then scans the hourly results to identify the largest cooling coil load
among the hours simulated and reports that as the peak coil load along with its associated coil entering and
coil leaving temperatures. During these simulations the terminal coil calculations are as follows:
Determine total supply airflow rate for the zone, Vsz from the primary supply air Vpz and the induction ratio
Rair:
Vsz = Vpz Rair
Determine the required supply air temperature for the current hour, solving the following equation for the
zone cooling supply air temperature, Tzcs:
Qzc,clg = ρa Cpa K Vsz (Tzone - Tzcs)
Calculate the induced airflow through the terminal, Vi:
Vi = Vsz - Vpz
Determine the required cooling coil outlet dry-bulb temperature, Tcco. Cooling coil outlet air mixes with
primary air before being delivered to the zone, so the following mixed air equation is solved for Tcco:
Tzcs = (VpzTps,c + ViTcco) / Vsz
Then solve for the cooling coil sensible load, Qcoil,c,s:
Qcoil,c,s = ρa Cpa K Vi (Tzone - Tcco)
An active chilled beam is a sensible-only cooling terminal, so the cooling coil sensible load is the only load
calculated for the terminal.
Because it is equipped with a drain pan, an induction beam is a total cooling terminal, able to provide both
sensible and latent cooling. Therefore, for induction beam terminals, the required latent cooling load is also
calculated. The latent cooling equations are summarized below. A detailed explanation of latent
calculations is found here: Cooling Coil Load Calculations
Qcoil,c,l = ρa hfg K Vi (ωzone - ωcco)
ωcco = BF (ωzone - ωadp) + ωadp
ωcco is the saturation specific humidity at Tadp
Tadp = (Tcco - TzoneBF) / (1 - BF)
5. Terminal Unit Heating Coil Capacity. The required heating coil capacity for each zone terminal is
determined from a simulation of system operation for the design heating condition. The simulation
determines the zone heating demand, the heating contribution (or load imposed) by primary air and the load
on the terminal heating coil load. During this simulation the terminal heating coil calculation is as follows:
Determine total supply airflow rate for the zone, Vsz from the primary supply air Vpz and the induction ratio
Rair:
Vsz = Vpz Rair
Determine the required supply air temperature for the current hour, solving the following equation for the
zone heating supply air temperature, Tzhs:
Qzc,htg = ρa Cpa K Vsz (Tzhs - Tzone)
Page 37 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Calculate the induced airflow through the terminal, Vi:
Vi = Vsz - Vpz
Determine the required heating coil outlet dry-bulb temperature, Thco. Heating coil outlet air mixes with
primary air before being delivered to the zone, so the following mixed air equation is solved for Thco:
Tzhs = (VpzTps,h + ViThco) / Vsz
Then solve for the heating coil sensible load, Qcoil,h,s:
Qcoil,h,s = ρa Cpa K Vi (Thco - Tzone)
Variable Definitions:
BF
=
Cooling coil bypass factor, dimensionless.
Fl
=
Primary supply duct leakage rate, percentage
ρaCpaK
=
Product of air density, heat capacity and unit conversion factor. Adjusted for
altitude .
ρahfgK
=
Product of air density, heat of vaporization and unit conversion factor.
Adjusted for altitude.
Rair
=
Airflow ratio, dimensionless. Ratio of supply air produced by terminal to
primary air entering the terminal.
Qcoil,c,l
=
Cooling coil latent load, BTU/hr or W.
Qcoil,c,s
=
Cooling coil sensible load, BTU/hr or W.
Qcoil,h,s
=
Heating coil sensible load, BTU/hr or W.
Qzc,clg
=
Cooling zone conditioning, BTU/hr or W. This is the zone sensible cooling
demand, corrected for zone air temperature and pulldown load.
Qzc,htg
=
Heating zone conditioning, BTU/hr or W. This is the zone sensible heating
demand, corrected for zone air temperature.
Qz,peak
clg
=
Peak zone sensible cooling load, BTU/hr or W.
Qz,peak
htg
=
Peak zone heating load, BTU/hr or W.
Tadp
=
Apparatus dew point temperature for cooling coil, F or C.
Tcco
=
Cooling coil outlet dry-bulb temperature, F or C.
Thco
=
Heating coil outlet dry-bulb temperature, F or C.
Tps,c
=
Primary supply air dry-bulb temperature for cooling, F or C.
Tps,h
=
Primary supply air dry-bulb temperature for heating, F or C.
Tzc
=
Zone cooling thermostat setpoint for occupied period, F or C.
Tzcs
=
Zone cooling supply air dry-bulb temperature, F or C. This is the air
temperature after cooling coil outlet air mixes with primary air.
Tzdcs
=
Design cooling supply air temperature for terminal, F or C.
Tzdhs
=
Design heating supply air temperature for terminal, F or C.
Tzh
=
Zone heating thermostat setpoint for occupied period, F or C.
Page 38 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Sizing Calculations for 4-Pipe Induction Systems
29.0 System Design Calculations ›› 29.5 Sizing Calculations for Induction Systems ››
Tzhs
=
Zone heating supply air dry-bulb temperature, F or C. This is the air
temperature after heating coil outlet air mixes with primary air.
Tzone
=
Zone air dry-bulb temperature, F or C. This is also the entering coil dry-bulb
temperature since induced room air enters the terminal cooling or heating
coil.
Vi
=
Induced airflow, CFM or L/s. This is room air induced into the terminal.
Vvf
=
Ventilation fan design airflow rate, CFM or L/s.
Voa
=
Outdoor ventilation airflow requirement for zone, CFM or L/s.
Vpz
=
Primary supply airflow rate to zone terminal, CFM or L/s.
Vsz
=
Supply airflow rate to zone, CFM or L/s. This is the sum of primary supply
airflow and induced airflow.
ωadp
=
Specific humidity at apparatus dew point condition, lb/lb or kg/kg.
ωcco
=
Specific humidity at cooling coil outlet, lb/lb or kg/kg.
ωzone
=
Specific humidity of zone air, lb/lb or kg/kg. This is also the specific
humidity at cooling coil inlet because induced room air enters the terminal
cooling coil.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Sizing Calculations for 4-Pipe Induction Systems
The configuration of components and the operation of 4-Pipe Induction systems differ significantly from other
types of HVAC systems. Consequently, unique sizing procedures are required. This help topic discusses
airflow and coil sizing calculations used for 4-Pipe Induction systems. Definitions for variables used in
equations are found at the end of the topic.
Primary Supply Airflow to Zone. The required primary supply airflow rate for each zone in the system is
computed by using the ventilation sizing method specified by the user because primary air is 100% outside air.
1. Sum of Space OA Airflows. With this method the primary airflow for a zone is the sum of the outdoor air
ventilation requirements for spaces in the zone.
2. ASHRAE Standard 62-2001 and Standard 62.1 (2004, 2007, 2010, 2013 editions). While the Standard 62
and 62.1 Ventilation Rate Procedures are applied to the system, the results of this calculation will match the
"Sum of Space OA Airflows" method. This is because primary air to each space is 100% outdoor air.
Primary Supply Fan. The required airflow rate for the primary supply fan is calculated by adding required
zone airflow rates together and then adjusting the total for duct leakage, if necessary:
Vpsf = (Sum of Vz,p all zones) / (1 - Fl/100)
Terminal Unit Cooling Coil Capacity. The required capacity for the cooling coil in each zone induction unit is
determined from simulations of system operation for design cooling days. For each hour simulated, the
primary supply airflow rate at the specified primary supply air setpoint temperature will satisfy a portion of the
zone conditioning requirement. The terminal cooling coil will be required to meet the remainder of the load.
Note that this simulation assumes the terminal cooling coil runs dry and thus provides sensible cooling only.
When simulations have been completed for all hours, results are inspected to identify the maximum terminal
coil load for each zone. This data is then reported on the Zone Sizing Summary report.
Page 39 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
29.6 System Load Calculations
29.0 System Design Calculations ››
Cooling Coil Load Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Terminal Unit Heating Coil Capacity. The required capacity for the heating coil in each induction unit is the
sum of the zone design heating load and the heating load caused by primary air entering the induction unit at
a temperature colder than the room setpoint. It is calculated as follows:
Qth = Qzh + ρaCpaK Vz,p (Tzh - Tsp)
Variable Definitions:
Fl
=
Supply duct leakage, percent.
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qth
=
Required terminal heating coil capacity, BTU/h or W.
Qzh
=
Zone design heating load, BTU/h or W.
Tsp
=
Primary supply air temperature, F or C. Specified by user.
Tzh
=
Zone occupied heating thermostat setpoint, F or C.
Vpsf
=
Required airflow for primary supply fan, CFM or L/s.
Vz,p
=
Primary airflow rate for zone, CFM or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculation procedures for system-level loads.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Load Calculations
This section documents the calculation of cooling coil loads. Based on the coil airflow rate and the entering
and leaving conditions determined during the simulation of system operation, sensible and latent coil load
components are calculated as shown below. This discussion applies to the following types of cooling coils:
a. Pre-cooling coils
b. Central cooling coils
c. Terminal cooling coils in induction systems
d. Cooling coils in terminal units such as fan coils and water source heat pumps.
Qc,s = ρaCpaK Vcoil (Tci - Tco)
Qc,l = ρahfgK Vcoil (ωci - ωco)
The specific humidity at the coil outlet is determined using bypass factor equations. The coil bypass factor is a
measure of the approach of the coil outlet state to the apparatus dewpoint (ADP) condition. To calculate the
coil outlet specific humidity, first calculate the ADP temperature:
Tadp = (Tco - TciBF) / (1 - BF)
Then use psychrometric laws to calculate the specific humidity at Tadp. Finally, the outlet specific humidity is
calculated using the equation:
ωco = BF(ωci - ωadp) + ωadp
These equations are based on the following fundamental equation:
Page 40 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Heating Coil Load Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Humidification Load Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
BF = (Tco - Tadp)/(Tci - Tadp) = (ωco - ωadp)/( ωci - ωadp)
Variable Definitions:
BF
=
Cooling coil bypass factor, dimensionless.
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535 x
10^6 J/kg
ρa
=
Density of air , adjusted for altitude, lb/cuft or kg/cubic
meter.
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qc,s
=
Sensible cooling coil load, BTU/h or W.
Qc,l
=
Latent cooling coil load, BTU/h or W.
Tadp
=
Cooling coil apparatus dewpoint temperature, F or C.
Tci
=
Cooling coil inlet air temperature, F or C.
Tco
=
Cooling coil outlet air temperature, F or C.
Vcoil
=
Coil airflow rate, CFM or L/s.
ωadp
=
Specific humidity at cooling coil apparatus dewpoint, lb/lb
or kg/kg.
ωci
=
Cooling coil inlet air specific humidity, lb/lb or kg/kg.
ωco
=
Cooling coil outlet air specific humidity, lb/lb or kg/kg.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Load Calculations
This help topic documents the calculation of heating coil loads. Based on the coil airflow rate and the entering
and leaving conditions determined during simulation of system operation, the heating coil load is calculated as
shown below. This discussion applies to:
a. Pre-heat coils
b. Central heating coils
c. Central reheat coils
d. Terminal reheat coils in supply terminals
Heating coil loads are computed using the equation:
Qc,h = ρaCpaK Vcoil (Tco - Tci)
where:
ρaCpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qc,h
=
Heating coil load, BTU/h or W.
Tci
=
Heating coil inlet temperature, F or C.
Tco
=
Heating coil outlet temperature, F or C.
Vcoil
=
Heating coil airflow rate, CFM or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 41 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Outdoor Ventilation Load Calculations
Humidification Load Calculations
This help topic describes the procedures used to calculation humifidication loads and to size humidifier
equipment. A single procedure is used for calculating humidification for cooling design, heating design and
energy simulation applications. Humidification sizing data is derived from calculations using weather and load
conditions at the winter design condition. The procedure is as follows:
1. For each hour considered, HAP performs a moisture balance for the entire system to determine the specific
humidity at each point in the system and the relative humidity in the zones. This calculation considers
moisture gains and losses due to people latent heat gain, miscellaneous latent heat gain or loss, infiltration
air, ventilation air and dehumidification occuring at cooling coils. For the design heating condition, only
infiltration, ventilation and dehumidification are considered since internal load components are not included
in the design heating analysis.
2. If the resulting relative humidity in zones is less than the minimum RH setpoint specified for humidification
control, the humidifier is activated. The required specific humidity of supply air leaving the humidifier, ωout,
is determined by recalculating the system moisture balance, this time assuming zones are maintained at the
minimum RH setpoint. This moisture balance calculation also determines the specific humidity of supply air
entering the humidifer section of the duct, ωin.
3. The humidification flow rate for the hour is then calculated as
Vh = ρaVsK(ωout -ωin)
4. The humidification load is calculated as:
Qh,l = ρahfgVsK(ωout -ωin)
For all six types of humidification devices modeled in HAP, the steam injection process is isothermal [1].
This means that the heat of evaporation comes from a source other than the supply air itself. The
temperature of air flowing through the humidifier section of the duct does not change.
Variable Definitions:
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535 x
10^6 J/kg
K
=
Unit conversion factor.
=
60 min/hr for English Units.
=
0.001 cubic meter / L for SI Metric units
ρa
=
Density of air , adjusted for altitude, lb/cuft or kg/cubic
meter.
Qh,l
=
Latent humidification load, BTU/hr or W.
Vh
=
Humidification flow rate, lb/hr or kg/s. This is the rate at
which moisture must be added to the supply
air stream to maintain zones at the specified
minimum RH condition.
Vs
=
Supply air flow rate through humidification section of duct,
CFM or L/s
ωin
=
Specific humidity of air entering the humidifier section of
duct, lb/lb or kg/kg.
ωout
=
Required specific humidity at outlet of humidifier section of
duct, lb/lb or kg/kg.
Reference:
[1] Eade, Robert, Humidification Looming Larger in IAQ, Engineered Systems, January 1996, pp 49-58.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 42 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Outdoor Ventilation Load Calculations
The ventilation load is defined as the net heat gain or loss for the system due to the entry of outdoor ventilation
air into the system, and the exhaust of an equal quantity of air from the system. For the basic case in which all
air is exhausted after flowing through the return plenum or duct, the sensible ventilation load is:
Qvs = ρaCpaK Vv (Toa - Tex)
For the more general case in which portions of ventilation air are exhausted directly from the zone and
exhausted after flowing through the return duct, the sensible ventilation load is:
Qvs = ρaCpaK (Vv - Vex,dir) (Toa - Tex)
+ [sum of {ρaCpaK Vex,dir (Toa - Tz)}, all zones]
In both of these calculation cases, the exhaust air temperature, Tex, is used. When attempting to duplicate
ventilation load calculations by hand, this exhaust temperature must be obtained from the System
Psychrometrics report. On this report, the exhaust temperature is equal to the air temperature at the return
outlet, provided that a ventilation reclaim device is not used or is not operating.
When calculating the latent ventilation load, the following equation is used. Direct exhaust air is not a
consideration in this case because the specific humidity of zone air and centrally exhausted air are the same:
Qvl = ρahfgK Vv (ωoa - ωex)
In the previous equations, the exhaust air humidity, ωex, is equal to the zone humidity. However, when a
ventilation reclaim device that provides latent reclaim is used, the exhaust humidity will differ from the zone
humidity.
Variable Definitions:
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535 x
106 J/kg.
ρa
=
Density of air , adjusted for altitude, lb/cuft or kg/cubic
meter.
CpaK
=
Product of air density, heat capacity and unit conversion
factor. Adjusted for altitude .
Qvl
=
Latent ventilation load, BTU/h or W.
Qvs
=
Sensible ventilation load, BTU/h or W.
Tex
=
Exhaust air temperature, F or C. This is air that has flowed
through a return duct or plenum before it is
exhausted.
Toa
=
Outdoor air temperature, F or C.
Tz
=
Zone air temperature, F or C.
Vex
=
Exhaust airflow rate, CFM or L/s. This refers to air
exhausted from the system after flowing
through the return duct or plenum.
Vex,dir
=
Direct exhaust airflow rate, CFM or L/s. This refers to air
exhausted directly from a zone to ambient
before it flows through a return duct or
plenum.
Vv
=
Outdoor ventilation airflow rate , CFM or L/s.
ωoa
=
Outdoor air specific humidity, lb/lb or kg/kg.
ωex
=
Exhaust air specific humidity, lb/lb or kg/kg. Same as zone
air specific humidity except when latent
ventilation reclaim is used.
ωz
=
Zone specific humidity, lb/lb or kg/kg.
Page 43 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Plenum Load Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Fan Heat Gain Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Plenum Load Calculations
Plenum loads account for heat removed by air flowing through a return air plenum. The user has the
opportunity to specify that fixed percentages of the roof, wall and lighting heat gains are removed by plenum
air. This constitutes a simple plenum heat gain model. During load calculations, the program computes the
heat gains and loads for the wall, roof and lighting components. Based on the specified plenum heat gain
percentages, portions of these loads or heat gains are assigned to the plenum:
1. Lighting to Plenum: The heat gain to the plenum due to lights is calculated as a percentage of total
overhead lighting heat gain .
Example: The total lighting heat gain for an hour is 2000 BTU/hr. The user specifies that 30% of the lighting
heat gain is removed by plenum air. Therefore, 600 BTU/hr of the lighting heat gain is assigned to the
plenum and the remaining 1400 BTU/hr is assigned to the room. This 1400 BTU/hr will be used in the room
transfer function equation to determine how it is converted into a room load.
2. Roof to Plenum: The heat gain to the plenum due to the roof is calculated as a percentage of the roof
load .
Example: The total roof load for an hour is 5000 BTU/hr. The user specifies that 70% of the roof load is
removed by plenum air. Therefore, 3500 BTU/hr of roof load is assigned to the plenum and the remaining
1500 BTU/hr is assigned to the room.
3. Wall to Plenum: The user specifies a "wall to plenum" percentage which represents the percentage of the
gross wall area for zones in the system adjacent to the plenum. It is assumed that this percentage applies
to each space served by a system. For each space HAP calculates the wall area adjacent to the plenum by
multiplying the specified wall-to-plenum percent by the gross wall area. The program then determines the
net wall area by subtracting window and door areas. Next, HAP calculates a percentage which is {Area of
Wall Adjacent to Plenum} / {Net Area of Wall}. It is this percentage that is multiplied by the total wall load for
the space to determine the wall load to plenum. This procedure is repeated for each space served by the
system. The wall-to-plenum loads for all spaces are then added together to obtain the total for the system.
Example: A user specifies a wall-to-plenum value of 15%. This means that 15% of the gross wall area is
adjacent to the plenum. In a particular space, the gross wall area is 1000 sqft. Therefore 150 sqft is
adjacent to the plenum. Accounting for windows and doors in this space, the net wall area is 775 sqft.
Therefore, the percentage of wall load assigned to the plenum will be 150 sqft / 775 sqft = 19.4%. If the wall
load for a particular hour is 2000 BTU/hr, 388 BTU/hr will be assigned to the plenum and the remaining
1612 BTU/hr will be assigned to the room.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Heat Gain Calculations
Fan heat gain is due to friction between air and the fan blades, the energy imparted to the air when the fan
compresses the air, and energy losses in the drive mechanism and in the fan motor. The program assumes
the fan motor is in the airstream and calculates fan heat gain as:
Qf = K Pf
Variable Definitions:
K
=
Unit conversion factor,
=
3412 (BTU/h)/kW for English units
Page 44 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Duct Heat Gain or Loss Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
Duct Leakage Calculations
29.0 System Design Calculations ›› 29.6 System Load Calculations ››
=
1000 W/kW for S.I. Metric units.
Pf
=
Fan input power , kW.
Qf
=
Fan heat gain, BTU/h or W.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duct Heat Gain or Loss Calculations
Duct heat gain or loss is due to heat conducted from the supply airstream through supply duct walls to the
surroundings. For single-duct air systems the program calculates one duct heat gain quantity based on the
total of sensible loads in zones served by the air system:
Qdhg = [ Sum of Qz, all zones ] Fdhg/100
For 2-Deck Multizone, 3-Deck Multizone and Dual Duct systems, the program computes separate duct heat
gain quantities for the cold and hot ducts based on separate summations of zone cooling and zone heating
loads:
Qcdhg = [ Sum of Qzc, all zones ] Fdhg/100
Qhdhg = [ Sum of Qzh, all zones ] Fdhg/100
During the system simulation, this heat gain or loss quantity is added to the air stream immediately
downstream of the air handling unit. It therefore affects the required air handler outlet supply temperature. For
example, if a design cooling supply temperature is specified by the user, it represents the supply temperature
at the zone terminal. Accounting for duct heat gain, the required supply temperature at the air handling unit
outlet is:
Tahu,out = Tsc - Qdhg/(ρaCpaK Vsys)
Variable Definitions:
Fdhg
=
Duct heat gain or loss factor specified by user, percent.
ρaCpaK
=
Product of air density, heat capacity and a unit conversion
factor. Adjusted for altitude .
Qcdhg
=
Cold duct heat gain, BTU/h or W.
Qdhg
=
Supply duct heat gain or loss, BTU/h or W.
Qhdhg
=
Hot duct heat loss, BTU/h or W.
Qz
=
Zone sensible load, BTU/h or W.
Qzc
=
Zone sensible cooling load, BTU/h or W.
Qzh
=
Zone sensible heating load, BTU/h or W.
Tahu,out
=
Required air handling unit outlet temperature, F or C.
Tsc
=
Design cooling supply air temperature specified by user, F
or C. Represents supply temperature at the
zone terminal.
Vsys
=
Total system supply airflow rate , CFM or L/s.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duct Leakage Calculations
Page 45 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm
Duct leakage is considered in system calculations to account for the loss of air from the supply duct to the
surroundings. In order to model duct leakage, the user is asked to specify the percentage of supply air leaving
the central supply fan that is lost before air arrives at the zone supply terminals.
In systems using a return air plenum HAP assumes that air leaked from the supply duct flows directly into the
plenum. In systems using ducted return, HAP assumes air leaked from the supply duct indirectly finds its way
into the return air stream. Therefore, the quantity of air leaked from the supply duct is added to the return
airflow. Further, HAP assumes air leaked from the supply duct is at the temperature of air leaving the central
air handler. Thus, the leakage of air will also alter the temperature of return air. The effects of duct leakage can
be evaluated using data from the System Psychrometrics report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 46 of 46
29.0 System Design Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9E32.htm