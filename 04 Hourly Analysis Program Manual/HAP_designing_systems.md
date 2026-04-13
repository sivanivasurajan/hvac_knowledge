14.0 Designing Systems
14.1 Overview for System Design Reports
14.0 Designing Systems ››
Overview for System Design Reports Form
14.0 Designing Systems ›› 14.1 Overview for System Design Reports ››
This chapter describes contents of HVAC system design reports in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of HVAC system design reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for System Design Reports Form
About System Design Reports. System Design Reports contain information used to size and select HVAC equipment for air systems, zones and spaces. Reports
also provide data useful when studying building or system performance or investigating problems with system operation. HAP offers nine different tabular reports and
three graphical reports containing system design information.
Using various menu options and toolbar buttons in HAP, there are four different ways of generating system design reports. These methods are described in the
Generating System Design Reports help topic. All four procedures require selection of report options on the System Design Reports window shown below.
The System Design Reports Window is used to specify which reports should be generated and how they should be generated:
1. The Working Area in the center of the window contains two tables used to select report options. The upper table contains sizing reports - the reports containing key
information used to size and select equipment. The lower table contains diagnostic reports - reports containing more detailed information useful for understanding
building load behavior and behavior of the air side systems. Each row in these tables contains specifications for a different report. Columns contain separate
specifications for each report:
a. The Table column is used to select the tabular version of a report. Place a check mark in the box opposite the report name to select the tabular version of that
report.
b. The Graph column is used to select the graphical version of a report. Place a check mark in the box opposite the report name to select the graphical version of
that report.
c. The Time Specifications column describes how individual reports should be generated. The Load Summary and System Psychrometrics reports each contain
data for one hour on one design day. Therefore, the month and hour for the report must be specified. The hourly reports contain 24-hour profiles for the design
day in each month of the year. For these reports the range of months to be included in the report must be defined.
The contents of each report are summarized later in this help topic.
2. Command Buttons appear along the bottom of the form. Five buttons are provided:
a. Press Restore Defaults to reset selections on the form to a standard set of defaults. This is often done when users wish to clear existing selections and then
begin selecting reports all over again.
b. Press Print to print the reports you’ve selected. Reports are directly printed without viewing them first.
c. Press Preview to view the reports you’ve selected. This launches the HAP Report Viewer and displays the reports you requested. The HAP Report Viewer
provides options for printing the reports as well as saving each report as a disk file in Rich Text Format (RTF).
d. Press Cancel to exit from the form and return to the HAP Main Program Window without generating reports.
e. Press Help to display this help topic.
Report Summaries. HAP offers three sizing reports and six diagnostic reports in tabular format. Graphical versions of three of the diagnostic reports are also
available. Each report is summarized below along with a brief description of the time specification options available for the report.
Sizing Reports - These reports contain information used to size and select HVAC equipment.
Page 1 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.2 Air System Sizing Summary Report
14.0 Designing Systems ››
Air System Sizing Summary Report
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
1. System Sizing Summary. The Air System Sizing Summary report provides sizing and selection data for centrally located components in an air system. These
components include cooling coils, heating coils, humidifiers and fans. For example in a rooftop or central AHU system, the report provides data for sizing
components in the rooftop or AHU. For a terminal system using a dedicated outdoor air system (DOAS), the report provides data for sizing components in the
DOAS unit. Length: 1 to 2 pages.
2. Zone Sizing Summary. HAP offers two versions of the Zone Sizing Summary report. The Zone Sizing Summary report for central HVAC systems such as rooftops
or AHUs provides data for sizing zone supply terminals and space supply diffusers in these kinds of systems. The Zone Sizing Summary report for terminal HVAC
systems such as fan coils, WSHPs, VRF indoor units, or chilled beams provides data for sizing and selecting each zone terminal unit as well as space supply
diffusers. Both versions of the report also contain peak cooling and heating load data for zones and spaces served by the system. Length: Varies widely depending
on the number of zones and spaces served by the system.
3. Ventilation Sizing Summary. The Ventilation Sizing Summary documents how the outdoor ventilation airflow rate for the system is calculated. When the "Sum of
Space OA Airflows" method is used, it documents how individual space ventilation requirements are calculated and summed to determine the system total. When
one of the "ASHRAE Std 62.1" methods is used, the report provides data showing how the Standard 62.1 Ventilation Rate Procedure is used to determine total
system outdoor air intake flow rate.
Diagnostic Reports - These reports contain more detailed information useful for investigating and understanding building load behavior and the behavior of air-side
systems.
4. System Load Summary. The Air System Design Load Summary report provides a list of component cooling loads for the air system for one design cooling hour
and a list of component heating loads for the design heating condition. If you mark the "peak" check box for this report, cooling data will be displayed for the month
and hour when the maximum central cooling coil load occurs. If the "peak" box is not checked, you can select from any design month and hour during the year. This
report is typically used when investigating how different load components contribute to the system load. Length: 1 page.
5. Zone Load Summary. The Zone Design Load Summary report provides a list of component cooling and heating loads for each zone in served by the air system. If
you mark the "peak" check box for this report, cooling data will be generated for the month and hour of the peak zone sensible load for each zone. If the "peak" box
is not checked, you can select from any design month and hour during the year. Heating data is always generated for the design heating condition. This report is
typically used when investigating the behavior of zone loads. Length: 2 zones per page.
6. Space Load Summary. The Space Design Load Summary provides a list of component cooling and heating loads for each space in each zone in an air system.
Individual loads for all wall, window, roof, skylight and door elements in a space are also listed. If you mark the "peak" check box for this report, cooling data will be
generated for the month and hour of the peak space sensible load for each space.. If the "peak" box is not checked, you can select from any design month and
month during the year. Heating data is always generated for the design heating condition. This report is used when investigating space load behavior. Length: A
minimum of 1 page per space.
7. Hourly Air System Loads. The Hourly Air System Design Day Loads report provides 24-hour profiles of air system coil loads and fan airflows for design cooling
days. For this report you must specify the range of months for which data will be generated. To generate the report for a single month, specify the same month as
the first and last months (e.g., July to July). This report is used when investigating system load behavior. Length: 2 months per page.
The graphical version of this report provides one graph for each month selected. The graph contains the 24-hour profiles for cooling and heating coil loads in the
system.
8. Hourly Zone Loads. The Hourly Zone Design Day Loads report contains 24-hour profiles of outdoor temperature, indoor temperature, indoor relative humidity,
zone supply airflow and zone loads for design cooling days. The report contains a separate sets of profiles for each zone in the system. For this report you must
specify the range of months for which data will be generated. To generate the report for a single month, specify the same month as the first and last months (e.g.,
July to July). This report is used when investigating zone load behavior or comfort levels within zones. Length: 2 zones per page per month.
The graphical version of this report provides one graph for each zone and each month selected. The graph contains the 24-hour profiles for zone sensible load and
zone conditioning.
9. System Psychrometrics. The System Psychrometrics report provides a detailed account of airflow rates, temperatures and humidities at key points within the air
system for one hour on a design cooling day. If you mark the "peak" check box for this report, the report will be generated for the month and hour when the peak
cooling coil load occurs. In addition, data for the winter design condition will also be provided. If you do not mark the "peak" box, you will be asked to choose the
design cooling month and hour for which data will be generated. This report is used when investigating details of system performance or control. Length: 1-2 pages.
The graphical version of this report plots the temperature and humidity values for each state point in the system on a psychrometric chart. Often system
psychrometric data can be interpreted more efficiently in this format than in the tabular format.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the contents of the Air System Sizing Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air System Sizing Summary Report
The Air System Sizing Summary report provides sizing and selection data for centrally located components in an air system. These components include cooling coils,
heating coils, humidifiers and fans. Sizing data for outdoor ventilation airflow is also provided. For a terminal type system such as fan coils or water source heat
pumps, this report contains sizing information for components in the dedicated outdoor air system (DOAS) AHU. Report Length: 1 to 2 pages.
A sample of this report for a VAV Reheat system is shown below. Following this figure, the format and content of the report is discussed.
Page 2 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Cooling Coil Sizing Data Tables
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
Report Format and Content. The Air System Sizing Summary report begins with two tables describing the general characteristics of the air system and the procedure
used to size it. These are followed by a series of tables each containing sizing information for one of the centrally located components of the system. The sample
report shown above is for a VAV Reheat system and contains sizing data for the central cooling coil, preheat coil, supply fan and outdoor ventilation air. The tables
contained in each copy of this report you generate will vary depending on the components in the system. Tables which can appear in this report are summarized
below.
1. Air System Information - Provides basic reference information for the system. This table lists the system name, equipment class, system type, the number of zones,
the total floor area in zones served by the system, and the city name for design weather data.
2. Sizing Calculation Information - Describes how the sizing calculation was performed.
a. Zone and Space Sizing Method list the methods for calculating zone and space airflow rates. These methods were selected during air system input.
b. Calculation Months lists the range of cooling design months included in the calculation. These months were specified when creating design weather data for the
project.
c. Sizing Data indicates whether system and zone airflow rates were "calculated" by the program or were "user-defined". The "user-defined" label means this sizing
data was specified earlier while inputting air system data. The user-defined option is typically used when studying system performance for retrofit applications.
3. Central Cooling Coil Sizing Data - Sizing data for the central cooling coil in an air system.
4. Cooling Coil Sizing Data - Sizing data for a cooling coil in a Dedicated Outdoor Air System (DOAS) unit used in conjunction with fan coils or water source heat
pumps, and also for the cooling coil in a standalone Make Up Air Unit / DOAS system.
5. Precool Coil Sizing Data - Sizing data for a precool coil located upstream of the main cooling coil in an air system.
6. Central Heating Coil Sizing Data - Sizing data for the central heating coil in an air system.
7. Heating Coil Sizing Data - Sizing data for the heating coil in a Dedicated Outdoor Air System (DOAS) unit used in conjunction with fan coils or water source heat
pumps, and also for the heating coil in a standalone Make Up Air Unit / DOAS system.
8. Preheat Coil Sizing Data - Sizing data for a preheat coil located upstream of the central heating coil in an air system.
9. Humidifier Sizing Data - Sizing data for a central humidifier.
10. Supply Fan Sizing Data - Sizing data for the central supply fan.
11. Hot Deck Supply Fan Sizing Data - Sizing data for the hot deck supply fan in a 2-Fan Dual Duct VAV system.
12. Ventilation Fan Sizing Data - Sizing data for the ventilation fan in a DOAS unit or in a standalone Make Up Air Unit / DOAS system.
13. Return Fan Sizing Data - Sizing data for the return fan in a central system.
14. Exhaust Fan Sizing Data - Sizing data for the exhaust fan in a DOAS unit or in a standalone Make Up Air Unit / DOAS system.
15. Outdoor Ventilation Air Data - The required outdoor ventilation airflow rate plus useful check figures.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Sizing Data Tables
Page 3 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
All cooling coil sizing tables on the Air System Sizing Summary report (central cooling coil, cooling coil, precool coil) have a similar format and content. A sample of
this table for a central cooling coil is shown above. Items in this table are as follows:
1. Total Coil Load is the maximum load for this cooling coil. It includes both sensible and latent components. This load is listed twice – once in MBH (kW) and once in
Tons (kW). The value in MBH is often needed for equipment selection. The value in Tons is sometimes a useful check figure for size.
2. Sensible Coil Load is the sensible component of the coil load for the month and hour when the maximum coil load occurs.
3. Coil Airflow at Time is the airflow rate for the coil for the month and hour when the maximum coil load occurs. For most systems it represents a constant airflow for
the duration of the hour.
For systems using cycled supply fan operation it represents the hourly averaged airflow rate. For example, a constant volume system which delivers 1000 CFM but
is cycled on for 95% of the hour will list the coil airflow as 950 CFM.
For VVT systems, this airflow is a weighted average value of airflow rates for the cooling and ventilation (or "float") modes occurring during the hour the peak load
occurs.
4. Max Block Airflow at Time is the maximum block airflow rate for the cooling coil. For certain types of systems the maximum block airflow can differ from the coil
airflow at the peak load time. In VAV systems, CAV systems using fan cycling, and 2-Deck Multizone, 3-Deck Multizone or dual duct systems, this typically occurs
when the month and hour for the peak coil load differs from the month and hour for peak airflow. Conditions which can cause a difference between these airflows
are summarized below. In the paragraphs below the term Vblock represents the maximum block airflow while Vcoil,peak represents the airflow at the time the peak coil
load occurs.
For central cooling coils, the following relationships between Vblock and Vcoil,peak can exist:
a. Single-Duct CAV, no fan cycling: Vblock will always equal Vcoil,peak.
b. Single-Duct CAV, with fan cycling: Vblock can be greater than Vcoil,peak if the supply fan is cycled on for less than 100% of the hour in which the maximum coil
load occurs.
c. Multizone or Dual Duct CAV: Vblock can be greater than Vcoil,peak if a portion of supply air is flowing through the neutral deck or hot deck for the hour when the
peak coil load occurs. Often this is the result of loads in zones served by the system peaking at different times.
d. VAV Systems: Vblock can be greater than Vcoil,peak when the time of the maximum diversified airflow for the supply fan differs from the time of the peak cooling
coil load.
For precool coils and for cooling coils in Dedicated Outdoor Air System (DOAS) or a standalone Make Up Air Unit / DOAS system, the following relationships
between Vblock and Vcoil,peak can exist:
a. For a precool coil downstream of the point where return air and ventilation air mix, Vblock can equal or exceed Vcoil,peak for the same reasons listed above for
central cooling coils.
b. For a precool coil upstream of the mixing point, Vblock will equal Vcoil,peak if the outdoor ventilation airflow is constant at all times. If proportional, scheduled or
CO2 sensor controls are used with ventilation, it is possible for Vcoil,peak to be less than Vblock since ventilation airflow will vary from hour to hour.
When the Vblock and Vcoil,peak differ, designers are faced with the dilemma of which airflow to use when selecting equipment. This problem is compounded by the
fact that both the coil and the fan must be selected together for many types of equipment. Guidelines are provided below:
a. Central Cooling Coils in CAV Systems Which Use Fan Cycling: Use Vblock together with the maximum coil load to select equipment. Vcoil,peak should not be used
because it represents an average hourly airflow rather than an actual airflow.
b. For Central Cooling Coils in VAV, 2-Deck Multizone, 3-Deck Multizone and Dual Duct Systems: Select the cooling coil using the Vcoil,peak. Then check the fan
performance data to confirm that the fan can operate at its specified maximum airflow and does not exceed the maximum RPM. Further, the fan motor must be
selected based on the motor BHP or kW at Vblock rather than Vcoil,peak.
c. For Precool Coils and Cooling Coils used in DOAS systems: Use Vcoil,peak. This will ensure that the coil has capacity to meet any smaller loads occurring at larger
airflows. Also check the coil face velocity at the maximum coil airflow to verify it does not exceed desired limits.
5. Sum of Peak Zone Airflows defines the maximum possible coil airflow rate. For a constant volume system this will equal the Maximum Block airflow. For a VAV
system it will typically be larger than the Maximum Block airflow since it does not include diversity. This value is useful for judging diversity in VAV systems and for
sizing components for special operating periods when all VAV box dampers are full open at the same time.
6. Sensible Heat Ratio defines the ratio of sensible coil load divided by total coil load. It is often useful as a check figure.
7. sqft/Ton or sqm/kW is the ratio of total floor area served by the air system divided by the maximum cooling coil load. This is often a useful check figure. It is only
displayed in sizing tables for central cooling coils.
8. BTU/hr/sqft or W/sqm is the ratio of maximum cooling coil load (in BTU/hr or W) divided by the total floor area served by the air system. This is often a useful
check figure. It is only displayed in sizing tables for central cooling coils.
9. Water Flow Rate. This item defines the required water flow rate for a chilled water cooling coil. It is calculated using the maximum cooling coil load and the coil
delta-T specified by the user in air system inputs. This delta-T defines the difference between outlet and inlet water temperatures for the coil. This item is only
displayed for a coil whose cooling source is chilled water.
10. Load Occurs At... lists the month and hour when the maximum cooling coil load occurs.
11. OA DB / WB lists the outdoor air dry-bulb and wet-bulb temperatures for the month and hour when the maximum coil load occurs.
12. Entering DB / WB lists the dry-bulb and wet-bulb temperatures of air entering the cooling coil for the month and hour when the maximum coil load occurs.
13. Leaving DB / WB lists the dry-bulb and wet-bulb temperatures of air leaving the cooling coil for the month and hour when the maximum coil load occurs.
14. Coil ADP lists the "apparatus dew-point" temperature for the coil for the month and hour when the maximum coil load occurs. The ADP temperature is the
theoretical temperature of air leaving the coil if it was cooled to saturation. It is provided for reference purposes and is only listed in sizing tables for the central
cooling coil.
15. Bypass Factor defines the cooling coil bypass factor used in coil calculations.
16. Resulting RH lists the weighted average relative humidity for zones served by the system for the month and hour when the maximum cooling coil load occurs. It is
a useful check figure for confirming that the system is maintaining desired comfort conditions in the zones. This item is only provided for central cooling coils.
Page 4 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Heating Coil Sizing Data Tables
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
17. Design Supply Temperature defines the required cooling supply air temperature at the zone terminals. This item is only displayed in sizing tables for central
cooling coils. When the sizing criteria specified by the user is supply temperature, the input value is listed on the report. When sizing criteria specified by the user is
CFM, L/s, CFM/sqft or L/s/sqm, the required supply temperature calculated by the program will be listed.
18. Zone T-stat Check describes the status of zone air temperatures for the month and hour when the maximum cooling coil load occurs. This item is only provided
for central cooling coils. The first value listed is the number of zone air temperatures which lie below the upper limit of the cooling thermostat throttling range. The
second number is the total number of zones in the system.
Example: The sample cooling coil sizing table above is for a VAV Reheat system which serves five zones. The cooling thermostat setpoint is 75 F with a throttling
range of 3 F. For July 1500 when the maximum cooling coil load occurs, the air temperature in all five zones is at or below 78 F. Therefore the output states that "5
of 5 OK". If one of the five zones was warmer than 78 F, the output would instead state "4 of 5 OK".
This item is a useful check figure for confirming that the system is maintaining desired comfort conditions in the zone for the hour when the maximum coil load
occurs. When one or more zones are warmer than the upper limit of the thermostat throttling range, it is often due to system operating problems in dealing with very
large pulldown loads. These problems can be investigated further by generating the Hourly Zone Design Day Cooling Loads or the System Psychrometrics reports.
19. Max Zone Temperature Deviation is used in conjunction with the Zone Tstat Check item above. It indicates the largest difference between a zone air temperature
and the upper limit of the cooling thermostat. When zone temperature problems occur, it is used to judge the severity of the problem. Note that if there are no zone
temperature problems, this item will be displayed as 0.
Example: The cooling setpoint is 74 F (23.3 C) and the throttling range is 2 F (1.1 K). Therefore the upper limit of the cooling thermostat is 74 + 2 = 76 F (24.4 C). If
the warmest zone is at 76.4 F (24.7 C), then the "maximum zone temperature deviation" will be listed as 0.4 F (0.2 K).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Sizing Data Tables
All heating coil sizing tables on the Air System Sizing Summary report (central heating coil, heating coil, preheat coil, central reheat coil) have a similar format and
content. A sample of this table for a central heating coil is shown above. Items in this table are as follows:
1. Max Coil Load lists the largest load calculated for the heating coil. The time when this load occurs is listed opposite the "Load occurs at..." item.
2. Coil Airflow at Peak Load Time provides the coil airflow rate at the time the maximum coil load occurs. For most systems it represents a constant airflow for the
duration of the hour.
For systems using cycled supply fan operation, however, it represents the hourly averaged airflow rate. For example, a constant volume system which delivers 1000
CFM but is cycled on for 95% of the hour will list the coil airflow as 950 CFM.
For VVT systems, this airflow is a weighted average value of airflow rates for the heating and ventilation (or "float") modes occurring during the hour the peak load
occurs.
3. Max Coil Airflow is the maximum airflow for this heating coil. For certain types of heating coils and air systems the maximum possible coil airflow can differ from the
coil airflow at the peak load time. Conditions which can cause a difference between these airflows are summarized below. In the following paragraphs Vmax
represents the maximum coil airflow while Vcoil,peak represents the airflow at the time of the peak coil load.
For central heating coils the following relationships between Vmax and Vcoil,peak can exist:
a. Single-Duct CAV, no fan cycling: Vmax will always equal Vcoil,peak.
b. Single-Duct CAV, with fan cycling: Vmax can be greater than Vcoil,peak if the supply fan is cycled on for less than 100% of the peak coil load hour.
c. Multizone or Dual Duct CAV: Vmax can be greater than Vcoil,peak if a portion of supply air is flowing through the neutral deck or cold deck for the hour when the
peak coil load occurs. This often occurs because zone airflow rates are sized based on cooling criteria. Consequently, a mixture of hot and neutral deck air, or
hot and cold deck air is required at the design heating condition.
For preheat coils and for heating coils in Dedicated Outdoor Air Systems (DOAS) and standalone Make Up Air Unit / DOAS systems, the following relationships
between Vmax and Vcoil,peak can exist:
a. For a preheat coil downstream of the point where return air and ventilation air mix, Vmax can equal or exceed Vcoil,peak for the same reasons listed above for
central heating coils.
b. For a preheat coil upstream of the mixing point, Vmax will equal Vcoil,peak if the outdoor ventilation airflow is constant at all times. If proportional, scheduled or CO2
sensor controls are used with ventilation, it is possible for Vcoil,peak to be less than Vmax since ventilation airflow varies from hour to hour.
For central reheat coils used for dehumidification control, Vmax can exceed Vcoil,peak if the peak load time occurs when a cycled system is not running 100% of the
hour, or in a VAV system in which less than 100% of design supply fan airflow is being used.
When Vmax and Vcoil,peak differ, designers are faced with the dilemma of which airflow to use when selecting equipment. Guidelines are provided below:
a. Central Heating Coils in CAV Systems Which Use Fan Cycling: Use Vmax and the maximum heating coil load. Vcoil,peak should not be used because it represents
an average hourly airflow rather than an actual airflow.
b. For All Other Cases: Use Vcoil,peak. This will ensure the coil has capacity to meet any smaller loads occurring at larger airflow rates. Also check coil face velocity
using the maximum coil airflow to make sure velocity does not exceed desired limits.
4. Water Flow Rate. This item defines the required water flow rate for a hot water heating coil. It is calculated using the maximum heating coil load and the coil delta-T
specified by the user. The delta-T defines the difference between inlet and outlet water temperatures for the coil. Data is displayed for this item only for coils whose
heating source is hot water.
5. Load Occurs At... lists the month and hour when the maximum heating coil load occurs. For preheat and central heating coils maximum heating coil data is taken
from the design heating condition. Thus, "Des Htg" will be listed for these coils. For a central reheat coil, the maximum load time will occur for a design cooling day
since this coil is part of the dehumidification control. In this case a specific month and hour will be listed.
6. BTU/hr/sqft or W/sqm defines the ratio of maximum heating coil load (in BTU/hr or W) divided by the total floor area served by the air system. This is often a useful
check figure. This item is only included in the sizing table for a central heating coil
7. Ent DB / Lvg DB provides the coil entering and leaving dry-bulb temperatures. This data is often needed for selecting heating coils.
Page 5 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Humidifier Sizing Data Table
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
Fan Sizing Data Tables
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
Outdoor Ventilation Sizing Table
14.0 Designing Systems ›› 14.2 Air System Sizing Summary Report ››
14.3 Zone Sizing Summary Report
14.0 Designing Systems ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Humidifier Sizing Data Table
The Humidifier Sizing Data table on the Air System Sizing Summary report contains information used to size and select humidification equipment. A sample of this
table is shown above. Items in this table are as follows:
• Max Steam Flow lists the flow rate of steam that must be added to the supply air stream to keep zones at the minimum RH setpoint. Steam flow calculations
are performed for the design heating condition.
• Airflow Rate lists the supply airflow rate for the design heating condition.
• Air Mass Flow lists the supply airflow rate in terms of mass flow (lb/hr or kg/hr) rather than in terms of volumetric flow (CFM or L/s). When selecting certain
types of humidification equipment mass flow is required.
• Moisture Gain defines the rise in specific humidity for air passing through the humidifier section of the supply duct (lb/lb or kg/kg). Moisture gain is sometimes
required for selecting humidification equipment. Otherwise, it serves as a useful check figure.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Sizing Data Tables
All fan sizing tables on the Air System Sizing Summary report (supply, hot deck, ventilation and return) have a similar format and content. A sample of this table for a
supply fan is shown above. Items in this table are as follows:
1. Actual Max. Airflow at Peak Airflow Time lists the maximum airflow for the fan and the month and hour when this maximum airflow occurs. Actual airflow that has
been adjusted for altitude is provided. In the sample above the peak airflow is 8155 CFM and this peak occurs during the design cooling day for August at 1600.
2. Standard Airflow provides the maximum fan airflow in terms of standard airflow for sea level conditions.
3. Actual max CFM/sqft or L/s/sqm is the ratio of the actual maximum fan airflow divided by the total floor area served by the system. It serves as a useful check
figure.
4. Fan Motor BHP is the brakehorsepower for the fan motor, computed using the maximum fan airflow and the user's fan input data.
5. Fan Motor kW is the input power for the fan motor, computed using the maximum fan airflow and the user's fan input data.
6. Fan Static is the fan total static pressure specified by the user. If the user supplied fan BHP or fan motor kW in the air system inputs, this item will not be provided.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Outdoor Ventilation Sizing Table
The final table on the Air System Sizing Summary defines the required outdoor ventilation airflow for the system. A sample of this table is shown above. Items in this
table are as follows:
1. Design Airflow defines the design outdoor ventilation requirement for the system. Further information about how this ventilation airflow is calculated is provided on
the Ventilation Sizing Summary report.
2. CFM/sqft or L/s/sqm is the design ventilation airflow divided by the total floor area served by the system. This value serves as a useful check figure.
3. CFM/person or L/s/person is the design ventilation airflow divided by the maximum coincident occupancy specified for the system. It serves as a useful check
figure. Maximum coincident occupancy is computed by summing the occupant values specified for each space in each zone served by the air system. The
calculation considers the occupant schedules specified, but does not consider diversity factors.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Zone Sizing Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Zone Sizing Summary Report for Central HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
Zone Sizing Summary Report for Central HVAC Systems
When dealing with central HVAC systems such as VAV or CAV systems, the Zone Sizing Summary provides data for sizing zone supply terminals and space supply
diffusers. The report also contains peak sensible cooling and heating load data for zones and spaces served by the system.
A separate version of the report is provided for terminal systems such as fan coils, VRF, water source heat pumps, induction beams, active chilled beams and 4-pipe
induction system.
Report Length: Varies with number of zones and spaces in system.
A sample of this report for a VAV Reheat system is shown below. Following this figure, the format and content of the report is discussed.
Report Format and Content. The Zone Sizing Summary report consists of four tables containing load and sizing information. Each table is summarized below.
1. Air System Information
Provides basic reference information for the system. This table lists the system name, equipment class, system type, the number of zones, the total floor area in
zones served by the system, and the city name for design weather data.
2. Sizing Calculation Information
Describes how the sizing calculation was performed.
Zone and Space Sizing Method list the methods for calculating zone and space airflow rates. These methods were selected during air system input.
Calculation Months lists the range of cooling design months included in the calculation. These months were specified when creating design weather data for the
project.
Sizing Data indicates whether system and zone airflow rates were "calculated" by the program or were "user-defined". The "user-defined" label means this sizing
data was specified earlier while inputting air system data. The user-defined option is typically used when studying system performance for retrofit applications.
Page 7 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Zone Terminal Sizing Table for Central HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
Zone Peak Sensible Loads for Central HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
3. Zone Terminal Sizing Data:
Sizing information for zone maximum and minimum airflow rates, terminal reheat coils, supplemental zone heating units and fan powered mixing box fans. This
data is used to select terminal equipment.
4. Zone Peak Sensible Loads Data:
Peak sensible cooling and heating loads for each zone, plus zone floor area and airflow per sqft or per sqm. This is reference information to assist understanding of
the sizing data in the previous table.
5. Space Loads and Airflows:
Peak sensible cooling and heating loads for spaces in each zone, plus required supply airflow rates for each space, the space floor area and the airflow per sqft or
per sqm.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Terminal Sizing Table for Central HVAC Systems
The Zone Terminal Sizing Data table on the Zone Sizing Summary contains sizing data for terminal equipment such as diffusers, VAV boxes, reheat coils and fan
powered mixing boxes, plus data for supplemental zone heating units. Each row in the table contains data for a separate zone. Columns in the table contain the
different sizing values. Columns in this table are as follows:
1. Zone Name lists the name assigned to the zone during air system inputs. If names were not specified during air system input, default names such as Zone 1, Zone
2, etc... will appear in this column.
2. Design Supply Airflow is the required supply airflow rate for the zone. Actual airflow is listed and thus includes adjustments for altitude. The calculation of this
sizing value depends on the zone and space airflow sizing method selected by the user. In three of the four sizing methods offered, zone airflow is calculated using
the maximum zone load. For cooling-only systems, the maximum zone sensible cooling load is used. For heating-only systems, the design heating load is used. For
systems providing cooling and heating, the program considers the maximum cooling and heating loads and determines which requires the larger supply airflow.
Finally, for the fourth sizing method, the zone airflow rate is the sum of required airflow rates for spaces in the zone. The help topic for zone sizing calculations
provides further information on this subject.
3. Minimum Supply Airflow is the minimum supply airflow rate required for the zone terminal. It applies to VAV and fan powered mixing box terminals. It is based on
the larger of the user’s minimum airflow specification (CFM/person, CFM/sqft, CFM, % of supply air, or ACH. L/s/person, L/s/sqm, L/s, % of supply air, or ACH), or
the outdoor ventilation airflow requirement. For constant volume supply terminals, the minimum airflow will equal the design airflow since these terminals provide the
same airflow for all operating conditions.
4. Zone Airflow per sqft or per sqm is the design airflow divided by the zone floor area. This value often serves as a useful check figure.
5. Reheat Coil Load is the required capacity for a terminal reheat coil in this zone. For information on how the required capacity is calculated, click here: Reheat
Capacity Calculation.
6. Reheat Coil Water Flow Rate is the required water flow rate for a hot water reheat coil. It is calculated using the required reheat coil capacity and the coil delta-T
specified by the user. The delta-T defines the difference between the inlet and outlet water temperatures for the coil. Flow rates are only listed when the heating
source for the reheat coils is hot water.
7. Zone Htg Coil Load lists the required heating capacity for a supplemental zone heating unit. These are baseboard or fan coil heating units in the zone which are
controlled either with an indoor thermostat or an outdoor thermostat. For information on how the required capacity is calculated, click here: Zone Heating Unit
Capacity Calculation.
8. Zone Htg Water Flow Rate is the required water flow rate for a hot water heating coil in a supplemental zone heating unit. It is calculated using the zone heating
unit capacity and the coil delta-T specified by the user. This delta-T is the difference between inlet and outlet water temperatures for the coil. Flow rates are only
listed when the heating source for the zone units is hot water.
9. Mixing Box Fan Airflow is the required airflow rate for a series or parallel fan powered mixing box fan in the zone terminal. Actual airflow is listed and therefore
includes adjustments for altitude. When the zone terminal is not a fan powered mixing box, a zero airflow will be listed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Peak Sensible Loads for Central HVAC Systems
Page 8 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Space Load and Airflow Sizing Table for Central HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
Zone Sizing Summary Report for Terminal HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
The Zone Peak Sensible Loads table on the Zone Sizing Summary contains peak sensible cooling and heating loads for each zone, and the zone floor area. Each row
in the table contains data for a separate zone. Each column contains a separate category of sizing information. Columns in this table are as follows:
1. Zone Name lists the name assigned to the zone during air system inputs. If names were not specified during air system input, default names such as Zone 1, Zone
2, etc... will appear in this column.
2. Zone Cooling Sensible is the peak zone sensible cooling load. It is determined by calculating hourly profiles of zone sensible cooling loads for design days and
then searching the profiles for the largest load.
3. Time of Peak Load lists the month and hour when the peak zone sensible cooling load occurs.
4. Zone Heating Load is the zone sensible load calculated at the design heating condition.
5. Zone Floor Area is the total floor area for the zone.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Load and Airflow Sizing Table for Central HVAC Systems
The Space Load and Airflow table on the Zone Sizing Summary contains peak sensible cooling and heating loads for spaces served by the system, and required
supply airflow rates for each space. Each row in this table contains data for a separate space. Columns in the table contain the different load and sizing values.
Columns in this table are as follows:
1. Zone Name / Space Name. This column provides a list of all spaces served by the system. Spaces are grouped according to zone.
2. Mult defines the space multiplier. All cooling load, heating load and space airflow data in the table is for a single space and therefore does not include this multiplier
factor. However, when investigating results it is sometimes necessary to calculate the total airflow or load for all spaces in a zone. Thus, the space multiplier is
provided so this calculation can be performed by the user.
Example: In the sample above "North Office" represents one of eight identical offices and therefore has a multiplier of 8. The required airflow for one of these offices
is 178 CFM. The total airflow for all six of these identical offices is 8 x 178 or 1024 CFM.
3. Cooling Sensible. When the space airflow sizing method selected by the user requires space airflow rates to be computed based on the space load, the maximum
sensible cooling load for the space is listed in this column. The month and hour for this load is reported in the "Time of Load" column.
When the chosen sizing method requires space airflows be calculated for coincident space loads or based on zone CFM/sqft or L/s/sqm, space sensible cooling
loads for the time the peak zone load will be listed.
In the sample figure above, space airflow rates have been calculated based on the peak space load.
4. Time of Peak Sensible Load defines the month and hour for the load listed in the "Cooling Sensible" column. When the space sizing method requires that airflows
be calculated from the peak space load, the month and hour for the peak sensible cooling load for each space will be listed.
When the chosen sizing method requires space airflows to be calculated for coincident space loads, or based on zone CFM/sqft or L/s/sqm, the time of the peak
zone load will be listed in this column.
5. Airflow defines the required airflow rate for the space. Airflow data is listed in actual terms corrected for altitude effects. This value can be used to size the supply
diffuser for the space.
6. Heating Load lists the space load for the design heating condition.
7. Floor Area lists the floor area for each space.
8. Space Airflow per sqft or per sqm is the space airflow divided by the space floor area. It often serves as a useful check figure.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Zone Sizing Summary Report for Terminal HVAC Systems
The version of the Zone Sizing Summary Report for terminal HVAC systems provides data for sizing each terminal unit and the space supply diffusers it serves. The
report also contains peak sensible cooling and heating load data for the zones and spaces in the system.
This version of the report is used for fan coils, VRF, water source heat pumps, induction beams, active chilled beams or 4-pipe induction systems. A separate version
of the report is provided for central systems such as VAV or CAV systems.
Report Length: Varies with number of zones and spaces in system.
A sample of this report for a packaged DX fan coil system is shown below. Following this figure, the format and content of the report is discussed.
Report Format and Content. The Zone Sizing Summary report consists of four tables containing load and sizing information. Each table is summarized below.
1. Sizing Calculation Information
Describes how the sizing calculation was performed.
Zone and Space Sizing Method list the methods for calculating zone and space airflow rates. These methods were selected during air system input. This
information is shown for all terminal systems except induction beams and active chilled beams, for which the zone and space sizing method is not applicable.
Calculation Months lists the range of cooling design months included in the calculation. These months were specified when creating design weather data for the
project.
Sizing Data indicates whether system and zone airflow rates were "calculated" by the program or were "user-defined". The "user-defined" label means this sizing
data was specified earlier while inputting air system data. The user-defined option is typically used when studying system performance for retrofit applications.
2. Terminal Unit Sizing Data
This section contains information required to size and select each terminal unit. The section is divided into two tables. The first table provides sizing data for
cooling duty. The second table provides sizing data for heating duty, the terminal fan and ventilation airflow.
3. VRF Outdoor Unit Sizing Table
This section only appears when the system type is Variable Refrigerant Flow (VRF). It contains cooling and heating capacity information required to size and select
the VRF outdoor unit.
4. Zone Peak Sensible Loads
This section contains peak sensible cooling and heating loads for each zone, plus zone floor area and airflow per sqft or per sqm. This is reference information to
assist understanding of the sizing data in the previous table.
5. Space Loads and Airflows:
Page 10 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Terminal Unit Sizing Tables for Terminal HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
Peak cooling and heating loads for spaces in each zone, plus required supply airflow rates for each space, the space floor area and airflow per sqft or per sqm.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Unit Sizing Tables for Terminal HVAC Systems
The Terminal Unit Sizing tables on the Zone Sizing Summary provide data used to size and select the terminal unit equipment. The first of two tables in this section
provides cooling sizing data. The second data provides heating, fan and ventilation sizing data. In these tables each row contains data for one zone's equipment.
Each column contains different sizing information for the equipment.
Terminal Unit Sizing Data - Cooling
Column content for this table is the same for all terminal systems.
1. Total Coil Load lists the maximum cooling coil load. This load includes both sensible and latent components. It is determined by calculating hourly profiles of
cooling coil loads for each design day and then identifying the largest coil load in these profiles. The month and hour when this load occurs are provided in the "time
of peak load" item in this sizing table.
For Active Chilled Beam systems, the total and sensible coil loads will be highlighted red if total is greater than sensible. This indicates a latent load exists on the
terminal coil. Because an Active Chilled Beam terminal is a sensible-only device which does not have a drain pan to collect condensed moisture, the presence of a
latent load indicates a design problem.
2. Sens Coil Load is the sensible component of coil load for the month and hour when the largest coil load occurs.
3. Coil Entering DB / WB provides the dry-bulb and wet-bulb temperatures of air entering the cooling coil for the time of the maximum coil load.
4. Coil Leaving DB / WB provides the dry-bulb and wet-bulb temperatures of air leaving the cooling coil for the time of the maximum coil load.
5. Water Flow Rate. This item defines the required water flow rate for a chilled water cooling coil. It is calculated using the maximum cooling coil load and the coil
delta-T specified by the user. The delta-T defines the difference between outlet and inlet water temperatures. Water flow rates are only provided for coils whose
cooling source is chilled water.
6. Time of Peak Coil Load lists the month and hour when the largest cooling coil load occurs.
7. Zone Airflow per Unit Floor Area lists the supply air CFM/sqft of L/s/sqm for the zone. This is often used as a check figure.
Terminal Unit Sizing Data - Heating, Fan, Ventilation
This table contains information for sizing the heating coil, the terminal fan and outdoor air ventilation airflow. Note that for terminal units without a fan (induction
beams, active chilled beams), this table omits the fan sizing data.
1. Heating Coil Load lists the maximum heating coil load. This load is obtained from a calculation of terminal unit operation for the design heating condition.
2. Heating Coil Ent / Lvg DB provides the dry-bulb temperatures of air entering and leaving the heating coil for the design heating condition.
3. Heating Coil Water Flow Rate. This item defines the required water flow rate for a hot water heating coil. It is calculated using the maximum heating coil load and
the coil delta-T specified by the user. The delta-T defines the difference between inlet and outlet water temperatures for the coil. Water flow rates are only displayed
for coils whose heating source is hot water.
4. Fan Design Airflow is the required airflow for the terminal unit fan. Actual airflow, which has been adjusted for altitude, is reported here.
5. Fan Motor BHP is the brakehorsepower for the fan motor, computed using the design fan airflow and the user's fan input data.
6. Fan Motor kW is the input power for the fan motor, computed using the design fan airflow and the user's fan input data.
7. OA Vent Design Airflow is the flow rate for outdoor ventilation air supplied to the terminal unit. When direct ventilation is used, this is untreated outdoor air at the
ambient temperature and humidity. When a Dedicated Outdoor Air System (DOAS) is used this is conditioned or unconditioned air supplied to the terminal unit by
the DOAS unit.
This column is shown for fan coil, water source heat pump, and VRF terminals.
Page 11 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
VRF Outdoor Unit Sizing Table
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
Zone Peak Sensible Loads for Terminal HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
8. Primary Airflow is the required primary supply airflow rate to an induction beam or active chilled beam terminal. This column is only shown for those two system
types.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
VRF Outdoor Unit Sizing Table
This section of the Zone Sizing Summary report only appears when the system type is Variable Refrigerant Flow (VRF). The table provides cooling and heating
capacity sizing information necessary to size and select the VRF outdoor unit for the system. Rows in the table contain component loads and the total required
capacity. Columns contain cooling and heating requirements. Items in this table include:
1. Peak Coincident Indoor Unit Loads. This row lists the largest combined indoor unit (IDU) load imposed on the outdoor unit (ODU). The outdoor unit serves
multiple indoor units whose loads vary independently. Typically the outdoor unit is sized on the peak coincident, or largest combined load, imposed by the indoor
units at one point in time, rather than being sized on the sum of individual peak IDU loads. Therefore, the peak coincident load accounts for load diversity among
the indoor units.
2. Estimated Piping / Line Losses. The ODU must also be sized to overcome refrigerant piping losses that occur between the outdoor unit and the indoor units.
When long lines exist, the VRF outdoor unit will have to generate extra cooling or heating output to overcome refrigerant pressure drop in the lines to satisfy loads
at the indoor unit. Refrigerant line length and vertical distance were specified on the Equipment tab of the Air System Properties window and are used to calculate
capacity correction factors to determine the line losses shown in this table. For example if the capacity correction factor for a given pipe length is 0.9, the outdoor
unit will have to provide 100/0.9 or 111 MBH of cooling output in order to meet a load of 100 MBH at the indoor units. Separate correction factors are calculated for
cooling duty and heating duty based on the piping length and vertical distance.
If the estimated line loss is shown as zero, it either means that you did not specify line length and vertical distance, or the line length and vertical distances are very
small resulting in negligible losses.
Note that refrigerant line losses vary with each particular VRF outdoor unit product line and model size. HAP uses capacity correction factors that are an average of
many manufacturer's products and models in order to represent "typical" losses. Therefore, when selecting equipment it is critical to consult actual product data to
determine the capacity correction factors for the specific product you are selecting, and then apply these correction factors to determine your actual losses and the
actual total required ODU capacity.
3. Total Required ODU Capacity. This is the sum of the peak coincident IDU load and the estimated line loss. As noted in the previous item, the line loss included in
this total is an estimated "typical" value. Therefore, when selecting equipment you should always determine the actual line losses for your product, recalculate the
line loss that applies to your specific product, and calculate a new total required capacity using that line loss.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Peak Sensible Loads for Terminal HVAC Systems
The Zone Peak Sensible Loads table on the Zone Sizing Summary contains peak sensible cooling and heating loads for each zone, and the zone floor area. Each row
in the table contains data for a separate zone. Each column contains a separate category of sizing information. Columns in this table are as follows:
1. Zone Name lists the name assigned to the zone during air system inputs. If names were not specified during air system input, default names such as Zone 1, Zone
2, etc... will appear in this column.
2. Zone Cooling Sensible is the peak zone sensible cooling load. It is determined by calculating hourly profiles of zone sensible cooling loads for design days and
then searching the profiles for the largest load.
3. Time of Peak Load lists the month and hour when the peak zone sensible cooling load occurs.
4. Zone Heating Load is the zone sensible load calculated at the design heating condition.
5. Zone Floor Area is the total floor area for the zone.
Page 12 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Space Load and Airflow Sizing Table for Terminal HVAC Systems
14.0 Designing Systems ›› 14.3 Zone Sizing Summary Report ››
14.4 Ventilation Sizing Summary Report
14.0 Designing Systems ››
Ventilation Sizing Summary Report
14.0 Designing Systems ›› 14.4 Ventilation Sizing Summary Report ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Load and Airflow Sizing Table for Terminal HVAC Systems
The Space Load and Airflow table on the Zone Sizing Summary contains peak sensible cooling and heating loads for spaces served by the system, and required
supply airflow rates for each space. Each row in this table contains data for a separate space. Columns in the table contain the different load and sizing values.
Columns in this table are as follows:
1. Zone Name / Space Name. This column provides a list of all spaces served by the system. Spaces are grouped according to zone.
2. Mult defines the space multiplier. All cooling load, heating load and space airflow data in the table is for a single space and therefore does not include this multiplier
factor. However, when investigating results it is sometimes necessary to calculate the total airflow or load for all spaces in a zone. Thus, the space multiplier is
provided so this calculation can be performed by the user.
Example: In the sample above "North Office" represents one of eight identical offices and therefore has a multiplier of 8. The required airflow for one of these offices
is 178 CFM. The total airflow for all six of these identical offices is 8 x 178 or 1024 CFM.
3. Cooling Sensible. When the space airflow sizing method selected by the user requires space airflow rates to be computed based on the space load, the maximum
sensible cooling load for the space is listed in this column. The month and hour for this load is reported in the "Time of Load" column.
When the chosen sizing method requires space airflows be calculated for coincident space loads or based on zone CFM/sqft or L/s/sqm, space sensible cooling
loads for the time the peak zone load will be listed.
In the sample figure above, space airflow rates have been calculated based on the peak space load.
4. Time of Peak Sensible Load defines the month and hour for the load listed in the "Cooling Sensible" column. When the space sizing method requires that airflows
be calculated from the peak space load, the month and hour for the peak sensible cooling load for each space will be listed.
When the chosen sizing method requires space airflows to be calculated for coincident space loads, or based on zone CFM/sqft or L/s/sqm, the time of the peak
zone load will be listed in this column.
5. Airflow defines the required airflow rate for the space. Airflow data is listed in actual terms corrected for altitude effects. This value can be used to size the supply
diffuser for the space.
6. Heating Load lists the space load for the design heating condition.
7. Floor Area lists the floor area for each space.
8. Space Airflow per sqft or per sqm is the space airflow divided by the space floor area. It often serves as a useful check figure.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Ventilation Sizing Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Sizing Summary Report
The Ventilation Sizing Summary report documents how the outdoor ventilation airflow rate for the system is calculated. The report uses different formats depending on
which method is selected to size ventilation airflow:
1. When the Sum of Space OA Airflows method is chosen, the report documents how individual space ventilation requirements are calculated and summed to
determine the system total. More information.
2. When the ASHRAE Std 62-2001 or ASHRAE Std 62-2001 (max only) method is chosen, the report documents how the Standard 62-2001 Ventilation Rate
Procedure is used to determine space and ventilation airflow rates. More information.
3. When the one of the ASHRAE Standard 62.1 methods is chosen (2004, 2007, 2010, or 2013 editions) , the report documents how the Standard 62.1 Ventilation
Rate Procedure is used to determine space and ventilation airflow rates. The report is generated in two different formats - one for central systems such as VAV or
CAV, and one for terminal systems such as fan coils, water source heat pumps, VRF, induction beam or chilled beam systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 13 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Vent Sizing Summary for Summation Method
14.0 Designing Systems ›› 14.4 Ventilation Sizing Summary Report ››
Vent Sizing Summary for Summation Method
This topic describes the format and content of the Ventilation Sizing Summary Report when the "Sum of OA Airflows" sizing method is selected. For this situation the
report documents how individual space ventilation requirements are calculated and summed to determine the system total. The report is generated using two similar
but separate formats.
1. Ventilation Sizing Summary for Central Systems - This format is used for central systems such as CAV, VAV, VVT, dual duct and triple duct systems. In this
format the report contains two tables (see Figure 1)
a. The Summary table lists the sizing method and the final result of the ventilation sizing calculation.
b. The Space Ventilation Analysis table documents how requirements for each space are determined.
2. Ventilation Sizing Summary for Terminal Systems - This format is used for terminal systems such as fan coils, water source heat pumps, VRF, PTACs, induction
beams and active chilled beams. In this format the report contains two sections (see Figure 2)
a. The Summary section lists the sizing method and the final result of the ventilation sizing calculation.
b. The Space Ventilation Analysis section contains a series of tables each documenting the calculation of outdoor airflow for one of the zone terminal units.
Contents of the report are described further below the figures. Each table is explained in more detail in subsections below Figure 1. For further information on the
ventilation sizing calculations, click here: Ventilation Sizing Calculations.
Figure 1. Vent Sizing Summary Format for Summation Method - Central Systems
Figure 2. Vent Sizing Summary Format for Summation Method - Terminal Systems
Page 14 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Vent Sizing Summary for ASHRAE Std 62-2001
14.0 Designing Systems ›› 14.4 Ventilation Sizing Summary Report ››
Summary Section
The Summary table presents the final results of the ventilation sizing calculation. Items in this table are as follows:
1. Ventilation Sizing Method lists the sizing method that was chosen for this system.
2. Design Ventilation Airflow Rate lists the required outdoor ventilation airflow rate for the system. For central systems this is the outdoor air intake for the system.
For terminal systems, it is the total outdoor airflow for a dedicated outdoor air system (DOAS) unit, if one is used.
Space Ventilation Analysis Section
The Space Ventilation Analysis section documents how the outdoor ventilation airflow requirement is calculated for each space served by the system. For central
systems there is one table containing all zones and spaces for the system. For terminal systems, a separate table is provided for each terminal unit zone.
In the table each row contains data for a space served by the system. Spaces are grouped according to the zones you have defined for the system. Each column
contains a different value used in the calculation of ventilation air for the space.
1. Space Name lists the name of the space whose data is shown in this row.
2. Multiplier lists the multiplier applied to this space. All data in the remaining columns of this row are for a single instance of this space. However, column totals
shown at the bottom of the table include the space multiplier shown here since column totals are intended to show grand totals for the system.
3. Floor Area is the total floor area for one instance of this space.
4. Maximum Occupants is the maximum number of occupants specified for this space. It is calculated by multiplying the people quantity defined for the space by the
largest design day schedule factor specified for occupants in the space. Typically this largest schedule factor will be 100%, but that is not always the case. For
example, if no schedule factors above 90% are defined, maximum occupants will be {People Quantity} x 0.90.
5. Maximum Supply Air is the design supply airflow for the space. This value is the same as shown on the Zone Sizing Summary report.
6. Required Outdoor Air. The next four columns show the space ventilation requirements defined as CFM/person, CFM/sqft, total CFM and % of supply air. In Metric
these columns show L/s/person, L/s/sqm, total L/s and % of supply air. These values were specified in space inputs.
7. Uncorrected Outdoor Air lists the ventilation airflow for the space resulting from data in the previous columns. It is the sum of requirements in the CFM/person,
CFM/sqft, CFM and % of supply air columns. For example, if a space only has a CFM/person requirement, the CFM/person value is multiplied by the maximum
occupants column to obtain the ventilation requirement. Or, if a space has both CFM/person and CFM/sqft requirements, CFM/person is multiplied by maximum
occupants and added to the result of CFM/sqft multiplied by total floor area. Thus, when a space has multiple requirements, the requirements are summed to
determine the total required airflow for the space.
Finally, system totals are shown at the bottom of relevant columns of the table. Note that while cells in the table show data for a single instance of each space, the
column totals include space multipliers. Space multipliers are shown in the second column from the left in this table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Vent Sizing Summary for ASHRAE Std 62-2001
This topic describes the format and content of the Ventilation Sizing Summary Report when the "ASHRAE Std 62-2001" or "ASHRAE Std 62-2001 (max only)" sizing
method is chosen. For this situation the report documents how the Standard 62-2001 Ventilation Rate Procedure is used to determine space and ventilation airflow
rates. The report, shown in Figure 1, contains three tables:
1. The Summary table provides the final results of the ventilation sizing calculation including the corrected and uncorrected ventilation airflow rates, the design
condition and the sizing method.
2. The ASHRAE Std 62 Analysis Details table documents key values used in the ASHRAE Standard 62 Ventilation Rate Procedure analysis, including the critical
space and the X, Y and Z air fraction values.
3. The Space Ventilation Analysis table documents how the uncorrected outdoor ventilation airflow, the uncorrected outdoor air fraction "Z", and the corrected
outdoor airflow are calculated for each space served by the system.
Each table is explained in more detail in subsections below Figure 1. For further information on the ventilation sizing calculations, click here: Ventilation Sizing
Calculations.
Figure 1. Vent Sizing Summary Format when ASHRAE Std 62-2001 Methods Used
Page 15 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Summary Table
The Summary table presents the final results of the ventilation sizing calculation. Items in this table are as follows:
1. Ventilation Sizing Method lists the sizing method that was chosen for this system.
2. Design Condition is only shown for a VAV system. If the "ASHRAE Std 62-2001" sizing method was chosen, ventilation airflow will be determined when all VAV
boxes are full open, or when all VAV boxes are at minimum position, whichever yields the larger ventilation requirement. If the "ASHRAE Std 62-2001 (max only)"
method was chosen, ventilation sizing will be done when VAV boxes are full open.
3. Design Ventilation Airflow Rate lists the required outdoor ventilation airflow rate for the system. This is the corrected ventilation airflow after critical space factors
are accounted for.
4. Uncorrected Outdoor Airflow Rate shows the sum of space ventilation requirements for spaces served by the system. It is provided so users can compare
uncorrected and corrected airflows to determine the size of the critical space correction.
ASHRAE Std 62 Analysis Details Table
This table documents key values used in the ASHRAE Standard 62 Ventilation Rate Procedure analysis such as the critical space and the X, Y and Z air fractions.
In this table each row contains one of the key values. Each column contains data for one of the design conditions considered. For VAV systems for which the
"ASHRAE Std 62-2001" sizing method is used, data will be provided for both the "terminal boxes full open" and "terminal boxes at minimum flow" conditions. For all
other cases, data will only be shown for the "terminal boxes full open" design condition. Values in the table are as follows:
1. Critical Space lists the name of the space having the highest outdoor air fraction Z. Z is the uncorrected space ventilation airflow divided by space supply airflow. Z
values for all spaces are shown in the Space Ventilation Analysis Table.
2. Critical Space Outdoor Air Fraction (Z) lists the outdoor air fraction Z for the critical space.
3. Uncorrected Outdoor Air Fraction (X) is the ratio of total uncorrected outdoor airflow for the system divided by total supply airflow for the system. The uncorrected
outdoor airflow total is the sum of uncorrected outdoor airflows for all spaces served by the system, as shown in the Space Ventilation Analysis Table.
4. Corrected Outdoor Air Fraction (Y) is the ratio of corrected outdoor airflow divided by total supply airflow for the system. Y is calculated using equation 6-1 from
the Standard: Y = X / [1 + X – Z], where the X and Z factors are those mentioned above. This equation determines how ventilation airflow must be adjusted to
ensure that all spaces in a multiple-space system receive the required amounts of outdoor ventilation air.
5. Required System Ventilation Airflow lists the corrected outdoor ventilation airflow rate. This is the sum of corrected space ventilation airflows shown in the Space
Ventilation Analysis Table.
Space Ventilation Analysis Table
The Space Ventilation Analysis table documents how the uncorrected outdoor ventilation airflow is calculated for each space served by the system. It also provides the
uncorrected outdoor air fraction "Z" and the corrected outdoor airflow for each space.
Note: When using the "ASHRAE Std 62-2001" sizing method with a VAV system, data in this table is for the design condition listed in the Summary table. This will
either be the condition "terminal boxes full open" or "terminal boxes at minimum flow". With this sizing method, the program calculates required ventilation airflows at
both conditions and chooses the worst case as the required ventilation airflow for the system. Data in this table documents that worst case.
In this table each row contains data for a space served by the system. Spaces are grouped according to the zones you have defined for the system. Each column
contains a different value used in the calculation of ventilation air for the space.
1. Space Name lists the name of the space whose data is shown in this row.
2. Multiplier lists the multiplier applied to this space. All data in the remaining columns of this row are for a single instance of this space. However, column totals
shown at the bottom of the table include the space multiplier shown here since column totals are intended to show grand totals for the system.
3. Floor Area is the total floor area for one instance of this space.
4. Maximum Occupants is the maximum number of occupants specified for this space. It is calculated by multiplying the people quantity defined for the space by the
largest design day schedule factor specified for occupants in the space. Typically this largest schedule factor will be 100%, but that is not always the case. For
example, if no schedule factors above 90% are defined, maximum occupants will be {People Quantity} x 0.90.
5. Maximum Supply Air is the design supply airflow for the space. This value is the same as shown on the Zone Sizing Summary report.
Page 16 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Vent Sizing Summary for ASHRAE Std 62.1 - Central Systems
14.0 Designing Systems ›› 14.4 Ventilation Sizing Summary Report ››
6. Minimum Supply Air is shown in place of the Maximum Supply Air under special circumstances: Only when the "ASHRAE Std 62-2001" method is used for a VAV
system, and the worst case ventilation airflow occurs for "terminal boxes at minimum flow". In this case, this column shows the supply airflow for the space when the
VAV box is at minimum flow.
7. Required Outdoor Air. The next four columns show the space ventilation requirements defined as CFM/person, CFM/sqft, total CFM and % of supply air. In Metric
these columns show L/s/person, L/s/sqm, total L/s and % of supply air. These values were specified in space inputs.
8. Uncorrected Outdoor Air lists the ventilation airflow for the space resulting from data in the previous columns. It is the sum of requirements in the CFM/person,
CFM/sqft, CFM and % of supply air columns. For example, if a space only has a CFM/person requirement, the CFM/person value is multiplied by the maximum
occupants column to obtain the ventilation requirement. Or, if a space has both CFM/person and CFM/sqft requirements, CFM/person is multiplied by maximum
occupants and added to the result of CFM/sqft multiplied by total floor area. Thus, when a space has multiple requirements, the requirements are summed to
determine the total required airflow for the space.
9. Uncorrected Outdoor Air Ratio Z is the ratio of the uncorrected outdoor air for a space divided by the maximum supply air for the space. When data in this table is
for the "terminal boxes at minimum flow" design condition, Z is calculated as uncorrected outdoor air divided by minimum supply air. The Z factor is used to
determine the critical space in a multiple-space system. The critical space requires the highest fraction of outdoor air in supply air. Because all spaces receive
supply air having the same outdoor air fraction, this critical space will influence the overall ventilation airflow for the system.
10. Corrected Outdoor Air lists the ventilation requirements after correction for critical space considerations. Standard 62-2001 requires that a corrected outdoor air
fraction "Y" be calculated using equation 6-1 of the standard: Y = X / [1 + X + Z]. Y is the required ratio of outdoor ventilation air divided by supply air for the system
to ensure that all spaces in the system receive the required amount of ventilation air. Y for the system is shown in the ASHRAE Std 62 Analysis Details table on this
report. The corrected outdoor air values are calculated as {corrected outdoor air fraction Y} x {space supply airflow rate}. When calculating for "terminal boxes full
open", the maximum space supply airflow is used. When calculating for "terminal boxes at minimum flow" the minimum space supply airflow is used.
Finally, system totals are shown at the bottom of relevant columns of the table. Note that while cells in the table show data for a single instance of each space, the
column totals include space multipliers. Space multipliers are shown in the second column from the left in this table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Vent Sizing Summary for ASHRAE Std 62.1 - Central Systems
This topic describes the format and content of the Ventilation Sizing Summary Report for the following application:
a. The ventilation sizing method is one of the ASHRAE Standard 62.1 editions (2004, 2007, 2010, 2013, or 2016).
b. The system is a central system such as single zone CAV, CAV Terminal Reheat, Variable Air Volume, VVT, and the dual and triple duct systems..
The report documents how the Standard 62.1 Ventilation Rate Procedure is used to determine space and system ventilation airflow rates. The report, shown in Figure
1, contains two tables:
1. The Summary table provides the final results of the ventilation sizing calculation including the sizing method, the design condition and the corrected and
uncorrected ventilation airflow rates.
2. The Space Ventilation Analysis table provides information showing how the uncorrected outdoor ventilation airflow is calculated. It also lists space ventilation
efficiency for each space served by the system. These are two of the key components in determining the total ventilation requirement for the system.
Each table is explained in more detail in subsections below Figure 1. For further information on the ventilation sizing calculations, click here: Ventilation Sizing
Calculations.
Figure 1. Vent Sizing Summary Format for ASHRAE Std 62.1 and Central Systems
Summary Table
The Summary table presents the final results of the ventilation sizing calculation. Items in this table are as follows:
1. Ventilation Sizing Method lists the sizing method that was chosen for this system.
2. Design Condition indicates the system operating condition used for sizing ventilation airflow. The program automatically performs ventilation sizing calculations for
both the design cooling and design heating condition. The larger of the two airflow values is chosen as the ventilation requirement for the system. All results shown
on this report are for the condition that yielded the larger ventilation requirement. For CAV systems, this item will be "Cooling Operation" if the ventilation
requirement is from design cooling or "Heating Operation" if the ventilation requirement is from design heating. For VAV systems, the standard requires calculation
at the minimum flow condition so the item will be "Minimum Flow (cooling)"or "Minimum Flow (heating)".
3. Occupant Diversity indicates the system diversity factor "D" used for calculating the uncorrected outdoor air intake value (paragraph 6.2.5.3 in Standard). If the
same diversity factor is specified for all zones in the system, this single diversity factor will be listed here. If different diversity factors for individual zones, a weighted
average value appears here.
Page 17 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Vent Sizing Summary for ASHRAE Std 62.1 - Terminal Systems
14.0 Designing Systems ›› 14.4 Ventilation Sizing Summary Report ››
4. Uncorrected Outdoor Air Intake combines breathing zone outdoor airflow rates for spaces in the system and accounts for diversity. In the Standard it is referred to
as "Vou" and is calculated by equation 6-6 in paragraph 6.2.5.3.
5. System Ventilation Efficiency is the space ventilation efficiency for the critical space. The critical space has the lowest space ventilation efficiency among all
spaces served by the system. Individual space ventilation efficiencies are shown in the Space Ventilation Analysis Table. In Standard 62.1 this is referred to as "Ev"
6. Outdoor Air Intake lists the required outdoor ventilation airflow rate for the system at the outdoor air intake. In the Standard this is referred to as "Vot". It is
calculated by dividing uncorrected outdoor air intake (Vou) by system ventilation efficiency (Ev) using equation 6-8, paragraph 6.2.5.4 in Standard.
Exception: When a system serves a single space, the Standard requires that the Outdoor Air Intake (Vot) be set to the Space Outdoor Airflow (Voz).
Space Ventilation Analysis Table
The Space Ventilation Analysis table documents how the uncorrected outdoor ventilation airflow is calculated for each space served by the system. The table also
provides the space ventilation efficiency for each space using ASHRAE Standard 62.1 Ventilation Rate Procedures.
In this table each row contains data for a space served by the system. Spaces are grouped according to the zones you have defined for the system. Each column
contains a different value used in the calculation of ventilation air for the space.
1. Space Name lists the name of the space whose data is shown in this row.
2. Multiplier lists the multiplier applied to this space. All data in the remaining columns of this row are for a single instance of this space. However, column totals
shown at the bottom of the table include the space multiplier since column totals are intended to show grand totals for the system.
3. Supply Air is the design supply airflow for the space. This column is only shown for constant volume air systems. In Standard 62.1 it is referred to as "Vpz".
4. Minimum Supply Air is the minimum supply airflow required for the space. This column is only shown for variable air volume systems. For VAV systems the
Standard requires use of minimum flow for VAV systems in the calculation (paragraph 6.2.5.1 in Standard). In Standard 62.1 it is referred to as "Vpz".
5. Space Floor Area is the total floor area for one instance of this space. In Standard 62.1 it is referred to as "Az"
6. Area Outdoor Air Rate (CFM/sqft or L/s/sqm) shows the CFM/sqft or L/s/sqm airflow requirement for the space. It was defined in space inputs. The floor-area
based component of the ventilation airflow will be this air requirement multiplied by the space floor area. In Standard 62.1 it is referred to as "Ra".
7. Time Averaged Occupancy lists the number of occupants considered for calculating ventilation requirements. If the occupant design day schedule specifies 100%
for all hours, the time average occupancy will equal the number of occupants specified for the space in space inputs. If the design day schedule fluctuates, then the
time averaging procedure described in paragraph 6.2.6.2 of the Standard will be used to adjust the number of occupants for variable occupancy. In Standard 62.1 it
is referred to as "Pz".
8. People Outdoor Air Rate (CFM/person or L/s/person) lists the occupant-based ventilation requirement for the space. It was defined in space inputs. The
occupant-based component of the ventilation airflow will be this requirement multiplied by the Time Averaged Occupancy value. In Standard 62.1 it is referred to as
"Rp".
9. Air Distribution Effectiveness shows the effectiveness assigned to this space, referred to as "Ez". If the zone containing this space was specified to use
computer-generated values, Ez will be determined based on the location of supply discharge and return grille, whether the system has cooling and/or heating
capability, the heating supply temperature, and heating setpoint, using values from Table 6.2.2.2 in ASHRAE 62.1-2013 or -2016, and from Table 6-2 in prior
editions of the standard. If the zone containing this space was specified with a user-defined Ez value, that value will be used directly without consideration of Table
6.2.2.2 or Table 6-2 data.
10. Space Outdoor Air is outdoor ventilation airflow requirement for the space. It is referred to as "Voz" in paragraph 6.2.2.3 of the Standard. This quantity is the
outdoor airflow in the supply air needed to deliver the required outdoor air to the breathing zone in the space. It is calculated as::
Voz = [ (CFM/person x Time Avg Occupancy) + (CFM/sqft x sqft floor area) ] / Ez , or
Voz = [(L/s/person x Time Avg Occupancy) + (L/s/sqm x sqm floor area) ] / Ez
where Ez is the air distribution effectiveness for the space.
11. Breathing Zone Outdoor Air is the required outdoor airflow to the breathing zone of the space, Vbz, from paragraph 6.2.2.1 of the standard. It is calculated as:
Vbz = [ (CFM/person x Time Avg Occupancy) + (CFM/sqft x sqft floor area) ] , or
Vbz = [ (L/s/person x Time Avg Occupancy) + (L/s/sqm x sqft floor area) ]
12. Space Ventilation Efficiency describes the ventilation efficiency for each space. In Standard 62.1 it is referred to as "Evz". It applies to cases where a system
serves multiple spaces. It is calculated using procedures in Appendix A of the Standard. For a system serving a single space and for a system providing 100%
outdoor air the space ventilation efficiency is not needed and is shown as 1.00.
Finally, values appear in the cells at the bottom of three columns in the table:
1. For the Supply Air and Minimum Supply Air columns, the sum of airflows in the column is shown at the bottom of the column. Note that this total includes space
multipliers.
2. For the Breathing Zone Outdoor Air column the sum of airflows in this column, including space multipliers, is shown. When no diversity is specified, this total will
match the Uncorrected Outdoor Air Intake (Vou) value in the Summary Table. When diversity is specified, the column total and the Summary Table values will differ;
the Summary Table value includes diversity while the column total does not..
3. For the Space Ventilation Efficiency column, the cell at the bottom of the column shows the critical space ventilation efficiency, "Ev". This is the lowest efficiency
value among all spaces in the system. This critical efficiency is used to derive the total ventilation requirement for the system (see Summary table).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Vent Sizing Summary for ASHRAE Std 62.1 - Terminal Systems
This topic describes the format and content of the Ventilation Sizing Summary Report for the following application:
a. The ventilation sizing method is one of the ASHRAE Standard 62.1 editions (2004, 2007, 2010, 2013, or 2016).
b. The system is one of the terminal type systems such as fan coils, water source heat pumps, VRF, induction beams or active chilled beams.
The report documents how the Standard 62.1 Ventilation Rate Procedure is used to determine space, terminal zone, and dedicated outdoor air system (DOAS)
ventilation airflow rates. The report, shown in Figure 1, is divided into two sections
1. The Summary section provides the outdoor air intake (Vot) results for each terminal zone, and the system total outdoor air intake flow for a DOAS unit, if one is
used.
2. The Space Ventilation Analysis section consists of a series of tables, one for each terminal zone, documenting how the outdoor air intake (Vot) airflow for that
zone is determined.
Page 18 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
The content for each section is described in more detail in subsections below Figure 1. For further information on the ventilation sizing calculations, click here:
Ventilation Sizing Calculations
Figure 1. Ventilation Sizing Summary for ASHRAE Standard 62.1 and Terminal Systems
Summary Section
The Summary section presents the final results of the ventilation sizing calculation, including the outdoor air intake flow (Vot) for each terminal unit zone, and the
system total outdoor air intake flow. Line items at the start of this section are as follows:
1. Ventilation Sizing Method lists the sizing method that was chosen for this system.
2. Design Condition indicates the system operating condition used for sizing ventilation airflow. The program automatically performs ventilation sizing calculations for
both the design cooling and design heating conditions. The larger of the two ventilation airflow results is chosen as the ventilation requirement for the system. All
results shown on this report are for the condition that yielded the larger ventilation requirement.
The section also contains a table summarizing the zone terminal unit outdoor air intake (Vot) airflow requirements. In a terminal system, each zone terminal unit
qualifies as a “ventilation system” for Standard 62.1 purposes. Therefore a separate ventilation rate procedure calculation is performed for each terminal unit zone to
determine the outdoor air intake requirement (Vot) for that zone. Each row in the table contains results for one zone in the system. Columns provide details
documenting the calculation of Vot for each zone:
1. Zone Name lists the name assigned to each terminal unit zone.
2. Zone Outdoor Airflow (Voz) – For zones containing a single space, the outdoor air intake flow (Vot) will be equal to the zone outdoor airflow (Voz) value listed in
this cell. The calculation of Voz is documented in tables in section 2 of the report.
Notes:
a. If a space multiplier is used, the Voz value here represents the zone total including multipliers.
b. If a zone contains multiple spaces, then this cell will be blank. The Vou cell to the right will be used instead.
3. Uncorrected Outdoor Air Intake (Vou) – For zones containing multiple spaces, the outdoor air intake flow (Vot) is equal to the uncorrected outdoor intake flow
(Vou) shown in this cell divided by the ventilation efficiency (Ev) for this terminal zone. Calculation of Vou and Ev is documented in tables in section 2 of the report.
Note:
a. If a zone contains a single space, then this cell will be blank. The Voz cell to the left will be used instead.
4. Ventilation Efficiency (Ev) lists the system ventilation efficiency for this terminal unit zone. For a multiple-space zone this is the minimum of space ventilation
efficiencies (Evz) shown in section 2 of the report for this zone. For a single-space zone, ventilation efficiency is not used and is shown as 1.0.
5. Outdoor Air Intake (Vot) lists the required outdoor air intake flow rate for the zone. As noted above, for a single space zone Vot = Voz. For a multiple space zone
Vot = Vou / Ez.
6. System Total – The sum of zone Vot values is listed at the bottom of the table. If a dedicated outdoor air system (DOAS) is used, this system total is the required
outdoor air intake flow for the DOAS unit. The DOAS unit must provide sufficient flow to meet the Vot requirements of each zone in the system.
Space Ventilation Analysis Section
The Space Ventilation Analysis section documents how the data shown in the summary section was derived. In this section a separate table is provided for each zone
since a separate Ventilation Rate Procedure is performed for each terminal unit zone. Each row in the table contains data for one space. Columns in the table
document the calculation of breathing zone airflow (Vbz), outdoor airflow (Voz) and space ventilation efficiency (Evz):
Page 19 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.5 Air System Design Load Summary Report
14.0 Designing Systems ››
Air System Design Load Summary Report
14.0 Designing Systems ›› 14.5 Air System Design Load Summary Report ››
1. Space Name lists the name of the space whose data is shown in this row.
2. Multiplier lists the multiplier applied to this space. All data in the remaining columns of this row are for a single instance of this space. However, column totals
shown at the bottom of the table include the space multiplier since column totals are intended to show grand totals for the terminal unit zone.
3. Supply Air is the design supply airflow for the space. In Standard 62.1 it is referred to as "Vpz".
4. Space Floor Area is the total floor area for one instance of this space. In Standard 62.1 it is referred to as "Az"
5. Area Outdoor Air Rate (CFM/sqft or L/s/sqm) shows the CFM/sqft or L/s/sqm airflow requirement for the space. It was defined in space inputs. The floor-area
based component of the ventilation airflow will be this air rate multiplied by the space floor area. In Standard 62.1 it is referred to as "Ra".
6. Time Averaged Occupancy lists the number of occupants considered for calculating ventilation requirements. If the occupant design day schedule specifies 100%
for all hours, the time average occupancy will equal the number of occupants specified for the space in space inputs. If the design day schedule fluctuates, then the
time averaging procedure described in paragraph 6.2.6.2 of the Standard may be used to adjust the number of occupants for variable occupancy. In Standard 62.1
it is referred to as "Pz".
7. People Outdoor Air Rate (CFM/person or L/s/person) lists the occupant-based ventilation requirement for the space. It was defined in space inputs. The occupant-
based component of the ventilation airflow will be this requirement multiplied by the Time Averaged Occupancy value. In Standard 62.1 it is referred to as "Rp".
8. Air Distribution Effectiveness shows the effectiveness assigned to this space, referred to as "Ez". If the zone containing this space was specified to use
computer-generated values, Ez will be determined based on the location of supply discharge and return grille, whether the system has cooling and/or heating
capability, the heating supply temperature, and heating setpoint, using values from Table 6.2.2.2 in ASHRAE 62.1-2013 or -2016, and from Table 6-2 in prior
editions of the standard. If the zone containing this space was specified with a user-defined Ez value, that value will be used directly without consideration of Table
6.2.2.2 or Table 6-2 data.
9. Space Outdoor Air is outdoor ventilation airflow requirement for the space. It is referred to as "Voz" in paragraph 6.2.2.3 of the Standard. This quantity is the
outdoor airflow in the supply air needed to deliver the required outdoor air to the breathing zone in the space. It is calculated as::
Voz = [ (CFM/person x Time Avg Occupancy) + (CFM/sqft x sqft floor area) ] / Ez , or
Voz = [(L/s/person x Time Avg Occupancy) + (L/s/sqm x sqm floor area) ] / Ez
where Ez is the air distribution effectiveness for the space.
10. Breathing Zone Outdoor Air is the required outdoor airflow to the breathing zone of the space, Vbz, from paragraph 6.2.2.1 of the standard. It is calculated as:
Vbz = [ (CFM/person x Time Avg Occupancy) + (CFM/sqft x sqft floor area) ] , or
Vbz = [ (L/s/person x Time Avg Occupancy) + (L/s/sqm x sqft floor area) ]
11. Space Ventilation Efficiency describes the ventilation efficiency for each space. In Standard 62.1 it is referred to as "Evz". It applies to cases where a terminal
unit serves multiple spaces. It is calculated using procedures in Appendix A of Standard 62.1. For a terminal unit zone containing a single space, Evz is 1.00. For a
terminal unit zone containing multiple spaces, Evz values will vary above or below 1.00.
Finally, values appear in the cells at the bottom of three columns in each table:
1. For the Supply Air column, the sum of airflows in the column is shown at the bottom of the column. Note that this total includes space multipliers.
2. For the Breathing Zone Outdoor Air column the sum of airflows in this column, including space multipliers, is shown. This total will match the Uncorrected Outdoor
Air Intake (Vou) value in the Summary Table.
3. For the Space Ventilation Efficiency column, the cell at the bottom of the column shows the critical space ventilation efficiency, "Ev". This is the lowest efficiency
value among all spaces in the terminal unit system. For a multiple-space zone, this critical efficiency is used to derive the total ventilation requirement for the
system (see Summary table).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Air System Design Load Summary Report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air System Design Load Summary Report
The Air System Design Load Summary report provides a list of component cooling loads for the air system for one design cooling hour and a list of component heating
loads for the design heating condition. Cooling data on this report can be generated for the hour of the peak central cooling coil load, or for a month and hour chosen
by the user. This report is typically used when investigating how different load components contribute to the system load. Length: 1 page.
A sample of this report for a VAV Reheat system is shown below. Following this figure, the format and content of the report is discussed in detail.
Page 20 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Report Format and Content. The Air System Design Load Summary report consists of one large table. Each row contains data for a different load component. Load
components are divided into three sections:
1. Zone Loads are grouped in the upper portion of the table. These are loads occurring in the zones served by the system and include items such as wall loads,
lighting loads and infiltration loads.
2. System Loads are grouped in the middle portion of the table. These are loads occurring outside the zones. They include items such as fan heat gain, ventilation
loads and plenum loads.
3. Coil Loads are grouped at the bottom of the table. These items show how the total system load is divided among the various coils in the system. Line items
appearing in this section of the table vary with system type.
The table contains seven columns: a column listing the load components, three columns containing cooling load data and three columns containing heating load data.
Columns for load data are as follows:
1. Details contains useful information associated with the cooling or heating load data. This includes areas for walls or roofs, wattages for internal loads and airflow
rates for ventilation loads and fan heat gains.
2. Sensible contains the sensible component of each load.
3. Latent contains the latent component of each load.
Line items in the table are described below in three separate sections, one for each of the major groupings of load components.
Component Zone Loads. The first section of the table lists zone component loads. Zone loads are the result of the first stage in the sizing calculations. For cooling,
zone loads are obtained by calculating the heat gain for each component and then using the heat gains in the room transfer function procedures to derive the load. Per
ASHRAE procedures, loads are calculated assuming that cooling is provided 24 hours per day and all zones are held exactly at the occupied cooling thermostat
setpoint. For heating, zone loads are computed as instantaneous heat losses for the design heating condition. Zone loads serve as the basis for system simulation
calculations whose results are shown in the middle and lower sections of the table.
Each component load in this section of the table is the sum of individual loads in all spaces in all zones served by the air system. Individual items are as follows:
1. Solar Loads include loads due to solar radiation entering zones through windows in wall exposures and skylights in roof exposures. The value in the "details"
column represents the total area for all windows and skylights.
2. Wall Transmission lists the transmission load for all above-grade vertical wall exposures. The area in the "details" column is the net wall area. Only the wall
transmission load reaching the zone will be listed. Any wall load assigned to a return plenum will be listed later in the system section of the table. Note: The load for
below-grade portions of walls is included in the Floor Transmission line item (see below).
3. Roof Transmission lists the transmission load for all horizontal and sloped roof exposures. The area in the "details" column is the net roof area. Only the roof
transmission load reaching the zone will be listed. Any roof load assigned to a return plenum will be listed later in the system section of this output.
4. Glass Transmission lists the transmission loads for all windows in wall exposures. The area in the "details" column is for all windows.
5. Skylight Transmission lists the transmission loads for all skylights in roof exposures.
6. Door Loads lists the total load for the door. This includes transmission of heat through both the opaque and glass portions of the door and the solar load for door
glass.
Page 21 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
7. Floor Transmission lists heat transmission through floors above unconditioned spaces, slab on grade floors and basement floors. When basement floors are
involved, this item also includes heat transferred through below grade walls. Readers should note that slab and basement floor transmission are not considered for
design cooling calculations. Finally, the area listed in the "details" column lists the total area for these three types of floors. Areas for floors above conditioned
spaces and basement wall areas are not included in this total area.
8. Partitions lists heat transmission for partitions adjacent to unconditioned spaces.
9. Ceiling lists heat transmission for ceilings below unconditioned spaces.
10. Overhead Lighting lists the lighting load for overhead lighting fixtures only. The value listed is for the portion of the lighting load assigned to the zone. The portion
of the lighting load assigned to a return plenum is provided later in the system load section of the table. The wattage listed in the "details" column is the total lighting
heat gain, and includes both the portions of the heat gain assigned to the zone and to a return plenum.
11. Task Lighting lists the loads due to any task lighting fixtures.
12. Electric Equipment lists the loads due to electric equipment heat gain.
13. People lists the loads due to sensible and latent occupant heat gains.
14. Infiltration lists loads due to infiltration air. For the cooling calculation the "design cooling" infiltration airflow specified in space inputs is used. For the heating
calculations the "design heating" infiltration airflow specified in space inputs is used.
15. Miscellaneous lists loads due to any miscellaneous sensible and latent heat gains specified by the user.
16. Safety Factor lists the safety BTU/h or W for each column of cooling and heating loads. The safety loads are computed by summing load quantities in all previous
rows in the table and multiplying this total by the safety factor percentage specified by the user. In the cooling "details" column the safety factors specified by the
user are listed in the following order: cooling sensible, cooling latent.
17. Total Zone Loads lists the sum of all load items in the zone load section of the table.
Component System Loads. The middle section of the table lists system component loads. These are loads occurring outside zones in the system. They include
items such as fan heat gains, the ventilation load and plenum loads. Loads in this section of the table are the result of calculations simulating the operation of the air
system in response to cooling and heating demands in the zones. Items in this section are as follows:
1. Zone Conditioning is the actual amount of heat which is removed from the zones (for cooling) or added to zones (for heating). For sensible cooling the zone
conditioning is based on the "total zone load" with corrections for the actual operating schedule (which may be less than 24 hours per day), for the use of set-up and
set-back temperatures in the unoccupied period, and for the variation of zone temperatures within the thermostat throttling range. These corrections are made using
the ASHRAE heat extraction procedures. Thus "zone conditioning" includes such heat quantities as pulldown loads, while "total zone load" does not.
For latent cooling the zone conditioning will equal the total zone load since latent loads are instantaneous.
For design heating, the zone conditioning will nearly equal to the total zone load because the transient behavior considered for cooling calculations is not
considered for a standard design heating calculation. Note that small differences between zone conditioning and total zone load may be seen due mathematics of
the system simulation process. These differences will generally be very small. If a large difference between the total zone heating load and the zone conditioning
occurs, it is usually due to a system operating problem. In such a case, the System Psychrometrics report for the design heating condition should be generated to
evaluate system performance in greater detail.
2. Plenum Wall Load lists the portion of the wall transmission load transferred to return plenum air. The "details" column lists the wall-load-to-plenum percentage
specified by the user.
3. Plenum Roof Load provides the portion of the roof transmission load transferred to plenum air. The "details" column lists the roof-load-to-plenum percentage
specified by the user.
4. Plenum Lighting Load lists the portion of overhead lighting heat gain transferred to return plenum air. The "details" column lists the lighting-load-to-plenum
percentage specified by the user.
5. Return Fan Load lists the heat gain for a return fan, if one is used. The "details" column lists the return airflow rate. When a return fan is not used, the
corresponding heat gains will be zero.
6. Ventilation Load lists the net heat gain or loss for ventilation air entering the system and exhaust air leaving the system. The "details" column lists the outdoor
ventilation airflow rate.
One of the common hand-calculation checks users perform involves the cooling and heating ventilation loads. To duplicate ventilation calculations by hand
successfully, users are strongly encouraged to refer to the discussion of ventilation load calculations.
7. Supply Fan Load lists the heat gain for the system supply fan. The "details" column lists the actual airflow through the supply fan.
8. Hot Deck Supply Fan. For 2-Fan Dual Duct VAV systems, the heat gain for the hot deck supply fan will also be listed. The "details" column lists the actual airflow
through the hot deck fan.
9. Space Fan Coil Fans lists the total heat gain for all fan coil units in zones served by the air system. For terminal systems such as fan coils or water source heat
pumps, these values will be heat gains for the terminal unit fans. For other systems, heat gains for supplemental zone fan coil heating units will be listed.
10. Duct Heat Gain/Loss. For the cooling condition, this item lists supply duct heat gain. For the heating condition, the item lists supply duct heat loss. The percent
duct heat gain/loss value specified by the user is provided in the "details" column.
11. Total System Loads contains the sum of system loads in each of the cooling and heating columns. These totals are computed starting with "zone conditioning"
and working downward. The totals represent the net amount of heat which must be removed from the system (for cooling) or added to the system (for heating) to
maintain comfort conditions in the zones.
Component Coil Loads. The lower section of the table lists individual coil loads for the system. This section shows how the heat removal or heat addition values
represented by the "total system loads" line are divided among different cooling and heating coils in the system. This section contains up to thirteen line items which
differ depending on the type of air system is involved. Items in this section are as follows:
1. Central Cooling Coil: Sensible and latent loads for a central cooling coil or the cold deck coil in 2-Deck Multizone, 3-Deck Multizone and dual duct systems.
2. Central Heating Coil: Sensible loads for a central heating coil in a Single-Zone CAV system or the hot deck coil in 2-Deck Multizone, 3-Deck Multizone and dual
duct systems.
3. Precool Coil: Sensible and latent loads for a precool coil.
4. Cooling Coil: Sensible and latent loads for a cooling coil in a dedicated outdoor air system (DOAS) or make up air unit (MAU).
5. Preheat Coil: Sensible loads for a preheat coil.
6. Heating Coil: Sensible loads for a heating coil in a dedicated outdoor air system (DOAS) or make up air unit (MAU).
7. Terminal Unit Cooling: The sum of sensible and latent loads for terminal cooling coils in all zones, such as those in terminal fan coil or water source heat pump
units, or coils in 4-pipe induction terminals.
8. Terminal Unit Heating: The sum of loads for terminal heating coils in all zones, such as heating coils in fan coil or water source heat pump units.
9. Central Reheat Coil: Sensible loads for a central reheat coil used for dehumidification control.
10. Humidification Load: Latent load for moisture added to the supply air stream by the humidifier.
Page 22 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.6 Zone Design Load Summary Report
14.0 Designing Systems ››
Zone Design Load Summary Report
14.0 Designing Systems ›› 14.6 Zone Design Load Summary Report ››
11. Terminal Reheat Coils: The sum of sensible loads for terminal reheat coils or heating coils in 4-pipe induction units for all zones in the system.
12. Zone Heating Unit Coils: The sum of heating loads for coils in supplemental zone heating units such as baseboard or fan coil units.
13. Total Conditioning: The sum of all items in the coil load portion of this output. Total conditioning values should closely match corresponding "Total System Loads"
values. Small differences between corresponding values may be seen due to the iterative procedure needed to determine system operating conditions. Larger
differences indicate a problem with system operation which should be investigated using the System Psychrometrics report.
For latent cooling loads, differences are also usually small. These differences are the result of the iterative calculation used to estimate the steady-state humidity
levels in the system. For most operating conditions this results in very small differences between the total system load and the total conditioning value. For
unusually warm coil conditions, it can result in differences larger than 2%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Zone Design Load Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Design Load Summary Report
The Zone Design Load Summary report provides a list of component cooling and heating loads for each zone served by the air system. Cooling data on this report can
be generated for the hour of the peak sensible load in each zone, or for a month and hour chosen by the user. Heating data is always generated for the design heating
condition. This report is typically used when investigating the behavior of zone loads. Length: 2 zones per page.
A sample of this report is shown below. Following this figure, the format and content of the report are discussed in detail.
Report Format and Content. The Zone System Design Load Summary report contains one table of loads for each zone in the system. All zone load tables have the
same format. Each row contains data for a different load component. The table contains seven columns: a column listing the load components, three columns
containing cooling load data and three columns containing heating load data. Columns for load data are as follows:
1. Details contains useful information associated with the cooling or heating load data. Examples include areas for walls or roofs and wattages for internal loads.
2. Sensible contains the sensible component of each load.
3. Latent contains the latent component of each load.
Zone loads are the result of the first stage of the sizing calculations. For cooling, zone loads are obtained by first calculating heat gains for all components in the zone,
and then using these heat gains in the room transfer function equations to derive cooling loads. Per ASHRAE procedures, these calculations assume cooling is
provided 24 hours per day and all zones are held exactly at the occupied cooling thermostat setpoint. For heating, zone loads are computed as instantaneous heat
losses for the design heating condition. The occupied heating thermostat setpoint is used for this calculation. These loads are later adjusted for the actual operating
schedule, for the use of set-up and set-back temperatures in the unoccupied period and for the variation of zone temperatures in the thermostat throttling range. These
adjusted loads are listed as "zone conditioning" on the Air System Design Load Summary .
Each component load in a zone table is the sum of individual loads in all spaces in a particular zone. Individual items are as follows:
1. Solar Loads include loads due to solar radiation entering zones through windows in wall exposures and skylights in roof exposures. The value in the "details"
column represents the total area for all windows and skylights.
2. Wall Transmission lists the transmission load for all vertical wall exposures. The area in the "details" column is the net wall area. Only the wall transmission load
reaching the zone will be listed. Any wall load assigned to a return plenum is not included.
3. Roof Transmission lists the transmission load for all horizontal and sloped roof exposures. The area in the "details" column is the net roof area. Only the roof
transmission load reaching the zone will be listed. Any roof load assigned to a return plenum is not included.
Page 23 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.7 Space Design Load Summary Report
14.0 Designing Systems ››
Space Design Load Summary Report
14.0 Designing Systems ›› 14.7 Space Design Load Summary Report ››
4. Glass Transmission lists the transmission loads for all windows in wall exposures. The area in the "details" column is for all windows.
5. Skylight Transmission lists the transmission loads for all skylights in roof exposures.
6. Door Loads lists the total load for the door. This includes transmission of heat through both the opaque and glass portions of the door and the solar load for door
glass.
7. Floor Transmission lists heat transmission through floors above unconditioned space, slab on grade floors and basement floors. When basement floors are
involved, this item also includes heat transferred through below grade walls. Readers should note that slab and basement floor transmission are not considered for
design cooling calculations. Finally, the area listed in the "details" column lists the total area for these three types of floors. Areas for floors above conditioned
spaces and for basement walls are not included in this total area.
8. Partitions lists heat transmission for partitions adjacent to unconditioned spaces.
9. Ceiling lists heat transmission for ceilings below unconditioned spaces.
10. Overhead Lighting lists the lighting load for overhead lighting fixtures only. The load value listed is for the portion of the lighting load assigned to the zone. The
portion of the lighting load assigned to a return plenum is not listed. The wattage listed in the "details" column is the total lighting heat gain, and includes both the
portions of the heat gain assigned to the zone and to a return plenum.
11. Task Lighting lists the loads due to any task lighting fixtures.
12. Electric Equipment lists the loads due to electric equipment heat gain.
13. People lists the loads due to sensible and latent occupant heat gains.
14. Infiltration lists loads due to infiltration air. For the cooling calculation the "design cooling" infiltration airflow specified in space inputs is used. For the heating
calculation the "design heating" infiltration airflow specified in space inputs is used.
15. Miscellaneous lists loads due to any miscellaneous sensible and latent heat gains specified by the user.
16. Safety Factor lists the safety BTU/h or W for each column of cooling and heating loads. The safety loads are computed by summing load quantities in all previous
lines in the table and multiplying this total by the safety factor percentage specified by the user. In the cooling "details" column the safety factors specified by the
user are listed in the following order: cooling sensible, cooling latent.
17. Total Zone Loads lists the total of all load items in the table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Space Design Load Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Design Load Summary Report
The Space Design Load Summary report provides a list of component cooling and heating loads for each space in each zone in an air system. Individual loads for all
wall, window, roof, skylight and door elements in a space are also listed. Cooling data on this report can be generated for the hour of the peak sensible load in each
space, or for a month and hour chosen by the user. Heating data is always generated for the design heating condition. This report is used when investigating space
load behavior.. Length: A minimum of 1 page per space.
A sample of this report is shown below. Following this figure, the format and content of the report are discussed in detail.
Page 24 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Report Format and Content. The Space Design Load Summary report contains one pair of tables for each space in the system. The first table in each pair contains
component load data for the space. The second table contains load data for each wall, window, door, roof and skylight element in the space. The contents of each
table are discussed separately below.
Component Loads for Space. Space loads are the result of the first stage of the sizing calculations. For cooling, space loads are obtained by first calculating heat
gains for all components in the space, and then using these heat gains in the room transfer function equations to derive cooling loads. Per ASHRAE procedures, these
calculations assume cooling is provided 24 hours per day and all zones are held exactly at the occupied cooling thermostat setpoint. For heating, space loads are
computed as instantaneous heat losses for the design heating condition. The occupied heating thermostat setpoint is used for this calculation. Space loads are later
combined to obtain total loads for each zone. During system simulation calculations these zone loads are adjusted for the actual operating schedules, the use of set-
up or set-back temperatures in the unoccupied period and the variation of zone temperatures within the thermostat throttling range. The adjusted loads are listed as
"zone conditioning" on the on the Air System Design Load Summary .
Each row in this table contains data for a different space load component. The table contains seven columns: a column listing the load components, three columns
containing cooling load data and three columns containing heating load data. Columns for load data are as follows:
1. Details contains useful information associated with the cooling or heating load data. Examples include areas for walls or roofs and wattages for internal loads.
2. Sensible contains the sensible component of each load.
3. Latent contains the latent component of each load.
Individual line items in this table are as follows:
1. Solar Loads include loads due to solar radiation entering spaces through windows in wall exposures and skylights. The value in the "details" column represents the
total area for all windows and skylights.
2. Wall Transmission lists the transmission load for all vertical wall exposures. The area in the "details" column is the net wall area. Only the wall transmission load
reaching the space will be listed. Any wall load assigned to a return plenum is not included.
3. Roof Transmission lists the transmission load for all roof exposures. The area in the "details" column is the net roof area. Only the roof transmission load reaching
the space will be listed. Any roof load assigned to a return plenum is not included.
4. Glass Transmission lists the transmission loads for all windows in wall exposures. The area in the "details" column is for all windows.
5. Skylight Transmission lists the transmission loads for all skylights in roof exposures.
6. Door Loads lists the total load for the door. This includes transmission of heat through both the opaque and glass portions of the door and the solar load for door
glass.
7. Floor Transmission lists heat transmission through a floor above unconditioned space, a slab on grade floor or a basement floor. When a basement floor is
involved, this item also includes heat transferred through below grade walls. Readers should note that slab and basement floor transmission is not considered for
design cooling calculations. Finally, the area listed in the "details" column does not include basement wall areas if a basement floor is involved.
8. Partitions lists heat transmission for a partition adjacent to an unconditioned space.
9. Ceiling lists heat transmission for a ceiling below an unconditioned space.
10. Overhead Lighting lists the lighting load for overhead lighting fixtures only. The load value listed is for the portion of the lighting load assigned to the space. The
portion of the lighting load assigned to a return plenum is not listed. The wattage listed in the "details" column is the total lighting heat gain, and includes both the
portions of the heat gain assigned to the space and to a return plenum.
11. Task Lighting lists the loads due to any task lighting fixtures.
Page 25 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.8 Hourly Air System Design Day Loads Report
14.0 Designing Systems ››
Hourly Air System Design Day Loads Report
14.0 Designing Systems ›› 14.8 Hourly Air System Design Day Loads Report ››
12. Electric Equipment lists the loads due to electric equipment heat gain.
13. People lists the loads due to sensible and latent occupant heat gains.
14. Infiltration lists loads due to infiltration air. For cooling calculations the "design cooling" infiltration airflow is used. For heating calculations the "design heating"
infiltration airflow is used.
15. Miscellaneous lists loads due to any miscellaneous sensible and latent heat gains specified by the user.
16. Safety Factor lists the safety BTU/h or W for each column of cooling and heating loads. The safety loads are computed by summing load quantities in all previous
lines in the table and multiplying this total by the safety factor percentage specified by the user. In the cooling "details" column the safety factors specified by the
user are listed in the following order: cooling sensible, cooling latent.
17. Total Space Loads lists the total of all load items in this table.
Envelope Loads for Space. The second table for each space provides input data and cooling and heating load data for all wall, window, door, roof and skylight
elements in the space. Separate blocks of information are provided for each wall and roof exposure. In the example above two blocks are provided for a north wall
exposure and a horizontal roof exposure. Within each block separate line items provide information for each wall, window, door, roof or skylight element. For each load
element eight columns of data are provided as described below:
1. Type of Load Element defines whether information in this row is for a wall, window, door, roof or skylight element.
2. Area lists the surface area of the element. For wall and roof elements, the net area is listed rather than the gross exposure area.
3. U-value defines the overall U-value for the element.
4. Shade Coeff lists the overall shade coefficient for a window or skylight element.
5. Cooling Trans provides the cooling transmission load for the element.
6. Cooling Solar provides the solar cooling load for the element. It is only applicable for windows, skylights and door glass.
7. Heating Trans provides the transmission load for the element computed as an instantaneous heat loss at the design heating condition.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Hourly Air System Design Day Loads report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Hourly Air System Design Day Loads Report
The Hourly Air System Design Day Loads report provides 24-hour profiles of air system coil loads and fan airflows for design cooling days. Profiles can be generated
for one month or for a series of months. This report is used when investigating system load behavior. Length: 2 months per page.
A sample of this report for a VAV Reheat system for the month of July is shown below. Following this figure, the format and content of the report are discussed in
detail.
Page 26 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
Report Format and Content. The Hourly Air System Design Day Loads report contains one table per month. Data is obtained from a simulation of air system
operation for the design cooling day in each particular month. The month name is listed at the top of the table. Rows in the table contain data for each hour of the day.
Columns contain profiles of outdoor temperatures, supply airflow rates and coil loads.
When dealing with central air systems such as VAV or CAV systems, the column headings are as follows:
1. Hour. According to standard program conventions, hours are listed from 0000 to 2300 local time. Data for hour 0000 represents loads occurring between 12:00
midnight and 1:00 am local time.
2. OA Temp lists the outdoor air dry-bulb temperature for the hour.
3. Supply Airflow provides the actual airflow rate, corrected for altitude, for the system supply fan. In 2-Fan Dual Duct VAV systems, this airflow is for the cold deck
supply fan.
4. Central Cooling Sensible lists the sensible component of the central cooling coil load or the cold deck coil load for 2-Deck Multizone, 3-Deck Multizone or dual
duct systems.
5. Central Cooling Total lists the total load for a central cooling coil or a cold deck coil in a 2-Deck Multizone, 3-Deck Multizone or dual duct system.
6. Central Heating lists the load on a central heating coil or the hot deck coil in a 2-Deck Multizone, 3-Deck Multizone or dual duct system.
7. Precool Coil lists the total load for a precool coil, if used.
8. Preheat Coil lists the load on a preheat coil, if used.
9. Terminal Cooling lists the sum of loads for terminal cooling coils in all zones in the system. Example: The terminal cooling coils in a 4-pipe induction systems.
10. Terminal Heating provides the sum of loads for terminal heating coils in all zones in the system. Examples include terminal reheat coils or heating coils in 4-Pipe
Induction systems.
11. Zone Heating Unit lists the sum of heating coil loads for supplemental zone heating units in all zones in the system.
When dealing with terminal air systems such as fan coils or water source heat pumps, a different set of column headings, shown above, is used. These column
headings are as follows:
1. Hour. According to standard program conventions, hours are listed from 0000 to 2300 local time. Data for hour 0000 represents loads occurring between 12:00
midnight and 1:00 am local time.
2. OA Temp lists the outdoor air dry-bulb temperature for the hour.
3. DOAS Airflow is the airflow rate for a dedicated outdoor air system (DOAS) used in conjunction with the zone terminal units, if applicable. This value is an actual
airflow rate, corrected for altitude.
4. Central Cooling Sensible, Central Cooling Total, Central Heating columns are not applicable when working with terminal systems.
5. Vent Cooling Coil lists the total load for the cooling coil in a dedicated outdoor air system (DOAS) unit.
6. Vent Heating Coil lists the load on the heating coil in a dedicated outdoor air system (DOAS) unit.
7. Terminal Cooling lists the sum of loads for cooling coils in all zone fan coil or water source heat pump units.
8. Terminal Heating provides the sum of loads for heating coils in all zone fan coil or water source heat pump units.
9. Zone Heating Unit column is not applicable when working with terminal systems.
Page 27 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.9 Hourly Zone Design Day Loads Report
14.0 Designing Systems ››
Hourly Zone Design Day Loads Report
14.0 Designing Systems ›› 14.9 Hourly Zone Design Day Loads Report ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Hourly Zone Design Day Loads report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Hourly Zone Design Day Loads Report
The Hourly Zone Design Day Loads report contains 24-hour profiles of outdoor temperature, indoor temperature, indoor relative humidity, zone supply airflow and
zone loads for design cooling days. The report contains a separate sets of profiles for each zone in the system. The report can be generated for a single month or for a
series of months. This report is used when investigating zone load behavior or comfort levels within zones. Length: 2 zones per page for each month.
A sample of this report for one zone for the month of July is shown below. Following this figure, the format and content of the report are discussed in detail.
Report Format and Content. Each table in the Hourly Zone Design Day Loads report contains hourly data for one zone for one design cooling day. The zone name
and design month are listed at the top of each table. Rows in the table contain data for separate hours of the day. Columns in the table contain profiles for
temperatures, relative humidities, loads and airflows. Columns in this table are as follows:
1. Hour. According to standard program conventions, hours are listed from 0000 to 2300 local time. Data for hour 0000 represents loads occurring between 12:00
midnight and 1:00 am local time.
2. OA Temp lists the outdoor air dry-bulb temperature for the hour.
3. Zone Temp lists the dry-bulb temperature of air in the zone. This data is the result of heat extraction calculations during the air system simulation which accounts
for the variation of zone temperatures within the thermostat throttling range, between occupied and unoccupied period setpoints and due to pulldown loads.
4. Zone RH lists the relative humidity of air in the zone. This data is the result of a humidity balance calculation performed during the air system simulation which
determines the steady-state humidities at all points in the system. Note that for certain hours of the day when the system is shut down, humidity calculations cannot
be performed. In these cases a dash is displayed in the column to indicate zone relative humidity is not available.
5. Zone Airflow lists the supply airflow rate for the zone. Airflow data is in actual terms and thus includes corrections for altitude. The zone airflow is calculated using
the "Zone Cond" heat removal quantity, the supply temperature and zone temperature values for the hour.
6. Zone Sensible Load is derived by calculating heat gains for all components in the zone and then using these heat gains in the room transfer function equations to
derive loads . Per ASHRAE procedures this calculation assumes that cooling is provided 24 hours per day and the zone temperature is held exactly at the occupied
cooling thermostat setpoint. These zone sensible loads are later corrected for the actual system operating schedule, the use of set-up and set-back temperatures in
the unoccupied period and the variation of zone temperatures within the thermostat throttling range to produce the "zone conditioning" value shown in the next
column. Thus, the zone conditioning is the actual amount of heat which is removed from the zone, not the "zone sensible".
7. Zone Cond refers to the "zone conditioning". This is the actual amount of heat removed from the zone or added to the zone by the air system. As described earlier,
it is derived per ASHRAE procedures by first calculating the zone sensible load and then correcting for actual operating conditions. It accounts for the dynamic heat
flow in the zone due to changing temperatures between unoccupied and occupied periods, and within the thermostat throttling range. Often, a large part of the
difference between the zone conditioning and the corresponding zone sensible load is the pulldown load component.
8. Terminal Cooling Coil provides the load for a terminal cooling coil in the zone. Examples include the cooling coil in a 4-pipe induction terminal, a fan coil unit or a
water source heat pump unit.
Page 28 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
14.10 System Psychrometrics Report
14.0 Designing Systems ››
System Psychrometrics Report
14.0 Designing Systems ›› 14.10 System Psychrometrics Report ››
9. Terminal Heating Coil lists the load for a terminal heating coil in the zone. Examples include a terminal reheat coil, the heating coil in a 4-pipe induction terminal, a
fan coil unit or a water source heat pump unit.
10. Zone Heating Unit lists the heating coil load for a supplemental baseboard or fan coil heating unit in the zone.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the System Psychrometrics report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Psychrometrics Report
The System Psychrometrics provides a detailed account of airflow rates, temperatures and humidities at state points within the air system for one hour on a design
cooling day. This report can be generated in four different ways:
1. Tabular Report, for Peak Hour - The first part of the report displays psychrometrics data for the design month and hour when the peak central cooling coil load
occurred. The second part displays data for the winter design condtion.
2. Tabular Report, for Specific Hour - The report displays data for a specific design cooling month and hour specified by the user.
3. Graphical Report, for Peak Hour - The first page displays the system level data plotted on a psychrometric chart for the design month and hour when the peak
cooling coil load occurs. The second page displays system level data for the winter design condition.
4. Graphical Report, for Specific Hour - System level data is plotted on a psychrometric chart for a cooling design month and hour specified by the user.
This report is used when investigating details of system performance or control. Length: 1-2 pages.
A sample of this report for a VAV Reheat system is shown below. Following this figure, the format and content of the tabular version of the report are discussed in
detail.
Report Format and Content. The System Psychrometrics report contains two tables. The first lists airflow rates, temperatures, humidities and load quantities for state
points within the air system. For central systems such as VAV and CAV, the second table provides information about the temperature, airflow, load and thermostat
status for the zones served by the system. When dealing with terminal systems such as fan coils and water source heat pumps, the second table contains
performance data for each zone fan coil or heat pump. Contents of each table are discussed separately below.
System Data Table. In this table each row contains data for state points within the air system. An example of a state point is the outlet of the central cooling coil.
Columns contain information about the temperature, specific humidity, airflow rate, CO2 level (ppm) and related loads at each of these points. The line items
appearing in this table vary depending on the system type and the components or controls used in the system. A description of all possible state points is provided
below.
1. Ventilation Air: The condition of air at the outdoor ventilation air intake. The sensible and latent heat values are the ventilation loads.
2. Ventilation Reclaim: The condition of ventilation air immediately after it passes through a ventilation reclaim device such as a heat wheel, a heat pipe, or a pump-
around heat exchanger. The sensible and latent heat values define the heat reclaim or loss for air flowing through the ventilation side of the device.
3. Preheat Coil: The condition of air at the outlet of the preheat coil. The sensible heat value is the preheat coil load.
Page 29 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
4. Precool Coil: The condition of air at the outlet of the precool coil. The sensible and latent heat values are the loads for the coil.
5. Vent - Return Mixing: The condition of air immediately downstream of the point where outdoor air and return air streams mix.
6. Central Cooling Coil: The condition of air immediately downstream of the central cooling coil. The sensible and latent heat values are the loads for the coil.
7. Central Heating Coil: The condition of air immediately downstream of the central heating coil. The sensible heat value is the load for the coil.
8. Supply Fan: The condition of air immediately downstream of the central supply fan. The sensible heat value is the fan heat gain.
9. Heating Supply Fan: The condition of air immediately downstream of the hot deck supply fan in a 2-Fan Dual Duct VAV air system.
10. Humidifier: The condition of air immediately downstream of the central humidifier. The latent heat value is the moisture gain supplied to the supply air stream by
the humidifier.
11. Cold Duct Supply: The condition of air provided to zone supply terminals. In Multizone and Dual Duct systems, this is the condition of cold deck air supplied to the
mixing box for the zone. The condition of air can change between the central air handler and the zone terminal due to duct heat gains and leakage. The sensible
heat value is the duct heat gain or loss.
12. Hot Duct Supply: The condition of hot deck air supplied to the mixing box for the zone in a Multizone or Dual Duct system. The sensible heat value is the duct
heat gain or loss.
13. Zone Air: The condition of air in the zone. In systems serving multiple zones, weighted average values for temperature and humidity are shown. The airflow is the
sum of all zone airflows. Sensible and latent heat values are the sum of zone conditioning values for all zones in the system.
14. Zone Direct Exhaust: The condition of zone air directly exhausted from zones via toilet exhausts, lab hoods, kitchen hoods or similar devices.
15. Return Plenum: The condition of air at the outlet of the return plenum. The sensible heat value is the total plenum heat gain.
16. Bypass Air: The condition of air bypassed from the supply duct to the return duct or plenum in a VVT system.
17. Duct Leakage Air: The condition of air leaked from the supply duct to the return plenum or duct.
18. Return Duct: The condition of return air after plenum, bypass and duct leakage effects are considered. When a return fan is not used, the return duct data defines
the temperature and humidity of recirculated air that will mix with outdoor ventilation air.
19. Return Fan: The condition of air immediately downstream of the return fan. When a return fan is used, this data defines the temperature and humidity of
recirculated air that will mix with outdoor ventilation air.
System Data Table Footnotes. Beneath the System Data table are footnotes which list the sensible heat conversion factor, the latent heat conversion factor and the
site altitude. These factors are used when performing hand calculations with airflows, temperatures and humidities shown in the System Data Table to check load
calculation results.
1. The sensible heat factor is air density times heat capacity times a unit conversion factor. For standard sea level conditions this factor is 1.08 BTU/(hr-CFM-F) in
English units and is 1.207 W/(L/s-K) in Metric units. Both the sea level value and the value adjusted for site altitude are shown. In any hand calculations the value
adjusted for site altitude must be used to obtain valid results.
2. The latent heat factor is air density times heat of vaporization for water times a unit conversion factor. For standard sea level conditions this factor is 4746.6 BTU/
(hr-CFM) in English units and is 2947.6 W/(L/s) in Metric units. Both the sea level value and the value adjusted for site altitude are shown. In any hand calculations
the value adjusted for site altitude must be used to obtain valid results.
3. Finally, the site altitude is provided for reference.
Zone Data Table (Central Systems). In this table each row contains data for a separate zone in the system. Columns contain data describing the temperature,
airflow, CO2 level (ppm) and load behavior of the zone. Columns in this table are as follows:
1. Zone Name lists the name assigned to the zone during air system inputs. If names were not specified during air system input, default names such as Zone 1, Zone
2, etc... will appear in this column.
2. Zone Sensible Load is derived by calculating heat gains for all components in the zone and then using these heat gains in the room transfer function equations to
derive loads. Per ASHRAE procedures this calculation assumes that cooling is provided 24 hours per day and the zone temperature is held exactly at the occupied
cooling thermostat setpoint. These zone sensible loads are later corrected for the actual system operating schedule, the use of set-up or set-back temperatures in
the unoccupied period and the variation of zone temperatures within the thermostat throttling range to produce the "zone conditioning" value shown in a subsequent
column. Thus, the zone conditioning is the actual amount of heat which is removed from the zone, not the "zone sensible".
3. T-stat Mode lists the operating mode for the zone thermostat. "Cooling" means the thermostat is calling for cooling. "Heating" means the thermostat is calling for
heating. "Deadband" means the zone temperature is in the deadband between cooling and heating setpoints and is therefore not calling for cooling or heating.
4. Zone Cond refers to the "zone conditioning". This is the actual amount of heat removed from the zone or added to the zone by the air system. As described earlier,
it is derived per ASHRAE procedures by first calculating the zone sensible load and then correcting for actual operating conditions. It accounts for the dynamic heat
flow in the zone due to changing temperatures between unoccupied and occupied periods, and within the thermostat throttling range. Often, a large part of the
difference between the zone conditioning and the corresponding zone sensible load is the pulldown load component.
5. Zone Temp is the air temperature for the zone.
6. CO2 Level is the estimated CO2 concentration in the zone, measured in parts per million (ppm).
7. Zone Airflow lists the supply airflow rate provided to the zone.
8. Terminal Heating Coil lists the load for a terminal heating coil in the zone. Examples include a terminal reheat coil or the heating coil in a 4-pipe induction terminal.
9. Zone Heating Unit lists the heating coil load for a supplemental baseboard or fan coil heating unit in the zone.
Zone Data Table (Terminal Systems). In this table each row contains data for a separate state point in a fan coil or water source heat pump system. Line items are
grouped into blocks for each fan coil or heat pump zone in the system. Columns contain data describing the temperature, airflow and load behavior of the zone. Line
items in each block of this table are as follows:
1. Ventilation Air: The airflow rate for outdoor ventilation air supplied to the terminal unit. When direct ventilation is used, this is untreated outdoor air at the ambient
temperature and humidity. When a dedicated outdoor air system (DOAS) is used this is treated or untreated air supplied to the terminal unit by the DOAS.
2. Cooling Coil Inlet: The condition of air entering the cooling coil in the terminal unit.
3. Cooling Coil Outlet: The condition of air leaving the cooling coil in the terminal unit. The sensible and latent heat values are the component loads for the cooling
coil.
For an Active Chilled Beam system, the total and sensible coil loads will be highlighted red when total is greater than sensible. This indicates a latent load exists on
the terminal coil. Because an Active Chilled Beam terminal is a sensible-only device which does not have a drain pan to collect condensed moisture, the presence
of a latent load indicates a design problem.
4. Heating Coil Inlet: The condition of air entering the heating coil in the terminal unit.
Page 30 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm
5. Heating Coil Outlet: The condition of air leaving the heating coil in the terminal unit. This is also the temperature of air delivered to the zone. The sensible heat
value is the heating coil load.
6. Zone: The condition of air in the zone. The sensible heat value is the zone conditioning quantity for this zone.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 31 of 31
14.0 Designing Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh44A5.htm