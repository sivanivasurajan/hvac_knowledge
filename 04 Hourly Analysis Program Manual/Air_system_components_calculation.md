31.0 Air System Component Calculations
31.1 Overview for System Component Calculations
31.0 Air System Component Calculations ››
Overview for System Component Calculations
31.0 Air System Component Calculations ›› 31.1 Overview for System Component Calculations ››
31.2 Fan Calculations
31.0 Air System Component Calculations ››
Fan Calculations
31.0 Air System Component Calculations ›› 31.2 Fan Calculations ››
This chapter describes calculations and control modeling for air system components.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how component calculation information in this chapter is organized.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for System Component Calculations
This is the first in a series of help topics describing assumptions and calculation procedures used to simulate various components and controls in air
systems. For further information, please click on the desired topic below.
Fans
Coil Capacity & Fan Controls
Outdoor Ventilation Air Control
Preheat Coils
Precool Coils
Outdoor Air Economizers
Ventilation Reclaim Devices
Humidification Control
Dehumidification Control
Zone Heating Units
Derivation of DX Unit Compressor Power from Standard EER and COP Ratings
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains fan performance calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Calculations
This topic documents how fan input power is calculated. The discussions apply to all fans evaluated by the program including:
Supply fans.
Hot Deck supply fans
Return fans.
Ventilation fans.
Fans in fan powered mixing boxes.
Fans in supplemental zone heating units.
Direct exhaust fans.
This topic is divided into four sections. Sections A and B describe calculations for CAV and VAV system fans, respectively. Sections C and D describe
the special calculations for baseline fan power allowance in different editions of ASHRAE Standard 90.1.
A. Constant Volume Fan Calculations
For constant volume fans, fan motor input power only needs to be calculated at the design airflow condition since these fans operate at the same level at
all times. Fan input power is calculated in different ways depending on how the fan performance data is specified:
Page 1 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
(1) When total static pressure and overall efficiency are defined, fan input power is:
Pf = Vf ΔPs K1 / ( ηo )
(2) When motor brakehorsepower is defined, input power is:
Pf = BHP K2 / ( ηe )
(3) When fan motor kW is directly specified, no calculations are necessary.
(4) When motor W/CFM or W/L/s is defined, input power is:
Pf = ( Pr Vf )/ 1000
(5) When fan performance is specified as "90.1 App. G Fan kW", system fan kW is calculated per the procedure described in ASHRAE Standard 90.1
Appendix G. Application of this procedure in HAP is described below in part C or D depending on the edition of 90.1 in effect.
Variable Definitions:
Pf
Pf
=
Fan input power, kW.
Vf
=
Design fan airflow rate, CFM or L/s.
ΔPs
=
Total static pressure across fan, in wg or Pa.
Pr
=
Input power per unit flow ratio, W/CFM or W/L/s.
BHP
=
Fan brakehorsepower, hp.
ηo
=
Overall fan efficiency, dimensionless. This is a combined value
for fan mechanical, drive and motor efficiencies.
ηe
=
Fan motor efficiency, dimensionless.
K1
=
Conversion factor.
=
1.173x10^-4 for English Units
=
(62.3 lbm water/cuft)(ft/12 in)(60 min/hr)(.001285 BTU/ft-lb)
(kW/3412 BTU/hr)
=
1x10-6 for S.I. Metric Units
=
(cubic meter/1000 L)(kW/1000 W)
K2
=
Conversion factor.
=
(.746 kW/hp)
B. Variable Volume Fan Calculations
For VAV fans, fan motor input power must first be calculated for the design airflow condition and then adjusted when the fan is operating at off-design
airflow levels. These calculations are described below.
1. Compute Fan Input Power at Design Airflow Rate. Fan input power at design airflow is computed using the procedure described in section A.
2. Adjust Fan Input Power for Part-Load Performance. Next, input power is adjusted for part-load operating conditions. Part-load factors are obtained
from Table 1 when one of HAP’s computer-generated fan models is used, or from user-defined part-load performance points. Part-load data in Table
1 is illustrated in Figures 1 thru 3. Whether part-load data is obtained from the table or user inputs, straight-line interpolation is used with the
performance points to determine the part-load factor at any specific airflow ratio. This airflow ratio is part-load airflow divided by design fan airflow.
Input power is then calculated as:
Pf,pl = Pf,fl Rpl / 100
Variable Definitions:
Pf,pl
=
Fan input power at part-load, kW.
Pf,fl
=
Fan input power at full load, kW.
Rpl
=
Fan part-load factor, %.
Table 1. Fan Efficiencies and Part-Load Factors
Eff
Percent Airflow
Fan Type
(%)
0%
10%
20%
30%
40%
50%
60%
70%
80%
90%
100%
Forward Curved (FC)
54
21
27
33
40
46
54
61
72
81
91
100
FC with Dampers
50
28
32
38
43
48
55
64
73
82
91
100
FC with Variable Frequency
Drive
48
6
7
9
13
19
25
35
44
60
77
100
FC with Variable Speed
Drive
44
6
7
9
13
19
25
35
44
60
77
100
FC with Inlet Guide Vanes
54
30
30
30
30
30
31
36
45
57
74
100
BI/AF
54
44
53
61
69
76
84
90
96
99
101
100
BI/AF with Inlet Guide Vanes
50
40
43
46
49
52
56
60
67
73
83
100
BI/AF with Variable Freq.
Drive
43
5
7
10
13
15
21
30
42
57
77
100
BI/AF with Variable Speed
Drive
42
5
7
10
13
15
21
30
42
57
77
100
Controlled Pitch Axial
54
4
6
8
12
17
24
33
45
60
78
100
ASHRAE Std 90.1 Appendix
G(1)
54
0
3
7
13
21
30
41
54
68
83
100
Page 2 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
(1) Note: Part-Load Performance curve for VAV fans is from ASHRAE Standard 90.1 Appendix G, Table G.3.1.3.15. Fan efficiency shown in this table is a HAP assumption and is not
dictated by ASHRAE Standard 90.1.
Page 3 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
C. Calculation of Fan Performance per ASHRAE Std 90.1-2004 Appendix G Section G3.1.2.9
In a project where the preference for Energy Standard is specified as ASHRAE Standard 90.1-2004, and fan performance for a system is specified as
"90.1 App. G Fan kW", system fan kW is calculated per the procedure described in ASHRAE Standard 90.1-2004 Appendix G section G.3.1.2.9. This fan
performance option is typically used when defining an air system in a Baseline Building used for a LEED Energy and Atmosphere Credit 1 analysis. The
basic fan performance calculation is described below in sub-section C-1. Application of the calculation to central and terminal air systems is then
discussed in sub-sections C-2 and C-3.
C-1. Basic Calculation
The basic calculation of the system fan power per Section G3.1.2.9 is described below. Application of this calculation to central systems and terminal
systems is then explained in sub-sections C-2 and C-3.
System fan power is calculated as:
Pf = (746 x BHP) / [ 1 - e^{-0.2437839 x ln(BHP) - 1.685541} ]
The fan brakehorsepower, BHP, is determined as follows, as prescribed in Table G3.1.2.9:
Constant Volume Systems (Baseline System Types 1-4)
If system supply airflow rate is less than 20,000 CFM (9438.9 L/s), then
BHP = 17.25 + (Vsa - 20000) x 0.0008625
Otherwise,
BHP = 17.25 + (Vsa - 20000) x 0.000825
Variable Volume Systems (Baseline System Types 5-8)
If system supply airflow rate is less than 20,000 CFM (9438.9 L/s), then
BHP = 24 + (Vsa - 20000) x 0.0012
Otherwise,
BHP = 24 + (Vsa - 20000) x 0.001125
Variable Definitions:
Pf
=
System fan input power, kW.
Vsa
=
Design supply airflow rate, CFM.
BHP
=
Fan brakehorsepower, hp.
C-2. Application of G3.1.2.9 to Central Systems
When performing calculations for air systems used with Rooftop, Vertical Packaged Unit, DX AHU and Chilled Water AHU equipment, the Section
G3.1.2.9 calculation is applied as follows.
The Section G3.1.2.9 calculation defines the total system fan kW. This total is the sum of any supply, return, exhaust and relief fans in the system, but
excludes power for fans in fan powered mixing box air terminals. In HAP the "90.1 App G Fan kW" option only appears for the central supply fan. When
this performance option is selected:
1. The program performs the calculation outlined in C-1 above and applies the resulting fan kW to the supply fan.
2. Input power for any return, exhaust or relief fans in the system is set to zero.
This procedure lumps the total system fan power allowance at the supply fan. This is done because the Standard does not specify any method of
dividing the fan power among separate fans, if multiple fans exist. Because supply, return, exhaust and relief fans operate at the same time, the
Page 4 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
convention of lumping the total system fan kW at the supply fan will result in the correct fan energy consumption being calculated for the Baseline
Building.
C-3. Application of G3.1.2.9 to Terminal Systems
When performing calculations for terminal equipment including packaged terminal air conditioner (PTAC) and packaged terminal heat pump (PTHP)
types of equipment, the Section G3.1.2.9 calculation is applied as follows.
The Section G3.1.2.9 calculation defines the total system fan kW. For terminal systems, the ASHRAE Standard 90.1 definition of a "system" is
interpreted to mean one zonal PTAC or PTHP unit. Therefore, the G3.1.2.9 calculation is applied separately to each zonal PTAC or PTHP unit. Note that
HAP allows one "air system" to contain multiple zonal PTAC or PTHP units for speed of data entry and calculation. As a result, the G3.1.2.9 calculation
is applied to each zonal PTAC or PTHP unit in a HAP air system.
Example: In HAP a Pkg DX Fan Coil system is defined containing 50 zones, meaning 50 PTAC units. HAP performs the G3.1.2.9 calculation 50 times in
this system to determine the supply fan kW for each of the 50 zonal PTAC units. The calculation described in C-1 above is used.
Note: If a terminal system is defined using a dedicated outdoor air system (DOAS) unit and the "90.1 App G Fan kW" option is specified for the terminal
fan performance, HAP will set the fan input power for the ventilation fan and exhaust fan to zero. This is because the Appendix G Baseline Systems 1
(PTAC) and 2 (PTHP) do not use a DOAS unit and therefore calculation of the fan power allowance for the DOAS unit is outside the scope of the
G3.1.2.9 procedure.
D. Calculation of Fan Performance per ASHRAE Std 90.1-2007 thru 2013 Appendix G Section G3.1.2.9
In a project where the preference for Energy Standard is specified as ASHRAE Standard 90.1-2007, -2010, or -2013, and fan performance for a system
is specified as "90.1 App. G Fan kW", system fan kW is calculated per the procedure described in ASHRAE Standard 90.1 Appendix G section
G.3.1.2.9. This fan performance option is typically used when defining an air system in a Baseline Building used for a LEED Energy and Atmosphere
Prerequisite 2 or Credit 1 analysis. The basic fan performance calculation is described below in sub-section D-1. Application of the calculation to central
and terminal air systems is then discussed in sub-sections D-2 and D-3.
D-1. Basic Calculation
The basic calculation of the system fan power per Section G3.1.2.9 is described below. Application of this calculation to central systems and terminal
systems is then explained in sub-sections D-2 and D-3.
For baseline systems 1 and 2 (PTAC and PTHP), the baseline fan power allowance is calculated as:
Pf = 0.3 x (Vsa) / 1000
For baseline systems 3 through 8, the baseline fan power allowance is calculated as:
Pf = BHP x 0.746 / ηm
where the fan motor efficiency ηm is obtained from 90.1-2007 Table 10.8 for the next motor size greater than the BHP and using data from the
"enclosed motor", 1800 rpm column in the table. BHP in this equation is calculated by two different equations, depending on HVAC system type. For
constant air volume systems, BHP is calculated as:
BHP = Vsa x 0.00094 + A
For variable air volume systems, BHP is calculated as:
BHP = Vsa x 0.00130 + A
The factor "A" in these equations is the total "Fan Power Limitation Pressure Drop Adjustment" factor. Its calculation is specified in Tables 6.5.3.1.1A
and 6.5.3.1.1B of Standard 90.1. The total adjustment factor A is the sum of individual adjustments for up to 11 different devices. To calculate the total
A, the following procedure is used:
a. Identify which of the 11 devices shown in Table D.1 are used in the proposed air system. Note that the device used in thee proposed system is the
criteria for inclusion even though we are ultimately calculating baseline fan power.
b. For each applicable device, identify the device pressure drop. As shown in Table D.1, ASHRAE specifies fixed pressure drop values for certain
devices and allows other pressure drops to be user defined based on conditions in the proposed air system. Note the use of pressure drop
conditions in the proposed air system rather than in the baseline system. Further, some of the user-defined pressure drop values have special
conditions attached to them. Readers should refer to 90.1 table 6.5.3.1.1B for details.
c. For each applicable device, identify the device airflow rate from the baseline air system. Table D.1 shows the airflow rates HAP will apply for each
device. Note that unlike the criteria for use of a device and device pressure drop, the airflow rate here is taken from the baseline air system, not the
proposed air system.
d. Then, for each applicable device, the device A factor is calculated as:
A = (Pressure Drop x Air Flow) / 4131
e. Finally, sum the device A values for the applicable devices to obtain the total A factor used in the BHP equation.
Further Information about "A" Factors. The adjustment factor "A" is intended to lessen or eliminate any fan power penalty for best practices used in
the proposed system. Certain devices used in a proposed system, such as high efficiency filters, heat recovery, or sound attenuation to name a few,
have beneficial effects for comfort or energy efficiency, but also increase the total fan pressure drop and therefore the fan energy use in the proposed
system. To lessen or eliminate the penalty for this increased fan energy in the proposed system, the fan power for the corresponding baseline system
is increased by the "A" factor adjustment. This rationale for the "A" factor adjustment is why you choose the devices based on what is used in the
proposed system and determine pressure drops based on those existing in the proposed system, but calculate the A factor with the baseline system
airflow rates.
Variable Definitions:
Pf
=
System fan input power, kW.
Vsa
=
Design supply airflow rate, CFM.
BHP
=
Fan brakehorsepower, hp.
ηm
=
Fan motor efficiency, decimal.
A
=
Fan power limitation pressure drop adjustment factor, hp.
Page 5 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.3 Coil Capacity and Fan Controls
31.0 Air System Component Calculations ››
Coil Capacity and Fan Controls
31.0 Air System Component Calculations ›› 31.3 Coil Capacity and Fan Controls ››
Table D-1. Fan Power Limitation Pressure Drop Adjustment Categories
Device (in Proposed System)
2007
2010
2013
Pressure Drop
Airflow
Fully ducted return and/or exhaust air systems
X
X
X
Fixed at 0.5 in wg
Return
Return and/or exhaust airflow control devices
X
X
X
Fixed at 0.5 in wg
Return
Exhaust filters, scrubbers or other exhaust treatment
X
X
X
User defined
OA Ventilation
Particulate filtration credit: MERV 9 thru 12
X
X
X
Fixed at 0.5 in wg
Supply Fan
Particulate filtration credit: MERV 13 thru 15
X
X
X
Fixed at 0.9 in wg
Supply Fan
Particulate filtration credit: MERV 16 and above, and electronically
enhanced filters
X
X
X
User defined
Supply Fan
Carbon and other gas-phase air cleaners
X
X
X
User defined
Supply Fan
Biosafety cabinet
X
X
User defined
Direct Exhaust
Energy recovery device
X
X
X
User defined
OA Ventilation
Coil runaround loop
X
X
Fixed at 0.6 in wg
OA Ventilation
Evaporative humidifier/cooler in series with another cooling coil
X
X
X
User defined
Supply Fan
Sound attenuation device
X
X
X
Fixed at 0.15 in wg
Supply Fan
Fume hood exhaust exception
X
Fixed at -1.00 in wg
Direct Exhaust
Exhaust system serving fume hoods
X
X
0.35 in wg
Direct Exhaust
Laboratory and vivarium exhaust systems in high-rise buildings
X
X
User defined
Direct Exhaust
Systems without central cooling device
X
Fixed at -0.60 in wg
Supply Fan
Systems without central heating device
X
Fixed at -0.30 in wg
Supply Fan
Systems with central electric resistance heat
X
Fixed at -0.20 in wg
Supply Fan
D-2. Application of G3.1.2.9 to Central Systems
When performing calculations for air systems used with Rooftop, Vertical Packaged Unit, DX AHU and Chilled Water AHU equipment, the Section
G3.1.2.9 calculation is applied as follows.
The Section G3.1.2.9 calculation defines the total system fan kW for a baseline system. This total is the sum of any supply, return, exhaust and relief
fans in the system, but excludes power for fans in fan powered mixing box air terminals. In HAP the "90.1 App G Fan kW" option only appears for the
central supply fan. When this performance option is selected:
1. The program performs the calculation outlined in D-1 above and applies the resulting fan kW to the supply fan.
2. Input power for any return, exhaust or relief fans in the system is set to zero.
This procedure lumps the total system fan power allowance at the supply fan. This is done because the Standard does not specify any method of
dividing the fan power among separate fans, if multiple fans exist. Because supply, return, exhaust and relief fans operate at the same time, the
convention of lumping the total system fan kW at the supply fan will result in the correct fan energy consumption being calculated for the Baseline
Building.
D-3. Application of G3.1.2.9 to Terminal Systems
When performing calculations for terminal equipment including packaged terminal air conditioner (PTAC) and packaged terminal heat pump (PTHP)
types of equipment, the Section G3.1.2.9 calculation is applied as follows.
The Section G3.1.2.9 calculation defines the total system fan kW for the baseline system. For terminal systems, the ASHRAE Standard 90.1 definition of
a "system" is interpreted to mean one zonal PTAC or PTHP unit. Therefore, the G3.1.2.9 calculation is applied separately to each zonal PTAC or PTHP
unit. Note that HAP allows one "air system" to contain multiple zonal PTAC or PTHP units for speed of data entry and calculation.
Example: In HAP a Pkg DX Fan Coil system is defined containing 50 zones, meaning 50 PTAC units. HAP performs the G3.1.2.9 calculation 50 times in
this system to determine the supply fan kW for each of the 50 zonal PTAC units. The calculation described in D-1 above is used.
Note: If a terminal system is defined using a dedicated outdoor air system (DOAS) unit and the "90.1 App G Fan kW" option is specified for the terminal
fan performance, HAP will set the fan input power for the ventilation fan and exhaust fan to zero. This is because the Appendix G Baseline Systems 1
(PTAC) and 2 (PTHP) do not use a DOAS unit and therefore calculation of the fan power allowance for the DOAS unit is outside the scope of the
G3.1.2.9 procedure.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains coil capacity and supply fan control modeling.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
Coil Capacity and Fan Controls
This topic documents how the program simulates various types of coil capacity, fan and supply air temperature reset controls. In the program, five
different options for coil capacity control are offered. The control chosen will govern coil, fan and supply temperature control. Each option is discussed
below.
1. Constant Temperature, Fan On. In the occupied period, the fan operates continuously to provide both conditioning and ventilation. The coil capacity
is controlled to provide a constant supply air temperature at all times. This control is frequently used in VAV systems and in Multizone or Dual Duct
CAV systems. In the unoccupied period, the same coil control is used, but the fan cycles on only when a demand for cooling or heating exists.
2. Constant Temperature, Fan Cycled. The coil capacity is controlled to provide a constant supply air temperature at all times. However, the fan and
the coil only cycle on when a demand for cooling or heating exists. This control is typically used for single-zone CAV systems, fan coils or water
source heat pumps.
3. Cycled or Staged Capacity, Fan On. In the occupied period, the fan operates continuously to provide both conditioning and ventilation. In a DX
cooling unit or DX heat pump the compressor is cycled or staged to control the output of the coil. In chilled water or hot water equipment, the supply
temperature or water flow is modulated to control output of the coil. The result of this control is that the supply temperature fluctuates during the hour.
For a DX cooling system, for example, the supply temperature is cold while the compressor is cycled on, but is warm when the compressor is cycled
off. Because all of HAP’s system simulation calculations operate on 1-hour time steps, HAP estimates an average hourly supply temperature for this
type of control. This temperature will vary from its design value when the compressor is cycled on for the entire hour, to a value which approaches the
room temperature when the compressor is cycled off for nearly the entire hour. Finally, in the unoccupied period, the system operates in a "constant
temperature, fan cycled" mode since the fan and coil will only operate when a cooling or heating demand exists.
4. Supply Reset Based on Greatest Zone Demand. For this control, supply air temperature is reset based on zone loads. The fan operates
continuously to ventilate and condition during the occupied period, and cycles on only when demands exist in the unoccupied period. The system
supply air temperature is determined by computing the required supply air temperatures for each zone served by the system. For cooling operation,
the coldest supply temperature among the zones is used as the supply temperature for the system. For heating operation, the warmest supply
temperature is used as the supply temperature for the system. This models the use of a discriminating controller for resetting supply temperature.
5. Supply Reset Based on Outdoor Air Schedule. For this control, supply air temperature is reset based on an outdoor air temperature schedule. The
fan operates continuously to ventilate and condition during the occupied period, and cycles on only when demands exist in the unoccupied period. For
this control the maximum and minimum supply air temperatures and their corresponding outdoor air temperatures must be known. The program then
uses the simple control profiles illustrated in Figures 1 and 2 to determine the system supply temperature as a function of outdoor air temperature.
For example, for the cooling control example shown in Figure 1, the design supply temperature is 57 F at a corresponding outdoor temperature (OAT)
of 95 F, and is 67 F at a corresponding OAT of 55 F. Above 95 F OAT, the supply temperature is held constant at 57 F. Below 55 F OAT, the supply
temperature is held constant at 67 F. Between 95 F and 55 F, the supply temperature varies as a linear function of outdoor temperature.
For the heating example in Figure 2, a similar control scheme is used. This example uses a supply temperature of 120 F at an OAT of 25 F, and a
supply temperature of 100 F at an OAT of 55 F.
Page 7 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.4 Outdoor Ventilation Air Control
31.0 Air System Component Calculations ››
Outdoor Ventilation Air Control
31.0 Air System Component Calculations ›› 31.4 Outdoor Ventilation Air Control ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of outdoor ventilation air controls.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Outdoor Ventilation Air Control
This topic documents how outdoor air ventilation control is simulated. The program offers four options for controlling outdoor ventilation air. Each is
discussed separately below.
1. Constant Airflow Control. With this control, outdoor ventilation airflow is maintained at its design value for all system operating hours when the
ventilation dampers are open. For constant volume systems, this condition can be maintained without special controls. For VAV systems, it is
assumed special controls are available to maintain a constant outdoor airflow rate as the supply airflow rate varies.
2. Proportional Airflow Control. This control option is offered in VAV air systems to model uncontrolled outdoor ventilation airflow. For all system
operating hours during which ventilation dampers are open, HAP models ventilation airflow as a constant percentage of the supply airflow rate. For
example, if ventilation is 25% of supply airflow at the design condition, it will remain as 25% of supply airflow as the supply fan airflow varies. The
program also provides the option of specifying a minimum ventilation flow rate. When used, the program assumes the proper controls are available to
prevent outdoor ventilation airflow from dropping below this level.
3. Scheduled Airflow Control. With this control, ventilation airflow is varied according to a predetermined hourly schedule. For each hour, a user-
defined schedule factor is multiplied by the design ventilation airflow rate to determine the ventilation flow rate for that hour.
4. Demand Controlled Ventilation (DCV) Control models the use of a CO2 sensor in each zone to control ventilation air. Since occupants are the
primary source of CO2 in most buildings, measuring CO2 is a means of indirectly measuring the number of occupants present in a zone. Outdoor
ventilation air can then be adjusted as CO2 levels change so the proper ventilation per occupant is maintained, while at the same time minimizing
ventilation air and therefore the cooling and heating loads due to ventilation. With DCV, the user establishes a control profile which relates zone CO2
differentials to ventilation airflow rates. The program performs a CO2 balance calculation to estimate CO2 levels at all points in the system.
Differentials between zone CO2 level and outdoor CO2 level are calculated and are used with the control profile to determine the amount of
ventilation air required in the system. For details on DCV simulation calculations click here: DCV Calculations.
Note: For VAV systems, if the supply airflow rate drops below the constant ventilation rate being maintained with Constant control, or the minimum
ventilation rate used with the other controls, the system will no longer be able to provide the specified ventilation airflow rate. Instead, the system will
operate with 100% outdoor air, but will be below the design ventilation rate specified.
Example: A VAV system is defined using Constant control for outdoor ventilation air. At the design condition, the supply fan airflow rate is 10000 CFM
and the ventilation airflow is 2000 CFM. Minimum dampers positions are such that VAV terminals close to 15% of design airflow. Therefore, when all
VAV terminals are at minimum position, the supply fan will handle 1500 CFM. At such a condition it will not be possible to provide 2000 CFM of outdoor
ventilation. 1500 CFM of outdoor air is the most that can be provided. This type of problem can be solved by specifying minimum airflow rates for the
VAV terminals which are in synch with the ventilation airflow for the system as a whole.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
Demand Controlled Ventilation Control
31.0 Air System Component Calculations ›› 31.4 Outdoor Ventilation Air Control ››
Demand Controlled Ventilation Control
Introduction. Demand Controlled Ventilation (DCV) control uses zone CO2 sensors to control ventilation air. This help topic explains how HAP
simulates DCV control.
HAP performs an iterative calculation to determine the steady state CO2 levels for each hour of operation simulated and the resulting control of outdoor
airflow rates. This involves estimating the CO2 level in each zone. The zone CO2 levels determine how the outdoor ventilation damper is positioned.
Outdoor ventilation airflow in turn influences CO2 levels in the system. Thus elements of the analysis are interrelated and an iterative solution is needed
to consider all feedback issues in the system. The following sections discuss each element in this calculation.
A. CO2 Generation by Space Occupants.
Occupants are the primary source of CO2 generation in occupied spaces. Further, occupants produce a predictable amount of CO2 based on activity
level. The total CO2 generated by occupants of a zone is calculated as the sum of CO2 generated by occupants in all spaces in the zone:
Vzone = Σ (Vspace)(Mspace), all spaces
The CO2 generated in each space is calculated as the number of occupants present times the CO2 generated per person:
Vspace = Nocc Vocc
where:
Vzone
=
Total volume of CO2 produced by occupants in a zone, CFM or L/s.
Vspace
=
Total volume of CO2 produced by occupants in a single instance of a space,
CFM or L/s
Mspace
=
Space multiplier. The number of spaces of this type in the zone.
Nocc
=
Number of occupants in the space for the current hour. This is the product of
the maximum occupants times the hourly schedule factor for the current hour.
Vocc
=
Total volume of CO2 produced by one occupant in the space, CFM or L/s.
This value depends on the occupant activity level as described in the following
paragraphs.
The calculation of CO2 generation for a single occupant is based on the fact that human activity is related to respiration. That is, the higher the level of
activity or exertion, the higher the level of respiration. During respiration the occupant exhales air that contains CO2 generated in the lungs. In HAP the
relationship between occupant activity and CO2 generation is calculated as follows:
Vocc = Qtot (K) / [M At]
English Units: Vocc = Qtot (0.00002667) CFM
SI Metric Units = Qtot (0.00004298) L/s
where:
Vocc
=
Total volume of CO2 produced by one occupant in the space, CFM or L/s.
Qtot
=
Total heat gain per occupant, BTU/hr/person or W/person. This is the sum of
sensible and latent heat gains defined by the occupant activity level, or directly
specified by the user.
K
=
Curve fit coefficient. 0.00883 CFM/Met in English or 0.25 L/min/Met in Metric.
Figure C-2 "Metabolic Data" from ANSI/ASHRAE Standard 62.1-2010,
Ventilation for Acceptable Indoor Air Quality, plots the relationship between
metabolic level and CO2 generation. The relationship can be represented as
the following equations:
CO2 generation in CFM = 0.00883 x Mets
CO2 generation in L/min = 0.25 x Mets
CO2 generation in L/s = 0.004167 x Mets
M
=
Heat flux for one metabolic unit or "Met", 18.4 BTU/hr/sqft or 58.04 W/sqm,
where the sqft or sqm area refers to body surface area At.
At
=
Body surface area for one "typical" occupant, sqft or sqm. For this analysis,
HAP assumes the average adult male has a body surface area of 19.4 sqft
(1.8 sqm) and the average adult female has a body surface area
approximately 85% of that for the male (16.5 sqft or 1.53 sqm). HAP considers
the typical space occupant to be an average of male and female body areas:
18.0 sqft or 1.67 sqm.
The equations above are the combination of two separate equations. Stating the equations separately helps to understand the formulation better. First
the heat flux per person in Mets is calculated as:
M = (Qtot BTU/hr/person) [1 Met / (18.4 BTU/hr-sqft)] [1 / (At sqft)]
Example: One occupant with activity level of "office work" has a sensible heat gain of 245 BTU/hr/person and a latent heat gain of 205 BTU/hr/person.
Therefore the total heat gain is 450 BTU/hr/person and the metabolic rate per person is:
M = (450 BTU/hr/person) (1/18.4 BTU/hr/person) (1/18.0 sqft) = 1.36 Met/person
Second, the correlation between metabolic rate and CO2 generation, obtained via a curve fit of ASHRAE Standard 62.1 data is:
CO2 generation in CFM = 0.0088 x M
Page 9 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
CO2 generation in L/s = 0.004167 x M
B. CO2 Mass Balance for Zones
Once the CO2 generation rate for zone occupants is known, a CO2 mass balance can be performed for each zone in the system to estimate the CO2
level measured by a CO2 sensor in the zone. This mass balance assumes a steady state level of CO2 will be reached each hour. The mass balance is
as follows:
0
=
CO2 in supply air entering zone
- CO2 in direct exhaust air leaving zone.
- CO2 in return air leaving zone via the return plenum or return duct.
+ CO2 in infiltration air entering the zone.
- CO2 in exfiltration air leaving the zone.
+ CO2 generated by occupants in the zone.
To solve this equation for the zone CO2 level, the CO2 level in supply air is assumed. Later this assumption will be checked and if necessary the
calculation will be repeated with an adjusted assumption. Knowing the supply CO2 level, all the airflows and the CO2 generation by occupants, the
equation can be solved for the zone CO2 level.
C. Determining Outdoor Damper Position and Outdoor Airflow
To determine outdoor damper position the DCV controller will first scan CO2 measurements by all zone CO2 sensors and identify the highest CO2 level.
It then uses this CO2 reading to determine the indoor-outdoor CO2 differential:
CO2 Differential = (Highest Zone CO2 Level) – (Outdoor Air CO2 Level)
This CO2 differential is used with the DCV control profile to determine the required outdoor ventilation airflow.
The figure below shows a sample control profile. In this example the outdoor CO2 level is 400 ppm. The minimum CO2 differential is 100 ppm which
equates to a CO2 level of 500 ppm and corresponds to a base ventilation rate of 810 CFM. The maximum CO2 differential is 700 ppm which equates to
a CO2 level of 1100 ppm and corresponds to a design ventilation rate of 2700 CFM. The DCV controller sets the outdoor damper position as follows:
a. If the CO2 differential determined by the DCV controller is less than the minimum setting of 100 ppm (which equals a CO2 level of 500 ppm), the
outdoor dampers will be set to provide the base ventilation rate of 810 CFM.
b. If the CO2 differential is greater than the maximum setting of 700 ppm (which equals a CO2 level of 1100 ppm) , the outdoor dampers will be set to
provide the design ventilation airflow of 2700 CFM.
c. If the CO2 differential is between the minimum and maximum settings, then the outdoor dampers will be set to provide the airflow corresponding to the
control profile. Thus, outdoor airflow is a linear function of CO2 differential in this range and ranges between the minimum (810 CFM) and maximum
(2700 CFM) values.
D. Calculation of System CO2 Levels
Next, the program uses the zone CO2 data from part C and the outdoor ventilation airflow data from part D to calculate CO2 levels in the remainder of
the system. This requires starting at the return grilles of all zones and working along the airflow path to determine CO2 levels at all state points in the
return portion of the system, and then into the supply portion of the system.
For example, return air from the zones mixes in the return plenum or duct to yield a mixed CO2 concentration in return air. Return air mixes with outdoor
air, to provide a mixed CO2 concentration in supply air which is delivered to the zones.
E. Evaluation of Results and Iteration
Page 10 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.5 Preheat Coil Control
31.0 Air System Component Calculations ››
Preheat Coil Control
31.0 Air System Component Calculations ›› 31.5 Preheat Coil Control ››
31.6 Precool Coil Control
31.0 Air System Component Calculations ››
Precool Coil Control
31.0 Air System Component Calculations ›› 31.6 Precool Coil Control ››
31.7 Outdoor Air Economizer Control
31.0 Air System Component Calculations ››
Outdoor Air Economizer Control
Finally, the supply air CO2 level produced by part D is compared with the initial assumption for supply air CO2 level that was made at the start of the
CO2 balance calculation in part B. If the two values differ by more than 10 ppm, the calculation in parts B, C and D is repeated using the new supply air
CO2 value. In this way the program iterates to converge on a solution in which the outdoor air flow, system CO2 levels and zone CO2 levels are all
balanced and consistent for the hour.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of the control for preheat coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Preheat Coil Control
This topic documents how preheat coil operation is simulated. Equations used to calculate preheat coil loads are provided in a separate help topic.
During air system simulations, the program calculates the inlet temperature for the preheat coil. Assumptions:
1. If the coil is downstream of the mixing point, the inlet temperature is the mixed air temperature.
2. If the coil is upstream of the mixing point, it is assumed the coil is positioned downstream of any ventilation reclaim coil. Therefore, when a ventilation
reclaim coil is not used, the preheat coil inlet temperature is the outdoor air temperature. When a ventilation reclaim device is used, the preheat coil
inlet temperature is equal to the reclaim coil outlet temperature.
If the preheat coil inlet temperature is lower than the coil setpoint, then the preheat coil operates to heat air to the setpoint temperature. Note that the
preheat coil will only operate during months when it has been scheduled on by the user.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of controls for precool coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Precool Coil Control
This topic documents how precool coil operation is simulated in program calculations. Equations used to calculate precool coil loads are discussed in a
separate help topic.
During air system simulations, the program calculates the inlet temperature and specific humidity for the coil. Assumptions:
1. If the precool coil is located downstream of the mixing point, the coil inlet condition is equal to the mixed air temperature and specific humidity.
2. If the precool coil is located upstream of the mixing point, the coil is assumed be positioned downstream of any ventilation reclaim coil. When a
ventilation reclaim device is not used, or the device is not operating, the precool coil inlet condition is equal to the outdoor air temperature and specific
humidity. When a ventilation reclaim device is operating, the precool coil inlet condition is assumed to be equal to the reclaim coil outlet temperature
and specific humidity.
In either case, if the inlet temperature is warmer than the precool coil setpoint, the precool coil operates to cool air to the setpoint temperature. The coil
will perform sensible cooling and, if conditions permit, will also perform latent cooling. Note that the precool coil will only operate during months it has
been scheduled on by the user.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of outdoor air economizer controls.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 11 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.0 Air System Component Calculations ›› 31.7 Outdoor Air Economizer Control ››
Outdoor Air Economizer Control
Outdoor air economizer control is used to vary the flow of outdoor air into the system in order to use cool outdoor air to reduce or eliminate the need for
mechanical cooling. Three types of economizer control can be simulated in HAP. Each is discussed in a separate section below. In these discussions,
the following terms are used:
• "Economizer cooling" refers to the use of outdoor air to reduce or eliminate cooling coil loads.
• "Mechanical cooling" refers to the use of mechanical equipment to provide cooling.
• "Normal ventilation" refers to the outdoor air ventilation airflow rate when the economizer is not operating.
A. Integrated Enthalpy Control
With this control the enthalpy of outdoor air and return air are measured and compared to determine when economizer dampers should modulate open.
Once activated, outdoor and return air dry-bulb temperatures are used to position the economizer dampers. This economizer control strategy is
illustrated in Figure 1. Operation of the control is discussed below, proceeding from right to left in the diagram.
1. When the enthalpy of outdoor air is greater than the enthalpy of return air, the control is not activated. The system receives normal outdoor ventilation
air. This is region A in Figure 1.
2. When the enthalpy of outdoor air is less than the enthalpy of return air, the economizer dampers are fully opened. Supply air is 100% outdoor air.
Economizer dampers are held in this position as long as mechanical cooling is still required. This is region B in Figure 1.
3. As the outdoor air temperature drops, a point will be reached where use of 100% outdoor air eliminates the need for mechanical cooling. Beginning at
this point, the economizer dampers modulate so that the mixture of outdoor and return air streams produces air at a temperature sufficient to eliminate
mechanical cooling. This is region in C in Figure 1.
4. At cooler temperatures, the economizer dampers finally modulate closed and the system returns to normal ventilation levels. No mechanical cooling is
required. This is region D in Figure 1.
Finally, in some cases, upper and lower cutoff temperatures will be specified. When the outdoor air dry-bulb temperature is greater than the upper cutoff
temperature, or lower than the lower cutoff temperature, economizer operation will be disabled automatically.
Figure 1. Integrated Enthalpy Economizer Control
B. Integrated Dry-Bulb Control
This control measures and compares outdoor air and return air dry-bulb temperatures to determine the economizer damper position. The economizer
control strategy is illustrated in Figure 2. Operation of the control is discussed below proceeding from right to left in the diagram.
1. When the outdoor temperature is greater than the return air temperature, the economizer dampers are closed. The system receives normal outdoor
ventilation air. This is region A in Figure 2.
2. When the outdoor temperature is less than the return air temperature, the economizer dampers are fully open. Supply air is 100% outdoor air.
Economizer dampers are held in this position as long as mechanical cooling is still required. This is region B in Figure 2.
3. As the outdoor air temperature drops, a point will be reached where use of 100% outdoor air eliminates the need for mechanical cooling. Beginning at
this point, the economizer dampers modulate so the mixture of outdoor and return air streams produces air at a temperature sufficient to eliminate
mechanical cooling. This is region in C in Figure 2.
4. At cooler temperatures, the economizer dampers finally modulate closed and the system returns to normal ventilation levels. No mechanical cooling is
required. This is region D in Figure 2.
Finally, in some cases, upper and lower cutoff temperatures will be specified. When the outdoor air dry-bulb temperature is greater than the upper cutoff
temperature, or lower than the lower cutoff temperature, economizer operation will be automatically disabled.
Page 12 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
Figure 2. Integrated Dry-Bulb Economizer Control
C. Non-Integrated Dry-Bulb Control
This control compares outdoor air and cooling coil outlet dry-bulb temperatures to determine the economizer damper position. The economizer control
strategy is illustrated in Figure 3. Operation of the control is discussed below proceeding from right to left in the diagram.
1. When the outdoor temperature is greater than the cooling coil outlet temperature, the economizer dampers are closed. The system receives normal
outdoor ventilation air. This is represented by regions A and B in Figure 3.
2. When the outdoor temperature is less than the cooling coil outlet temperature, the economizer dampers modulate open. Dampers are positioned so
that the of outdoor air and return air eliminate the need for mechanical cooling. This is region in C in Figure 3.
3. At cooler temperatures, the economizer dampers finally modulate closed and the system returns to normal ventilation levels. No mechanical cooling is
required. This is region D in Figure 3.
Finally, in some cases, upper and lower cutoff temperatures will be specified. When the outdoor air dry-bulb temperature is greater than the upper cutoff
temperature, or lower than the lower cutoff temperature, economizer operation will be automatically disabled.
Figure 3. Non-Integrated Dry-Bulb Economizer Control
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 13 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.8 Ventilation Reclaim Device Operation
31.0 Air System Component Calculations ››
Ventilation Air Reclaim Operation
31.0 Air System Component Calculations ›› 31.8 Ventilation Reclaim Device Operation ››
This section describes modeling of ventilation air-to-air heat recovery equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Reclaim Operation
Ventilation heat reclaim refers to equipment that transfers heat or heat and moisture between the outdoor ventilation and exhaust air streams in order to
reduce loads on air system cooling or heating coils. Examples of ventilation reclaim systems include:
• Air-to-air heat exchangers
• Heat pipes
• Heat wheels
• Desiccant wheels
• Pump around systems
A simple performance model is used to simulate ventilation reclaim device operation. This model determines the total heat transferred and the electrical
power consumed by the device. Assumptions:
1. The reclaim device transfers heat between the exhaust air stream and the outdoor ventilation air stream. The reclaim coil in the outdoor ventilation air
stream is upstream of the point where outdoor air mixes with return air and is upstream of any precool or preheat coils.
2. The device is available to operate for all months it is scheduled ON.
3. During these months, the device selectively transfers heat between air streams for all system operating hours when outdoor ventilation and exhaust
airflow exists. For example, if the system is performing cooling, the ventilation reclaim system will cool the outdoor ventilation airstream if possible, but
will not turn on if operation would heat the ventilation airstream. When the air system is performing heating, the reclaim system will warm the
ventilation air stream if possible, but will not turn on if operation would cool the ventilation airstream.
Example 1: VAV Air Handling Unit with Heat Recovery Ventilator (HRV) device.
Outdoor Air
Dry-Bulb
Exhaust Air Dry-
Bulb
AHU Cooling
Coil Status
Operating Description
95 F (35.0 C)
77 F (25.0 C)
ON
HRV is energized and motor runs at full speed. HRV transfers heat from outdoor
ventilation to exhaust air stream to cool incoming outdoor air. This reduces the load on
the AHU coil.
70 F (21.1 C)
77 F (25.0 C)
ON
HRV is off. Outdoor air bypasses the HRV wheel. The outdoor air to exhaust air
delta-T permits transfer of heat from exhuast to ventilation air stream, thereby heating
the ventilation air. However, the AHU is in cooling mode and heating the ventilation air
would increase the cooling coil load. Therefore, the HRV turns off.
Example 2: Dedicated Outdoor Air System (DOAS) AHU with Heat Recovery Ventilator (HRV) device.
Outdoor Air
Dry-Bulb
Exhaust Air Dry-
Bulb
DOAS
Discharge
Cooling
Setpoint
DOAS
Discharge
Heating
Setpoint
Operating Description
95 F (35.0 C)
77 F (25.0 C)
75 F (23.9
C)
70 F (21.1
C)
HRV is energized and motor runs at full speed. HRV transfers heat from
outdoor ventilation to exhaust air stream to cool incoming outdoor air. The
DOAS cooling coil operates to achieve the 75 F DOAS discharge setpoint,
but the cooling coil load is reduced due to pre-cooling by the HRV.
72 F (22.2 C)
77 F (25.0 C)
75 F (23.9
C)
70 F (21.1
C)
HRV is off. Outdoor air bypasses the HRV. Because the outdoor air-dry-
bulb is between the DOAS discharge setpoints, no HRV cooling or heating is
needed and the DOAS cooling and heating coils are off.
68 F (10.0 C)
77 F (25.0 C)
75 F (23.9
C)
70 F (21.1
C)
HRV is energized. However, running the HRV motor at full speed will
overheat the incoming air above the 70 F DOAS discharge setpoint.
Therefore, the motor speed is modulated so the heat recovered heats the
incoming air just enough that the 70 F DOAS discharge setpoint is met.
50 F (10.0 C)
68 F (20.0 C)
75 F (23.9
C)
70 F (21.1
C)
HRV is energized and motor runs at full speed. HRV transfers heat from
exhaust to outdoor ventilation air stream to heat incoming outdoor air. The
DOAS heating coil operates to achieve the 70 F DOAS discharge setpoint,
but the heating coil load is reduced due to the pre-heating by the HRV.
4. The reclaim device control will modulate operation if necessary to prevent overheating or overcooling the ventilation airstream, as noted in Example 2
above.
5. According to user specifications, the unit either transfers sensible heat only, or both sensible and latent heat.
6. A single thermal efficiency value is used to calculate heat reclaim for all operating hours. When both sensible and latent reclaim are offered,
manufacturers typically provide one efficiency rating value for the equipment. Consequently, this single rating value is used for both sensible and
latent heat transfer calculations. In addition it is assumed that thermal efficiency remains relatively constant and does not change significantly with
operating temperatures.
Page 14 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.9 Humidification Control
31.0 Air System Component Calculations ››
Humidification Control
31.0 Air System Component Calculations ›› 31.9 Humidification Control ››
7. The device consumes its specified electrical power when providing the maximum available heat reclaim. When device operation is modulated or
cycled to overheating or overcooling, energy use by the device is reduced. For example, if the necessary heat recovery is 60% of the potential heat
recovery, 60% of the specified device power is allocated for the hour.
For all operating hours, heat transfer is calculated using the following equations. Latent reclaim is only calculated if the user has specified the device
provides both sensible and latent heat transfer capabilities.
Qs = ρa Cpa Vex εvr K (Tex - Ta)
Ql = ρa hfg Vex εvr K (ωex - ωa)
where:
Cpa
=
Specific heat of air, .24 BTU/lbm-F or 1004.8 J/kg-K.
εvr
=
Thermal efficiency of ventilation reclaim device, decimal.
This value represents the fraction of the total
possible heat transfer that occurs. It is user-
defined.
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535 x
10^6 J/kg
K
=
Conversion factor used to provide correct units,
=
60 min/hr for English units or
=
cubic meter / 1000 L for S.I. Metric units.
ρa
=
Air density , lbm/cuft or kg/cubic meter. Adjusted for
altitude.
Qs
=
Sensible heat transfer, BTU/hr or W.
Ql
=
Latent heat transfer, BTU/hr or W.
Tex
=
Exhaust air temperature, F or C.
Ta
=
Outdoor air temperature, F or C.
Vex
=
Exhaust airflow rate, CFM or L/s.
ωex
=
Exhaust air specific humidity, lb/lb or kg/kg.
ωa
=
Outdoor air specific humidity, lb/lb or kg/kg.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains modeling of humidifiers and humidification control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Humidification Control
Humidification control is used to maintain humidity at a minimum level in zones served by the air system. A humidification system uses steam injection in
conjunction with a humidity sensor to control humidity. Assumptions:
1. Control is based on a measurement of the relative humidity in the zones.
2. When the zone humidity is above the minimum RH setpoint defined by the user, the control system takes no action and allows the humidity to float.
3. When the zone humidity begins to drop below the minimum RH setpoint, the control calls for moisture to be added at the air handler.
4. Moisture is assumed to be added downstream of the supply fan and cooling coils.
5. Moisture is added by injecting steam into the supply air stream. For all six types of humidification devices modeled in HAP, the steam injection
process is isothermal [1]. This means that the heat of evaporation comes from a source other than the supply air itself. The temperature of air flowing
through the humidifier section of the duct does not change. Humidification flow rate and load calculations are discussed in a separate help topic.
6. Sufficient moisture is added to the supply air stream to maintain the zone humidity at the minimum RH setpoint.
HAP provides options for modeling six common types of steam humidification systems. The thermodynamics of the steam injection process are the
same for all six systems. Only the energy cost will vary among the six types (note that energy costs for humidification systems will be added in HAP v4.1
when energy simulation features are moved to the Windows format). The six humidification system types offered in HAP are as follows:
a. Self-Contained Steam: Electric - An electric resistance heating element heats water in a reservoir to produce steam which is injected into the supply
air stream.
b. Self-Contained Steam: Natural Gas - A gas-fired heat exchanger heats water in a reservoir to produce steam which is injected into the supply air
stream.
c. Self-Contained Steam: Propane A propane-fired heat exchanger heats water in a reservoir to produce steam which is injected into the supply air
stream.
d. Direct Steam Injection - Clean steam obtained directly from the central steam boiler is injected into the supply air stream.
e. Heated Pan: Steam HX - Steam obtained from the central steam boiler flows through a heat exchanger immersed in a water reservoir to produce
clean steam which is injected into the supply air stream.
Page 15 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.10 Dehumidification Control
31.0 Air System Component Calculations ››
Dehumidification Control
31.0 Air System Component Calculations ›› 31.10 Dehumidification Control ››
31.11 Zone Heating Unit Operation
31.0 Air System Component Calculations ››
Supplemental Zone Heating Unit Operation
31.0 Air System Component Calculations ›› 31.11 Zone Heating Unit Operation ››
f. Heated Pan: Hot Water HX - Hot water obtained from the central boiler plant flows through a heat exchanger immersed in a water reservoir to
produce clean steam which is injected into the supply air stream.
Reference:
[1] Eade, Robert, Humidification Looming Larger in IAQ, Engineered Systems, January 1996, pp 49-58.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of active dehumidification control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Dehumidification Control
Dehumidification control is used to maintain humidity at a maximum level in zones served by the air system. A dehumidification system uses a humidity
sensor in conjunction with a central cooling coil and reheat coil to control humidity. Assumptions:
1. Control is based on a measurement of the relative humidity in the zones.
2. When the zone humidity is below the maximum RH setpoint defined by the user, the control system takes no action and allows the humidity to float.
3. When the zone humidity begins to rise above the maximum RH setpoint, the control calls for extra dehumidification by the central cooling coil.
4. The central cooling coil outlet temperature is decreased to condense additional moisture from the supply air stream. To prevent overcooling of zones
in the system, a reheat coil downstream of the central cooling coil and supply fan heats air to the proper supply temperature.
5. A sufficient amount of moisture is condensed at the central cooling coil to maintain the zone humidity at the maximum RH setpoint.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes modeling of control for supplemental zone heating units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supplemental Zone Heating Unit Operation
This help topic describes assumptions and calculations for the operation of supplemental zone heating units. These are baseboard or fan coil heating
units located in zones served by the air system. Zone heating units may be controlled by a room thermostat or by an outdoor thermostat. Assumptions
and calculations for each type of control are described in separate sections below.
A. Zone Heating Units Controlled by an Outdoor Thermostat
The purpose of heating units controlled by an outdoor thermostat is to offset envelope transmission heat loss in order to reduce zone heating
requirements and improve comfort.
This type of zone heating unit is activated any time the outdoor air temperature drops below a user-defined "trip temperature". When operating, heat
output from the unit varies as a linear function of outdoor air temperature. Unit output is zero when outdoor air temperature equals the trip temperature
and is maximum when outdoor air temperature equals the winter design dry-bulb. Below the winter design temperature, heat output remains at its
maximum level. Figure 1 provides a sample control profile in which the trip temperature is 45 F and the winter design dry-bulb temperature is 0 F. Using
this kind of control profile, unit heat output is calculated for any outdoor air temperature between the winter dry-bulb and the trip temperature using the
following equation:
Qh = Qmax ( Ttr - Ta ) / ( Ttr - Twdb )
where:
Qh
=
Zone heating unit output, BTU/hr or W.
Qmax
=
Zone heating unit capacity, BTU/hr or W. The default
capacity calculated by the program is the sum
of wall, window, roof, door and floor heat loss
for the design heating condition.
Ttr
=
Outdoor air trip temperature, F or C.
Ta
=
Outdoor air temperature, F or C.
Twdb
=
Outdoor air winter design dry-bulb temperature, F or C.
Page 16 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
31.12 DX Cooling and Heating Equipment
31.0 Air System Component Calculations ››
Derivation of DX Unit Compressor Power from Standard EER and COP Ratings
31.0 Air System Component Calculations ›› 31.12 DX Cooling and Heating Equipment ››
Operating Assumptions:
1. It is assumed the zone heating units are able to provide the heat quantity called for by the control profile at all times.
2. When a fan coil zone heating unit is used, it is assumed the unit fan runs continuously whenever the outdoor air temperature falls below the trip
temperature. Fan coils provide a constant volume of air whose temperature varies with the required heat output (i.e. the coil is cycled or supply
temperature is reset). Fan heat gain contributes to unit output so Qh in the previous equation is the sum of fan heat gain and coil output.
Note that the operation of zone heating units with outdoor thermostat control is independent of the indoor thermostat. Therefore the unit does not
respond to zone heating loads and cannot maintain the zone at a fixed heating setpoint. Because the relationship between zone load and outdoor air
temperature is non-linear, the zone heating unit may over heat or under heat the zone at different times. If the specified zone trip temperature too warm,
it is also possible for the zone heating unit to increase zone cooling loads. Users should be careful when specifying the trip temperature to minimize
situations in which the heating unit increases cooling system loads.
B. Zone Heating Units Controlled by an Indoor Thermostat
The purpose of heating units controlled by an indoor thermostat is to provide sufficient heat to maintain the zone within specified room temperature
levels. It operates alone or in tandem with the central HVAC system to accomplish this function.
These zone heating units are activated at certain times when the zone thermostat calls for heating. Rules governing when zone heating units are
activated vary with system type. System operation documentation provides further information on these rules.
Baseboard zone heating units are assumed to be cycled on and off at a sufficient level to meet the zone heating load for each hour. Fan coil zone
heating units are also cycled on and off. While cycled on, the fan coil provides a constant volume of air at the design heating supply temperature
specified for the unit. Total heat output from the fan coil is computed as fan heat gain plus heating coil output.
For both baseboards and fan coils, the heating units will provide heating up to the maximum heating capacity calculated or specified for the unit. When
the zone heating load exceeds the unit’s capacity, the heating unit continues to produce maximum heat output, but the zone air temperature will fall
below the lower limit of the heating thermostat throttling range.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how DX equipment compressor or compressor and outdoor fan power are derived from standard EER, SEER, COP and HSPF
ratings.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Derivation of DX Unit Compressor Power from Standard EER and COP Ratings
This topic describes how compressor kW needed for DX equipment simulations is derived from user entered values of EER, SEER, COP and HSPF.
Part A below describes basic principles involved with the calculation. Parts B thru F then describe the calculation procedures used for each class of DX
equipment.
A. Basic Principles
Page 17 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
Accurate simulation of DX cooling and heating equipment performance must account for energy consumption of the key components in the equipment.
Example: For rooftop equipment the key components are the indoor fan, compressors and outdoor fans.
An indoor fan may run continuously during occupied hours while compressors and outdoor fans modulate or cycle to meet cooling demands. Because
the operation of individual components differs significantly, indoor fan operation must be calculated separately from the operation of compressor and
outdoor fans. This creates the need to know separate design values for indoor fan kW and compressor + outdoor fan kW as the basis for the simulation.
The most accurate approach to energy simulation is to obtain these input kW values from manufacturer's performance ratings for a specific model and
size of the DX unit. However, in many practical situations input power data for a unit cannot be directly defined this way:
1. When modeling equipment for a Baseline Building in a LEED® Energy and Atmosphere Credit 1 analysis, hypothetical equipment is modeled. The
equipment must have the minimum prescriptive efficiency, defined in terms of EER, SEER, COP or HSPF by ASHRAE Standard 90.1.
2. When screening design alternatives in the preliminary design phase of a project, data sufficient for specific equipment selections is not yet available,
so approximate efficiency levels in terms of EER, SEER, COP or HSPF must be used to model the equipment.
3. Even in the detailed design phase of a project, specific equipment selections may not be available requiring equipment to be modeled on the basis of
EER, SEER, COP or HSPF ratings typical of a particular type or model of equipment.
AHRI and ISO/AHRI standard ratings of EER, SEER, COP and HSPF include power data for the energy consuming components in the equipment or
related to the equipment such as compressors, indoor fan, outdoor fans and/or water pumps. When the basis for equipment modeling is a standard EER,
SEER, COP or HSPF, energy simulation software must have the ability to extract design input power values for the separate components needed for an
accurate simulation.
To successfully extract this data, there are two key challenges.
The first challenge is separating power components embedded in a standard EER, SEER, COP or HSPF.
1. Rooftop, Vertical Packaged Units, Split DX AHUs - The AHRI Standards for rating these types of equipment include compressor, outdoor fan and
indoor fan power components in the EER, SEER, COP or HSPF. If a seasonal rating such as SEER or HSPF is defined, it must first be converted to
an equivalent design EER or COP. Then the simulation software must be able to extract the compressor + OD fan kW. Indoor Fan kW is determined
from user fan performance specifications.
2. Water-Cooled Vertical Packaged Units - The AHRI Standard for rating this type of equipment EER includes the compressor and indoor fan power
components. The simulation software must be able to extract compressor kW. Indoor fan kW is determined from user fan performance specifications.
3. Water Source Heat Pumps, Groundwater Source Heat Pumps, Ground Source Heat Pumps - The ISO/AHRI Standard for this equipment includes
compressor power and allowances for indoor fan and water pump power in the EER and COP. The simulation software must be able to extract
compressor kW. Indoor fan kW and water pump kW are determined from separate user specifications.
The second challenge is correcting for the application's design condition. A standard EER or COP is determined for a prescribed operating condition. For
example, air-cooled DX cooling equipment is rated at 95 F (35 C) OADB entering condenser temperature. The peak cooling load for equipment can often
occur at a different operating condition. If the required equipment capacity established at one operating condition is used with an EER or COP rated at a
different condition to determine compressor kW, the resulting kW can sometimes be significantly over- or under-estimated. The importance of this issue
is best explained with an example.
Example: Consider a rooftop application in a hot climate such as Phoenix, AZ, USA. The required cooling capacity is 180 MBH (52.8 kW). This peak load
occurs when the outdoor air dry bulb temperature (OADB) is 110 F (43.3 C). The AHRI standard EER rating for this equipment is 10.0 MBH/kW (2.93
kW/ikW) and the AHRI standard specifies this rating is determined at 95 F OADB (35 C). Our hypothetical rooftop which has a 180 MBH capacity at 110
F OADB, will have a capacity of about 197 MBH at 95 F OADB. If we ignore the difference between the capacity at the design condition of 110 F and the
capacity standard rating condition of 95 F, and use the 180 MBH capacity directly with the 10.0 EER, the resulting compressor + outdoor fan kW value
will be 15.1 kW (correcting for typical indoor fan conditions). On the other hand, if we account for the capacity difference and use the 197 MBH capacity
with the 10.0 EER, and further correct the resulting compressor + outdoor fan kW back to the 110 F condition, we will obtain a value of 18.8 kW.
Therefore, neglecting to account for the difference in design versus rating conditions results in a compressor + outdoor fan kW value that is
underestimated by approximately 20%. This will result in annual energy consumption for the rooftop being underestimated by a similar margin.
A similar problem can occur if the OADB at which the peak cooling load occurs is much less than 95 F. In that case, neglecting to account for the
different design verus standard rating conditions will result in rooftop energy consumption being overestimated.
To meet all of these challenges, the HAP algorithm for extracting compressor power from an EER, SEER, COP or HSPF ratings:
1. Converts SEER to equivalent EER, or HSPF to equivalent COP, if a seasonal rating is specified.
2. Separates the power components embedded in the EER or COP to obtain compressor + outdoor fan kW for air-cooled equipment and compressor kW
for water-cooled equipment.
3. Accounts for the difference between the design condition associated with peak capacity and the rating condition prescribed for the EER or COP.
The following sections describe how this general procedure is applied to each class of equipment modeled in HAP.
B. Air-Cooled DX Cooling Equipment.
This section summarizes the procedure for deriving compressor + outdoor fan kW from a standard EER rating for air-cooled DX cooling equipment. This
equipment includes rooftop units, air-cooled vertical packaged units, split DX AHUs and split and packaged DX fan coil units. EER rating procedures for
these types of equipment are specified in AHRI Standards 210/240, 340/360 and 390.
1. If a seasonal energy efficiency ratio (SEER) is specified, it must first be converted to an equivalent full load EER rating. This conversion is done as
follows:
EER = 6.0852 + 0.3973 x SEER
This equation is a regression curve fit of published SEER and EER ratings for a group of different sizes and types of equipment from multiple
manufacturers.
2. Next, known data is gathered. The gross cooling capacity at design is known either because it was directly specified by the user, or was derived via
the auto-sizing option. This cooling capacity is shown in Figure 1a as data point 1.
Also known is the design outdoor air dry-bulb temperature (OADB) corresponding to this design condition is also specified. Figure 1a shows a
scenario where the design OADB is warmer than the standard rating OADB of 95 F (35 C).
Finally, the indoor fan design input kW is calculated based on user specifications for fan performance. Fan heat gain is fan power x 3.412. Fan
Performance Calculations.
Page 18 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
3. The net cooling capacity at design is calculated by subtracting indoor fan heat gain from the gross cooling capacity. This is shown as data point 2 in
Figure 1a.
4. The net cooling capacity at the AHRI standard rating condition is then derived. This is approximated from a function that relates cooling capacity to
OADB. The function, shown in Figure 1a, is derived from a correlation of performance data for a range of air-cooled DX equipment. If capacity is
known at one OADB, the function allows us to estimate the corresponding capacity at any other OADB. This net cooling capacity is shown as data
point 3 in Figure 1a.
5. The total input power is derived from the net cooling capacity at AHRI conditions and the EER value: Total Input Power = Net Cooling Capacity / EER.
This is shown as data point 4 in Figure 1b.
6. The total input power at the specified design condition is derived next. This is approximated from a function that relates input power to OADB. The
function, shown in Figure 1b, is derived from a correlation of performance data for a range of air-cooled DX equipment. If input power is known at one
OADB, the function allows us to estimate the corresponding input power at any other OADB. This input power is shown as data point 5 in Figure 1b.
7. The compressor + outdoor fan kW at the design condition is finally calculated: Compressor + Outdoor Fan kW = Total Input Power at Design - Indoor
Fan kW. This is shown as data point 6 in Figure 1b.
C. Air Source Heat Pump Equipment
This section summarizes the procedure for deriving compressor + outdoor fan kW from a standard COP rating for air source heat pump equipment. This
equipment includes rooftop units, split DX AHUs, and split and packaged DX fan coil units. COP rating procedures for these types of equipment are
found in AHRI Standards 210/240 and 340/360.
Page 19 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
1. If a heating seasonal performance factor (HSPF) is specified, it must first be converted to an equivalent full load COP rating. This conversion is done
as follows:
COP = 3.3557 + 0.0145 x HSPF
This equation is a regression curve fit of published HSPF and COP ratings for a set of different sizes and types of equipment from multiple
manufacturers.
2. At the start of this procedure the gross heating capacity at design is known. The heating capacity is either directly specified by the user, or is derived
via the auto-sizing option. This heating capacity is shown in Figure 2a as data point 1.
Also known is the design outdoor air dry-bulb temperature (OADB) corresponding to this design condition. Figure 2a shows a scenario where the
design OADB is colder than the standard rating OADB of 47 F (8.3 C).
Finally, the indoor fan design input kW is calculated based on user specifications for fan performance. Fan heat gain is fan power x 3.412. Fan
Performance Calculations.
3. The net heating capacity at design is calculated by adding indoor fan heat gain to the gross heating capacity. This is shown as data point 2 in Figure
2a. See Section B for a discussion of the rationale regarding derivation of fan power and fan heat.
4. The net heating capacity at the AHRI standard rating condition is then derived. This is approximated from a function that relates heating capacity to
OADB. The function, shown in Figure 2a, is derived from a correlation of performance data for a range of air source heat pump equipment. If capacity
is known at one OADB, the function allows us to estimate the corresponding capacity at any other OADB. This net heating capacity is shown as data
point 3 in Figure 2a.
5. The total input power is derived from the net heating capacity at AHRI conditions and the COP value: Total Input Power = Net Heating Capacity /
(COP x 3.412). This is shown as data point 4 in Figure 2b.
6. The total input power at the specified design condition is derived next. This is approximated from a function that relates input power to OADB. The
function, shown in Figure 2b, is derived from a correlation of performance data for a range of air source heat pump equipment. If input power is known
at one OADB, the function allows us to estimate the corresponding input power at any other OADB. This input power is shown as data point 5 in
Figure 2b.
7. The compressor + outdoor fan kW at the design condition is finally calculated: Compressor + Outdoor Fan kW = Total Input Power at Design - Indoor
Fan kW. This is shown as data point 6 in Figure 2b.
Page 20 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
D. Water-Cooled DX Cooling Equipment (W/C VPAC Units)
This section summarizes the procedure for deriving compressor kW from a standard EER rating for water-cooled vertical package units. EER rating
procedures for this type of equipment is found in AHRI Standards 210/240 and 340/360.
1. The gross cooling capacity at design is known at the start of this procedure. The cooling capacity is either directly specified by the user, or is derived
via the auto-sizing option. This cooling capacity is shown in Figure 3a as data point 1.
Also known is the design entering water temperature (EWT) corresponding to this design condition. Figure 3a shows a scenario where the design
EWT is warmer than the standard rating EWT of 85 F (29.4 C).
Finally, the indoor fan design input kW is calculated based on user specifications for fan performance. Fan heat gain is fan power x 3.412. Fan
Performance Calculations.
2. The net cooling capacity at design is calculated by subtracting indoor fan heat gain from the gross cooling capacity. This is shown as data point 2 in
Figure 3a. See Section B for a discussion of the rationale regarding derivation of fan power and fan heat.
3. The net cooling capacity at the AHRI standard rating condition is then derived. This is approximated from a function that relates cooling capacity to
EWT. The function, shown in Figure 3a, is derived from a correlation of performance data for a range of water-cooled DX equipment. If capacity is
known at one EWT, the function allows us to estimate the corresponding capacity at any other EWT. This net cooling capacity is shown as data point
3 in Figure 3a.
4. The total input power is derived from the net cooling capacity at AHRI conditions and the EER value: Total Input Power = Net Cooling Capacity / EER.
This is shown as data point 4 in Figure 3b.
5. The total input power at the specified design condition is derived next. This is approximated from a function that relates input power to EWT. The
function, shown in Figure 3b, is derived from a correlation of performance data for a range of water-cooled DX equipment. If input power is known at
one EWT, the function allows us to estimate the corresponding input power at any other EWT. This input power is shown as data point 5 in Figure 3b.
6. The compressor kW at the design condition is finally calculated: Compressor kW = Total Input Power at Design - Indoor Fan kW. This is shown as
data point 6 in Figure 3b.
Page 21 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
E. WSHP, GWSHP, GSHP Equipment - Cooling Duty
This section summarizes the procedure for deriving compressor kW from a standard cooling EER for water source heat pump (WSHP), groundwater
source heat pump (GWSHP) and ground source heat pump (GSHP) equipment. EER rating procedures for these types of equipment are found in
ISO/AHRI Standard 13256-1.
1. At the start of this procedure the gross cooling capacity at design is known. The cooling capacity is either directly specified by the user, or is derived
via the auto-sizing option. This cooling capacity is shown in Figure 4a as data point 1.
Also known is the design entering water temperature (EWT) corresponding to this design condition. Figure 4a shows a scenario where the design
EWT is warmer than the standard rating EWT.
Finally, the indoor fan design input kW is calculated based on user specifications for fan performance. Fan heat gain is fan power x 3.412. Fan
Performance Calculations.
2. The gross cooling capacity at the ISO/AHRI standard rating condition is then derived. This is approximated from a function that relates cooling
capacity to EWT. The function, shown in Figure 4a, is derived from a correlation of performance data for a range of water source heat pump
equipment. If capacity is known at one EWT, the function allows us to estimate the corresponding capacity at any other EWT. This gross cooling
capacity is shown as data point 2 in Figure 4a.
Note that each class of heat pump equipment uses a different standard rating EWT:
Equipment Type
Standard Rating
EWT
Page 22 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
WSHP
86 F (30 C)
GWSHP
59 F (15 C)
GSHP
77 F (25 C)
3. The ISO net cooling capacity at design is calculated next. According to the ISO/AHRI Standard, the net cooling capacity is the gross cooling provided
by the coil minus the portion of fan heat due fan power needed to overcome to internal static losses. Because the split of fan heat due to internal and
external static losses requires data not readily available to the user, the ISO net cooling capacity is estimated as follows:
Qnet = Qtot - 3.412 (Pfan - Pfan,ext)
where:
Qnet = ISO net cooling capacity, MBH (kW)
Qtot = Gross cooling capacity, MBH (kW)
Pfan = Fan input power, kW. Calculated in step 1 of the procedure.
Pext = Portion of fan input power required to overcome external static, kW. Estimated as 4% of total WSHP input power. This 4% factor was derived
from a study of WSHP ratings for a range of units.
The ISO net cooling capacity is shown as data point 3 in Figure 4a.
4. The total input power is then derived. This calculation requires two steps:
Peff = (ISO Net Cooling Capacity) / EER
The ISO/AHRI standard defines EER in terms of an "effective" input power, Peff, where:
Peff = Ptot - Φfa + Φpa
And where:
Ptot = Total input power for the unit, kW.
Φfa = Fan power allowance, kW. This is the portion of fan power needed to overcome external static losses. Approximated as 4 % of Ptot.
Φpa = Pump power allowance, kW. This is the portion of water pump input kW needed to overcome flow resistance in the condenser.
Approximated as 1 % of Ptot.
After calculating Peff from net capacity and EER, Ptot is derived from the second equation. Ptot is shown in Figure 4b as data point 4.
5. The total input power at the specified design condition is derived next. This is approximated from a function that relates input power to EWT. The
function, shown in Figure 4b, is derived from a correlation of performance data for a range of water source heat pump equipment. If input power is
known at one EWT, the function allows us to estimate the corresponding input power at any other EWT. This input power is shown as data point 5 in
Figure 4b.
6. The compressor kW at the design condition is finally calculated: Compressor kW = Total Input Power at Design - Total Indoor Fan kW. This is shown
as data point 6 in Figure 4b.
Page 23 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
F. WSHP, GWSHP, GSHP Equipment - Heating Duty
This section summarizes the procedure for deriving compressor kW from a standard heating COP for water source heat pump (WSHP), groundwater
source heat pump (GWSHP) and ground source heat pump (GSHP) equipment. COP rating procedures for these types of equipment are found in
ISO/AHRI Standard 13256-1.
1. At the start of this procedure the gross heating capacity at design is known. The heating capacity is either directly specified by the user, or is derived
via the auto-sizing option. This heating capacity is shown in Figure 5a as data point 1.
Also known is the design entering water temperature (EWT) corresponding to this design condition. Figure 5a shows a scenario where the design
EWT is colder than the standard rating EWT.
Finally the indoor fan design input kW is calculated based on user specifications for fan performance. Fan heat gain is fan power x 3.412. Fan
Performance Calculations.
2. The gross heating capacity at the ISO/AHRI standard rating condition is then derived. This is approximated from a function that relates heating
capacity to EWT. The function, shown in Figure 5a, is derived from a correlation of performance data for a range of water source heat pump
equipment. If capacity is known at one EWT, the function allows us to estimate the corresponding capacity at any other EWT. This gross heating
capacity is shown as data point 2 in Figure 5a.
Note that each class of heat pump equipment uses a different standard rating EWT:
Equipment Type
Standard Rating
EWT
WSHP
68 F (20 C)
GWSHP
50 F (10 C)
GSHP
32 F (0 C)
3. The ISO net heating capacity at design is calculated next. According to the ISO/AHRI Standard, the net heating capacity is the gross heating provided
by the coil plus the portion of fan heat due to fan power needed to overcome internal static losses. Because the split of fan heat due to internal and
external static losses requires data not readily available to the user, the ISO net heating capacity is estimated as follows:
Qnet = Qtot + 3.412 (Pfan - Pfan,ext)
where:
Qnet = ISO net heating capacity, MBH (kW)
Qtot = Gross heating capacity, MBH (kW)
Pfan = Fan input power, kW. Calculated in step 1 of procedure.
Pext = Portion of fan input power required to overcome external static, kW. Estimated as 4% of total WSHP input power. This 4% factor was derived
from a study of WSHP ratings for a range of units.
The ISO net heating capacity is shown as data point 3 in Figure 5a.
4. The total input power is then derived. This calculation requires two steps:
Peff = (ISO Net Heating Capacity) / (COP x 3.412)
The ISO/AHRI standard defines COP in terms of an "effective" input power, Peff where:
Peff = Ptot - Φfa + Φpa
And where:
Ptot = Total input power for the unit, kW.
Φfa = Fan power allowance, kW. This is the portion of fan power needed to overcome external static losses. Approximated as 4 % of Ptot.
Page 24 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm
Φpa = Pump power allowance, kW. This is the portion of water pump input kW needed to overcome flow resistance in the heat pump evaporator
(i.e., the water to refrigerant heat exchanger). Approximated as 1 % of Ptot.
After calculating Peff from net capacity and COP, Ptot is derived from the second equation. Ptot is shown in Figure 5b as data point 4.
5. The total input power at the specified design condition is derived next. This is approximated from a function that relates input power to EWT. The
function, shown in Figure 5b, is derived from a correlation of performance data for a range of water source heat pump equipment. If input power is
known at one EWT, the function allows us to estimate the corresponding input power at any other EWT. This input power is shown as data point 5 in
Figure 5b.
6. The compressor kW at the design condition is finally calculated: Compressor kW = Total Input Power at Design - Total Indoor Fan kW. This is shown
as data point 6 in Figure 5b.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 25 of 25
31.0 Air System Component Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhBE48.htm