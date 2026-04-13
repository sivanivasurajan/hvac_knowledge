15.0 Designing Plants
15.1 Overview for Plant Design Reports Form
15.0 Designing Plants ››
Overview for Plant Design Reports Form
15.0 Designing Plants ›› 15.1 Overview for Plant Design Reports Form ››
This chapter describes the contents of plant design reports in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of plant design reports in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Plant Design Reports Form
About Plant Design Reports. Plant Design Reports contain information used to size and select equipment for central cooling and
heating plants such as chillers and boilers. HAP offers three different tabular reports and one graphical report containing plant design
information.
Using various menu options and toolbar buttons in HAP, there are four different ways of generating plant design reports. These
methods are described in the Generating Plant Design Reports help topic. All four procedures require selection of report options on
the Plant Design Reports form shown below.
The Plant Design Reports Form is used to specify which reports should be generated and how they should be generated. The form
is divided into two sections:
1. The Working Area in the center of the form contains a table used to select report options. Each row in this table contains
specifications for a different report. Columns contain separate specifications for each report:
a. The Table column is used to select the tabular version of a report. Place a check mark in the box opposite the report name to
select the tabular version of that report.
b. The Graph column is used to select the graphical version of a report. Place a check mark in the box opposite the report name to
select the graphical version of that report.
c. The Time Specifications column describes how individual reports should be generated. The Hourly Chiller Load Profiles report
contains 24-hour load profiles for the design day in each month of the year. For this report the range of months to be included in
the report must be specified.
The contents of each report are summarized later in this help topic.
2. Command Buttons appear along the bottom of the form. Five buttons are provided:
Page 1 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
15.2 Cooling Plant Sizing Summary Report
15.0 Designing Plants ››
Cooling Plant Sizing Summary Report
15.0 Designing Plants ›› 15.2 Cooling Plant Sizing Summary Report ››
a. Press Restore Defaults to reset selections on the form to a standard set of defaults. This is often done when users wish to clear
existing selections and then begin selecting reports all over again.
b. Press Print to print the reports you’ve selected. Reports are directly printed without viewing them first.
c. Press Preview to view the reports you’ve selected. This launches the HAP Report Viewer and displays the reports you
requested. The HAP Report Viewer provides options for printing the reports as well as exporting report images to the Windows
clipboard and to bitmap image files.
d. Press Cancel to exit from the form and return to the HAP Main Program Window without generating reports.
e. Press Help to display this help topic.
Report Summaries. HAP offers three plant design reports in tabular format. A graphical versions of one of the reports is also
available. Each report is summarized below:
1. The Cooling Plant Sizing Summary report provides sizing data for a chiller plants, cooling requirements for a changeover plant
using reversible chillers, and sizing data for cooling and heat recovery chillers in a heat recovery plant. It also contains information
about coincident air system loads at the time of the peak plant load. This report option can only be used if one of the plants you
selected on the HAP main program window is a cooling plant, a changeover plant or a heat recovery plant. Length: 1 page; longer
for plants serving a large number of air systems.
2. The Heating Plant Sizing Summary report provides sizing data for hot water plants, steam plants, and the heating requirements for
a changeover plant using reversible chillers. It also contains information about coincident air system and service hot water loads at
the time of the peak plant load. This report option can only be used if one of the plants you selected on the HAP main program
window is a heating plant, a changeover plant or a heat recovery plant. Length: 1 page; longer for plants serving a large number of
air systems.
3. The Hourly Load Profiles report contains 24-hour profiles of chilled water loads for each design day. For this report you must
specify the range of months for which data will be generated. To generate the report for a single month, specify the same month as
the first and last months (e.g., July to July). This report is used when investigating chilled water load behavior and also when sizing
thermal energy storage systems. Length: 3 monthly load profiles per page.
The graphical version of this report provides one chilled water load profile graph for each month selected.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Cooling Plant Sizing Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Plant Sizing Summary Report
The Cooling Plant Sizing Summary report provides sizing data for a chiller plant or the cooling requirements for a changeover plant
using reversible chillers. It also contains information about coincident air system loads at the time of the peak plant load. A sample of
this report is shown below. Following this figure, the format and content of the report are discussed.
Page 2 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
Report Format and Content. The Cooling Plant Sizing Summary report contains three to five tables which describe the plant, the
peak load for the plant and coincident air system loads at the time of the peak plant load. Each table is discussed below.
The Plant Information Table provides reference information for the plant whose sizing data is shown on the report:
1. Plant Name lists the reference name you assigned to the plant.
2. Plant Type lists the type of plant being studied.
3. Design Weather lists the city name for the design weather data you created for this project.
The Cooling Plant Sizing Data Table provides information about the maximum plant load:
1. Maximum Plant Load lists the peak cooling load for the plant. This load is determined using a two step process. In the first step
hourly cooling coil loads for all air systems served by the plant are added together. This calculation produces a profile of total
hourly cooling loads for the plant. Any multipliers assigned to systems served by the plant are used to determine the number of
times coil loads for an air system are added to the plant profile. In the second step, hourly values in the plant cooling load profile
are inspected to identify the maximum cooling load. This value is reported as the Maximum Plant Load. It represents the peak
coincident cooling load on the plant.
Cooling coil loads included in this calculation depend on the plant type. The table below describes the rules for this calculation.
Plant Type
Cooling Sources for Coils Included in
Calculation of Maximum Plant Load
Generic Chilled Water
"Any" and Chilled Water
Generic Changeover
"Any" and Chilled Water
Chiller Plant
Chilled Water only.
Remote Chilled Water
Chilled Water only.
Changeover
Chilled Water only.
2. Load Occurs at lists the design month and hour when the maximum plant load occurs.
3. sqft/Ton or sqm/kW is the ratio of total floor area served by the plant divided by the maximum plant load. It serves as a useful
check figure.
4. Floor Area Served by Plant lists the total floor area served by the plant. This value is the sum of floor areas for all zones in all
systems served by the plant.
The Coincident Cooling Loads Table provides a list of cooling coil loads for all air systems served by the plant for the month and
hour when the maximum plant load occurs. This information is useful when investigating the distribution of cooling loads among
Page 3 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
15.3 Heating Plant Sizing Summary Report
15.0 Designing Plants ››
Heating Plant Sizing Summary Report
15.0 Designing Plants ›› 15.3 Heating Plant Sizing Summary Report ››
systems served by the plant. In this table each row contains data for one of the air systems served by the plant. Columns in the table
provide information about the system and its cooling load:
1. Air System Name is the reference name you assigned to the system.
2. Multiplier is the multiplier factor assigned to the system when the system was linked to the plant. Multipliers are used when an air
system represents one of a number of identical systems served by the plant.
3. System Cooling Coil Load lists the air system cooling coil load for the month and hour when the maximum plant load occurs. A
note at the bottom of the table documents what this coil load includes.
Readers should note that coil loads shown in this table do not include the multiplier factor for the system. Example: A system was
linked to a plant using a multiplier of 2. Its coincident cooling coil load listed in the table is 25 Tons. This means the coil load for one
of these air systems is 25 Tons. Because the multiplier is 2, the two systems impose a total load of 50 Tons on the central plant.
Chiller Design Capacities. For plants other than "Generic Chilled Water", the report will contain an additional table listing the design
capacities of the chillers in the plant. If the autosizing option is used the capacities displayed are those calculated by the program
based on peak plant load plus the oversizing factor, divided between the chillers according to user specifications. If capacities are
directly specified, the specified capacities will be shown.
Dedicated Heat Recovery Chiller. For a Heat Recovery Plant using a Dedicated Heat Recovery Chiller (DHRC), an additional table
will be provided listing the heating capacity of the DHRC. If autosizing is used, the program calculates this capacity based on the
simulation profiles of cooling and heating loads in the building. If the capacity is directly specified, the specified capacity is listed.
This table will only appear if the energy simulation has already been run for the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Heating Plant Sizing Summary report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Plant Sizing Summary Report
The Heating Plant Sizing Summary report provides sizing data for hot water plants, steam plants or the heating requirements for a
changeover plant using reversible heat pumps. It also contains information about coincident air system loads at the time of the peak
plant load. A sample of this report is shown below. Following this figure, the format and content of the report are discussed.
Page 4 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
Report Format and Content. The Heating Plant Sizing Summary report contains three tables which describe the plant, the peak load
for the plant and coincident air system loads at the time of the peak plant load. Each table is discussed below.
The Plant Information Table provides reference information for the plant whose sizing data is shown on the report:
1. Plant Name lists the reference name you assigned to the plant.
2. Plant Type lists the type of plant being studied.
3. Design Weather lists the city name for the design weather data you created for this project.
The Heating Plant Sizing Data Table provides information about the maximum plant load:
1. Maximum Plant Load lists the peak heating load for the plant. This load is calculated by summing heating coil loads for the design
heating condition for all air systems and/or service hot water systems served by the plant. Heating coil loads included in this
calculation depend on the plant type. The table below describes the rules for this calculation. Any multipliers assigned to air
systems served by the plant are used to determine the number of times coil loads for an air system are added to the plant load
total.
Plant Type
Heat Sources for Air System Heating Coils
Included in Calculation of Maximum Plant
Load
Generic Hot Water Plant
"Any" and Hot Water
Generic Steam Plant
"Any" and Steam
Generic Changeover
"Any" and Hot Water
Generic Service Hot Water
None
Hot Water Plant
Hot Water only
Steam Boiler Plant
Steam only
Changeover
Hot Water only
Service Hot Water
None
Remote Source Hot Water
Hot Water only.
Remote Source Steam
Steam only.
In addition, any of the plant types in this table may also include service hot water heating loads. Those loads are added to the
loads from the air system heating coils.
2. Load Occurs at indicates that the peak load is calculated for the "winter design" heating condition.
Page 5 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
15.4 Hourly Load Profiles Report
15.0 Designing Plants ››
Hourly Load Profiles Report
15.0 Designing Plants ›› 15.4 Hourly Load Profiles Report ››
3. BTU/hr/sqft or W/sqm is the ratio of maximum plant load to the total floor area served by the plant. It serves as a useful check
figure.
4. Floor Area Served by Plant lists the total floor area served by the plant. This value is the sum of floor areas for all zones in all
systems served by the plant.
The Coincident Heating Loads section provides a list of heating loads for all air system coils and/or service hot water loads served
by the plant for the design heating condition. This information is useful when investigating the distribution of heating loads among
systems served by the plant. In this table each row contains data for one of the air systems served by the plant. Columns in the table
provide information about the system and its cooling load:
1. Air System Name is the reference name you assigned to the system.
2. Multiplier is the multiplier factor assigned to the system when the system was linked to the plant. Multipliers are used when an air
system represents one of a number of identical systems served by the plant.
3. System Heating Coil Load lists the air system heating coil load for the design heating condition.
Readers should note that coil loads shown in this table do not include the multiplier factor for the system. Example: A system was
linked to a plant using a multiplier of 2. Its coincident heating coil load listed in the table is 400 MBH. This means the coil load for
one of these air systems is 400 MBH. Because the multiplier is 2, the two systems impose a total load of 800 MBH on the central
plant.
4. Coincident Service Hot Water Load lists the service hot water (SHW) load coincident with the peak heating time. This item only
appears if the plant serves SHW loads.
5. Pasteurization Loads - When the plant serves SHW loads, and the SHW system includes a storage tank with Pasteurization
cycles, additional items are included on the report:
a. Maximum Pasteurization Load defines the maximum load for pasteurization cycles.
b. "Load Occurs at" is the time when the maximum pasteurization load occurs.
c. Estimated Pasteurization Heater Capacity is the program-calculated capacity for the supplemental pasteurization heater. This
item only appears when the "autosize heater" option is selected for pasteurization.
Boiler and Heat Pump Design Capacities. For plants other than "Generic Chilled Hot Water" or "Generic Steam", the report will
contain an additional table listing the design capacities of the boilers or heat pumps in the plant. If the autosizing option is used the
capacities displayed are those calculated by the program based on peak plant load plus the oversizing factor, divided between the
boilers or heat pumps according to user specifications. If capacities are directly specified, the specified capacities will be shown.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes the content of the Chiller Hourly Load Profiles report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Hourly Load Profiles Report
The Hourly Load Profiles report contains 24-hour profiles of chilled water or changeover plant loads for each design day. This report is
used when investigating load behavior and also when sizing thermal energy storage systems. A sample of this report is shown below
and contains profiles for the months of May, June and July. Following this figure, the format and content of the report are discussed in
detail.
Page 6 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm
Report Format and Content. The Hourly Load Profiles report contains one table for each group of three months. In each table, rows
contain data for the hours of the day. One pair of columns is provided for each month and list the outdoor air dry-bulb temperature
and the plant cooling load. The month name is listed at the top of each pair of columns. Columns in this table are as follows:
1. Hour. According to standard program conventions, hours are listed from 0000 to 2300 local time. Data for hour 0000 represents
loads occurring between 12:00 midnight and 1:00 am local time.
2. OA Temp lists the outdoor air dry-bulb temperature for the hour.
3. Total Cooling is the total cooling load for the plant. For "Generic Chilled Water" and "Generic Changeover" plant types, the loads
include any coil whose source is "any" or "chilled water". For Chiller, Changeover and Remote Chilled Water plants, the loads only
include coils whose source is "chilled water".
The daily sum of plant cooling loads is shown at the bottom of the Total Cooling column (in ton-hours or kWh). This value is useful
when sizing thermal energy storage systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 7
15.0 Designing Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh1246.htm