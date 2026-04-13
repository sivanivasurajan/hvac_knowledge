1.0 Getting Started
1.1 Welcome to the Hourly Analysis Program
1.0 Getting Started ››
Welcome to the Hourly Analysis Program
1.0 Getting Started ›› 1.1 Welcome to the Hourly Analysis Program ››
1.2 What's New in HAP?
1.0 Getting Started ››
What's New in HAP?
1.0 Getting Started ›› 1.2 What's New in HAP? ››
This chapter provides an overview of software capabilities and of procedures for using the program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides a high level overview of program capabilities.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Welcome to the Hourly Analysis Program
Welcome to HAP. Welcome to Carrier’s Hourly Analysis Program (HAP). HAP is a computer tool which assists engineers in designing HVAC systems for commercial buildings.
HAP is two tools in one. First it is a tool for estimating loads and designing systems. Second, it is a tool for simulating energy use and calculating energy costs. In this capacity it
is useful for LEED®, schematic design and detailed design energy cost evaluations. HAP uses the ASHRAE-endorsed transfer function method for load calculations and detailed
8,760 hour-by-hour energy simulation techniques for the energy analysis.
This program is released as two similar, but separate products. The "HAP System Design Load" program provides the system design and load estimating features. The full "HAP"
program provides the same system design capabilities plus energy analysis features. This Quick Reference Guide deals with both programs.
HAP System Design Features. HAP estimates design cooling and heating loads for commercial buildings in order to determine required sizes for HVAC system components.
Ultimately, the program provides information needed for selecting and specifying equipment. Specifically, the program performs the following tasks:
• Calculates design cooling and heating loads for spaces, zones, and coils in the HVAC system.
• Determines required airflow rates for spaces, zones and the system.
• Sizes cooling and heating coils.
• Sizes air circulation fans.
• Sizes chillers and boilers.
HAP Energy Analysis Features. HAP estimates annual energy use and energy costs for HVAC and non-HVAC energy consuming systems in a building by simulating building
operation for each of the 8,760 hours in a year. Results of the energy analysis are used to compare the energy use and energy costs of alternate HVAC system designs so the
best design can be chosen. Specifically, HAP performs the following tasks during an energy analysis:
• Simulates hour-by-hour operation of all heating and air conditioning systems in the building.
• Simulates hour-by-hour operation of all plant equipment in the building.
• Simulates hour-by-hour operation of non-HVAC systems including lighting and appliances.
• Uses results of the hour-by-hour simulations to calculate total annual energy use and energy costs. Costs are calculated using actual utility rate features such as stepped,
time-of-day and demand charges, if specified.
• Generates tabular and graphical reports of hourly, daily, monthly and annual data.
Further Information: Click on any of the following topics for further information:
• A quick tutorial on running HAP system design or HAP energy analysis .
• What’s new in HAP.
• Using the main program window.
• Designing systems and plants.
If you have questions about the program: In the United States or Canada, please e-mail software.systems@carrier.utc.com. In other countries, please contact your local Carrier
sales office or local Carrier distributor.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes new features and changes made in the newest version of HAP, and also describes feature updates in previous HAP releases.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What's New in HAP?
This topic describes new and changed features in HAP v5.11.
A. HAP v5.11 Detailed List of Enhancements
This section provides details on the changes in HAP v5.11.
1. EIA Price Data - Updated the Energy Information Administration (EIA) electric and natural gas price data for US states using the latest published data for 2016.
2. BSO Import - Updated the "Import BSO Project Data" to import data from Building System Optimizer v1.60.
3. Help Menu - Added an option to the Help Menu to link to the program "What's New?" information that normally appears at program startup.
4. Problem Fixes - Corrected 7 problems identified in HAP v5.10
a. System Sizing I - If a single duct VAV system was configured with one or more VAV reheat terminals, and the minimum airflow for those terminals was specified as "% of
supply air", in certain cases the minimum zone airflow reported was too small. Minimum zone airflow is calculated as the larger of the specified minimum flow, the outdoor
ventilation requirement for the zone, or the airflow required to meet the design heating load for the zone. The error only occurred if minimum airflow was dictated by the
design heating load. Note that this error did not affect zones with VAV cooling only, series fan powered mixing box, or parallel fan powered mixing box terminals. Further,
the error did not occur if minimum airflow as specified with units other than "% of supply flow".
Page 1 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v5.1
1.0 Getting Started ›› 1.2 What's New in HAP? ››
If you have a v5.10 project with air systems affected by this problem, the systems must be recalculated in v5.11 to eliminate the problem. To force recalculation, open and
save the VAV system. Then print/view design reports to recalculate. If you wish to force a recalculation for the whole project, then open and save weather data. That will
automatically mark all systems for recalculation.
b. System Sizing II - The "VRF Outdoor Unit Sizing Data" table on the Zone Sizing Summary report listed incorrect cooling values in certain situations. If the indoor units
performed latent as well as sensible cooling at the indoor coil, the program incorrectly omitted the latent component from the cooling data shown in the VRF Outdoor Unit
Sizing table.
If you have a v5.10 project with VRF systems affected by this problem, the systems must be recalculated in v5.11 to eliminate the problem. To force recalculation, open
and save the VRF system. Then print/view design reports to recalculate. If you wish to force a recalculation for all systems in the project, then open and save weather
data. That will automatically mark all systems for recalculation.
c. System Sizing III - The Air System Hourly Design Day Cooling Loads report incorrectly omitted data for terminal heating coil loads. This includes loads for heating coils in
reheat terminals and in fan coil or WSHP units. This heating coil data was correctly calculated and was shown on other design reports. It was only omitted on this particular
report.
d. Building Wizard - When the Building Wizard was used to generate spaces and ASHRAE 90.1 schedules were selected in the Wizard, the generated schedules were
incorrect. For occupants this affected all building types except "assembly". For lighting and electric equipment this affected all building types. Note that fan / thermostat
schedules in Equipment Wizard were not affected by this problem.
e. Building Simulation - On the LEED v4 and LEED 2009 Summary reports, in the "Performance Rating Energy Consumption and Cost by Fuel Type" table, the Site Energy
Use Percent Savings total value was incorrect when running in SI Metric units. This value is in the Energy Model Sub Total row in the second cell from the right. The site
energy use percent savings values for individual energy sources were correct. Only the totals cell was incorrect.
f. Space Input - The ventilation standard shown at the bottom of the General tab incorrectly showed Standard 62.1-2010 for a very specific situation. The error only occurred
after creating a new project and accepting the default ventilation standard of Standard 62.1-2013 on the Project Preferences screen. The effect of the error is largely
cosmetic since 62.1-2010 and 62.1-2013 have the same space usage types, and ventilation airflow requirements.
g. gbXML Import - When importing a gbXML file that defined multiple window assemblies, only the last of the window assemblies was imported into HAP.
h. Calculation Status Window - Air system simulation calculations failed with an "Error 6: Overflow" error for a specific situation. This error occurred in the calculation status
window that appears while calculations are running, and only occurred when an air system contained an unusually large number of spaces. For example, a system serving
3000 spaces would trigger the error.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v5.10?
This topic describes new features in HAP v5.10. A summary of enhancements appears in Section A. Detailed discussions of those enhancements are found in Section B.
Section C describes changes in any updates made to v5.10.
A. HAP v5.10 (v5.1.0.14) Summary List of Enhancements
This section summarizes enhancements in HAP v5.10. Further details on these enhancements are found in section B.
1. Support for LEED and ASHRAE Standards
a. Support for LEED v4 compliance.
b. Updated LEED 2009 EA Credit 1 summary report.
c. Support for ASHRAE Standard 90.1-2013 compliance.
d. Support for ASHRAE Standard 62.1-2016 compliance.
2. New Modeling Capabilities
a. New options for determining or specifying Zone Air Distribution Effectiveness.
b. New options for specifying design heating supply temperature for reheat terminals.
3. Productivity Enhancements
a. New VRF Outdoor Unit (ODU) sizing data on design report..
b. Update EIA electric and gas prices for the United States.
4. Problem Fixes
a. 9 documented problems in v5.01 were corrected.
B. HAP v5.10 (5.1.0.14) Detailed List of Enhancements
This section provides details on the feature changes in HAP v5.10.
1. Support for LEED and ASHRAE Standards
a. Support for LEED v4 Compliance. Added a project preference option for LEED v4. With this option selected, HAP will generate a LEED summary report that contains
data formatted in a manner matching key portions of the current LEED v4 Energy Performance Calculator spreadsheet. This is the spreadsheet used for data submission
for the LEED v4 Minimum Energy Performance prerequisite and the LEED v4 Optimize Energy Performance credit. In addition to the spreadsheet-type data, the report also
contains a LEED v4 points table. Read more.
b. Updated LEED 2009 EA Credit 1 Summary Report. For LEED 2009 applications, the HAP LEED summary report was updated to provide data matching the format of key
portions of the current LEED Energy Performance Calculator spreadsheet. This spreadsheet is used for LEED 2009 Energy and Atmosphere Prerequisite 2 and Credit 1
submittals. The LEED Performance Calculator format is continually updated and prior versions of HAP used a report format matching an older version of the spreadsheet.
In addition to the spreadsheet-type data, the report also contains a LEED 2009 points table. Read more.
c. Support for ASHRAE Standard 90.1-2013 Compliance. ASHRAE Standard 90.1-2013 was added as a project energy standard option on the Project Preferences
window. When this option is selected and you choose the "ASHRAE Minimum Efficiency" option for equipment, HAP will derive equipment efficiency using the 90.1-2013
tables of required minimum efficiencies.
In addition, the "ASHRAE Minimum Efficiency" option has been added for Variable Refrigerant Flow (VRF) equipment, both when using 90.1-2013 and 90.1-2010 as the
project preference. These were the first two editions of Standard 90.1 specifying minimum efficiency requirements for VRF.
d. Support for ASHRAE Standard 62.1-2016 Compliance. ASHRAE Standard 62.1-2016 was added as a project ventilation standard option on the Project Preferences
window. When this option is selected, ventilation requirements can be selected from 2016 space usage types in space inputs. System inputs offer an option to calculate
system ventilation requirements using the 62.1-2016 Ventilation Rate Procedure.
2. New Modeling Capabilities
Page 2 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
a. New Options for Zone Air Distribution Effectiveness. For ASHRAE Standard 62.1 applications, new air system inputs were added to specify the location of the supply
diffuser and return grille in zones, and the design heating supply temperature for terminals, where it was not already being specified. These additional inputs expand the
range of the automatic calculation of air distribution effectiveness to cover all applications represented in Standard 62.1 Table 6.2.2.2 (Table 6-2 in older editions).
In addition, for special applications an option was added to allow air distribution effectiveness to be directly entered by the user. When this option is used, HAP does not
automatically derive the air distribution effectiveness.
b. New Options for Reheat Terminals. New air system inputs were added to define the design heating supply air temperature for reheat terminals in VAV reheat, single zone
constant volume, constant volume terminal reheat, and dual or triple duct constant volume systems. Design heating supply air temperature was already specified for series
and parallel fan powered mixing box terminals in earlier versions.
With this addition, reheat coil capacity sizing calculations are now temperature based. Capacity is derived from coil flow, inlet temperature and the specified reheat coil
design heating supply temperature. In prior versions of HAP the capacity was sized on zone load and primary air reheat. With this change in sizing calculations, you will
generally find reheat coil capacities to be equal to or larger than reported in previous versions of HAP. Read more.
This addition can also affect design zone supply airflow rates. For example, in a CAV Reheat system, the zone supply airflow rate is the larger of airflow needed to meet
the peak zone sensible cooling load at the design supply cooling temperature, or airflow needed to meet the peak zone heating load at the reheat coil design supply heating
temperature. That change can result in larger supply airflow rates than reported in prior versions of HAP. For VAV systems, the minimum VAV box airflow can be affected
since the minimum airflow must be able to meet the design zone heating load at the specified reheat coil design supply heating temperature. In some cases, the minimum
VAV terminal airflow will be larger than reported in previous versions of HAP.
Finally, this new input is used in ASHRAE Standard 62.1 calculations to determine air distribution effectiveness in those cases where the supply-air-to-room delta-T for
heating is a consideration in setting the effectiveness.
3. Productivity Enhancements
a. New VRF Outdoor Unit Sizing Data on Design Report. The Zone Sizing Summary report for Variable Refrigerant Flow (VRF) systems was updated to include a sizing
table for the VRF outdoor unit (ODU). This table lists the peak coincident load for all indoor units in cooling and heating, an estimate of pipe loss factor, and the total
capacity requirement for the ODU. Further details: VRF Outdoor Unit Sizing Table.
b. Updated EIA Electric and Gas Prices for the United States. Energy Information Administration (EIA) default prices for electricity and natural gas were updated to use the
latest available data. This data was published in October 2016 and is for the 2015 calendar year. Statewide average commercial sector prices are provided for each US
state. The defaults are used in the Utility Rate Wizard and are also documented in the help system here:EIA Electric and Fuel Prices.
4. Other Enhancements
a. Air System Design Reports – Added a CFM/ton check figure to the central cooling coil section of the Air System Sizing Summary report.
b. Air System Design Reports – Added a System Psychrometrics graph for design heating condition. When the graph is selected for the “peak” time, HAP will generate
psychrometric process graphs both for the design cooling and design heating conditions.
c. Air System Simulation Reports – Modified the Zone Temperature Report for the special case where a system has zero occupied period operating hours for the year (i.e.
all hours are in the unoccupied period). In this case the report shows maximum and minimum occupied temperatures as “na”.
d. LEED Reports - The Baseline Performance – Performance Rating Method Compliance table now displays process energy cost as a percentage of total baseline energy
cost with 1 decimal place rather than as a whole number (e.g. 24.6% rather than 25%). This helps in clarifying compliance with the 25% minimum rule. This change was
made both in the LEED v4 Optimize Energy Performance Summary report and the LEED 2009 EA Credit 1 Summary report.
e. Spaces - Increased the maximum limit for electric equipment heat gain from 99 W/sqft (1065 W/sqm) to 1000 W/sqft (10763 W/sqm).
f. Plants - Increased the maximum size for service hot water storage tanks from 1500 gal (5678 L) to 99999 gal (378537 L).
g. Chillers - Reduced minimum chiller EWCT limit from 45 F (7.2 C) to 35 F (1.7 C).
h. User Interface - On the HAP main window, the status bar now displays the current project preference selections for LEED rating method, energy standard, and ventilation
standard.
i. ASHRAE 90.1 Templates - Updated the ASHRAE 90.1-2007 template project archive to include additional prescriptive door constructions.
5. Problem Fixes
a. Air System Design Reports – For an air system using a preheat coil, the System Psychrometrics report incorrectly displayed the preheat coil airflow. The value shown in
the preheat coil airflow cell was actually the preheat coil load rather than the coil airflow. This was only a display error. HAP correctly calculated coil airflow and coil load,
but failed to display the data in the proper cells of the report table.
b. Air System Design Calculations – In certain situations, a “Subscript out of range” error occurred when performing design calculations for a system which specified
ASHRAE Standard 62.1 ventilation sizing. This error only occurred when the volume of a space served by the system was unusually large, such as a space with floor to
ceiling height of 50 ft (15 m) or larger.
c. Air System Input Report – The estimated maximum load shown for a VRF outdoor unit (ODU) was incorrect. This was only a cosmetic display problem. HAP correctly
calculates the estimated maximum load and the ODU cooling and heating capacities when auto-sizing is used. The only error was display of the maximum load.
d. Air System Inputs – When defining a Split DX Fan Coil terminal system, the Terminal Cooling equipment input screen incorrectly labeled the equipment performance input
as “Compressor kW” rather than “Compressor + Outdoor Fan kW”.
e. Plant Simulation – In a Dedicated Heat Recovery Chiller (DHRC) heat recovery plant with multiple cooling-only chillers, in certain off-design situations the plant operated
with an extra cooling only chiller running.
f. Weather Data – In certain situations when importing a simulation weather file, a “this weather file could not be imported” or “subscript out of range” error occurred. These
errors occurred if the weather file being imported was formatted using the TMY2, TMY3, ASHRAE IWEC or ASHRAE IWEC2 formats. The error did not occur when
importing a file with the EnergyPlus EPW format.
g. Space Inputs - In certain situations when saving a space, a "validation error" message appeared, but no input items were highlighted red as being invalid. As a result, the
space could not be saved. This only occurred if the space had previously been modified via the global change feature, the space had no exterior walls, and global change
was used to apply a CFM/sqft (L/s/sqm) infiltration value.
h. Equipment Wizard – In some situations, if a VRF system was defined with DOAS set to “not used”, the options for Demand Controlled Ventilation and Ventilation Reclaim
were still shown. These options are not valid for a terminal system using direct ventilation.
i. Project Management – In certain situations where individual air systems, plants, or buildings in a project were deleted, the data files containing the deleted items were not
removed from the project. This had no adverse effects on HAP operation. It only resulted in the disk space usage and archive file size being larger than necessary.
C. HAP v5.10 (v5.1.0.16) Problem Fixes
HAP v5.10 was updated on August 28, 2017 to correct five problems identified since its initial release August 10. This update was designated HAP v5.1.0.16. Issues resolved in
this update are as follows:
1. Air System Design Calculations - If the project energy standard was set to ASHRAE 90.1-2010 and supply fan performance was specified as "90.1 App G Fan kW", the
calculated system fan power allowance kW was incorrect. This error only occurred when using 90.1-2010 as the energy standard.
2. Air System Design Calculations - If the project ventilation standard was set to ASHRAE 62.1-2016 and the ventilation sizing method was for an air system was set to
"ASHRAE 62.1-2016", an error message "Unknown / Invalid OutVent sizing method: 7" appeared. This prevented design calculations from being run.
Page 3 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v5.0
1.0 Getting Started ›› 1.2 What's New in HAP? ››
3. Plant Design Reports - When running design calculations for a "Hot Water Plant" containing Service Hot Water (SHW) capability or a "Standalone SHW" plant, and in which
the Pasteurization feature was turned on, a "Subscript out of Range" error occurred. This only prevented the Hot Water Plant Sizing Summary from being generated. The
sizing calculations completed successfully and would not prevent energy simulations from being successfully run.
4. Chiller Input Data - When using the "Import" feature to import Carrier 30-series chiller performance data generated by Carrier Electronic Catalog, an "Error 430" message
appeared. This prevented data chiller from being imported.
5. Project Data Management - The Help button on the "Convert HAP" window failed to display help information. This window appears after you select the "Convert HAP v4.x or
v5.x Project" option on the Project Menu.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v5.0
This topic describes new features in HAP v5.00 and v5.01, the two versions prior to HAP v5.10. It is intended as reference information for v5.10 users interested in learning what
feature updates were included in these previous versions. The topic is divided into four sections:
A. HAP v5.01 Overview - Provides a high level overview of the major changes in v5.01.
B. HAP v5.01 Detailed List of Enhancements - Provides a high level overview of the major changes in v5.01.
C. HAP v5.00 Overview - Provides a high level overview of the major changes in v5.00.
D. HAP v5.00 Detailed List of Enhancements - Provides a complete description of changes in v5.00.
A. HAP v5.01 Summary List of Enhancements
1. Plant Modeling
a. Added ability to import performance data for air-cooled heat recovery chillers.
2. Problem Fixes
a. Corrected 4 reported problems.
B. HAP v5.01 Detailed List of Enhancements
1. Plant Modeling
a. Importing Performance Data for Air-Cooled Heat Recovery Chillers
Added the ability to import performance data from Carrier Electronic Catalog (E-CAT) for air cooled chillers with heat recovery features.
These chillers are equipped with both an air-cooled condenser and a water-cooled condenser. When operating in air-cooled condenser mode, the chiller uses the air-
cooled condenser to reject heat to the atmosphere. When the chiller runs in heat recovery mode it switches to the water-cooled condenser, rejecting heat to a hot water
loop to serve space heating and/or service water heating loads.
Versions of E-CAT Packaged Chiller Builder (North America) prior to v3.49s could export data for air cooled heat recovery chillers, but could only deliver performance map
data for the air-cooled condenser mode. HAP imported this data and provided default water-cooled condenser performance data which had to be customized by the user
(for example by manually entering load line data). Beginning with Packaged Chiller Builder v3.49s, performance maps for both air-cooled and water-cooled condenser
modes can be exported for these machines. HAP v5.01 has been modified to import both performance maps. This simplifies modeling of this type of equipment, reducing
labor to configure performance data for the equipment.
Contact your local Carrier sales office for information about air-cooled heat recovery chillers and to obtain a chiller performance data file for use in HAP. These chiller data
files are imported into HAP using the “Import Chiller Data” button on the Chiller Properties window. For information on modeling plants with air-cooled heat recovery plants
in HAP, please refer to Carrier eHelp #32 – Modeling A/C Chillers with Heat Recovery Condensers, available at www.carrier.com/commercial/en/us/software/hvac-system-
design/software-support .
2. Problem Fixes
The following four problems were corrected.
a. Air System Inputs – On certain computers, when opening an air system for editing, an “Error 380 Invalid Property Value” message appeared. This error is related to a
missing font file on the computer.
b. Plant Simulation – For a plant using air-cooled heat recovery chillers, when a chiller was operating at in water-cooled condenser mode at very low cooling loads, energy
input for the chiller was overstated. This problem only occurred if the air-cooled heat recovery chiller data was imported from Carrier E-CAT. It was due to a problem
calculating chiller performance in low-load cycling mode.
c. Weather Data – On the Weather Properties window, when Winnemucca, Nevada was selected as the city a “No Current Record” error message appeared.
d. What’s New Window – There was no way to disable the “What’s New” window that appears at program startup. The “Do not show me this message again” check box was
omitted from this window so the message could not be turned off.
C. HAP v5.00 Summary List of Enhancements
1. Air System Design and Modeling
a. Added simulation model for variable speed rotary compressor VRF condensing units.
b. Added ASHRAE Standard 62.1-2013 ventilation defaults and Ventilation Rate Procedure sizing calculations.
c. Revised the Ventilation Sizing Summary report for terminal systems to more clearly communicate the sizing of zone ventilation airflow and airflow for a dedicated outdoor air
system (DOAS).
d. Updated terminology to consistently use Dedicated Outdoor Air System (DOAS) throughout the program.
2. Wizard Features
a. Added ability to model waterside economizer for air-cooled chiller plants in the Equipment Wizard.
b. Updated Energy Information Administration (EIA) utility price defaults to use the latest published data (2014).
c. Add interoperability features to default utility price data based on location selection, to synchronize electric and gas prices, and to default HVAC equipment operating
schedule based on building type.
3. Other Features
a. Added option to import project data from Building System Optimizer into HAP.
Page 4 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
b. Updated air system, plant, and building simulation reports to export data to comma separated value (CSV) file format.
4. Bug Fixes
a. Corrected 9 reported problems.
D. HAP v5.00 Detailed List of Enhancements
1. Air System Design and Modeling
a. Variable Speed Rotary Compressor VRF Condensing Units
Added simulation performance curves for variable speed rotary compressor VRF condensing units. Features for modeling this equipment were added both to the detailed
user interface and the Equipment Wizard. With this addition, HAP now offers three types of performance models for VRF: variable speed rotary, variable speed scroll, and
digital scroll.
This new model is presented in the same manner as the two scroll models. On the Air System Properties window Equipment tab, you specify basic characteristics of the
condensing unit such as capacity, EER, COP, compressor type, and controls. During the energy simulation HAP applies these basic, widely available inputs to the
performance curves to create a scaled performance model for the VRF condensing unit. The model then calculates how the efficiency of the VRF condensing unit changes
each hour with changing operating conditions. For cooling these conditions include outdoor air dry-bulb, indoor air wet-bulb, line length, line vertical, part-load ratio, and
heat recovery. For heating these conditions include outdoor air dry-bulb, indoor air dry-bulb, line length, line vertical, part-load ratio, defrost cycles, and heat recovery.
b. ASHRAE Standard 62.1-2013
Added features for sizing outdoor ventilation air per ASHRAE Standard 62.1-2013. 62.1-2013 can now be selected as the project Ventilation Standard on the Project
Preferences screen. This allows ventilation requirements to be defaulted for spaces based on space usage type. It also allows air system ventilation sizing calculations to
performed per the 62.1-2013 Ventilation Rate Procedure.
c. Ventilation Sizing Summary
Revised the Ventilation Sizing Summary report for terminal systems such as fan coils, water source heat pumps, VRF, PTACs, induction beams and chilled beams to more
clearly communicate sizing results. In these systems each terminal unit qualifies as a separate “ventilation system” for Standard 62.1 purposes, and therefore a separate
Ventilation Rate Procedure calculation is performed for the spaces in each zone to determine a zone Vot. If a dedicated outdoor air system (DOAS) is used, the DOAS
airflow is the sum of zone Vot airflows.
Note that HAP has always used this calculation approach for terminal type systems. However the format of the Ventilation Sizing Summary report in previous versions did
not clearly communicate all the details of that calculation approach. Read more.
d. Dedicated Outdoor Air System Terminology
In prior versions of HAP, a terminal type system could include ventilation air provided by a “common ventilation unit” which preconditions outdoor air and distributes it to
zones. This has been updated to use the more common terminology “Dedicated Outdoor Air System (DOAS)”.
In addition the “Tempering Ventilation” system type, which can be used to model standalone make up air systems or standalone DOAS systems has been renamed “Make
Up Air / DOAS” for greater clarity.
2. Wizard Features
a. Waterside Economizer for Air-Cooled Chiller Plants
Updated the Equipment Wizard to allow modeling of integrated waterside economizer with air-cooled chiller plants. In this type of plant a cooling tower or dry cooler is used
to precool water in the chilled water return pipe. When the tower or cooler capacity is less than the plant load, the waterside economizer reduces the mechanical cooling
load on the air cooled chillers for partial free cooling. When the tower or cooler capacity exceeds the plant load, the waterside economizer provides 100% free cooling,
allowing the chillers to turn off.
This feature has been available in the detailed user interface since HAP v4.8 In HAP v5.0 the capability has been added to the Equipment Wizard.
b. EIA 2014 Utility Prices for US States
Updated Energy Information Administration (EIA) electric and natural gas price defaults offered in the Utility Rate Wizard to use the latest published data (2014 state
averages).
c. Wizard Interoperability
In a Full Wizard session, when you select a weather location in the United States, Energy Information Administration (EIA) prices for that US state are defaulted in the Utility
Rate Wizard.
In a Full Wizard session, the operating schedule for an HVAC equipment alternative will default based on the building type specified in Building Wizard. This defaulting
occurs when you create a new alternative.
In the Utility Rate Wizard, if you select an EIA price for electricity, the natural gas price is defaulted using EIA data for the same state. In addition, choosing an EIA price for
natural gas defaults the electric price for the same state.
3. Other Features
a. Import BSO Project Data
Added an option to the Project Menu to import project data from a Building System Optimizer project. Building System Optimizer (BSO) is a Carrier eDesign tool for rapid
energy modeling and screening of alternatives in the schematic design phase of projects. With this import feature, scenarios created in BSO can be loaded into HAP for
more detailed study as a project moves from schematic design to detailed design. Read more.
b. Simulation Reports
Updated air system, plant, and building simulation reports to export data to comma separated value (CSV) file format. In CSV format, the data can be more easily loaded
into spreadsheet tools such as Microsoft® Excel.
This feature replaces the option to export data to a fixed-column TXT-format file. While that TXT file could also be loaded into spreadsheets, the process was less direct
than loading a CSV file.
On the air system and plant simulation report selection screens, monthly, daily and hourly results can be exported to CSV by checking one of the boxes in the “CSV”
column. On the building simulation report selection screen, hourly energy use profiles can be exported to CSV by checking the CSV box for this report option. Read more:
Air System Reports, Plant Reports, Building Reports.
4. Problem Fixes
The following nine problems were corrected.
a. Air System Inputs – When the “90.1 Appendix G Fan kW” option was selected for supply fan performance, the button to display the A-Factor Calculations input screen
appeared in the wrong position on the screen, obscuring other inputs.
b. System Design Reports – For an induction beam or active chilled beam system in which a zone contains multiple spaces, and in which the zone primary airflow is set by
induction supply requirements rather than outdoor air ventilation requirement, the Ventilation Sizing Summary report showed incorrect Voz values for spaces in that zone.
This was a cosmetic error. Calculation of ventilation airflow requirements for the system was correct. Only display of the space Voz data was incorrect.
Page 5 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v4.9
1.0 Getting Started ›› 1.2 What's New in HAP? ››
c. Building Simulation I – For a very specific sequence of steps it was possible to create a complex electric rate with zero steps in the energy charge. If that electric rate was
used in a building simulation an “Error 5: Index out of bounds” error message appeared.
d. Building Simulation II – The unmet load hours shown on the LEED EAc1 Summary Report incorrectly included unmet loads for service hot water (SHW) systems. Unmet
load hours should only contain data for space conditioning systems. This error only occurred for projects modeling a standalone SHW system.
e. Building Wizard – When a wall, roof, or window assembly created in the detailed user interface was selected in the Building Wizard, the overall U-value was shown as
zero. In addition, an “Error 9: Subscript Out of Range” error occurred when generating the Building Wizard input report. These were cosmetic errors. Wizard inputs were
still successfully transformed into spaces, assemblies and schedules for the detailed HAP interface and were reliable for use in load calculations and energy simulations.
Note that these problems did not occur when selecting one of the Building Wizard default wall, roof or window assemblies.
f. Utility Rate Wizard – When price data for remote steam was entered, it was incorrectly assigned to the remote hot water meter in the building when wizard data was
transformed into detailed inputs.
g. Reports – Under specific conditions an “Error 521: Unable to open clipboard” error occurred when generating reports.
h. gbXML Import – For a very specific set of conditions the gbXML Import feature linked the wrong window or door assembly to spaces. This only occurred when the window
names in gbXML exceeded 30 characters, and the first 30 characters of each name matched the first 30 characters of other names.
i. Example Problem Results PDF – Example problem results listed in the Example Problems Results PDF document did not match results produced by the HAP v4.9
example problem. This PDF document is used by customers performing validation of the program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v4.9
This topic describes new features in HAP v4.90 and v4.91, the two versions prior to HAP v5.00. It is intended as reference information for v5.00 users interested in learning what
feature updates were included in these previous versions. The topic is divided into four sections:
A. HAP v4.91 Overview - Provides a high level overview of the major changes in v4.91.
B. HAP v4.91 Detailed List of Enhancements - Provides a high level overview of the major changes in v4.91.
C. HAP v4.90 Overview - Provides a high level overview of the major changes in v4.90.
D. HAP v4.90 Detailed List of Enhancements - Provides a complete description of changes in v4.90.
A. HAP v4.91 Summary List of Enhancements
This section summarizes enhancements in HAP v4.91. Further details on these enhancements are found in section B.
1. Report Enhancements
a. Revised the LEED 2009 EA Credit 1 Summary Report to include data for LEED template Table 1.4.2A (Envelope and Glazing Data).
b. Revised the Zone Sizing Summary report to group data more effectively equipment selection applications.
c. Revised the Air System Sizing Summary report to clarify report content for dedicated outdoor air system (DOAS) applications.
d. Revised the Cooling Plant Sizing Summary to include sizing information for a dedicated heat recovery chiller used in a heat recovery plant.
2. Building Wizard
a. Updated the ASHRAE Standard 90.1-2010 prescriptive wall and roof assemblies.
3. Printing
a. Revised printing workflow throughout the program to give users more control over printing options and standardize how those options are presented.
4. Documentation
a. Added a new Documentation Menu with options for displaying the Quick Reference Guide, standards compliance, and other information.
b. Updated web links on the Help Menu to link to Carrier’s new commercial products web site.
c. Added at template project archive containing ASHRAE 90.1-2010 constructions, ASHRAE 90.1-2010 Appendix G baseline system types, and ASHRAE default schedules.
5. Miscellaneous Features
a. Added the ability to specify a custom prefix when duplicating a building with spaces and equipment.
6. Bug Fixes
a.Corrected 15 reported problems.
B. HAP v4.91 Detailed List of Enhancements
This section provides further details on the feature changes in HAP v4.91.
1. Report Enhancements
a. LEED 2009 EA Credit 1 Summary Report
Added a new section modeled on Table 1.4.2A (Envelope and Glazing Data) from the LEED online template. This section contains two tables. The first table reports gross
wall area and glazing areas for each of the principal building exposures (N, NNE, NE, ENE, etc…), both for the Baseline 0-Degree building and the Proposed Building. The
second table reports total roof and skylight areas for the same buildings. The program automatically processes all spaces in each building to compile area data by
orientation, and grand totals for the whole building. This data is organized in a format similar to that of the LEED online template so it can be easily transcribed into the
template.
This addition was requested by users due both to the LEED requirement that this data be submitted, and the labor required to compile the data manually.
This table was also added to the LEED NC 2.2 Credit 1 Summary Report.
Read more.
b. Zone Sizing Summary
Reorganized the content of this report to group data for equipment selection of air terminals and terminal equipment together at the start of the report. This was done in
response to user feedback. It makes the report more effective to use and easier to understand.
For central systems (e.g., VAV, constant volume) the first table in the report contains maximum and minimum airflow, reheat coil capacity, fan powered mixing box airflow
and capacity data for supplemental heating units for each zone. Reference information about the zone peak sensible cooling and heating loads has been moved to the
second table in the report. Space peak sensible loads and airflows are found in a final table. Read more.
Page 6 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
For terminal systems (e.g., fan coils, WSHPs) the first two tables in the report contain design airflow, cooling capacity, cooling coil inlet and outlet conditions, heating
capacity, heating coil inlet and outlet conditions, fan selection data, and ventilation airflow requirements. Reference information about zone peak sensible cooling and
heating loads is moved to the third table in the report. Space peak sensible loads and airflows are found in a final table. Read more.
c. Air System Sizing Summary
Revised the title of this report to “Common Ventilation Unit Sizing Summary” when this report is generated for a terminal type system (e.g., fan coils, WSHPs, VRF, etc…).
For terminal systems the report contains sizing information for the coils and fans in the common ventilation unit, also known as a dedicated outdoor air system (DOAS) air
handler. Previously, use of the title “Air System Sizing Summary” caused confusion about the content of this report. This change was designed to clarify content and
eliminate such confusion.
d. Cooling Plant Sizing Summary
For heat recovery plants using a dedicated heat recovery chiller (DHRC), the required capacity for the DHRC was added to this report. Because the DHRC is sized during a
simulation run, this item will only appear on the sizing report after the plant simulation has been run.
2. Building Wizard
a. ASHRAE Standard 90.1-2010 Wall and Roof Assemblies
Upgraded the 90.1-2010 wall and roof assemblies, revising the material layer sequences and properties. Building Wizard offers preconfigured wall and roof constructions
designed to meet the ASHRAE 90.1-2010 prescriptive requirements for each climate zone. In the original data in HAP v4.90 the overall assembly U-values matched the
prescriptive requirements, but certain details involving seqeunce of material layers and/or continuous insulation specified in 90.1-2010 Appendix A were not included. All
90.1-2010 default wall and roof assemblies have now been updated to comply with these details.
3. Printing
a. Printing Workflow
Upgraded the printing workflow throughout the program to provide more control over printing options and to standardize how those options are presented. This was done in
response to user requests. Specific changes include:
The standard Windows printer selection window will appear each time you print, similar to behavior in other tools like Microsoft Office. This allows you to select a printer
type and modify properties such as single sided / double-sided, black&white/color, and page orientation.
A Printer Setup option was added to the Reports Menu on the main HAP window to allow you to select printer type and printer options at the start of a HAP session, or at
any point thereafter.
Your selection of printer type and printer options will be retained for the duration of your HAP session, or until you change them.
4. Documentation
a. Documentation Menu
Added a new Documentation Menu to the menu bar on the HAP main window. Options on this menu allow the display of electronic documentation including the HAP Quick
Reference Guide, the example problem reference results document, documents describing HAP compliance with industry standards, and a tutorial on using HAP for LEED
Energy and Atmosphere Credit 1. The HAP Quick Reference Guide option was moved from the Help Menu. The other documents were formerly found on the Carrier web
site.
Read more.
b. Help Menu Web Links
Items on the Help Menu which link to pages on the Carrier web site were updated to use the new web addresses for these pages on Carrier’s newly introduced commercial
products web site.
c. ASHRAE 90.1-2010 Template Project
Added a template project containing ASHRAE 90.1-2010 wall, roof and window prescriptive constructions, ASHRAE 90.1-2010 Appendix G baseline HVAC systems. and
ASHRAE default schedules. This project archive is installed in the Archives folder.
Template projects are useful time saver when starting new projects. After installing HAP v4.91, first retrieve and save this project on your computer. Subsequently you can
use the Import Project Data option on the Project Menu to import constructions, systems and/or schedules into your projects to save time recreating this data yourself.
Note that HAP v4.91 continues to install an ASHRAE 90.1-2007 template project containing similar data compliant with the 90.1-2007.
5. Miscellaneous Features
a. Duplicate Building (with Spaces and Equipment)
Modified this option to allow a custom prefix to be specified. Previously all data copied with this option would have the prefix [B000] for a baseline building or [P] for a
proposed building, according to user selection. A third option was added to allow you to specify a customized prefix that will be used for all data that is duplicated. This is
helpful when using the Duplicate feature for applications other than LEED projects.
6. Bug Fixes
a. Air Systems – After creating and saving an air system, it did not appear in the systems list on the main screen and therefore could not be edited or calculated. This error
only occurred when energy analysis features were turned off in HAP, and in the System Design Load program. This problem had been fixed shortly after release of v4.90
and was available for download beginning in January 2015. v4.91 also contains the fix.
b. Air System Design Calculations – When performing design calculations for an air system in which ventilation calculations were performed per ASHRAE Standard
62.1-2010, and one or more spaces specified outdoor air requirement in terms of CFM (L/s) or “% of supply air”, the ventilation sizing results were incorrect. CFM (L/s) and
“% of supply air” specifications are outside the scope of Standard 62.1 and the program should display an error message to notify the user data must be corrected before
calculations can be performed. The program handled this properly for 62.1-2004 and 62.1-2007, but not for 62.1-2010.
c. Plant Simulation I – For very specific conditions the condenser water pump energy use for a chiller plant was incorrect. This error only occurred for a chiller plant which
used a shared cooling tower and the plant control “Sequenced with Part Load Chiller: High and Low Loads”.
d. Plant Simulation II – When simulating a hot water plant created in Equipment Wizard which used an air to water heat pump, the simulation halted and displayed an error
cannot find tower record in database for record #0. As a result the simulation could not be completed.
e. Utility Rate Wizard I – After defining a detailed electric rate with time of day pricing, the next time the data was edited the time of day pricing table would appear as empty
in certain specific situations. Input data had been saved properly but was not displayed on the input screen.
f. Utility Rate Wizard II – For a detailed electric rate, the Demand Charge Steps and Demand Charge pricing table sections of the input sometimes contained incorrect data
that did not match data entered on the input screen. The entered data was correctly saved and used in calculations. Only the display on the input report was incorrect.
g. Building Wizard I – Five of the ASHRAE prescriptive wall and roof assemblies offered in Building Wizard had U-values that deviated slightly from the ASHRAE 90.1-2010
required values.
h. Building Wizard II – The overall weights for wall and roof assemblies offered in the Building Wizard were incorrectly listed as 10 lb/sqft (48.82 kg/sqm). This was a
cosmetic error which only affected display of data on the screen and on reports. It did not affect wall or roof load calculations.
i. Equipment Wizard I – In specific circumstances when defining a changeover plant, the list of chiller types was incorrect.
j. Equipment Wizard II – When launching the Equipment Wizard, a message Error 76: Path not found: Wizards\EW\_AirSys\_Base\_05.2.gif occurred. This error occurred on a
a very limited number of computers.
k. ASHRAE 90.1-2007 Template Archives – For ASHRAE baseline system types 7 and 8 the minimum primary airflow for the parallel fan powered mixing box terminals was
incorrectly set to 50% instead of 30%.
l. Main Window I – Under special conditions the right hand panel in the HAP main window was blank. This only occurred in certain situations using the “list view” option for
the right hand panel.
Page 7 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
m. Main Window II – After editing a cooling tower and then exiting the program or opening a different project, HAP did not display a warning message that the project needed
to be saved.
n. Main Window III – If a library item (schedules, walls, roofs, windows, doors, shades, chillers, towers, boilers, electric rates or fuel rates) was entered having a name that
begins with one or more space characters, the name would not be saved. For example in a schedule the entered name would be replaced with “Schedule 1”.
o. Building Simulation – When generating the LEED EA Credit Summary report, HAP requires that corresponding Miscellaneous Energy Use items in the four baseline
buildings have exactly identical names. When names were edited so names differed only in the use of upper and lower case letters, HAP generated an error message
which prevented the calculations from running. The validation rules have been relaxed so names must still match but can differ in the use of upper and lower case
letters.\*\*\*
C. HAP v4.90 Summary List of Enhancements
This topic summarizes enhancements in HAP v4.90. Further details on these enhancements are found in section B.
1. Plants
a. Added a new "Heat Recovery" plant type for use in energy simulations.
b. Added a new "Generic Heat Recovery" plant type for use in design calculations.
c. Added features for modeling six plant heat recovery schemes within the "Heat Recovery" plant type.
2. Chillers
a. Added options for including double bundle condenser, desuperheater and heat recovery condenser components in the chiller and for specifying related performance data.
b. Updated the DX free cooling feature to make modeling this feature easier..
3. Wizards
a. Revised the Building Wizard to provide more extensive default choices for wall, roof and window assemblies, and to display details to help users understand the
construction and performance of the selected wall, roof or window assembly type.
b. Revised the Equipment Wizard to include options for modeling heat recovery plants and six types of heat recovery schemes.
c. Revised the Utility Rate Wizard to allow remote steam price structures to be defined when working with absorption chiller plants.
4. Miscellaneous Features
a. Revised the Ventilation Sizing Summary system design report, when using ASHRAE Standards 62.1-2004, -2007 or -2010 calculations, to Standard 62.1 terminology and to
display Standard 62.1 variable names for quantities shown on the report.
b. Added simulation weather data for 37 new cities and updated data for 24 further cities..
5. Bug Fixes
a. Corrected 8 problems identified in HAP v4.80.
D. HAP v4.90 Detailed List of Enhancements
This section provides further details on the feature changes in HAP v4.90.
1. Plants
a. Heat Recovery Plant Type.
Added a new "Heat Recovery" plant type for energy simulations. This is a special type of plant that combines all the equipment and controls for a chilled water cooling plant
and a hot water heating plant, and the equipment to recover heat from the cooling system for use in meeting hot water heating loads.
b. Generic Heat Recovery Plant Type.
Added a new "Generic Heat Recovery" plant type for plant design calculations. With this single plant, both peak cooling and heating load capacities can be determined..
c. Heat Recovery Schemes.
The new "Heat Recovery" plant type offers models for six different heat recovery schemes:
Dedicated heat recovery chiller (DHRC) in parallel with cooling-only chillers
Air-cooled chillers with heat recovery condensers
Heat exchange in condenser loop
Dedicated heat recovery chiller in condenser loop
Double-bundle chillers
Chillers with desuperheaters
Further Information
2. Chillers
a. Double Bundle Condensers, Desuperheaters and Heat Recovery Condensers.
Added features for defining three types of heat recovery components in chillers: Double Bundle Condensers, Desuperheaters and Heat Recovery Condensers. These heat
recovery components must be defined for a chiller included in a heat recovery plant using double bundle chillers, desuperheaters or heat recovery condensers, respectively.
Further Information
b. DX Free Cooling
Upgraded features for modeling DX free cooling in air-cooled chillers. HAP now supplies typical default performance data when DX free cooling is selected. In addition,
performance may now be defined in terms of % full load capacity and kW/Ton (ikW/kW). Both enhancements assist with schematic design studies for which machine-
specific performance data is not yet available.
Further Information
3. Wizards
a. Building Wizard.
Revised the Building Wizard to provide more extensive default choices for wall, roof and window assemblies, and to display details to help users understand the
construction and performance of the selected wall, roof or window assembly type.
Previously the Building Wizard offered three choices for wall and roof assemblies (Light, Medium and Heavy walls), and two options for window assemblies (Standard and
High Performance). These default offerings have been expanded to include ASHRAE 90.1-2010 wall and roof assemblies by climate zone. These assemblies have
Page 8 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
performance which meets 90.1-2010 prescriptive performance requirements. Default offerings for windows include ASHRAE 90.1-2010 assemblies by climate zone which
meet the prescriptive performance requirements for U-value and Shade Coefficient. In addition, further defaults are offered for common types of single-pane, double-pane
and triple-pane windows, with clear, reflective and tinted glazings as well as low-e coatings.
When a wall or roof assembly is selected from the drop-down list, the sequence of material layers and the overall U-value are now displayed for reference. When a window
assembly is selected, the U-value and Shade Coefficient are displayed for reference.
Further Information
b. Equipment Wizard
Revised the Equipment Wizard to include options for modeling heat recovery plants. The same six heat recovery schemes described in item 1c above are offered in the
Equipment Wizard.
Further Information
c. Utility Rate Wizard.
Revised the Utility Rate Wizard to add pricing information for remote steam. This feature was added for applications using chilled water plants with steam-driven absorption
chillers.
Further Information
4. Miscellaneous Features
a. Ventilation Sizing Summary.
Revised the Ventilation Sizing Summary system design report. When using ASHRAE Standard 62.1-2004, -2007 or -2010 as the ventilation sizing method, the report now
uses Standard 62.1 terminology and displays the Standard 62.1 variable names for quantities shown on the report. The original format for this report, introduced in 2005,
used general descriptive labels for items on this report because there was not widespread familiarity among users with the Standard 62.1 terminology. More recently, due
code related work and especially as a result of LEED projects, there is broader familiarity and acceptance of the Standard 62.1 terminology in the engineering community.
Based on requests from HAP customers we have revised the report to use Standard 62.1 terminology and to also indicate the Standard 62.1 variable names for each
quantity on the report for easier comprehension.
Further Information
b. Simulation Weather Data.
Added or updated simulation weather data for 42 cities. All of the new and updated city files are automatically installed with the program and can be selected via the "Add
From HAP Library" window in the Weather Properties window.
Simulation weather data was added for the following cities:
Oranjestad, Aruba
Nassau, Bahamas
Bridgetown, Barbados
Barranquilla, Colombia
Cali, Colombia
San Jose, Costa Rica
Santo Domingo, Dominican Republic
San Salvador, El Salvador
St. George, Grenada
Guatemala City, Guatemala
San Pedro Sula, Honduras
Tegucigalpa, Honduras
Kingston, Jamaica
Culiacan, Mexico
Hermosillo, Mexico
Mexicali, Mexico
Tijuana, Mexico
Torreon, Mexico
Dunedin, New Zealand
Hamilton, New Zealand
Hokitika, New Zealand
Invercargill, New Zealand
Kaitaia, New Zealand
Masterton, New Zealand
Napier, New Zealand
Nelson, New Zealand
New Plymouth, New Zealand
Paraparaumu, New Zealand
Queenstown, New Zealand
Rotorua, New Zealand
Tauranga, New Zealand
Managua, Nicaragua
Doha, Qatar
Ljubljana, Slovenia
Port of Spain, Trinidad and Tobago
Simulation weather data was updated for the following cities:
Manama, Bahrain
Porto Alegre, Brazil
Rio de Janeiro, Brazil
Chengdu, China
Guangzhou, China
Changsha, China
Jinan, China
Tianjin, China
Wuhan, China
Xian, China
Abidjan, Ivory Coast
Kuwait City, Kuwait
Monterrey, Mexico
Rabat, Morocco
Auckland, New Zealand
Page 9 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v4.8
1.0 Getting Started ›› 1.2 What's New in HAP? ››
Christchurch, New Zealand
Wellington, New Zealand
Muscat, Oman
Dhahran, Saudi Arabia
Jeddah, Saudi Arabia
Durban, South Africa
Pretoria, South Africa
Dubai, United Arab Emirates
5. Bug Fixes
a. System Calculations - If a 2-pipe fan coil system was defined with hot water heating and 2-pipe changeover controls, was saved, and then later edited to change the
heating source from hot water to electric resistance, the 2-pipe changeover controls were not automatically removed As a result, during system design and system
simulation calculations, the program continued to calculate changeover control, resulting in faulty control of the cooling coil. Cooling could be unavailable for many hours.
During those hours zone air temperatures could rise to extreme levels. Instead, changeover controls should be disabled when the heating source is no longer hot water.
b. Plant Simulations - While running the simulation for a plant using air-cooled chillers, the simulation halted and displayed and "Error 91" message. This error only occurred
when the user was attempting to model waterside economizer and had selected free cooling and specified "one tower for each water-cooled chiller" as the cooling tower
configuration. To model waterside economizer with air-cooled chillers the configuration "one tower shared by all water-cooled chillers" must be used.
c. HAP Wizards - After selecting the "Full Wizard Session" on the Wizards Menu or clicking the "Full Wizard Session" button on the toolbar, the Full Wizard screen appeared
immediately followed by an "Error 3265" error message. This error only occurred when the current opened project was one of the ASHRAE 90.1-2007 template projects
which automatically install with the program. The error was due to bad data in these template projects.
d. System Design Calculations I - When calculating ventilation airflow requirements using ASHRAE Standard 62.1-2004, -2007 or -2010 for a system with parallel fan
powered mixing box (PFPMBX) air terminals, two errors could cause ventilation airflow results to be incorrect in specific situations. If the delta-T between heating supply
temperature and heating setpoint was less than 15 F, the program set the air distribution effectiveness to 0.8 instead of 1.0. In addition, in a situation where the space
outdoor airflow rate (Voz) was larger than the specified minimum primary supply airflow (Vpz), Vpz was incorrectly adjusted to a value larger than Voz. Note that many
PFPMBX systems will not be affected by these conditions and produce correct system outdoor air intake airflow (Vot) results. In cases where air system characteristics do
trigger the error, Vot could be either overstated or understated depending on conditions.
e. System Design Calculations II - When calculating ventilation airflow requirements using ASHRAE Standard 62.1-2004, -2007 or -2010 for a system with series fan
powered mixing box air terminals, two errors could cause ventilation airflow results to be incorrect in specific situations. For the ventilation airflow calculation for the heating
design condition, the primary supply airflow rate (Vpz) was incorrectly being set to the primary airflow at maximum supply airflow conditions rather than the minimum
primary supply flow. In addition, in a situation where the space outdoor airflow rate (Voz) was larger than the specified minimum primary supply airflow (Vpz), Vpz was
incorrectly adjusted to a value larger than Voz. Depending on air system characteristics, these errors could cause the outdoor air intake airflow (Vot) to be either
unchanged, overstated or understated.
f. System Design Calculations III - For an air system serving one zone containing one space in which ventilation airflow was calculated per ASHRAE Standard 62.1-2004,
-2007, or -2010, the Ventilation Sizing Summary displayed incorrect values of "Uncorrected Outdoor Airflow" (Voz). The report also displayed the diversity factor which is
extraneous information for this scenario and should not be shown. However, note that the outdoor air intake airflow (Vot) was calculated and reported correctly in this case.
Only the "Uncorrected Outdoor Airflow" items were shown incorrectly.
g. System Design Calculations IV - When calculating ventilation airflow requirements using ASHRAE Standard 62.1-2004, -2007, or -2010, for certain system types with a
design heating supply air temperature exactly 15 F higher than the occupied heating thermostat setpoint, the program incorrectly set the air distribution effectiveness (Ez) to
1.0 instead of 0.8. The affected system types were single zone CAV, VVT, dual duct CAV, 2-deck multizone, 3-deck multizone and terminal units such as fan coils and
WSHP. Note that cooling only systems, systems with a heating SAT to room delta-T other than 15 F or systems in which cooling mode dictates the outdoor intake airflow
(Vot), this error had no effect. In those cases where the error did affect results, it typically caused ventilation airflow to be understated.
h. System Design Calculations V - When calculating ventilation airflow requirements using ASHRAE Standard 62.1-2004, -2007, or -2010, for 2-Fan Dual Duct VAV or 1-Fan
Dual Duct VAV systems in which the design heating condition determines the worst case outdoor air intake airflow (Vot), the combined hot deck and cold deck airflow rate
was incorrectly calculated. This could cause the outdoor air intake airflow (Vot) for the system to be either understated or overstated.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v4.8
This topic describes new features in HAP v4.80. It is intended as reference information for v4.80 users interested in learning what feature updates were included in this previous
version. The topic is divided into two sections:
A. HAP v4.80 Summary List of Enhancements - Summarizes the key changes in each major section of v4.80.
B. HAP v4.80 Detailed List of Enhancements - Provides a complete description of changes in v4.80.
A. HAP v4.80 Summary List of Enhancements
This topic describes enhancements in HAP v4.80. Further details on these enhancements are found in section B.
1. Air Systems
a. Added Induction Beam (IB) air system model.
b. Added Active Chilled Beam (ACB) air system model.
c. Added system design calculations and system design reports for IB and ACB systems
d. Added system simulations for IB and ACB systems to calculate hour by hour energy performance of these systems.
e. Added ability to export system design results to Carrier Electronic Catalog for selection of Induction Beam air terminals.
2. Plants
a. Added ability to model waterside economizer with air-cooled chiller plants.
3. Wizards
a. Added features for modeling Induction Beam (IB) systems in the Equipment Wizard..
b. Added features for modeling Active Chilled Beam (ACB) systems in the Equipment Wizard
4. Bug Fixes
a. Corrected 13 problems identified in HAP v4.70.
B. HAP v4.80 Detailed List of Enhancements
This section provides details on the feature changes in HAP v4.80.
Page 10 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1. Air Systems
a. Induction Beam Air Systems.
b. Active Chilled Beam Air Systems.
The Air System Properties window has been updated to allow input of these two new system types. Key changes:
To select these system types, go to the General tab and specify Equipment Type = Terminal Systems and then select Induction Beams (IB) or Active Chilled Beams
(ACB) as the System Type. For both system types a common ventilation system (i.e. Dedicated Outside Air System or DOAS) is required.
The Ventilation System Components tab offers most of the same components and features as offered for other terminal systems like fan coils and water source heat
pumps. For IB and ACB systems the option of closing outdoor dampers for unoccupied periods and using recirculated air is offered in the Ventilation data view. For IB
systems an option is offered in the Ventilation Fan data view to run the ventilation fan at reduced airflow during unoccupied periods.
The Zone Components tab contains modifications to the Common Data view - design supply air temperatures are not required for IB or ACB systems. The Terminal
Units data view offers options for defining the terminal induction ratio and cooling coil bypass factor.
c. System Design Calculations and Reports – HAP performs system sizing calculations for the IB and ACB systems. Modifications were made to the Zone Sizing Summary
report to display the primary supply airflow requirement and to remove terminal fan sizing data when IB or ACB systems are calculated.
d. System Simulation – HAP simulation engines were updated to model the hour by hour energy performance of the Induction Beam and Active Chilled Beam systems.
e. Export to Carrier Electronic Catalog – Equipment sizing results can be exported to Carrier Electronic Catalog (E-CAT) for use in selection of induction beam air terminal
equipment. This is done using the Publish Equipment Sizing Requirements option on the toolbar or the Project Menu. The "Publish" feature also allows sizing results for
many other equipment types to be exported to E-CAT.
2. Plants
a. Waterside Economizer for Air-Cooled Chiller Plants.
Added the ability to model waterside economizer free cooling in chiller plants using air-cooled chillers. In such a plant a cooling tower or dry cooler turns on and operates
when it can deliver cold enough water to provide 100% free cooling (non-integrated waterside economizer) or when it can deliver cold enough water to precool return water
and provide partial or 100% free cooling (integrated water side economizer). Previously this feature was limited to chiller plants containing water-cooled chillers.
To use this feature:
(i) Create a chiller plant
(ii) On the Configuration tab check the box for free cooling and specify the type of free cooling.
(iii) Also on the Configuration tab specify that "one tower is shared by all water-cooled chillers". In a plant that contains only air-cooled chillers, this will mean one tower or
dry cooler is shared among the air cooled chillers for purposes of free cooling.
(iv) On the Schedule of Equipment tab select a cooling tower, dry cooler or geo/well source that will serve as the heat rejection device or system providing free cooling.
During the plant simulation, the software will evaluate hour by hour conditions. When conditions are favorable for free cooling the heat rejection device or system will turn
on to provide partial or 100% free cooling, depending on the type of free cooling specified and the current conditions.
3. Wizards
a. Induction Beam Air Systems
b. Chilled Beam Air Systems.
The Equipment Wizard was modified to add features for modeling Induction Beam (IB) and Active Chilled Beam (ACB) systems. These features appear on the System and
Equipment input screen and on the System and Equipment Details screen for terminal systems.
4. Bug Fixes
a. Plant Design Calculations I – In certain situations, when running plant design calculations for a Service Hot Water (SHW) plant or a Hot Water Plant or Steam Plant which
served both space and SHW loads, the calculation halted and displayed an error message "Error 6 Overflow for SHW Plant Design Calculations". This problem only
occurred if the SHW maximum consumption rate was defined in terms of gal/person/day (L/s/person/day) and the occupant population was larger than 1450.
b. Plant Design Calculations II – When plant design calculations were run for one of the "Generic" plant types, any required air system design calculations were not
automatically run first. This resulted in plant peak load being incorrect. Note that if design calculations for the air systems served by the plant had previously been run after
the latest changes to the system, no error occurred. The error only occurred if air system design calculations had not previously been run at all, or if changes to the air
systems had made since the design calculations were last run..
c. Plant Design Calculations III – In certain situations, when running plant design calculations for a Service Hot Water (SHW) plant or a Hot Water Plant or Steam Plant
which served both space and SHW loads, the calculation would halt and display an error message "Unable to load schedule data." This problem only occurred if air
systems served by the plant have one or more spaces containing zero occupants.
d. Editing Plants I – In certain situations, when opening the Plant Properties window to edit data, the program halted and displayed the following error "Error 91 Object
Variable or With Block Variable Not Set". This problem only occurred if one of the air systems linked to the plant had been changed to use a different source of cooling or
heating. For example, this could involve a system originally defined as a chilled water AHU which was linked to a cooling plant, and then later the system was changed into
a packaged rooftop and therefore no longer contains chilled water coils.
e. Editing Plants II - For an unusual sequence of steps, the shared ground source for a hot water plant using water-to-water heat pumps was not displayed on the plant
properties window or the plant input report. The required sequence involved starting with a project created in HAP v4.6 or a prior version that contained a hot water boiler
plant, converting the data to HAP v4.7 format, editing the boiler plant and changing it to use water-to-water heat pumps and a shared geo source. This data is correctly
saved and used in calculations. But if you later edit the plant or generate the plant input report, the shared geo source will not be displayed.
f. Editing Plants III - When running HAP with energy analysis features turned off and hidden, the program did not offer options in the plant inputs for choosing plant types
"Generic SHW Plant" and "Generic Changeover Plant".
g. Editing Plants IV - When running in SI Metric units and defining a hot water plant or chilled water plant with a primary/secondary distribution system, the secondary pump
design flow rate is incorrectly displayed on the Distribution tab. This value is automatically calculated from the equipment specified on the Schedule of Equipment tab. The
calculated value is correct and will be correctly used in calculations. The error is only in the screen display of the data. If you generate a plant input report you will see the
flow correctly displayed there.
h. Editing Plants V - When running in SI Metric units and defining a remote chilled water or remote hot water plant the secondary pump flow rate defined on the Distribution
tab is incorrectly saved. This will cause simulated pump input energy to be incorrect.
i. Air Systems – When a cooling-only air system was defined with dehumidification control and the dehumidification reheat source was defined as hot water or steam, HAP
failed to properly record the reheat source. This prevented linking the air system to a hot water plant or steam plant. As a result, energy costs for dehumidification reheat
could not be calculated in this case. This error was present in both v4.70 and earlier versions.
j. Editing Air Systems I – Under certain conditions, when adding spaces to zones in an air system, some of the items in the "selected spaces" box were shown as blank lines.
This was a display issue only. The selected spaces were properly saved and used in calculations.
k. Editing Air Systems II - For Rooftop, Vertical Packaged Unit and Split DX AHU VAV systems, if one of the temperature reset options was chosen for cooling capacity
control, the next time the system was edited, the program changed capacity control to "cycled or staged capacity, fan on". The original reset control was saved and used in
calculations. The problem only occurred if the system was later edited.
Page 11 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v4.7
1.0 Getting Started ›› 1.2 What's New in HAP? ››
l. Main Window - In certain situations the left-hand tree panel in HAP's main window became unresponsive. The program did not respond to clicking items in the left-hand
panel. This error only occurred on computers using two monitors in which specific configuration settings were used, and HAP was running on the secondary monitor rather
than the primary monitor. HAP should now run on all dual-monitor configurations. This error was present in both v4.70 and earlier versions.
m. Program Startup - When starting the program for the first time, the program would halt and display an error message "Run time error 372. Failed to load control
'RichTextBox' from 'RICHTX32.OCX". This error only occurred on certain configurations of Windows 7 and Windows 8 computers. This error was present in both v4.70 and
earlier versions.
n. Touch Screen Computers - When starting the program on a computer having touch screen capabilities the program would halt and display Windows operating system
message "Hourly Analysis Program has encountered a problem and needs to close". HAP is now compatible with desktop, laptop and tablet computers having touch
screen capabilities, as long as the computer is running a Windows operating system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v4.7
This topic describes new features in HAP v4.70. It is intended as reference information for v4.80 users interested in learning what feature updates were included in this previous
version. The topic is divided into two sections:
A. HAP v4.70 Summary List of Enhancements - Summarizes the key changes in each major section of v4.70.
B. HAP v4.70 Detailed List of Enhancements - Provides a complete description of changes in v4.70.
A. HAP v4.70 Summary List of Enhancements
This section summarizes enhancements in HAP v4.70. Further details on these enhancements are found in section B.
1. Plants
a. Expanded hot water plants to allow use of air-to-water and water-to-water heat pumps in addition to boilers.
b. Added changeover plants using air-to-water and water-to-water reversible chillers.
c. Added service hot water (SHW) plants with flexible options for modeling tankless or storage systems, passive, pumped or recirculating systems, use of boilers or heat
pumps as heat source, and pasteurization cycles.
d. Added option for changeover, hot water, steam or remote source plants serving combined space heating and SHW loads.
e. Added prioritization controls for plants serving combined space heating and SHW loads.
f. Added "generic" plant options for changeover and SHW plants for quick sizing calculations.
g. Updated plant sizing reports for changeover and SHW plants.
2. Chillers
a. Added air-to-water reversible chillers using scroll or screw compressors.
b. Added water-to-water reversible chillers using scroll or screw compressors.
c. Added air-to-water heat pumps using scroll or screw compressors.
d. Added water-to-water heat pumps using scroll or screw compressors.
e. Added "average operating loss" input item to account for input energy lost to the environment and therefore not rejected through the condenser.
f. Expanded outdoor air temperature limits for air-cooled chillers to 140 °F (60 °C) to support modeling of extreme operating conditions.
3. Air Systems
a. Expanded options for changeover control in 2-pipe chilled water air handler and 2-pipe fan coil systems.
b. Added option for calculating ventilation requirements per ASHRAE Standard 62.1-2010 ventilation rate procedure.
c. Added ability to automatically assign DX cooling, DX heat pump and combustion equipment efficiency based on ASHRAE Standard 90.1-2010 minimum efficiency
requirements.
d. Added ability to automatically calculate Standard 90.1 Appendix G baseline fan power allowance using ASHRAE Standard 90.1-2010.
e. Revised algorithm for deriving design input power from HSPF ratings for small air-source heat pumps.
4. Buildings
a. Revised the LEED EA Credit 1 reports to include an end use category for service hot water (SHW) when an SHW plant is modeled.
5. Spaces
a. Added ASHRAE Standard 62.1-2010 space usage options and defaulting for space ventilation requirements.
b. Made minor revision to search and replace option to improve usability.
6. Boilers
a. Revised feature for creating boilers directly from the Plant Properties window to simplify input and reduce data entry errors.
7. Schedules
a. Revised feature for creating schedules directly from the Air System Properties and Plant Properties windows to simplify input and reduce data entry errors.
8. Wizards
a. Added changeover plants using air-to-water or water-to-water reversible chillers.
b. Expanded hot water plant options to allow use of air-to-water or water-to-water heat pumps in addition to boilers.
c. Added ability to model service hot water (SHW) loads.
d. Added ability to specify geothermal, surface and well water sources for chiller plants.
e. Revised plant diagrams to display the new plant configurations.
f. Replaced the "Hydronic Fan Coil" equipment type with separate "4-Pipe Fan Coil" and "2-Pipe Fan Coil" options
g. Added changeover controls for 2-Pipe Fan Coil and Chilled Water AHU equipment types.
h. Revised default values for self-contained electric humidifiers.
i. Updated Energy Information Administration (EIA) default electric and gas prices to use the latest published data (2011 and 2010).
j. Removed the confirmation message that appears when pressing the Finish button to improve usability.
9. Other
a. Added ASHRAE Standard 62.1-2010 as a ventilation standard option in Project Preferences.
b. Added ASHRAE Standard 90.1-2010 as an energy standard option in Project Preferences
c. Updated the help system and Quick Reference Guide to document new features.
d. Automatically install project archive containing ASHRAE 90.1 default schedules.
e. Automatically install project archives containing ASHRAE 90.1-2007 template projects containing prescriptive envelope constructions and Appendix G baseline systems.
B. HAP v4.70 Detailed List of Enhancements
Page 12 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
This section provides details on the feature changes in HAP v4.70.
1. Plants
a. Hot Water Plants with Heat Pumps - Expanded hot water plants to allow use of air-to-water and water-to-water heat pumps, in addition to boilers. For retrofit applications,
heat pumps and boilers can also be used in parallel in the same plant.
An auxiliary source of heat can be defined for a plant, to be used in conditions when heat pump capacity or efficiency is insufficient. Boilers or remote sources can be used
for auxiliary purposes.
b. Changeover Plants - Added changeover plants using air-to-water and water-to-water reversible chillers.
Changeover plants provide chilled water when running in cooling mode and hot water when running in heating mode using a single set of reversible chillers. Based on the
total composite load profile from all cooling and heating coils linked to the plant, the chillers will switch between heating and cooling mode as needed. This type of reversible
equipment is most often used in moderate climates where energy efficiency measures may take precedence over small variations in occupant comfort.
Changeover plants support most configuration options available to chiller and hot water plants, including plant sequencing controls, leaving chilled and hot water
temperature reset controls, waterside economizers, and auxiliary heating.
Single or multiple reversible chillers can be configured in parallel. For water-to-water reversible chillers, a geothermal loop can be defined which acts as both a heat source
and a heat sink depending on plant operating mode.
A “generic” changeover plant has also been added which can be used solely for design sizing. This type of plant will accumulate both heating and cooling loads from all air
systems and determine the peak coincident loads in both operating modes.
c. Service Hot Water (SHW) Plants - Added service hot water (SHW) plant models. Modeling options support tankless systems and storage-tank based systems. HAP will
simulate the service hot water system in hour-by-hour fashion, modeling water usage and required energy consumption to meet required supply temperatures.
Service hot water modeling options are broken into three main categories of inputs: consumption, distribution, and storage.
Consumption inputs are used to define the hourly usage of service hot water, and can be specified either in terms of an absolute flow rate (gpm or L/s), in terms of
occupancy (volume per person per day), or directly in terms of peak daily energy use. A schedule can be selected which describes the daily consumption profile.
Distribution can be accomplished without a pump by relying on mains pressure, or with a dedicated pump. If a dedicated pump is used, it can be configured to run cycled
with the usage profile or in a continuous recirculation mode. The pump model accounts for piping losses and pumping efficiency.
If storage options are used, the simulation will model a storage tank whose temperature is held between minimum and design setpoints, including jacket losses. Optionally,
if required by local regulations, stored water pasteurization can be enabled which will model the increased energy consumption needed to heat the stored water for
sterilization purposes. Heating for pasteurization which exceeds the plant’s normal capacity is provided by an electric immersion heater.
d. Combined Space and SHW Plants, Prioritization Controls – Added options for plants serving both space heating and SHW loads. Hot water, steam, remote source and
changeover plants offer this option. Combined plants not sized to meet the combined space and SHW peak load can use prioritization controls. Prioritization whether
space or SHW loads have priority and can be controlled by time of day schedules or an outdoor air temperature threshold.
e. Generic Plants – Added "generic" plant options for changeover and SHW plants. The "generic changeover" plant option does not require detailed specification of
equipment components and controls. It provides a fast way to define and calculate peak loads for a plant. The "generic service hot water" only requires specification of the
SHW demand, distribution and storage characteristics, and allows a quick way to specify and calculate peak loads for this type of plant.
f. Plant Sizing Reports – Updated plant sizing reports for changeover and SHW plants. For changeover plants, the program determines the peak loads for both cooling and
heating mode. For SHW plants the program determines the peak service hot water load, and the peak pasteurization heating load, if applicable.
2. Chillers
a. Reversible Chillers – Added air-to-water and water-to-water reversible chillers. Reversible chillers produce chilled water to serve cooling loads when running in cooling
mode. The equipment can reverse cycle to supply hot water to serve heating loads when running in heating mode. Options are provided for modeling air-to-water
packaged scroll, water-to-water packaged scroll, and water-to-water packaged screw machines.
Input data includes design data (temperatures, capacities, input power, flow rates) for both cooling and heating mode, as well as separate performance maps for cooling
and heating duty. Default data representing typical part-load performance maps for each type of reversible chiller is supplied by the program.
b. Heat Pumps – Added air-to-water and water-to-water heat pumps. Options are provided for modeling air-to-water packaged scroll, water-to-water packaged scroll, and
water-to-water packaged screw machines.
Input data includes design data (temperatures, capacity, input power, flow rates) for heating duty, and a heating performance map. Default data representing typical part-
load performance for each type of heat pump is supplied by the program.
Because the existing chiller screen has been re-used for heat pumps, users familiar with the definition of cooling-only chillers should have only a small learning curve to take
advantage of the new equipment types.
c. Average Operating Loss – Added an input for “average operating loss” to account for energy lost by the chiller or heat pump to its local environment, rather than being
rejected at its condenser coil. This is an improvement in the accuracy of the chiller model in HAP. When energy loss occurs, it will lead to less work by heat rejection
equipment for cooling duty. It will also reduce heat pump capacity in heating applications.
d. Outdoor Air Temperature Limits – Expanded outdoor air temperature limits for chillers to 140 °F (60 °C) to support applications with more extreme operating conditions.
3. Air Systems
a. Changeover Control – Expanded options for changeover control in 2-pipe chilled water air handler and 2-pipe fan coil systems. Previous versions of HAP offered monthly
schedules to designate months in cooling mode or heating mode. These options have been expanded to include changeover based on outdoor air temperature, with a
temperature deadband and a minimum cycle time. In addition, when changeover control is based on monthly schedules, the program forces monthly schedules to be
mutually exclusive. That is, it checks schedules to make sure no month has both cooling and heating scheduled as available.
The new inputs for changeover control are found on the Equipment tab of the Air System Properties window. Please refer to the "Changeover Controller" topic in section
11.6 of the help system for a complete explanation of the new inputs.
b. ASHRAE Standard 62.1-2010 – Added an option for calculating air system ventilation airflow requirements per the ASHRAE Standard 62.1-2010 ventilation rate procedure.
This option is offered when ASHRAE Standard 62.1-2010 is selected on the Project Preferences screen as the ventilation standard for the project.
c. ASHRAE Standard 90.1-2010 – Added the ability to automatically assign DX cooling, DX heat pump and combustion heating equipment efficiency based on ASHRAE
Standard 90.1-2010 minimum equipment efficiency requirements. Based on equipment type and capacity, the program will assign the EER or SEER for DX cooling
equipment, the COP or HSPF for DX heat pump equipment or the combustion heating efficiency for gas, propane or oil furnace heaters.
In addition the program will perform the Appendix G baseline fan power allowance calculation per 90.1-2010 when the "App G Fan kW" option is selected for supply fan
performance.
These calculation options are enabled when ASHRAE Standard 90.1-2010 is specified on the Project Preferences screen as the energy standard for the project.
These options may have greatest use once LEED version 4 is released. LEED 2009 references ASHRAE Standard 90.1-2007, so 2007 should continue to be used as the
energy standard for HAP projects pursuing LEED 2009 certification.
d. HSPF Conversion Algorithm – Revised the algorithm for deriving design input power from HSPF ratings for small air-source heat pumps. To simulate air-to-air heat pump
operation HAP requires the compressor and outdoor fan kW at the heat pump design rating condition. Off-design and part-load correction factors are applied to the design
kW to determine input kW for each operating hour in the simulation. When HSPF is entered to define heat pump performance, HAP first derives an equivalent COP from
the HSPF and then derives compressor plus outdoor fan kW from the COP rating. The conversion from HSPF to COP is based on a correlation of data from manufacturer's
published ratings. Because HSPF and COP are poorly correlated, the original correlation had a slight downward slope so that as HSPF increased COP decreased. The
correlation has been improved so increasing HSPF yields increasing COP for better accuracy.
4. Buildings
a. LEED EA Credit 1 Report – Revised this report to include an end use category for service hot water when a service hot water (SHW) plant is defined. In prior versions of
HAP service hot water energy use was specified directly as a "miscellaneous energy use" item in Building inputs. HAP would then display this service hot water item as a
Page 13 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v4.6
1.0 Getting Started ›› 1.2 What's New in HAP? ››
separate end use in the LEED EA Credit 1 report tables. With the addition of SHW plant models in HAP v4.7, the EA Credit 1 report was revised to report heating energy
use for this SHW plant as a separate line item.
5. Spaces
a. ASHRAE Standard 62.1-2010 – Added ASHRAE Standard 62.1-2010 space usage options. When a space usage option is selected, the CFM/person and CFM/sqft
(L/s/person and L/s/sqm) ventilation requirements will be defaulted. These options appear when Standard 62.1-2010 is selected on the Project Preferences screen as the
ventilation standard for the project.
Standard 62.1-2010 added five new space usage categories, revised the ventilation requirements for four space usage categories, and eliminated two other categories.
These changes are reflected in the HAP data when Standard 62.1-2010 is specified.
b. Search and Replace – When exiting from the space global search and replace window, the OK button will always be enabled. Previously, if global changes had already
been executed, you were required to press the Cancel button to return to the main window. Many software users found this counterintuitive.
6. Boilers
a. Creating Data from Plants – The Plant Properties window offers a feature to let you create a new boiler without leaving the Plant window. Previously this feature did not
control the type of boiler created, so a steam boiler could be created for a hot water plant, or a hot water boiler could be created for a steam plant. HAP now controls the
boiler type so only hot water boilers can be created for hot water plants, and only steam boilers can be created for steam plants. This reduces data input errors.
7. Schedules
a. Creating Data from Air Systems or Plants – The Air System and Plant Properties windows offer a feature to let you create a new schedule without leaving the Air System
or Plant window. Previously this feature did not control the type of schedule created. For example, when creating a fan/thermostat schedule for an air system, a user could
inadvertently create a fractional schedule. This resulted in an input error. HAP now controls the type of schedule created so it always defaults to the required schedule
type. This reduces data input errors.
8. Wizards
a. Changeover Plants – Added ability to model changeover plants using air-to-water and water-to-water reversible chillers.
b. Hot Water Plants – Expanded hot water plant options to allow use of air-to-water and water-to-water heat pumps in addition to boilers.
c. Service Hot Water – Added the ability to model service hot water (SHW). Plants with SHW selected will serve both space heating loads and the specified SHW loads.
SHW is included in a plant on the Heating Plant Wizard screen. Press the Details button to display the Heating Plant Details screen where consumption, storage tank and
pasteurization cycle characteristics of the SHW system can be defined.
d. Chiller Plant Heat Rejection – Added the ability to specify a geothermal well field, surface water or well water as the sink for condenser heat rejection.
e. Plant Diagrams – Revised plant diagrams to display the new plant configurations including changeover plants, hot water plants using heat pumps and heating plants
including service hot water.
f. Hydronic Fan Coils – Replaced the "Hydronic Fan Coil" equipment type with separate options for "2-Pipe Fan Coil" and "4-Pipe Fan Coil" equipment.
g. Changeover Controls – Added changeover control options for 2-Pipe Fan Coil and Chilled Water AHU equipment types. Changeover can be controlled by scheduling
cooling and heating by month, or can be controlled by an outdoor air setpoint. These options appear on the Detailed System and Equipment input screen which is
displayed by pressing the Details button on the main System and Equipment wizard screen.
h. Electric Humidifiers – When a self-contained electric humidifier is specified, the equipment wizard will now default electric input kW for the equipment based on typical
values from manufacturer's ratings. Previously data was not defaulted and a user had to specify input kW in the HAP detailed interface.
i. EIA Prices – Updated Energy Information Administration (EIA) default prices for electricity and gas. EIA calculates and publishes average electricity and gas prices by US
state. This data can be selected from drop-down lists in the Utility Rate Wizard. Previously defaults were from 2009. HAP has been updated to use the latest published
EIA data. All electric data is for 2011. Gas data is a mix of 2011 and 2010 prices. The reference table of EIA prices in the HAP help system has also been updated with
this new data.
j. Confirmation Message – When clicking Finish to exit a Wizard, HAP previously displayed a message to explain how Wizard input data had been converted into detailed
HAP data. Software users commented this message was not necessary. In HAP v4.70 this message has been removed.
9. Other
a. Project Preferences – Added options to select ASHRAE Standard 62.1-2010 as the ventilation standard and to select ASHRAE 90.1-2010 as the energy standard for a
project. See section 3 (Air Systems) and section 5 (Spaces) for further information on how these standards are used in the program.
b. ASHRAE 90.1 Default Schedules – When HAP v4.7 is installed, a project archive containing default schedules from the ASHRAE 90.1 User's Manual is automatically
installed. Lighting, equipment, occupant and service hot water schedules for different building types are contained in the archive.
You can load and save this template project using the "Retrieve HAP v4.7 Data" option on the Project Menu. The archive is in the \E20-II Archives folder and the file name
is HAP47\_Schedules.E3A. Once the data is saved as a project, you can use the "Import Project Data" option on the Project Menu to import ASHRAE schedules into your
working projects.
c. ASHRAE 90.1-2007 Template Projects – When HAP v4.7 is installed, a series of project archive files containing data to assist with LEED 2009 projects is automatically
installed. There is one archive for each ASHRAE climate zone. The project archives contain wall, roof and window assemblies complying with ASHRAE Standard
90.1-2007 prescriptive requirements for a particular climate zone. The archives also contain air system templates for the Appendix G Performance Rating Method baseline
system types. The same baseline systems are provided in each climate zone.
To load one of these archives, use the "Retrieve HAP v4.7 Data" option on the Project Menu. The archives are placed in the \E20-II\Archives folder and have file names
such as HAP47-ASHRAE-90-1-2007-Zone-1.E3A.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
What was New in HAP v4.6
This topic describes new features in HAP v4.60 and v4.61, the two versions prior to HAP v4.70. It is intended as reference information for v4.70 users interested in learning what
feature updates were included in these previous versions. The topic is divided into five sections:
A. HAP v4.61 Overview - Provides a high level overview of the major changes in v4.61.
B. HAP v4.61 Detailed List of Enhancements - Provides a high level overview of the major changes in v4.61.
C. HAP v4.60 Overview - Provides a high level overview of the major changes in v4.60.
D. HAP v4.60 Summary List of Enhancements - Summarizes the key changes in each major section of v4.60.
E. HAP v4.60 Detailed List of Enhancements - Provides a complete description of changes in v4.60.
A. HAP v4.61 Overview
This section describes enhancements in HAP v4.61. HAP v4.61 includes changes in two areas:
1. User Interface Updates involving three minor changes related to lighting analysis, default schedules and air source heat pump humidity control (see B for details).
2. Bug Fixes. Nine problems identified in v4.60 were corrected (see B for details).
Page 14 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
B. HAP v4.61 Detailed List of Enhancements
This section provides details on the feature changes in HAP v4.61:
1. User Interface Updates. Three minor enhancements were made to the HAP user interface.
a. Lighting Analysis - Revised the limits for the lighting ballast multiplier to accept values from 0.1 to 2.0. Previously ballast multipliers below 1 could not be entered. This
change supports three lighting analysis tasks. The first is modeling of modern fluorescent lighting fixtures having ballast factors less than 1.0. The second is modeling
lighting retrofits of the ballast to more efficient (lower) levels. Using the global search and replace feature lighting fixtures in large groups of spaces can be modified to
reduce the ballast multiplier to levels below 1.0. Third, the ballast multiplier can be used as a short cut method of modeling lighting fixture wattage reduction, again using
the global search and replace feature.
b. Default Schedules - Updated the ASHRAE Default Schedules archive file to include typical schedules for elevators and service hot water demand. This archive file is
automatically installed with the program. To utilize data from this resource, first use the Project/Retrieve option. From the \E20-II\Archives folder select the archive file
named "HAP46\_Default\_Schedules\_and\_Utility\_Rates.E3A". After the data is retrieved, save the project. Subsequently in as you create new projects, use the
Project\Import HAP Project Data option to import schedules and utility rates into your project. The archive contains ASHRAE default schedules for occupants, lighting,
HVAC system, elevators and service hot water for Assembly, Healthcare, Hotel, Light Manufacturing, Office, Parking Garage, Restaurant, Retail, School, and Warehouse
space usage types.
c. Air Source Heat Pumps with Humidity Control - For rooftop heat pumps and split DX AHU heat pumps which use a humidistat to control humidity, the auxiliary heater
provides dehumidification reheat. The maximum limit for the auxiliary heat upper cutoff OADB was increased from 80 F to 130 F (26.6 C to 54.4 C) so systems can be
configured to provide dehumidification reheat at high outdoor air dry-bulb conditions.
2. Bug Fixes - Problems identified in HAP v4.60 were corrected.
a. Editing Data - In certain situations when editing and then saving a Schedule, Wall, Roof, Window, Door or External Shade Geometry an "Error 3360 - Query is too complex"
error occurred and prevented saving of the data. This error only occurred when the item was linked to more than 265 spaces. For example, a schedule that was linked to
300 spaces would trigger the error.
b. Equipment Wizard - When creating a VRF scenario with the Equipment Wizard in which the "one VRF system per floor" configuration was selected, the program incorrectly
created one VRF system for the building rather than floor-by-floor systems.
c. Weather Wizard - On computers using non-English versions of Windows, such as French Windows or Spanish Windows, an "Error 3061" error occurred when launching
the Weather Wizard. This error prevented use of the Weather Wizard.
d. Importing Weather Files - On computers using certain "Regional and Language Option" settings, importing simulation weather from an external file failed. One example is
Regional and Language Options set to "Spanish [Spain]".
e. Calculating Air Systems - In certain situations while running air system design calculations or air system simulations an "error occurred while loading air system" error
message appeared. This error prevented completion of the calculations and display of output reports for the air system.
f. WSHP and W/C VPAC Simulations - The following problems existed with simulation results for water-cooled VPAC and WSHP systems. To generate correct results in
HAP v4.61, please open and save the air system and then rerun the simulation.
i. For W/C VPAC and WSHP systems using a cooling tower for heat rejection, the cooling tower fan kWh was omitted from results (zero kWh was reported).
ii. For W/C VPAC, WSHP and W/C Chiller Plants usinig a dry cooler for heat rejection, the dry cooler fan kWh was incorrect.
iii. For W/C VPAC systems using a cooling tower or dry cooler for heat rejection, cooling compressor kWh was incorrect. It tended to be overstated for cooling towers and
understated for dry coolers.
iv. For WSHP systems using a dry cooler for heat rejection, cooling compressor kWh was incorrect and tended to be understated.
g. 2-Speed Fan Control. For systems using 2-speed supply fan control, if the low speed airflow was set to a value of 73% or higher, cooling compressor energy use was
reported as zero.
h. Air-Cooled Chiller DX Free Cooling - When the DX Free Cooling feature for air-cooled chillers was used, the simulation algorithm did not cycle the refrigerant pump and
condenser fans to match the chiller load. As a result, chiller energy use for DX Free Cooling hours was overstated. In DX Free Cooling mode the chiller's compressors are
turned off and a small refrigerant pump circulates refrigerant between the evaporator and condenser. The temperature difference between evaporator and condenser drives
the refrigerating effect. The refrigerant pump and condenser fans should cycle to match cooling output with chiller load.
i. Boiler Plant Sizing - When a very specific sequence of steps was used to create and then modify a hot water or steam boiler plant, an error occurred which resulted in the
plant peak heating loading being set to zero. This also resulted in an "Error 6 - Overflow" error during plant simulation calculations. The sequence of steps required to
trigger this error involved creating a DX fan coil system with electric heat in the Equipment Wizard and then later revising the system in the HAP main window to switch to
hot water or steam heat.
C. HAP v4.60 Overview
This topic describes enhancements in HAP v4.60. Major enhancements in v4.60 relate two major themes
1. Theme 1 - Expanded Equipment Modeling Capabilities. Responses to the summer 2011 customer survey indicated a high level of interest in expanding capabilities for
modeling HVAC equipment and controls. HAP v4.60 represents the first installment in satisfying these requests by adding models for:
a. Variable Refrigerant Flow (VRF) equipment.
b. Two-speed fan control for single-zone CAV packaged and split DX equipment.
c. Two-state compression in single-zone CAV packaged and split DX equipment.
d. Multiple boilers, boiler sequencing controls and hot water reset controls for boiler plants.
e. Condensing and non-condensing boilers.
f. Variable speed / variable flow condenser pumps and dry coolers for chiller plants.
In addition, existing simulation models were upgraded for all air-cooled DX cooling equipment types and all air source heat pump heating equipment types.
2. Theme 2 - Expanded Productivity Features. HAP v4.60 also contains new productivity features, including the ability to:
a. Merge multiple projects into one large project, to facilitate more efficient collaboration in project teams.
b. Preserve space and zone assignments when changing system type for an existing air system.
c. Import simulation weather data from external file formats such as EnergyPlus EPW, ASHRAE IWEC, ASHRAE IWEC2, NOAA TMY2 and NOAA TMY3.
D. HAP v4.60 Summary List of Enhancements
A complete summary list of enhancements in HAP v4.60 is provided below. More detailed explanations are found in section C.
1. Main Window
a. Expanded "project import" feature to allow full merging of projects.
2. Weather
a. Added feature to import simulation weather data from external sources such as EnergyPlus (EPW), ASHRAE IWEC, ASHRAE IWEC2, NOAA TMY2 and NOAA TMY3
formatted files.
Page 15 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
3. Air Systems
a. Added Variable Refrigerant Flow (VRF) equipment models.
b. Upgraded air-cooled DX cooling models for all applicable equipment types
c. Upgraded air source heat pump (ASHP) models for all applicable equipment types.
d, Added 2-speed supply fan control for single-zone CAV rooftop, split DX AHU, and packaged vertical unit equipment.
e. Added 2-stage compression for single zone CAV rooftop, split DX AHU, and packaged vertical unit cooling equipment.
f. Added feature to specify upper cutoff temperature for ASHP auxiliary heat.
g. Added condenser pump inputs (formerly in cooling towers) for WSHP, GWSHP, GSHP and water-cooled vertical packaged unit equipment.
h. Space and zone assignments are now preserved when system type is changed.
i. Removed "constant temperature, fan cycled", "reset based on greatest zone demand", and "reset based on OAT schedule" capacity control options for single-zone CAV
rooftop, split DX AHU and vertical packaged unit equipment.
j. Expanded input formats to allow input power for small wattage fans and compressors to be specified more accurately.
4. Plants
a. Added multiple boilers, sequencing control and hot water reset control to boiler plants.
b. Added variable speed / variable flow condenser water pump control and dry coolers for chiller plants.
c. Added condenser pump inputs (formerly in cooling towers) for chiller plants.
5. Cooling Towers
a. Added dry cooler model.
b. Moved condenser pump performance inputs to plants and air systems.
6. Boilers
a. Added models for condensing and non-condensing boilers.
7. Wizards
a. Added option for Variable Refrigerant Flow (VRF) equipment.
b. Added 2-speed fan control for single-zone CAV rooftop, split DX AHU and vertical packaged unit equipment.
c. Added 2-stage compression for single-zone CAV rooftop, split DX AHU and vertical packaged unit equipment.
d. Added options for variable speed condenser pumps and dry coolers in chiller plants.
e. Added options for multiple boilers, sequencing control and hot water reset control in boiler plants.
f. Added options for condensing and non-condensing boilers in boiler plants.
g. Added options to select Energy Information Administration (EIA) electricity and gas prices for US states in the Utility Rate Wizard.
8. Bug Fixes
a. Corrected problems identified in HAP v4.51.
E. HAP v4.60 Detailed List of Enhancements
This section provides details on the feature changes in HAP v4.60.
1. Main Program Window
a. Merging Projects - The "Import Project Data" option on the Project Menu was expanded to handle space, air system, plant and building data. Previously the option only
allowed the lower level project elements - weather, schedules, walls, roofs, windows, doors, external shade geometries, chillers, cooling towers, boilers, electric rates and
fuel rates - to be imported from one project into another. By including all sixteen categories of HAP project data in the feature, users can effectively merge complete
projects together. This is often useful in large projects where individual team members initially model portions of the building separately and then combine the data for final
energy modeling calculations.
Note that when importing space, air system, plant or building data from one project into another, HAP automatically imports all linked items. For example, if you import 10
spaces, HAP will identify all of the wall, roof, window and door assemblies linked to the spaces, plus the linked schedules and shade geometries and import those
automatically with the spaces.
2. Weather
a. Importing Simulation Weather Files - An "Import Weather File" option was added to the Simulation tab of the Weather Properties window to allow simulation weather data
from an external source to be imported into your project. Previously the only source for simulation weather data was the Carrier library of 500+ city files. In recent years the
availability of 8,760-hour simulation weather files has grown dramatically. While Carrier will continue expanding and updating it's library of pre-processed, quality inspected
weather files, it is important for users have the ability to access weather from other sources as soon as it is published. This new "Import" option can translate files in
commonly used formats: EnergyPlus EPW, ASHRAE IWEC (International Weather for Energy Calculations), ASHRAE IWEC2 (IWEC version 2), NOAA TMY2 and NOAA
TMY3..
Note that simulation weather files from external sources sometimes contain bad data points. Bad data points are temperature, humidity or solar values far larger or smaller
than should occur for a given location at a given time, and are usually due to weather station equipment malfunctions or data processing errors. After using the "Import
Weather File" option we recommend reviewing the simulation weather reports to determine if the data is reliable for use in your simulations. HAP displays a message after
the data is imported with recommended procedures for verifying the quality of the data.
3. Air Systems
a. Variable Refrigerant Flow (VRF) Equipment Models - Added air-side and equipment models for VRF equipment. Cooling-only, cooling with electric heat, and heat pump
system configurations are offered, with digital scroll or variable speed scroll condensing unit options.
b. Upgraded Air-Cooled DX Cooling, ASHP Equipment Models - Equipment simulation models which calculate the off-design and part-load performance of air-cooled DX
equipment and air source heat pump equipment were upgraded. Previous versions of HAP use 2-dimensional models which calculate changes in equipment capacity and
efficiency as a function of outdoor air dry-bulb temperature and part-load ratio. These algorithms were upgraded with a 4-dimensional model based on correlations of
performance data for current DX equipment. For cooling equipment, the new model considers changes in capacity and efficiency as a function of outdoor air dry-bulb
temperature, entering coil wet-bulb temperature, airflow and part-load ratio. For heat pump heating equipment the model considers performance as a function of outdoor air
dry-bulb temperature, entering coil dry-bulb temperature, airflow and part-load ratio. Both old and new models include considerations for defrost cycles below 40 F (4.4 C)
OADB.
c. 2-Speed Fan Model - A model for 2-speed indoor fan control was added to single zone CAV rooftop, split DX AHU and vertical packaged unit systems. Indoor fan speed
control is specified in the supply fan section of air system inputs. Three options are offered: "1-speed fan, cooling and heating", "2-speed fan cooling, 1-speed fan heating",
"2-speed fan, cooling and heating".
Page 16 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
d. 2-Stage Compression Model - A model for 2-stage compression was added for single-zone CAV rooftop, split DX AHU and vertical packaged unit cooling equipment. In
the cooling equipment performance inputs users can now choose between "1-stage compression, single circuit" and "2-stage compression, separate circuits" options. The
1-stage option models single stage on/off cycling of the compressor. The 2-stage option models two stages of capacity, and cycles between high stage, low stage and off.
e. ASHP Auxiliary Heat Cutoff Temperature - Added an input for the upper cutoff temperature for air source heat pump auxiliary heat. This was primarily added to help
users comply with LEED® project requirements - that in a baseline ASHP system auxiliary heat shall not operate above 40 F (4.4 C) OADB. While it is rare for auxiliary
heat to run above 40 F OADB in a LEED baseline simulation due to the 25% heating capacity oversizing rule, it was time consuming for engineers to prove this in LEED
submissions. This new input provides a simple way for users to document that HAP explicitly prevents auxiliary heat running above a specified cutoff point.
f. Condenser Pump Performance Inputs - Condenser pump performance inputs were moved from Cooling Tower Properties to the Air System Properties. These inputs only
appear for WSHP, GWSHP, GSHP and water-cooled vertical packaged unit equipment, on the Miscellaneous Components window under the Equipment tab.
g. Preserving Space and Zone Assignments - HAP was revised to preserve space and zone assignments when system type is changed. This feature is useful when
copying and editing systems, an especially frequent task in LEED projects. Previously, changing the system type in an existing system reset all of the space and zone
assignments and required the user to re-specify this data. In HAP v4.60 this is no longer necessary. Note that when changing from a multiple zone system to a "CAV -
Single-Zone" or to a "Tempering Ventilation" system, only space assignments for the first zone can be preserved since both system types are limited to having only one
zone.
h. Obsolete Capacity Control Options - The following three capacity control options were removed for single-zone CAV rooftop, split DX AHU and vertical packaged unit
equipment: "constant temperature, fan cycled", "reset based on greatest zone demand", "reset based on OAT schedule". "Constant temperature, fan cycled" was removed
because modern equipment typically runs fan-on during occupied hours to comply with ventilation requirements. The latter two control options apply to single-zone CAV
chilled water AHU equipment and are not used for DX equipment. When converting existing v4.5 projects to v4.6 format, the converter automatically changes capacity
control to "cycled or staged compressor, fan on" if any of these obsolete options were used for these equipment types.
i. Expanded Input Formats for Small Wattage Equipment - Input data formats for fan motor and compressor motor power inputs were expanded to allow more complete
specification of power for smaller wattage equipment. For example, fan motor input kW for a fan powered mixing box terminal was formerly limited to one decimal place. A
245 watt motor would have to be defined as 0.2 or 0.3 kW, leaving a margin of error versus the actual motor power. In HAP v4.60, the motor can be specified as 0.245 kW
to eliminate this margin of error.
LEED® is a registered trademark of the United States Green Building Council
4. Plants
a. Expanded Boiler Plant Models - Boiler plant models were expanded to allow multiple boilers, sequencing control and hot water reset controls. Hot water and steam boiler
plants can now contain up to 12 boilers connected in parallel. Boilers can be equally unloaded or sequenced on load. For hot water boiler plants, hot water supply
temperature can be controlled as a fixed temperature, reset according to return water temperature or reset according to an outdoor air temperature schedule.
b. Expanded Chiller Plant Models - Chiller plant models were expanded to allow variable speed / variable flow condenser water systems and to allow use of dry coolers for
heat rejection.
c. Condenser Pump Performance Inputs - Because of the addition of variable speed / variable flow condenser water systems (above), condenser pump performance inputs
were moved from Cooling Tower Properties to Plant Properties. These inputs appear on a new Condenser Water tab in the Plant Properties window.
5. Cooling Towers
a. Dry Coolers. Features for modeling dry cooler equipment were added. This equipment uses a water-to-air heat exchanger to reject heat by sensible heat transfer.
b. Condenser Pump Performance Inputs. Condenser pump performance inputs were removed from the Cooling Tower Properties window. For heat rejection equipment
used with chiller plants, condenser pump performance inputs were moved to the plant input data. For heat rejection equipment used with water source heat pump systems
or water-cooled vertical packaged unit systems, the condenser pump performance inputs were moved to the air system input data. When converting existing v4.5 projects
to v4.6 format, the converter automatically moves condenser pump performance data to the proper new location.
6. Boilers
a. Expanded Boiler Models. Two new modeling options were added for condensing and non-condensing boiler equipment. The names of the modeling options were also
changed to better communicate the differences between the models. The full set of four model options offered in HAP v4.60 is:
> Constant Efficiency - A simple model in which a single efficiency value is used for all operating conditions.
> User Defined Curve - A simple 1-dimensional model in which the user defines boiler efficiency as a function of part-load ratio.
> (NEW) Condensing Boiler - A 2-dimensional model in which a correlation of condensing boiler equipment performance calculates boiler efficiency as a function of part-
load ratio and hot water supply temperature.
> (NEW) Non-Condensing Boiler - A 2-dimensional model in which a correlation of non-condensing boiler equipment performance calculates boiler efficiency as a function
of part-load ratio and hot water supply temperature.
7. Wizards
1. Equipment Wizard Upgrades - The equipment wizard was updated to offer the new modeling features added in the main HAP input screens:
> Variable Refrigerant Flow (VRF) equipment.
> 2-speed fan control for single-zone CAV rooftop, split DX AHU and vertical packaged unit equipment.
> 2-stage compression for single-zone CAV rooftop, split DX AHU and vertical packaged unit cooling equipment
> Variable speed condenser pumps and dry coolers in chiller plants.
> Multiple boilers, sequencing control and hot water reset control in boiler plants.
> Condensing and non-condensing boilers.
2. Utility Rate Wizard Upgrades - Added options to select Energy Information Administration (EIA) electricity and gas prices for US states. The EIA is an agency of the US
government which compiles and publishes average utility prices by state. EIA state average prices are often used for LEED energy modeling projects. Previously a user
had to look these prices up in the HAP help system and manually enter them in the utility rate wizard screen. In HAP v4.60, a user can now select the rates from a drop
down list, to automatically insert the prices in the input screen. This feature uses the latest EIA published data which is for 2009. For projects outside the US, electric and
gas prices can still be directly defined..
8. Bug Fixes
a. Zone Heating Units. In certain situations problems occurred saving fan performance data for zone heating units of type "Fan Coil, Room Tstat Control" and "Fan Coil, OAT
Control" when performance was defined as total static pressure.
b. LEED Summary Report - In certain situations the LEED Summary report showed zero energy cost data for a Baseline or Proposed building. If the report was immediately
re-generated all the data appeared correctly.
c. Project Management. In certain situations input and calculation data for air systems, plants and buildings was retained in a project after the system, plant or building was
deleted. This unnecessarily increased the footprint of the project folder on your hard disk or network server. It also resulted in project archive files being larger than
necessary.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 17 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
What was New in HAP v4.5
1.0 Getting Started ›› 1.2 What's New in HAP? ››
What was New in HAP v4.5
This topic describes new features in HAP v4.50 and v4.51, the two versions prior to HAP v4.60. It is intended as reference information for v4.60 users interested in learning what
feature updates were included in these previous versions. The topic is divided into five sections:
A. HAP v4.51 Overview - Provides a high level overview of the major changes in v4.51.
B. HAP v4.51 Detailed List of Enhancements - Provides a high level overview of the major changes in v4.51.
C. HAP v4.50 Overview - Provides a high level overview of the major changes in v4.50.
D. HAP v4.50 Summary List of Enhancements - Summarizes the key changes in each major section of v4.50.
E. HAP v4.50 Detailed List of Enhancements - Provides a complete description of changes in v4.50.
A. HAP v4.51 Overview
This topic describes enhancements in HAP v4.51. HAP v4.51 includes changes in four areas:
1. Streamlining Report Generation. The report generating software in HAP has been revised to bundle reports as a single document file.
2. Adjusting LEED Summary Report Format and Conventions. The format of the LEED 2009 EAc1 Summary Report was revised to match the most recent layout of the
LEED 2009 EAp2 online template. Procedures for compiling LEED unmet load hours were revised.
3. Bug Fixes - Problems identified in HAP v4.50 were corrected.
4. Miscellaneous - Minor adjustments were made to program input limits and program documentation..
B. HAP v4.51 Detailed List of Enhancements
This section provides details on the feature changes in HAP v4.51:
1. Streamlining Report Generation. The report generating software in HAP has been revised to bundle reports as a single document file.
In HAP v4.50 and prior versions, for example, if you selected three air system and requested 5 different system design reports, HAP would generate 15 report documents (3
systems x 5 reports), one for each individual report requested. This did not pose any problems if you were only viewing reports. But if the reports were printed, they would
print as 15 separate print jobs. If saving to disk, the reports had to be saved individually as 15 Word RTF documents. If printing using a PDF converter, 15 separate PDFs
would be generated. For many applications this was inconvenient for users.
For the same scenario in HAP v4.51, the program will generate one report document containing all 15 reports. If you print the report, it prints as one print job. If you save to
disk, it saves as one large Word RTF document. If you print using a PDF converter, it generates a single PDF document.
Note that this changes how you work with reports in the Report Viewer. Previously you used the Next and Previous buttons to advance forward or backward through the
individual report documents. Now, since there is a single large document, you use the scroll bar and [PgDn], [PgUp] to scroll through all the pages in the bundled report.
This change applies to all categories of reports generated by HAP.
2. Adjusting LEED Summary Report Format and Conventions. The following changes have been made to the LEED Summary Report.
a. Format and Process Energy - The format of the LEED 2009 Summary report in HAP v4.50 was based on the format of the LEED 2009 EAp2 online template as of Fall
2009. The format of the EAp2 template has changed since that date. In Fall 2009, the EAp2 template specified process energy must be at least 25% of proposed building
energy use. Subsequently the template was revised to require process energy cost to be at least 25% of baseline building energy cost. The format of the LEED 2009
Summary report has been revised to report data according to the latter requirement.
b. LEED Unmet Load Hours - Three adjustments were made to the scheme for compiling LEED unmet load hours.
First, the tolerance for zone temperatures out of range was adjusted from 0.1 F to 1.0 F.
Second, Tempering Ventilation systems, which do not control room temperature, will no longer report temperature hours out of range.
Third, zone temperatures out of range will not be reported for occupied hours when cooling or heating is not available - either because cooling is not selected, heating is not
selected for a system, or because a coil is scheduled off. For example, a heating-only system previously reported hours out of range when room temperatures were hot,
even though the system had no cooling capability.
Hours when zone temperature is out of range contribute to the Unmet Load Hours shown on the LEED EAc1 Summary Report. These changes will reduce the quantity of
Unmet Load Hours by removing hours that should not be counted. Note however that most LEED applications require both cooling and heating to be modeled so cooling-
only, heating-only and systems with cooling or heating scheduled off during certain times of year should typically not be used in a LEED EAc1 analysis.
3. Bug Fixes - Problems identified in HAP v4.50 were corrected.
a. Weather Wizard. For certain cities selected in the Weather Wizard, the program asked the user to specify the location of the simulation weather data file. The program
should automatically locate the file itself. The cities include those in North Carolina, North Dakota, Sacramento, CA, Winnipeg, MB and Kuwait City, Kuwait.
b. Building Wizard - I. Corrections were made to the wall and roof assemblies generated by the Building Wizard. The medium weight roof contained an incorrect layer.
Certain inside and outside surface resistances were also adjusted.
c. Building Wizard - II. The U-value and shade coefficient data for the Standard and High Performance window options were revised to be more in line with current window
products.
d. Time Zone Data. Time zone data was incorrect for cities in Libya and Oman.
e. Simulation Failure. When running simulations for certain air system configurations, the simulation would fail with an "Error 6, overflow in cAirSysAnnual.DXEquipCalcs"
error message. This happened most frequently with VVT air systems, but could occur with other system types too.
f. User-Defined Sizing. For a terminal type system (fan coils, WSHPs), the zone ventilation airflow input on the Sizing tab, Zone Sizing data view would not permit zero
ventilation airflow to be entered.
g. LEED Unmet Load Hours - I. The LEED Summary Report included unmet load hours compiled for Tempering Ventilation systems. Because these systems do not control
space temperature, zone temperature out of range statistics should not be compiled.
h. LEED Unmet Load Hours - II. The LEED Summary Report included unmet load hours compiled for hours when a system had cooling or heating scheduled off. Zone
temperature out of range statistics should only be compiled when for times when the system is controlling room temperature. For example, a heating-only system reported
many zone temperature out of range hours for times when the room temperature was hot, even though the system did not include cooling capability. Note however that
most LEED applications require cooling and heating to be modeled, even if the actual design does not include that capability. Therefore cooling-only and heating-only
systems, and scheduling of coils typically should not be used in LEED EAc1 analyses.
i. LEED Summary Report. When two or more miscellaneous energy use items in a building had the same name, the energy cost tables in the LEED Summary report omitted
data for one of the energy use items for the Proposed building. For example, if two items were named "Tankless Water Heater", the proposed building data would only
report energy use and cost for one of the items.
j. Converting Data from Old Projects. When using the "Convert HAP v4.x Data" option on the Project Menu to convert an "active" project where the active project contained
data for HAP plus other eDesign or E-CAT programs, the data conversion sometimes failed with an "Error 42510".
4. Miscellaneous
a. Input Limits - Minor adjustments were made to input limits for soil conductivity, cooling EER and ambient cut-off temperature for air-cooled DX equipment.
Page 18 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
b. Program Documentation - Minor additions and corrections were made to the program help system. These involved topics dealing with outdoor ventilation airflow
calculations, derivation of DX unit compressor power from standard EER and COP ratings, translation of data from older HAP versions and project data management.
C. HAP v4.50 Overview
Major enhancements made in v4.50 relate to two major themes:
1. Theme 1 - Making HAP Easier to use for LEED Analysis. : Building upon features first introduced in v4.40, HAP v4.50 includes further modifications designed to make you
more productive in LEED projects. This applies both to existing projects registered under LEED NC-2.2 and new projects registering under LEED 2009. Specific modifications
include:
a. Project Preferences - Expanded of the Project Preferences feature to allow you to specify the Energy Standard (ASHRAE 90.1-2004 or 90.1-2007) and the LEED Rating
System (NC-2.2 or 2009) which applies to the current project. HAP automatically adapts its calculations and report formats to your specified preferences. Specifically, the
90.1 preference affects Appendix G baseline fan power allowance calculations and the defaulting of ASHRAE 90.1 minimum equipment efficiencies. The LEED preference
affects the formatting of the LEED Summary Report.
b. Equipment Efficiencies - Added a feature to default ASHRAE 90.1 minimum equipment efficiencies based on your ASHRAE 90.1 project preference (2004 or 2007).
Currently this feature applies to DX cooling, heat pump heating and furnace heater equipment.
c. Baseline Fan Power - Added features for automatically calculating the baseline fan power allowance per ASHRAE Standard 90.1-2007.
d. LEED Summary Report - Revised this report to adjust its format and content based on your stated project preference for the LEED Rating System - either LEED NC-2.2 or
LEED 2009.
e. LEED Style Unmet Loads - Revised calculations to comply with the new definition of "unmet loads" in ASHRAE Standard 90.1-2007.
f. SEER and HSPF - Added features to allow equipment performance to be defined in terms of SEER and HSPF.
2. Theme 2 - Expanding Features for Preliminary or Schematic Design. : Also building upon features introduced in v4.40, HAP v4.50 expands features for quickly and
efficiently performing schematic design analyses. Specific enhancements include:
a. Full Wizard Session - Expanded the Full Wizard Session feature to include Wizards for quickly defining weather data and utility rates. With the expanded Full Wizard
feature, you can quickly configure 100% of the data needed for a schematic analysis in a matter of minutes.
b. Wizards Menu - Expanded the Wizards Menu to include options for running the new Weather and Utility Rate wizards individually as a means of quickly adding data to an
existing HAP project.
c. Weather Wizard - This new wizard allows weather data to be quickly selected by one of two approaches - graphically by clicking on countries, states/provinces and cities in
map images, or by selecting from drop-down lists.
d. Utility Rate Wizard - This new wizard makes entry of electric and fuel pricing data vastly easier. Simple pricing data for electricity and fuels can be defined all on one
screen. For detailed electric rates, the wizard guides you through the rate definition, eliminating much of the uncertainty that can occur when using the traditional HAP input
screens.
D. HAP v4.50 Summary List of Enhancements
A summary list of enhancements in HAP v4.50 is provided below. More detailed explanations are found in subsequent topics and via the hot links below.
1. Main Window
a. Expanded Project Preferences to include Energy Standard (90.1-2004 or 2007), LEED (NC-2.2 or 2009) and currency.
b. Upgraded "gbXML Import" feature to more efficiently work with files from AutoDesk Revit 2010 and eliminate import failures previously seen when importing gbXML from
this source..
c. Expanded Help Menu to include User's Manual and links to web-based support and training information.
d. Converted program to use HTML-help format for better compatibility with Windows 7 and Windows Vista.
e. Added "What's New" pop-up window which appears at program start-up.
f. Revised report "save as RTF" feature to remember the destination folder you specify.
g. Added a template project which contains ASHRAE 90.1 default schedules and current EIA commercial sector average electric and gas prices for all 50 US states and the
District of Columbia.
2. Wizards
a. Expanded Full Wizard Session to include Weather and Utility Rate Wizards.
b. Expanded Wizards Menu to include Weather and Utility Rate Wizards.
c. Added new Weather Wizard for rapid specification of weather data.
d. Added new Utility Rate Wizard to simplify specification of energy and fuel price data.
3. Weather
a. HAP v4.50 automatically installs the full simulation weather library, eliminating the need to manually copy files.
4. Air Systems
a. Added feature to automatically ASHRAE 90.1 minimum efficiencies for DX and combustion heating equipment.
b. Added ability to specify and calculate baseline fan power allowance per ASHRAE 90.1-2007.
c. Added feature for defining equipment performance in terms of SEER and HSPF.
d. Revised air system defaults to better match commonly used DX equipment settings and heating SATs.
e. Revised terminology for coil capacity control options to make them easier to understand.
5. Plants
a. Revised input screen validation procedures to make it easier to define chilled water plants.
b. Revised the algorithm for DX free cooling in air-cooled chillers.
6. Buildings
a. Revised LEED Summary Report to display in LEED NC-2.2 or LEED 2009 format based on your project preference.
b. Revised calculation of LEED unmet cooling and heating loads to comply with definitions in ASHRAE 90.1-2007.
7. Cooling Towers
a. Changed "River, Sea or Well Water" option to "Geo, Well or Surface Water" to make its use clearer.
8. Utility Rates
a. Made currency a project-level preference so it only has to be defined once per project.
b. Revised emission analysis feature to consider only CO2e (CO2 equivalent).
9. Documentation
a. Updated help system and Quick Reference Guide to document new features.
10. Bug Fixes
a. Corrected a number of problems identified in HAP v4.41.
Page 19 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
E. HAP v4.50 Detailed List of Enhancements
This section provides details on the feature changes in HAP v4.50.
1. Main Program Window
a. Project Preferences - Expanded of the Project Preferences feature to allow you to specify the Energy Standard (ASHRAE 90.1-2004 or 90.1-2007) and the LEED Rating
System (NC-2.2 or 2009) which applies to the current project. HAP automatically adapts its calculations and report formats to your specified preferences. Specifically, the
90.1 preference affects Appendix G baseline fan power allowance calculations and the assignment of ASHRAE 90.1 minimum equipment efficiencies. The LEED preference
affects the formatting of the LEED Summary report. Read More.
b. gbXML Import. Upgraded the "gbXML Import" feature to more efficiently work with gbXML formatting conventions in files generated by AutoDesk Revit Mechanical 2010.
c. Help Menu. Expanded Help Menu to include a link to the User's Manual, support contact information, and web links to eDesign support, eDesign software, eDesign training
and Carrier commercial equipment web sites.
d. On-Line Help. Updated use HTML-help format to ensure compatibility with Windows 7 and Windows Vista, thereby eliminating the need for the special Microsoft patch file
to make the WinHelp4-format online help system work.
e. What's New. Added a "What's New" pop-up window which appears at program start-up and explains the new features of this version. This feature can be turned off once it
is no longer needed by checking a "do not show again" box.
f. Save as RTF. Revised reporting features so the "Save as RTF" feature remembers any changes you make to the destination path for saving report. Any change you make
to the path during a HAP session will remain in effect throughout that session. You can save reports to the same custom folder over and over without having to respecify the
destination path for each report.
g. Template Project. When you install HAP, an archive file named HAP45\_Schedules\_and\_Utility\_Rates.E3A is installed in the \E20-II\Archives folder. This archive is a
template project which contains ASHRAE 90.1 default schedules and the current Energy Information Agency (EIA) commercial sector average electric and natural gas
prices for all 50 US states and the District of Columbia. To use this data, retrieve this archive into a new project and save. Then use the Import Data from Project option to
import schedules and utility rates from the template project into other projects you create.
2. Wizards
a. Full Wizard Session - Expanded the Full Wizard Session feature to include Wizards for quickly defining weather data and utility rates. With the expanded set of wizards,
you can configure 100% of the data needed for a schematic analysis in a matter of minutes.
b. Wizards Menu - Expanded the Wizards Menu. The updated menu includes options for running Weather, Building, Equipment or Utility Rate wizards individually as a means
of quickly adding data to an existing project. The menu also includes an option for launching a Full Wizard Session which integrates all four wizards together and allows a
complete analysis to be configured in minutes.
c. Weather Wizard - This new wizard allows weather data to be quickly selected by one of two approaches - graphically by clicking on countries, states/provinces and cities in
map images, or by selecting from drop-down lists.
d. Utility Rate Wizard - This new wizard makes entry of electric and fuel pricing data vastly easier. Simple pricing data for electricity and all applicable fuels can be defined on
one input screen. For defining more detailed electric rates the wizard guides you through the process, eliminating much of the uncertainty that can exist when using the
traditional HAP input screens for utility rates.
3. Air Systems
a. Equipment Efficiencies - Added a feature to automatically determine ASHRAE 90.1 minimum equipment efficiencies based on your ASHRAE 90.1 project preference
(2004 or 2007). This feature applies to DX cooling equipment, heat pumps and furnace heaters.
b. Baseline Fan Power - Added features for automatically calculating the baseline fan power allowance for the procedures mandated in ASHRAE Standard 90.1-2007. This
involves additions to the air system inputs to allow specification of fan power allowance adjustment data, and changes to the calculation algorithms.
c. SEER and HSPF - Added features to allow air-cooled DX equipment performance to be defined in terms of SEER for cooling and HSPF for heating. For certain types of
small tonnage equipment, ASHRAE 90.1 minimum efficiency requirements and manufacturers ratings are in these units. As with the existing features for inputting AHRI
standard ratings of EER and COP, the program will automatically convert SEER and HSPF ratings to equivalent compressor and outdoor fan kW during calculations.
d. Capacity Control. Revised coil capacity control option names to make them more understandable. "Cycled or Staged Compressor, Fan On" was changed to "Cycled or
Staged Capacity, Fan On".
e. Defaults. Revised the air system defaults to set low ambient control on and to adjust default minimum OADB settings for air-cooled DX cooling equipment, and to change
default heating supply temperatures from 110 F (43.3 C) to 95 F (35 C).
4. Plants
a. Chiller Plant Validation. Revised validation procedures that occur when saving inputs for chiller plants. Previously chiller condenser and cooling tower water flow rates had
to match within 0.05 gpm (0.003 L/s). That tolerance has been revised to 20 gpm (1.25 L/s).
b. DX Free Cooling Algorithm. Revised the simulation algorithm for DX Free Cooling in air-cooled chillers to cycle the refrigerant pump and condenser fans when DX Free
Cooling capacity exceeds the chiller load.
5. Buildings
a. LEED Summary Report - Revised this report to adjust its format and content based on your stated project preference for the LEED Rating System. When your preference
is LEED NC-2.2, the report formats to match the NC-2.2 EA Credit 1 submittal template. When your preference is LEED 2009, the report formats to match the LEED 2009
EA Prerequisite 2 submittal template, where results from the performance rating method are now tabulated.
b. LEED Style Unmet Loads - Revised calculations to comply with the new definition of "unmet loads" in ASHRAE Standard 90.1-2007. This definition mandates that a single
hour can only result in one unmet load for cooling or heating. So, if 50 zones have temperatures above the cooling range, this counts as 1 unmet cooling load hour, not 50
unmet cooling load hours.
6. Electric Rates
a. Currency. Made currency a project-level preference so it only has to be defined once per project rather than requiring it be defined in each utility rate that is created.
b. Emission Factors. Revised the emission analysis feature to consider only CO2e (CO2 equivalent). Separate calculations for NOx and SO2 have been eliminated.
7. Bug Fixes
Problems in HAP v4.41 that were corrected in HAP v4.50 are listed below.
Air Systems
a. SFPMBX Terminal Fan Sizing. When using the sizing method "Zone Airflow = Sum of Space Airflows, Space Airflow = Based on Individual Space Peak Loads", if airflow
for a zone was adjusted due to the minimum zone airflow, minimum ventilation or minimum exhaust air overrides, the SFPMBX terminal fan airflow was not updated to
match the adjusted zone supply airflow rate.
b. Ventilation Airflow Sizing for Terminal Units. When using the ASHRAE Standard 62.1-2004 or 62.1-2007 sizing methods for ventilation for a terminal system (Hydronic
FCUs, DX FCUs, WSHPs, GWSHPs, GSHPs) that included a common ventilation unit, in certain situations the program incorrectly set the air distribution effectiveness to
1.0 rather than 0.8, and in all cases incorrectly set the space ventilation efficiency to 1.0. This could result in the ventilation air requirement reported by the program being
less than required per Standard 62.1.
c. Heating-Only WSHP Applications. For a WSHP, GWSHP or GSHP system configured for heating-only operation (cooling coil schedule set to OFF for all months), and
loop flow defined in terms of gpm/Ton (L/s/kW) or delta-T, the simulation reported zero energy use for the heat pumps, water pumps, cooling tower and auxiliary boiler.
Loop water flow was calculated based on cooling sizing data which was zero in this case. A zero loop flow prevented the loop from turning on.
d. ASHP Dehumidification Reheat. For a Rooftop or Split DX AHU air source heat pump system in which active dehumidification control was specified, energy use to meet
the dehumidification reheat load was omitted. For hours when simultaneous cooling and heating coil loads occurred, the heat pump served the cooling load and the
dehumidification reheat load was dropped. Instead the heat pump auxiliary heater should serve the dehumidification reheat load.
Page 20 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.3 Using HAP to Design and Analyze Systems, Plants and Buildings
1.0 Getting Started ››
Using HAP to Design Systems and Plants
1.0 Getting Started ›› 1.3 Using HAP to Design and Analyze Systems, Plants and Buildings ››
e. Publishing Sizing Requirements. If GSHP or GWSHP air systems were "published" to pass equipment sizing requirements to Carrier Electronic Catalog (E-CAT), the
equipment tags produced for these systems were unusable in E-CAT for running equipment selections.
Buildings
a. Simulation Reports. For a very specific set of conditions, the bar graphs shown on the Monthly Component Cost and Monthly Energy Cost reports contained invalid data.
The bars did not match the tabular data shown in the report. The required conditions to trigger this error included (1) selecting two or more buildings at the same time for
reporting, (2) selecting the Use Profiles graph report, and (3) selecting the Monthly Component Costs and/or Monthly Energy Costs reports.
b. LEED Summary Report - When running in SI Metric units, the footnote items for fuels which appear below the Energy Type Summary table displayed the incorrect energy
equivalent for fuel units of measure. For example, for natural gas the footnote might read "1 Cubic Meter = 10.349 MJ" instead of "1 Cubic Meter = 37.257 MJ".) This was a
cosmetic error that only affected the display of the footnote. No calculation results were affected by this error.
Fuel Rates
a. Fuel Rate Input Report. In a complex fuel rate, the "Step Type" in the Fuel Charge table was incorrectly labeled as "Energy" rather than "Fuel".
gbXML Import
a. Occupant Heat Gains. If the occupant heat gain data in the gbXML file is defined in SI Metric units, the import algorithm failed to import the data. Both occupant sensible
and latent heat gains were set to 0 W/person.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section summarizes how to use HAP for system design and energy modeling.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using HAP to Design Systems and Plants
This section briefly describes how to use HAP to design systems and plants. This description is specifically for detailed design applications. All such applications require the
same general five step procedure:
1. Define the Problem. First define the scope and objectives of the design analysis. For example, what type of building is involved? What type of systems and equipment are
required? What special requirements will influence system features?
2. Gather Data. Before design calculations can be performed, information about the building, its environment and its HVAC equipment must be gathered. This step involves
extracting data from building plans, evaluating building usage and studying HVAC system needs. Specific types of information needed include:
a. Climate data for the building site.
b. Construction material data for walls, roofs, windows, doors, exterior shading devices and floors, and for interior partitions between conditioned and non-conditioned regions.
c. Building size and layout data including wall, roof, window, door and floor areas, exposure orientations and external shading features.
d. Internal load characteristics determined by levels and schedules for occupancy, lighting systems, office equipment, appliances and machinery within the building.
e. Data concerning HVAC equipment, controls and components to be used.
3. Enter Data Into HAP. Next, use HAP to enter climate, building and HVAC equipment data. When using HAP, your base of operation is the main program window . From the
main program window, first create a new project or open an existing project . Then define the following types of data which are needed for system design work:
a. Enter Weather Data. Weather data defines the temperature, humidity and solar radiation conditions the building encounters during the course of a year. These conditions
play an important role in influencing loads and system operation. To define weather data, a city can be chosen from the program's weather database, or weather
parameters can be directly entered. Weather data is entered using the weather input form .
b. Enter Space Data. A space is a region of the building comprised of one or more heat flow elements and served by one or more air distribution terminals. Usually a space
represents a single room. However, the definition of a space is flexible. For some applications, it is more efficient for a space to represent a group of rooms or even an
entire building.
To define a space, all elements which affect heat flow in the space must be described. Elements include walls, windows, doors, roofs, skylights, floors, occupants, lighting,
electrical equipment, miscellaneous heat sources, infiltration, and partitions. Data is entered using the space input form .
While defining a space, information about the construction of walls, roofs, windows, doors and external shading devices is needed, as well as information about the hourly
schedules for internal heat gains. This construction and schedule data can be specified directly from the space input form (via links to the construction and schedule forms),
or alternately can be defined prior to entering space data.
Space information is stored in the project database and is later linked to zones in an air system.
c. Enter Air System Data. An Air System is the equipment and controls used to provide cooling and heating to a region of a building. An air system serves one or more zones.
Zones are groups of spaces having a single thermostatic control. Examples of systems include central station air handlers, packaged rooftop units, packaged vertical units,
split systems, packaged DX fan coils, hydronic fan coils and water source heat pumps. In all cases, the air system also includes associated ductwork, supply terminals and
controls.
To define an air system, the components, controls and zones associated with the system must be defined as well as the system sizing criteria. This data is entered on the
air system input form . Each project can contain up to 5000 systems.
d. Enter Plant Data. A Plant is the equipment and controls used to provide cooling or heating to coils in one or more air systems. Examples include chiller, changeover, hot
water, service hot water, and steam boiler plants.
This step is optional; it is only required if you are sizing plants. To define a plant for design purposes, the type of plant and the air systems it serves must be defined. This
data is entered on the plant input form . Each project can contain up to 100 plants.
4. Use HAP to Generate Design Reports. Once weather, space, air system and plant data has been entered, HAP can be used to generate system and plant design reports.
To generate design reports, go to the main program window and select the desired air systems or plants. Next choose the "Print/View Design Results" menu bar option,
toolbar button, or pop-up menu option. For systems this displays the System Design Reports form ; for plants this displays the Plant Design Reports form . Select the desired
report options on this form. If calculations are needed to supply data for these reports, the program will automatically run the calculations before generating the reports. If all
the data needed for the reports already exists, reports are generated immediately.
5. Select Equipment. Finally, use data from the reports you generated to select the appropriate cooling and heating equipment from product catalogs or electronic catalog
software. System and plant design reports provide information necessary to select all the components of your HVAC system including air handlers, packaged equipment,
supply terminals, duct systems, piping systems and plant equipment.
Carrier can provide electronic catalog computer programs to make selecting equipment quick and easy. Please contact your local Carrier sales office or Carrier distributor for
details.
Page 21 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Using HAP to Perform Energy Analyses
1.0 Getting Started ›› 1.3 Using HAP to Design and Analyze Systems, Plants and Buildings ››
HAP Energy Analysis For Preliminary Design
1.0 Getting Started ›› 1.3 Using HAP to Design and Analyze Systems, Plants and Buildings ››
HAP Energy Analysis For Detailed Design
1.0 Getting Started ›› 1.3 Using HAP to Design and Analyze Systems, Plants and Buildings ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using HAP to Perform Energy Analyses
HAP is designed with features to help you efficiently compare energy costs of HVAC design alternatives both in the preliminary design phase of a project and in the detailed
design phase of a project:
1. In the Preliminary or Schematic Design Phase of a project a variety of HVAC designs and equipment types may be under consideration. The goal of energy analysis in this
phase of a project is to quickly compare the energy cost performance of many design alternatives to identify a small group of designs with the best performance for further,
more detailed study. Simplification and approximation may be appropriate here both because much may not yet be known about the building and because speed is important
in evaluating the alternatives. The HAP Wizard interface is designed to help you quickly perform these types of energy analysis. Read more.
2. In the Detailed Design Phase of a project one or a small set of HVAC designs is under consideration. The goal of energy analysis in this phase of a project is to carefully
analyze and optimize the design. The goals here may also include generating documentation for LEED Energy and Atmosphere Credit 1. Given these goals, more detailed
definition of the building and its HVAC equipment is typically needed. The HAP detailed design interface is designed to help you perform these types of energy analysis. Read
more.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP Energy Analysis For Preliminary Design
This topic briefly describes how to use the HAP to estimate annual energy use and energy cost for HVAC designs in the preliminary or schematic design phase of a project.
Analysis work requires a general five step procedure:
1. Define the Problem. First define the scope and objectives of the energy analysis. For example, what type of building is involved? What type of systems and equipment are
required? What alternate designs or energy conservation measures are being compared in the analysis?
2. Gather Data. Before energy simulations can be run, general information about the building, its environment, the types of HVAC and non-HVAC equipment, and its energy
prices must be gathered. This step involves extracting data from building plans, evaluating building usage, studying HVAC system needs and acquiring utility rate schedules.
Specific types of information needed include:
a. Climate data for the building site.
b. General information about building size, shape, layout and number of floors.
c. General information about the type of wall, window and roof envelope construction to be used.
d. General information about the space usage in the building which will affect occupant density and lighting and equipment usage levels.
e. General information about the type of air-side systems, equipment and components to be considered.
f. General information about prices for electric service and any fuel sources used in the building.
3. Enter Data Into HAP. Next, use HAP to enter data for the analysis. When using HAP, your base of operation is the main program window. From the main program window,
first create a new project or open an existing project.
From the main program window choose the "Full Wizard Session" option on the Wizards menu, or click the "Full Wizard Session" button on the toolbar. The Full Wizard
Session window provides access to all of the HAP Wizards:
a. The Weather Wizard - Used to quickly configure weather data for the building site.
b. The Building Wizard - Used to rapidly define the size, shape, layout, envelope and internal loads for the building spaces.
c. The Equipment Wizard - Used to easily create HVAC design alternatives.
d. The Utility Rate Wizard - Used to quickly assemble electric and fuel pricing data.
After entering data on the Wizard input screens, press the Finish button in the lower left of the Full Wizard Session window. HAP converts your Wizard data into a full set of
detailed HAP inputs and displays them in the main window. This data includes weather, spaces, air systems, plants, buildings and all of the data these contain such as
schedules, wall, roof, window and door assemblies, chillers, towers, boilers and utility rates.
4. Use HAP to Generate Simulation Reports. Once all input data has been entered or generated, HAP can be used to generate reports showing energy cost results.
To generate building simulation reports, go to the main program window and select the buildings representing your set of HVAC design alternatives. Next choose the
"Print/View Simulation Results" option on the Reports Menu. This displays the Building Simulation Reports Selection dialog. Choose the desired reports. Then press Preview
to display the reports or press Print to directly print the reports. HAP will automatically run any necessary calculations first before generating the reports.
When comparing annual energy cost for a preliminary design type of analysis, the Annual Cost Summary and Annual Energy & Emission Summary reports are most frequently
used. These reports compare energy cost or energy use for the design alternatives side by side on a single page.
Simulation reports for individual air systems and plants included in your analysis can also be generated. Use the same procedure but select air system or plant items instead.
System and plant simulation reports provide more detailed performance information for individual pieces of equipment. These reports are often useful for learning about
equipment performance and for troubleshooting unexpected results.
5. Evaluate Results. Finally, use data from the simulation reports you generated to draw conclusions about the most favorable design alternatives.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP Energy Analysis For Detailed Design
This topic briefly describes how to use the HAP to estimate annual energy use and energy cost for HVAC designs in the detailed design phase of a project.
Note that certain steps are identical or similar to those used for system design. If a system design has already been performed for a building, all of the data entered for design
can be reused for the energy analysis, and this significantly reduces the effort needed to complete the energy analysis. Also note that energy analysis features are only available
in the HAP program and not in HAP System Design Load.
All analysis work requires the same general five step procedure:
1. Define the Problem. First define the scope and objectives of the energy analysis. For example, what type of building is involved? What type of systems and equipment are
required? What alternate designs or energy conservation measures are being compared in the analysis?
2. Gather Data. Before energy simulations can be run, information about the building, its environment, HVAC and non-HVAC equipment, and its energy prices must be gathered.
This step involves extracting data from building plans, evaluating building usage, studying HVAC system needs and acquiring utility rate schedules. Specific types of
information needed include:
a. Climate data for the building site.
b. Construction material data for walls, roofs, windows, doors, exterior shading devices and floors, and for interior partitions between conditioned and non-conditioned regions.
Page 22 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Fundamental Terminology
1.0 Getting Started ›› 1.3 Using HAP to Design and Analyze Systems, Plants and Buildings ››
c. Building size and layout data including wall, roof, window, door and floor areas, exposure orientations and external shading features.
d. Internal load characteristics determined by levels and schedules for occupancy, lighting systems, office equipment, appliances and machinery within the building.
e. Data for HVAC equipment, controls and components to be used.
f. Data for chilled water, hot water and/or steam plants, if applicable.
g. Data for non-HVAC energy-consuming equipment.
h. Utility rate information for electric service and any fuel sources used in the building.
3. Enter Data Into HAP. Next, use HAP to enter data for the analysis. When using HAP, your base of operation is the main program window. From the main program window,
first create a new project or open an existing project. Then define the following types of data which are needed for energy analysis work:
a. Enter Weather Data. Weather data defines the temperature, humidity and solar radiation conditions the building encounters during the course of a year. These conditions
play an important role in influencing loads and system operation throughout the year. Both design and simulation weather data are needed. To define design weather data,
a city can be chosen from the program's weather database, or weather parameters can be directly entered. Simulation weather is selected by loading a simulation weather
file from the library provided with the program or by importing data from an external source. This step is also used to define the calendar for your simulation year. All three
types of data are entered using the weather input form.
b. Enter Space Data. A space is a region of the building comprised of one or more heat flow elements and served by one or more air distribution terminals. Usually a space
represents a single room. However, the definition of a space is flexible. For some applications, it is more efficient for a space to represent a group of rooms or even an
entire building.
To define a space, all elements which affect heat flow in the space must be described. Elements include walls, windows, doors, roofs, skylights, floors, occupants, lighting,
electrical equipment, miscellaneous heat sources, infiltration, and partitions. Space data is entered using the space input form.
While defining a space, information about the construction of walls, roofs, windows, doors and external shading devices is needed, as well as information about the hourly
schedules for internal heat gains. This construction and schedule data can be specified directly from the space input form (via links to the construction and schedule forms),
or alternately can be defined prior to entering space data.
Space information is stored in the project database and is later linked to zones in an air system.
c. Enter Air System Data. An Air System is the equipment and controls used to provide cooling and heating to a region of a building. An air system serves one or more zones.
Zones are groups of spaces having a single thermostatic control. Examples of systems include central station air handlers, packaged rooftop units, packaged vertical units,
split systems, packaged DX fan coils, hydronic fan coils and water source heat pumps. In all cases, the air system also includes associated ductwork, supply terminals and
controls. In the case of packaged DX, split DX, electric resistance heating and combustion heating equipment, the system also encompasses this DX or heating equipment.
For example, when dealing with a gas/electric packaged rooftop unit, the "air system" includes the DX cooling equipment and the gas heating equipment.
To define an air system, the components, controls and zones associated with the system must be defined as well as the system sizing criteria. For energy analyses,
performance information about DX cooling equipment and electric and combustion heating equipment must also be defined. All of this data is entered on the air system
input form.
d. Enter Plant Data. A Plant is the equipment and controls used to provide cooling via chilled water or heating via hot water or steam to coils in one or more air systems.
Examples include chiller plants, hot water plants, steam boiler plants and remote source cooling and heating plants.
This step is optional; it is only required if chilled water, hot water or steam plants are used in your building. To define a plant for energy analysis purposes, the type of plant
and the air systems it serves must be defined along with its configuration, controls and distribution system information. This data is entered on the plant input form.
e. Enter Utility Rate Data. Utility rate data defines the pricing rules for electrical energy use and fuel use. An electric rate structure must be defined for all energy studies. One
fuel rate for each non-electric fuel source must also be defined. Electric rate data is entered using the electric rate form. Fuel rate data is entered using the fuel rate form.
f. Enter Building Data. A Building is simply the container for all energy-consuming equipment included in a single energy analysis case. One Building is created for each
design alternative being considered in the study. Building data consists of lists of plants and systems included in the building, utility rates used to determine energy costs
and data for non-HVAC energy or fuel use. Data is entered using the building form.
4. Use HAP to Generate Simulation Reports. Once all input data has been entered, HAP can be used to generate simulation reports.
To generate building simulation reports, go to the main program window and select the desired buildings. If data for a single building is being evaluated, select only one
building. If energy use and costs for a number of alternatives is being compared, select a group of buildings. Next choose the "Print/View Simulation Results" option on the
Reports Menu. This displays the Building Simulation Reports Selection dialog. Choose the desired reports. Then press Preview to display the reports or press Print to directly
print the reports. If system, plant or building calculations are needed to supply data for your reports, HAP will automatically run these calculations first. Otherwise, if no
calculations are needed the reports will be generated immediately.
Simulation reports for individual air systems and plants included in your analysis can also be generated. Use the same procedure but select air system or plant items instead.
System and plant simulation reports provide more detailed performance information for individual pieces of equipment. They are often useful for learning about equipment
performance and for troubleshooting unexpected results.
5. Evaluate Results. Finally, use data from the simulation reports you generated to draw conclusions about the most favorable design alternative. In many cases energy use and
energy cost data will be used for further study of lifecycle economics.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fundamental Terminology
HAP organizes information about a building and its HVAC equipment into the six categories shown below. These are arranged in a hierarchy that permits you to assemble the
description of your building and its HVAC equipment in a flexible manner. The key terms for each component category are defined below, beginning with the lowest in the
hierarchy and working upward.
1. An Element is a component of the building structure or building use associated with heat gain or loss. Elements include walls, windows, doors, roofs, skylights, floors,
partitions, lighting, people, electric equipment, miscellaneous heat sources and infiltration. An element is described by its characteristics which affect heat transfer. A wall, for
example, is described by its area, orientation, and the materials from which it is constructed.
2. A Space is a region of the building comprised of one or more heat flow elements and served by one or more air distribution terminals. Usually a space represents a single
room. However, the definition of a space is flexible. For some applications, it is more efficient for a space to represent a group of rooms or even an entire building.
3. A Zone is a group of one or more spaces having a single thermostatic control. In some systems, each room contains a thermostat. Thus, each zone would contain one space
representing a single room. In other situations, one thermostat is allocated to a group of rooms. In this case, the zone would contain several spaces.
4. An Air System is the equipment and controls used to provide cooling and heating to a region of a building. An air system serves one or more zones. The presence of a
thermostat in each zone permits specific control of air temperature in each zone. Examples of systems include central station air handlers, packaged rooftop units, packaged
vertical units, split systems, packaged DX fan coils, hydronic fan coils and water source heat pumps. In all cases, the air system also includes associated ductwork, supply
terminals and controls. For energy analysis applications, the system also includes DX cooling, electric resistance heating and combustion heating apparatus.
5. A Plant is the equipment and controls used to provide cooling or heating to coils in one or more air systems. Examples include chiller plants, hot water plants and steam boiler
plants.
6. A Building is the structure containing all the HVAC systems under consideration. When performing energy analysis studies, annual energy costs are computed for the building
and all the energy consuming systems it contains. Taken literally, a building represents one individual structure. However, the definition of a building is flexible. It can also
represent a group of structures. For example, a "building" could represent a campus in which all the structures are served by a common set of plant equipment.
During system design work, the first five of these items are dealt with. The "building" item is only dealt with when performing annual energy studies.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 23 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.4 Program Operation
1.0 Getting Started ››
The HAP Main Program Window
1.0 Getting Started ›› 1.4 Program Operation ››
This section describes features of the HAP main window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
The HAP Main Program Window
This topic discusses HAP’s main program window which appears when you start the program. Much of the work you will perform defining data and generating reports is done
using features of the main program window. Key elements and features of the main program window are discussed below. Related information which may be useful can be found
in separate topics dealing with input forms , project management , and a program tutorials for system design and energy analysis .
The HAP main program window consists of six components used to operate the program. Working from top to bottom in the figure above:
1. The Title Bar lists the program name and the name of the current project. If you are running HAP System Design Load or are running the full HAP but in System Design mode,
the program name will be "HAP System Design Load". If you are running the full HAP program with energy analysis features turned on, the program name will simply be
"HAP". At the right-hand end of the title bar are command buttons for minimizing and maximizing the program window and for exiting from the program.
2. The Menu Bar lies immediately below the title bar. The menu bar contains seven pull-down menus used to perform common program tasks. To use menu options, first click on
the menu name to "pull-down" its list of options. Then click on the name of the desired option. The seven pull down menus are as follows:
Project Menu
Edit Menu
View Menu
New
Duplicate
Large Icons
Open
Delete
Small Icons
Save
Select All
List
Save As
Invert Selection
Details
Delete
Replace
Toolbar
Properties
Rotate
Status Bar
Archive
Duplicate Bldg (w/ Spaces & HVAC Eqpt)
Preferences
Retrieve
Perform LEED (90.1 PRM) Rotations
Convert HAP v3.2 Data
Convert HAP v4.x or 5.x Data
Publish Eqpt Sizing Requirements
Send Email...
Export to Engr. Economic Analysis
Import Project Data
Import gbXML
Import Building System Optimizer Data
Reports Menu
Wizards Menu
Documentation Menu
Help Menu
Print Input Data
Weather Wizard
Quick Reference Manual
Contents and Index
View Input Data
Building Wizard
Example Problem Reports
Contact Software Support
Print/View Design Results
Equipment Wizard
ASHRAE 90.1 Energy Cost Budget
eDesign Support Web Site
Print/View Simulation Results
Utility Rate Wizard
ASHRAE 140 Test Results
Check for Program Updates
Full Wizard Session
ASHRAE 183 (Peak Load Calculations)
eDesign Software Training
ASHRAE 90.1 Appendix G
eDesign Software Web Site
Page 24 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
HAP Input Forms
1.0 Getting Started ›› 1.4 Program Operation ››
Using HAP for LEED EA Credit 1
Carrier Commercial Web Site
US Federal Regulation 10 CFR Part 434
About HAP
3. The Toolbar lies immediately below the menu bar and contains a series of buttons used to perform common program tasks. Each button contains an icon which represents
the task it performs. These buttons duplicate many of the options found on the pull-down menus.
To determine the function of a toolbar button, simply place the mouse cursor over a button. A "tooltip" will appear listing the function of that button.
4. The Tree View is the left-hand panel in the center of the main program window. It contains a tree image of the major categories of data used by HAP. The tree view acts as the
"control panel" when working with program data:
a. To display a list of items in one of the categories of data, click once on the category name. For example if you click on the Space category name, a list of spaces you have
entered will appear in the list view panel on the right side of the main program window. Once a list of items appears, you can click on items in the list view to perform such
tasks as creating new data, editing data and generating reports.
b. To display a pop-up menu of options for the category, right-click on the category name. The "category pop-up menu" will appear. Options on this menu will perform tasks on
all items in a given category. For example, if you right-click on the System category name, the System category pop-up menu will appear. If you select the Print Input Data
option, input data for all systems in your project will be printed. Because options on the category pop-up menu operate on all items in a category, you should be careful
using these options.
c. To display a summary of project contents, click once on the Project category name. A list of the major data categories (weather, spaces, systems, plants) will appear. If the
"details" format is used for the list view, the quantity of items you have defined for each category will also be shown. For example, the summary shows the number of
spaces and systems which have been defined.
To display a summary of project library contents, click once on the Project Libraries category name. A list of the library categories (schedules, walls, roofs, windows, doors,
shades) will appear. If the "details" format is used for the list view, the quantity of items you have defined in each category will be shown. For example, the summary shows the
number of wall and roof assemblies you have defined.
5. The List View is the right-hand panel in the center of the main program window. It contains a list of data items in alphabetical order for one of the categories of data in your
project. For example, when the space category is selected, the list view shows a list of spaces you have entered. The list view acts as the second part of the "control panel"
when working with program data. By selecting items in the list view you can:
a. Create new items . Example: Creating a new schedule.
b. Edit existing items . Example: Editing a wall assembly you previously defined.
c. Duplicate an existing item. Example: Creating a new space using defaults from an existing space.
d. Duplicate a building with all of its spaces and HVAC equipment. This is used in a LEED EA Credit 1 analysis to make a copy of the Proposed Design building and all of its
spaces, systems, plants, chillers, cooling towers and boilers to use as the basis for assembling the Baseline Building.
e. Delete existing items. Example: Deleting three systems you previously entered.
f. Search and replace existing space data. Example: Change lighting W/sqft from 2.0 to 1.8 for 40 spaces all at one time.
g. Rotate the orientation of existing spaces. Example: Rotate the orientation of 35 spaces by 45 degrees clockwise all at one time.
h. Perform LEED (90.1 PRM) rotations for a building. This is used in a LEED EA Credit 1 analysis to make three copies of the Baseline 0 Degree building and in those copies
rotate the spaces 90, 180 and 270 degrees as required by the analysis rules.
i. View or print input data. Example: Printing input data for four window assemblies you previously entered.
j. View or print system design reports. Example: Viewing design reports for two air systems you defined.
k. View or print plant design reports . Example: Printing a design report for a chiller plant.
l. View or print system, plant or building energy simulation reports (HAP users only). Example: Printing a building simulation report listing annual energy use and energy costs.
There are usually at least two or three ways of performing each task. For example, after selecting items in the list view, an option on the Edit or Report Menu can be selected,
or a button on the Toolbar can be pressed, or an item pop-up menu can be displayed by right-clicking on the selected items.
6. The Status Bar is the final component of the main program window and appears at the bottom of the window. Working from left to right, the left hand end of the status bar lists
pertinent messages such as maximum and minimum limits for an input. The center section of the bar lists the current selections for the project LEED version, ventilation
standard, and energy standard. Finally, the current date and time appear at the right-hand end of the status bar.
Further information on program operation can be found in separate topics dealing with input forms , and project management. Tutorials for system design and energy analysis
are also provided. Complete example problems can be found in the HAP Quick Reference Guide.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP Input Forms
This topic discusses the basic operating principles of HAP’s input forms. While much of your work with the program is done on the main program window , the actual entry of data
is done using input forms. An input form appears when you choose to create a new item or edit an existing item in the main program list view. A separate input form is provided
for each category of HAP data.
Page 25 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Figure 1. A Simple Input Form
Simple Input Forms. Many input forms have a simple appearance as shown above. These simple kinds of input forms consist of three components:
1. The Title Bar is found at the top of the input form. It lists the type of data contained in the input form and the name of the current item being edited. In the example above, data
for a window assembly named "4x6 Double Glazed with Blinds" is being edited. The title bar also contains a close button. If you press this button, the program will return to the
main program window without saving any changes you made on the form. Thus, the close button performs the same function as the Cancel button.
2. The Data Area is the middle portion of the form. It contains all the data describing the current item. In the example above, the data area contains information describing a
window assembly: its dimensions, framing properties, internal shades, glazings and the thermal performance of the window.
While entering information in the data area, you can display explanations of each input item by pressing the F1 key. For example, if you press F1 while the cursor is on the
"Frame Type" item in the figure above, the help topic for "Window Frame Type" will appear automatically. This feature is useful for learning about the program while you work.
3. The Command Buttons are found in the lower right-hand portion of the form. All forms contain three buttons:
a. When you press the OK button, the program will save any changes you made on the input form and will then return to the main program window.
b. When you press the Cancel button the program will return to the main program window without saving any changes you made on the input form. The Cancel button
performs the same function as the close button in the title bar.
When you press the Help button an overview description of the current input form will be displayed. This overview describes how the input form is organized and how to use it.
It also contains links to help topics for the individual input items on the form.
Figure 2. A Tabbed Input Form
Tabbed Input Forms. For certain categories of HAP data, the input form has a more complex appearance as shown above. This input form contains the same basic elements
(title bar, data area, command buttons) as discussed earlier, but the data area contains multiple categories of information rather than a single set of information. Categories of
data are represented as tabs in a notebook.
In the figure above, data for a space is shown. Space data is divided into five categories:
1. General data
2. Internal load data
3. Wall, Window, Door data
4. Roof, Skylight data
5. Infiltration data
6. Floor data
7. Partition data
To switch between the different categories of data, simply click on the tab title. For example, to switch to the "Walls, Windows, Doors" category of data, click on the "Walls,
Windows, Doors" tab.
HAP Input Forms. Input forms are provided in HAP for the following types of data:
Weather Data
Spaces
Air Systems
Plants
Page 26 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.5 Working with Projects
1.0 Getting Started ››
Project Data Management
1.0 Getting Started ›› 1.5 Working with Projects ››
Buildings (HAP only)
Schedules
Wall Assemblies
Roof Assemblies
Windows
Doors
External Shading Geometries
Chillers (HAP only)
Cooling Towers (HAP only)
Boilers (HAP only)
Electric Rates (HAP only)
Fuel Rates (HAP only)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes features for managing project data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Project Data Management
This topic discusses projects and the management of project data.
What is a Project? All the data you enter and calculate in HAP is stored together within a "project". A Project is simply a container for your data. However, a project can hold
data for other programs as well as HAP. For example, if you create a project for a building design job, it might contain load estimating and system design data from HAP, air
handler selection data from the Carrier AHUBuilder program, and air terminal selection data from the Carrier Air Terminal Selection program. Keeping this data together in a
single container is often more efficient than keeping the data in several separate locations.
Using Projects. HAP provides a variety of features for performing common tasks with projects. You can:
1. Create a new project by using the New option on the Project Menu.
2. Edit data in an existing project by using the Open option on the Project Menu.
3. Save changes in a project by using the Save option on the Project Menu
4. Save changes to a new project using the Save As option on the Project Menu
5. Delete an existing project using the Delete option on the Project Menu.
6. Edit descriptive data for the project, such as the project name, using the Properties option on the Project Menu.
7. Archive project data for safe keeping using the Archive option on the Project Menu.
8. Retrieve data that you earlier archived using the Retrieve option on the Project Menu.
9. Convert data from a previous version of HAP using one of the Convert HAP Data options on the Project Menu.
10. Import data from another project into the current project using the Import Data option on the Project Menu.
11. Import data from a gbXML file using the Import gbXML option on the Project Menu. For example, a gbXML file generated by a CAD tool can be imported into HAP to speed
the process of transferring data from floor plan drawings into HAP.
How Project Data is Stored. When a new project is saved for the first time, you designate the folder which will hold the project files (either by accepting the default folder \E20
II\Projects\ProjectName or by specifying a folder yourself). This folder is the permanent storage location of project data. When you open the project to work with its data,
temporary copies of the project’s data files are made. As you enter data, make changes and perform calculations, all this data is stored in the temporary copy of the data files.
Only when you use the Save option on the Project Menu are the changes you’ve made are copied to permanent storage. Therefore, if you ever need to undo changes you’ve
made to a project, simply re open the project without saving the changes you’ve made. When you re-open the project, the changes stored in the temporary copy of the data files
are discarded, and data from your last project/save is restored.
Recommended Project Management Practices. Project data represents an important investment of your time and effort. And, as the saying goes, ‘time is money’. Therefore it
is important to safeguard your investment in project data. We recommend adopting the following practices when working with projects:
1. Create a separate project for each job you work on. It is usually more efficient to keep data for separate jobs in separate projects. It is also safer to store data in smaller,
focused units. If you keep data for all jobs in a single project, and this project becomes damaged, your data loss will be greater than if you keep data for separate jobs in
separate projects.
2. Use a descriptive name for the project so you can quickly recognize what it contains, both now and when you need to refer to the project in the future. Because the selection
list for projects is arranged alphabetically it is useful to use a consistent naming convention. Many firms begin the project name with their internal project number followed by
descriptive text (e.g., P2002-47 Lincoln School).
3. Save early and often. While entering data, changing data and generating reports, save the project periodically. This practice is useful in the event that you make a mistake and
need to undo changes. If the last time you saved the project was 15 minutes ago, undoing your mistake will only cause you to lose 15 minutes of work. On the other hand, if
the last time you saved the data was 4 hours ago, undoing a mistake may cause you to lose 4 hours worth of work.
4. Archive your data periodically for safekeeping. These days data on hard disks is relatively safe. However, it is still possible for hard disk drives to become damaged, or for files
on the hard disk to be damaged or erased. Therefore it is a good practice to periodically archive your project data. Data can be archived to a separate location on your hard
disk, to a network drive or to an external drive. For example, if you archive data for a large project at the end of each day and your hard disk drive fails, at most you will have
lost one day’s worth of work. On the other hand, if data for the same large project was never archived and your hard disk drive fails, all the project data would be lost.
Project Data Quantities. A project can contain all of the data for your analysis. This can include multiple variations of the building and its HVAC systems and equipment.
Maximum limits on the quantity of data items in a project are shown below:
Data Category
Maximum
Number of Items
Weather
1
Spaces
32000
Page 27 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Creating a New Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Opening an Existing Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Saving a Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Saving a Project as a New Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Deleting a Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Air Systems
5000
Plants
250
Buildings
100
Schedules
Unlimited
Wall, Roof, Window, Door Assemblies
Unlimited
Shade Geometries
Unlimited
Chillers, Cooling Towers, Boilers
Unlimited
Electric Rates, Fuel Rates
Unlimited
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Project
A new project is typically created when starting a design job. The project will serve as the container for all your input and calculation data for the job. To create a new project:
1. Choose the New option on the Project Menu.
2. If changes to the current project have not yet been saved, HAP will ask you if you want to save the current project before creating a new one.
3. Then a new "Untitled" project will be created. No data for this project will be permanently stored until the first time you use the Save option on the Project Menu.
4. When you choose the Save option on the Project Menu, you’ll be asked to name the project.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Opening an Existing Project
Before you can enter data, edit data and generate reports for an existing project , you first need to open the project:
1. Choose the Open option on the Project Menu.
2. The Open Project dialog will appear. It contains a list of all existing projects arranged in alphabetical order. Select the desired project from this list.
3. If changes to the current project have not yet been saved, HAP will ask you if you want to save the current project before opening another one.
4. Then the project you selected will be loaded into memory. When you are returned to the HAP main program window, data for the project you selected will be displayed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Saving a Project
The Save option on the Project Menu is used to permanently store data you entered or changes you’ve made to a project . While working with a project, its data is stored in
temporary copies of the project data files. Saving the project copies your new data and your modified data to permanent storage. To save a project, simply choose the Save
option on the Project Menu. Note that when you save a new project for the first time, you will be asked to name the project. Thereafter, when you save the project data will be
saved under this project name automatically.
By default the program will save data under \E20-II\PROJECTS in a folder whose name is the same as the project name. Many users elect to accept this storage convention.
However, for those who wish to save the data elsewhere, the software provides a feature to save the project in any folder on any drive accessible to your computer. The only
requirement is that when the project is first saved the storage folder must be empty.
As a sound data management practice, we recommend saving the project periodically as you work with it. If you ever need to undo a mistake you’ve made, you can re open the
project without saving it. This restores the project data from your last project save, but any changes made since the last save will be lost. If project data is saved frequently,
undoing a mistake will only cause a small amount of data to be lost.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Saving a Project as a New Project
The Save As option on the Project Menu is used to store changes to your current project data in a new project rather than the existing project. Typically this feature is used when
making a copy of a project. To save a project as a new project:
1. First choose the Save As option on the Project Menu.
2. You will be asked to specify a name for the new project. By default the project will be saved under \E20-II\PROJECTS in a folder whose name is the same as the project name.
However, users may override this default and save the data in any other folder. The only requirement is that when the project is first saved the folder must be empty.
3. HAP then saves your current project data in the new project folder and closes the old project. All subsequent changes to project data and saving of project data will affect the
new project you created.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 28 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Editing Project Properties
1.0 Getting Started ›› 1.5 Working with Projects ››
Archiving a Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Retrieving a Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Converting HAP v4.x or v5.x Data
1.0 Getting Started ›› 1.5 Working with Projects ››
Deleting a Project
To delete a project :
1. First, choose the Delete option on the Project Menu. The Delete Project dialog will appear.
2. On the Delete Project dialog choose the project you wish to delete.
3. HAP data files for the selected project will then be erased. If the project only contained HAP data, the project itself will be erased. However, if the project contained data from
other programs, the project will remain in existence along with the data from these other programs.
Example: A project contains HAP and AHUBuilder data. You choose the Project/Delete option from within HAP. Only the HAP data will be erased. The project will continue to
exist and will contain only data for AHUBuilder.
The Project/Delete option should be used with care. When project data is deleted it is permanently lost and cannot be recovered.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing Project Properties
The Properties option on the Project Menu is used to enter or change the descriptive information for a project . When this menu option is selected the Project Properties dialog
appears. It contains the descriptive items listed below. Of these the Project Name is the only item that must be defined since it is used throughout HAP for various purposes. All
of the other items are for the user’s own reference and are therefore optional.
1. Project Name: A reference name for the project. It appears on all HAP reports, in the title bar of the HAP main program window and on selection lists when opening and
deleting projects. It is important to use a descriptive name for the project so you can easily determine what data the project contains. Note that after a project has been saved
for the first time its project name cannot be changed, except by using the Save As option on the Project Menu.
2. Job Number: A reference number for the project. Users often enter the internal billing number or company reference number for the project here.
3. Contact Type: An item that defines who the client for the project is: a contractor, owner, architect, etc…
4. Contact Name: The name of the client or a person in the client’s firm who is the contact for this project.
5. Salesperson: The name of the salesperson working with you on the project to supply HVAC equipment information.
6. Date: A significant date for the project. Some users specify the date the project was created. Others specify the contract date or a delivery date.
7. Notes: Notes concerning the status of the project or any other pertinent information.
Press the OK button on the Project Properties dialog to exit and save the changes you made. Press the Cancel button on the Project Properties dialog to exit without saving
changes.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Archiving a Project
The Archive option on the Project menu saves project data in one compressed file for safekeeping. A project is typically archived when saving it for backup storage, for future
reference, or when transferring data from one computer to another. In order to archive data for a project:
1. First open the project you wish to archive. When you choose the Archive option, HAP data for the currently open project will be archived.
2. Choose the Archive option on the Project Menu.
3. You will then be asked to specify the name of the archive file and the destination drive and folder where the archive file will be written. Use a descriptive name for the archive
file so you will be able to recognize it easily when you need to use it in the future. The destination folder you specify can be on any connected drive such as your main hard
disk drive, a network drive, or an external drive. Once a file name and folder has been specified, press the Save button.
4. The program then compresses the HAP data files for the current project, placing the data in a single ZIP-format file in the destination folder you specified.
Note: Archiving data does not remove it from the project. It merely stores a copy of the data for safekeeping. You can continue working with the current project data after it has
been archived.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Retrieving a Project
The Retrieve option on the Project menu restores data that was previously archived using the Project/Archive option. The Archive option saves project data in one compressed
file for safekeeping. The Retrieve option uncompresses the archive data and makes it available for use again. A project is typically retrieved when receiving archive data from
another computer, when referring to an old project that was archived for safekeeping, or when restoring backup data after a hard disk failure. In order to retrieve data for a
project:
1. First create a new project or open the project you want to retrieve data into. Data is always retrieved into the currently open project. Often users create a new project to receive
retrieved data so existing data will not be overwritten. For example, if the current project contains HAP data, when you retrieve archived HAP data it will replace all of the
current data. Thus, if you do not want to lose data in the current project, you must create a new project before retrieving.
2. Choose the Retrieve option on the Project Menu. The program will display a dialog asking you to identify the archive file you wish to retrieve data from.
3. Once a file is identified, the program will display its vital statistics. These statistics include the name of the archived project and the data contained in the archive. You are
asked to confirm that this is the archive data you want to retrieve. Press the Retrieve button to begin retrieval, or the Browse button to select a different archive file.
4. The selected data will then be retrieved from the archive file and placed in the current project. When you return to the HAP main program window, the HAP data you retrieved
will be displayed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 29 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Converting HAP v3.2 Data
1.0 Getting Started ›› 1.5 Working with Projects ››
Converting HAP v4.x or v5.x Data
The Convert HAP v4.x or v5.x Data option on the Project Menu is used to convert data from any of the HAP versions v4.0 thru v5.0 into a format compatible with the current
version of HAP. Typically this option is used when you started a project with an earlier version and want to complete the work using the current version of HAP.
Data can be converted from either an active project or an archive file. An active project is one that would appear on the Open Project dialog if you set the project filter to an option
like "Hourly Analysis Program v5.0" or "Show All Projects". An archive file is a .E3A file you produced using the "Archive" option in the previous version of HAP to store project
data for backup or archival purposes. Procedures for converting data from each source are provided below.
A. Converting Data in an Active Project
This procedure applies for the case where an active project contains data for one of the HAP versions v4.0 thru v5.0. This old version data will be converted to HAP v5.1 format
and saved in the same project folder as the original data.
1. Start HAP v5.1
2. Select the project whose data is to be converted.
a. Choose the Open option on Project Menu.
b. In the Open Project dialog change the filter at the bottom of the dialog to show projects of the HAP version you are converting from. For example, if converting from v5.0 to
v5.1, choose to show projects from "Hourly Analysis Program v5.0". Any version HAP v4.0 through v5.0 can be selected.
You can also set the filter to "Show All Projects" if you wish.
c. Choose the desired project from the list. If this project has never been opened with HAP v5.1 before, a blank set of files in v5.1 format will be created when you open the
project. Thus, when you return to the main window you’ll see a project containing no data yet. Continue with steps 3 thru 6 to fill it with converted data.
3. Start the conversion process by choosing "Convert HAP v4.x or v5.x Data" on the Project Menu.
4. A message will appear warning that v5.1 data in the current project will be overwritten by converted data. This is OK since at this point you have a blank set of v5.1 files in the
project. Press "Yes" to continue.
5. On the "Convert HAP v4.x or v5.x Data" dialog, press the "Active Project" button, indicating you want to convert data from an active project.
6. Old version data in the project will then be converted to HAP v5.1 format. At the end of the conversion a message will appear indicating whether the conversion was
successful. Important information about the data conversion can be displayed via the Help button in this message window, or via the following help topic: About Translation of
HAP v4.x or v5.x Data.
7. After inspecting the converted data, use the Save option on the Project Menu to save the data.
B. Converting an Archive File
This procedure applies for the case where data from one of the HAP versions v4.0 thru v5.0 is in an archive file. Data in the archive file will be extracted and then converted to
HAP v5.1 format. Data will be saved in the current HAP v5.1 project folder.
1. Start HAP v5.1
2. Select the project in which converted data will be stored.
a. Users typically choose the New option on the Project Menu to create a new, untitled project and then save this project after converting the data.
b. An alternative is to use the Open option on the Project Menu to open an existing project. However, if that project already contains HAP v5.1 data the existing data will be
replaced by converted data and will be lost. Therefore using Project/Open should only be done when the existing project doesn’t yet have v5.1 data or loss of the existing
data is not a concern.
3. Start the conversion process by choosing "Convert HAP v4.x or v5.x Data" on the Project Menu.
4. If an existing project was opened in step 2, a message will appear warning that v4.9 data in the current project will be overwritten by converted data. If it is OK to proceed,
press the Yes button.
5. On the "Convert HAP v4.x or v5.x Data" dialog, press the "Archive File" button, indicating you want to convert data from an archive file.
6. In the File Open dialog choose the archive file you wish to convert data from. That archive file must contain data from one of the HAP versions v4.0 thru v5.0.
7. The contents of the archive file will be extracted and then converted to v5.1 format. At the end of the conversion a message will appear indicating whether the conversion was
successful. Important information about the data conversion can be displayed via the Help button in this message window, or via the following help topic: About Translation of
HAP v4.x or v5.x Data.
8. After inspecting the converted data, use the Save option on the Project Menu to save the data.
How Previous Version Data is Converted. When data from a previous version of HAP is converted to be compatible with the current version, it is "translated" rather than
"transferred". It is important to make a distinction between "translation" of data and "transfer" of data:
a. "Data Transfer" refers to the simple copying of data. The result of a data transfer is an exact copy of the original data. No data is added, deleted or modified.
b. The result of "Data Translation" is the original data with missing items added, unusable items discarded and other items reorganized.
Fortunately translation of data from one version of HAP to the next preserves the vast majority of your data. To view information about items adjusted during translation and
about which categories of data are converted, press the Help button in the status message window that appears at the end of the translation process, or click here: Translation of
HAP v4.x or v5.x Data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting HAP v3.2 Data
The Convert HAP v3.2 Data option on the Project Menu is used to convert data from HAP v3.2 or System Design Load v1.2 for use in the current version of HAP. HAP v3.2 and
System Design Load v1.2 were the last DOS versions of HAP (released between 1995 and 2000) and therefore require a different conversion process than required when
converting data from a HAP v4.x or v5.x version. Typically this option is used when you started a project with the earlier version and want to complete the work using the current
version of HAP. The procedure is described below:
1. First, make sure the data you wish to convert has been loaded into a project folder for the HAP v3.2 or System Design Load v1.2. For example, when converting HAP v3.2
data, the data being converted must be stored in one of the HAP v3.2 data folders which are found under \E20-II\HAP32. Note that it is not possible to convert data directly
from a HAP v3.2 archive file. The archive file must first be retrieved into a HAP v3.2 project folder.
2. Next, while running the current version of HAP, open the project in which you want to store the converted data. In most cases, users will create a new project and store the
converted data in this project to avoid overwriting and destroying data in an existing project.
3. Then choose the Convert HAP v3.2 Data option on the Project Menu. A dialog will appear. It is used to identify the data folder containing previous version data you want to
convert. HAP v3.2 and System Design Load v1.2 stored data in a rigid tree structure. Therefore, if you are looking for HAP v3.2 data folders, they will be found beneath the
\E20-II\HAP32 folder. If you are looking for System Design Load v1.2 data folders, they will be found beneath the \E20 II\SDL12 folder.
Page 30 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Publishing Equipment Sizing Requirements for use in E-CAT
1.0 Getting Started ›› 1.5 Working with Projects ››
4. Choose the data folder containing the data you wish to convert. Important Note: Make sure you double-click on the folder name so its folder icon appears as an open folder. If
the icon does not appear as an open folder, the folder has not been correctly selected.
5. Then the program will read data from the HAP v3.2 or System Design Load v1.2 data folder, convert it to a format compatible with the current version of HAP and save the
data in the current project. When the conversion is finished, the program displays a message indicating whether the data translation was successful or failed. Important
information about the data conversion can be displayed by pressing the Help button in this message window, or via the following topic: About Translation of HAP v3.2 Data.
Finally, when you return to the HAP main program window, the data you converted will be displayed.
How Previous Version Data is Converted. When data from the previous version of HAP is converted to be compatible with the current version, it is "translated" rather than
"transferred". It is important to make a distinction between "translation" of data and "transfer" of data:
a. "Data Transfer" refers to the simple copying of data. The result of a data transfer is an exact copy of the original data. No data is added, deleted or modified.
b. The result of "Data Translation" is the original data with missing items added, unusable items discarded and other items reorganized.
Because HAP v3.2 data is being translated across multiple HAP releases, significant changes to data content can occur. To view information about items adjusted during
translation and about which categories of data are converted, press the Help button in the status message window that appears at the end of the translation process or click here:
About Translation of HAP v3.2 Data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Publishing Equipment Sizing Requirements for use in E-CAT
The Publish Equipment Sizing Requirements option on the Project Menu is used to electronically link HAP sizing results with Carrier Electronic Catalog (E-CAT) to make
selecting equipment faster and easier. A toolbar button is also provided for this purpose.
The traditional process for equipment selections involves first running a system design tool like HAP to generate equipment sizing requirements, then printing the requirements,
and finally manually entering the requirements into an equipment selection tool like E-CAT. With the Publish option in HAP the printing and manual data entry steps are
eliminated. Once you Publish equipment sizing requirements, the data is immediately available to drive equipment selections in E-CAT.
There are two ways to use the Publish feature to make equipment selections easier. The first is the collaboration scenario where you are doing the design work and your Carrier
sales engineer is assisting you with selections. This procedure is described in part A below. The second is the do-it-yourself scenario where you are doing both the design work
and the equipment selections. This procedure is described in part B below.
A. Collaboration Scenario
1. Use HAP to perform sizing calculations for your air systems and plants (if applicable).
2. When the design is finished and you're ready for equipment selection, select the "Publish Equipment Sizing Requirements" option on the Project Menu, or click the
corresponding toolbar button.
3. In the Publish Equipment Sizing Requirements window (Figure 1), select the systems and/or plants whose sizing requirements you wish to publish. This window consists of a
list of all systems and plants in the current project for which sizing calculations have been run. To select an item in the list, check the box to the left of the item. When finished
choosing items to publish, press the OK button.
Figure 1. Publish Equipment Sizing Requirements
4. Next, choose the "E-mail Sales Engineer" option on the Project Menu or click the corresponding button on the toolbar. This feature is used to send an archive of your project to
your Carrier sales engineer so he or she can use the data to perform equipment selections. Note that you should always check with your Carrier sales engineer before sending
e-mail. Click here for information about e-mailing data to your sales engineers.
B. Do-It-Yourself Scenario
1. Use HAP to perform sizing calculations for your air systems and plants (if applicable).
2. When the design is finished and you're ready for equipment selection, select the "Publish Equipment Sizing Requirements" option on the Project Menu, or click the
corresponding toolbar button.
3. In the Publish Equipment Sizing Requirements window (Figure 1), select the systems and/or plants whose sizing requirements you wish to publish. This window consists of a
list of all systems and plants in the current project for which sizing calculations have been run. To select an item in the list, check the box to the left of the item. When finished
choosing items to publish, press the OK button.
4. HAP will then publish data for the systems and plants you selected. For each system or plant selected one or more equipment tags will be generated. For example, for a 45-
zone water-source heat pump system, 45 equipment tags would be created - one for each heat pump unit.
5. Next, run Carrier X Builder Framework.
6. In the project tree on the left side of the X Builder main window, click the "+" symbol next to the project containing your design data to open the project (the same project used
in steps 1-4). Then click the "+" symbol next to the Tags item in this project to display the equipment tags in the project. The list of tags will include all those tags you created
with the Publish option in steps 2-4.
7. Single click on an equipment tag item to display information about the tag.
8. Double-click on an equipment tag item to launch the product wizard which allows you to perform a select-by-performance calculation. Many of the equipment sizing
requirements displayed in the product wizard screens default using data obtained from HAP. Finally, from the list of candidate selections meeting your requirements, choose
the equipment unit you wish to use.
Page 31 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Sending Email to Your Sales Engineer
1.0 Getting Started ›› 1.5 Working with Projects ››
Exporting Building Simulation Data for use in Engr. Economic Analysis
1.0 Getting Started ›› 1.5 Working with Projects ››
Importing Data From Another Project
1.0 Getting Started ›› 1.5 Working with Projects ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Sending Email to Your Sales Engineer
The Send Email to Sales Engineer option on the Project Menu is used to automatically archive the current project and e-mail it to your Carrier sales engineer so the sales
engineer can perform equipment selections against your data.
Integration features that link HAP with the Carrier Electronic Catalog (E-CAT) Builder programs are steadily being added. These electronic links between HAP and Builder
programs can increase your productivity. It is no longer necessary to print the sizing results and manually enter the data into a Builder program to run selections. Now this data
can flow electronically between programs.
You can use HAP sizing results in a Carrier E-CAT Builder to select equipment yourself. Or you collaborate with your sales engineer to have the sales engineer do the selections.
In the latter case, the "Send Email to Sales Engineer" feature helps with this collaboration.
When collaborating with your Carrier sales engineer, its important to do four things before using the "Send Email..." feature:
a. Contact your Carrier sales engineer to make sure he or she is able to assist you with equipment selections.
b. Make sure you have specified the e-mail address of your Carrier sales engineer via the Preferences option on the View Menu.
c. Make sure you have finished running system design calculations for your systems in your project.
d. Use the Publish Equipment Sizing Requirements button on the HAP toolbar to generate the requirements needed by E-CAT programs for making selections.
Once you're ready to send data, steps in the process are as follows:
1. Select the "Send Email to Sales Engineer" option on the Project Menu or press the "Send Email..." button on the toolbar.
2. HAP will automatically save your current project, if necessary.
3. HAP will then automatically archive the project. You'll be asked to name the archive file.
4. HAP will then launch your e-mail software, create an e-mail addressed to your Carrier sales engineer and attach the archive file to the e-mail.
5. You will need to add the subject for the e-mail and write the e-mail message asking your sales engineer to select equipment against the systems in your project. Finally press
the Send button to send the e-mail.
Notes:
a. The "Send Email..." feature requires that you use e-mail software installed on your computer hard disk. This is called "client-based" e-mail. In addition the software must
comply with the Microsoft MAPI standard for email messaging. Most client-based e-mail software does comply. Examples include Microsoft Outlook and Eudora. Note that if
you use web-based e-mail like Yahoo or Hotmail, the feature will not work. In that case you use an the alternate approach - use the archive option on the Project Menu to
archive your project and then compose an e-mail to your sales engineer and attach your archive file.
b. Some configurations of computers, computer networks, or e-mail software will prevent the "Send Email..." feature from working. This is typically due to security settings that
prevent a software program from remotely launching your e-mail program or from remotely creating e-mail messages. If this problem exists, an error message will appear
when you try to use the "Send Email..." feature. One possible solution is to make sure your e-mail software is running before you use the feature in HAP. If this does not
resolve the problem, you will need to create and send the e-mail yourself by running your e-mail software, creating a message and attaching the HAP archive file.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Exporting Building Simulation Data for use in Engr. Economic Analysis
The Export to Engineering Economic Analysis option on the Project Menu shares HAP data with the Carrier Engineering Economic Analysis (EEA) program to help you construct
and perform lifecycle studies more efficiently. HAP will export energy cost data and equipment lists from your building simulations for use in the EEA program. A toolbar button is
also provided for this purpose.
The following procedure is used to export and then incorporate cost data in a lifecycle analysis:
1. Use HAP to create a building energy analysis which culminates in running the building simulation calculation.
2. Select the Export to Engineering Economic Analysis option on the Project Menu or the click the corresponding toolbar button. HAP will automatically export energy cost data
for all simulated buildings in your project.
3. Start the Engineering Economic Analysis (EEA) program.
4. In the EEA program, open the project which contains the HAP energy analysis data. To do this, choose Open on the Project Menu. In the Open Project window, set the filter at
the bottom of the window to "Show all Projects" and then select the project.
5. Then create a "Study" in EEA using the New option on the Study Menu.
6. With your new Study highlighted in the tree, choose the Import HAP Data option on the Study Menu. HAP cost data will be imported. For each simulated building in HAP, a
separate Design Case will be created within the Study.
7. Finally, edit these Design Cases to add further information about investment and maintenance costs. In each Design Case you will see a list of HVAC equipment in the
investment cost table that is defaulted from HAP data for your building design - you will need to add purchase and installation cost data for these. You will also see energy cost
information in the operating cost table defaulted from HAP results for the building simulation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Importing Data From Another Project
The Import HAP Project Data option on the Project Menu is used to transfer data from another HAP project into the current project. This option has two major applications:
1. Transferring one or a few categories of data from one project into a new project. For example, you may use similar wall, roof or window assemblies in all your projects. Rather
than manually recreating this data in each new project, you can use the Import HAP Project Data option to transfer wall, roof and window assemblies from an existing project
into your new project.
2. Merging whole projects together. For large building projects, individual project team members sometimes model parts of the building in separate HAP projects early in the
project. Later in the project cycle, team members may wish to combine their work together into one large project for final design or simulation calculations. The Import HAP
Project Data option provides a quick way of merging projects together.
The Application Information discussion at the end of this topic explains how to use the Import HAP Project Data option for each of these scenarios.
Page 32 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Basic Procedure. Data is imported using the following procedure.
1. Run HAP and open the project you want to import data into. This project is the destination for imported data.
2. Choose the Import HAP Project Data option on the Project Menu.
3. The Select Project window will appear. It allows you to choose the HAP project from which you want to import data. This is the source of imported data.
4. The “Select Data to Import” window appears next as shown in the figure above.. It is used to specify the data items in individual data categories you wish to import. Your work
with this window involves selecting a data category (in the left-hand panel) and then selecting items in that category (in the center panel) to be imported. Repeat this process
for all categories you wish to import data from. Press the Import button in the lower right when ready to import the selected data.
The window contains four key components:
a. The Data Categories box on the left lists the data categories from which items can be imported. To select a particular data category click on its name. It will be highlighted
to show it is selected. In the figure above Schedules has been selected.
b. The Source Project box in the center of the window lists items available for importing from the source project. To select an item place a check mark in the box next to the
item. To quickly select all items in the category, press the “Select All” button below the list box. To quickly unselect all items, press the “Unselect All” button. In the figure
above the source project contains four schedules. The first three have been selected and will be imported.
c. The Current Project box on the right lists items in the selected data category in the current project. This information is provided for reference only. Often it is useful to
review the contents of the current project before deciding which items to import from a source project. In the figure above the current project does not contain any
schedules yet.
d. Command Buttons appear in the lower right part of the window. Press Import to import the items you selected. As mentioned earlier items from multiple categories can
be imported all in one session. Press Cancel to exit without importing data. Press Help to display this help topic.
5. Next, the Import Data confirmation window appears as shown below. It lists the number of data items selected in each data category and provides a chance to review and
approve your selections. If the quantities are correct, press the Yes button to continue. To revise selections press the No button to return to the Select Data to Import window.
6. The data you selected will then be imported from the source project into the current project. A status monitor will show the progress of this work.
7. When data has been imported a confirmation window will appear. Its appearance is similar to the Import Window shown above. Its purpose is to confirm the data imported
successfully. In most cases the quantities shown in the confirmation window will match those in the original Import Data window. However, when you select data categories
with linked items, the number of items shown as imported on the second confirmation window will be larger than on the first. For example, if you selected spaces to be
Page 33 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Importing Data From a gbXML File
1.0 Getting Started ›› 1.5 Working with Projects ››
imported, these spaces may link to one or more schedules, wall, roof, window or door assemblies, or to external shade geometries. To provide a complete representation of
the spaces you requested, HAP will automatically identify and import all linked schedules, walls, roofs, windows, doors, and shade geometries. These linked items will then be
included in the tally on the second confirmation screen. Data categories in a HAP project that have linked items are spaces, air systems, plants, buildings and, in some cases,
electric rates and fuel rates.
Note: There is only one situation where data is changed while being imported. If the source project (the project you are importing from) uses a different Ventilation Standard
preference than the destination project (the project you are importing to), the imported data must be adjusted so it will be compatible with the destination project. This involves
setting space usage value to "user-defined" and changing the ventilation standard setting for each space. In air systems, the ventilation calculation method input is
synchronized with the destination project's ventilation preference. For example if a system being imported uses "ASHRAE Standard 62.1-2004" as the calculation method,
and the destination project uses "ASHRAE Standard 62.1-2007" as the project preference, the air system will be altered to use 62.1-2007 as the ventilation calculation method.
Application Information. The general steps above should be applied as follows for the two major applications of the Import HAP Project Data option:
(A) Transferring One or a Few Categories of Data from One Project to Another
1. Run HAP. Open the "destination" project you want to import data into. This is often a new project..
2. Choose the Import HAP Project Data option on the Project Menu.
3. Select the "source" project from which data will be imported. This may be another existing project or a project you have set up as a "template", containing commonly used data
that you import into each new project you create.
4. In “Select Data to Import” window choose the first data category you wish to import in the left-hand panel, and then the individual items you wish to import from that category in
the middle panel.
5. Repeat step 4 for each category of data you want to import.
6. Click the Import button.
7. Check the data on the confirmation window. If data is correct, press Yes to import the data.
(B) Merging Whole Projects
1. Run HAP. Open the "destination" project you want to import data into. This could be a new project, or more frequently it will be an existing project that contains a portion of
the building you are modeling.
2. Choose the Import HAP Project Data option on the Project Menu.
3. Select the "source" project from which data will be imported. This will be a project containing one of the other portions of the building being modeled.
4. In “Select Data to Import” window choose the "Building" category in the left-hand panel. Typically for merge scenarios, there will only be one Building item in the project.
Check the box to select that item.
5. Click the Import button.
6. Check the data on the confirmation window. If data is correct, press OK to import the data.
7. Repeat steps 2 through 6 if there are further projects containing portions of the building that need to be merged into the current project.
As noted earlier, the Import option imports the data you selected and the software identifies all linked items and automatically imports those as well. Therefore if you select one
Building item for import, HAP will import that Building and will automatically import all plants, air systems, spaces, schedules, walls, roofs, windows, doors, shades, chillers,
towers, boilers, electric rates and fuel rates it identifies as linked to that Building. In this way the full content of a building from the source project can be combined into the
destination project.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Importing Data From a gbXML File
The Import gbXML Data option on the Project Menu is used to read data from a gbXML-format file created by another software program and use it to automatically generate
HAP space, wall, roof, window, door and schedule data. This feature can help you greatly reduce the time and effort needed to transfer building information from floor plan
drawings into HAP for use in load calculations and energy analyses. For example, you might use a CAD tool to extract floor plan information from drawing files and write the data
in gbXML format, and then use HAP to read the gbXML to produce spaces and construction data. This electronic transfer replaces the manual process of taking data off drawings
and manually entering it into HAP.
About gbXML. gbXML is increasingly being accepted as a neutral format for exchanging building data between such tools as Computer Aided Drafting (CAD), Building
Information Modeling (BIM) and engineering analysis software programs. "gbXML" stands for "green building XML". "XML stands for "extensible mark-up language" which is a
language for representing information. While the name suggests a use for green building applications, gbXML is usable for any application, green or otherwise. Certain CAD
software vendors offer tools to produce gbXML-format files from CAD drawings or BIM data. As long as a tool generates gbXML data which conforms to the gbXML
"schema" (the rules for formatting the data) v0.34 or later HAP will be able to read and translate the gbXML data.
Typical Operating Procedure. The typical procedure for creating, importing and using gbXML data generated from CAD drawings involves the following steps.
1. CAD floor plan drawings for a building are created or received.
2. Use your CAD-related tool to extract information from the floor plan drawings and save the data in gbXML format.
3. Run HAP.
4. If importing data for the first time for this building, create a new, untitled project. Or, if drawings have been revised and you are updating data you previously imported into HAP,
then open the project that contains the building data.
5. Choose the "Import gbXML" option on the Project Menu.
6. In the Choose gbXML File window, choose the gbXML file you created in step #2.
Page 34 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
7. If the project already contains data (as when you are updating previously imported data), you will be asked whether the gbXML should be used to "Replace Existing" items or
to "Create New" items. For more information about this feature click here: Replace Existing Feature.
8. HAP will then read the gbXML and translate the data into a format HAP can use.
9. At the end of the translation, HAP will ask if you’d like to display the gbXML Translation Report. This report summarizes the space data that was imported and also lists any
problems encountered during the translation. For more information on this report, click here: gbXML Translation Report.
10. When the program returns to the Main Window, save the project.
11. Then review, revise and add to the imported data. Tools that create gbXML provide varying quantities of information which ranges from simple to extensive. The amount of
building data written to gbXML depends on the tool you use and the amount of effort invested before exporting the gbXML. For example, if the gbXML file only contains
information about surface areas for walls, roofs, windows, doors, and floors, you will need to add information about constructions, internal loads, infiltration, etc... after the data
has been imported in order to complete the definition of the spaces.
Note: Its best not to revise the names of imported items such as spaces, walls, roofs, windows, doors or schedules. If you anticipate updating data later when building
drawings are revised, you’ll need the original item names in order to match the revised data with the original data. See the "Tips for Optimizing Transfer" paragraph below for
more details.
12. Finally you can proceed with creating the rest of your analysis to calculate loads, size equipment and estimate energy costs.
Tips for Optimizing Transfer. The following tips can make your use of the data more efficient once it has been imported into HAP.
1. Provide meaningful names to items before exporting gbXML. Tools which generate gbXML allow you to assign names to spaces, wall assemblies, roof assemblies, etc...,
or will default them if you don’t assign names. Your use of the data after it is imported into HAP will be easier if you assigned meaningful names to items so you can tell them
apart. If you don’t assign names before gbXML is exported, some tools assign the same name to all items. For example, all spaces might be named "Engineering Space".
Even though HAP will import the names as "Engineering Space(1)", "Engineering Space(2)" to differentiate them, it tends to be harder to work this kind of data than if the
spaces have meaningful names like "Room A101", "Room A102" etc...
2. Provide unique names to items before exporting to gbXML. When naming items before gbXML is exported, it is important to assign unique names to the items. This is
critical if you anticipate importing gbXML into HAP multiple times during the course of the project as floor plan drawings are revised. The "Replace Existing" feature (mentioned
earlier) uses the item names to determine what existing HAP data must be replaced with new data from gbXML. For example, if the software finds a space named "Room
A101" in gbXML, it will search for a space with the same name in HAP in order to determine what data should be replaced. If unique names are not used in the tool that
exports gbXML, HAP will not be able to match items and correctly replace the data. For example, if every space in the CAD tool is named "Engineering Space" and the spaces
in HAP are named "Engineering Space(1)", "Engineering Space(2)", etc.., when HAP imports the data a second time it will not be able to match the gbXML space data named
"Engineering Space" with existing spaces in HAP with names like "Engineering Space(1)" and therefore will not be able to replace the existing data.
3. Provide unique names for each unique window, skylight or door before exporting to gbXML. If the tool you use to generate gbXML allows you to create window, skylight
or door construction data, special care needs to be taken when assigning unique names to these constructions. A unique window, skylight or door construction should be
defined in gbXML for each unique set of dimensions for the window, skylight or door. The definition of a window or skylight construction in gbXML is limited to the performance
data only – U-value and Solar Heat Gain Coefficient or Shade Coefficient. Similarly, the door construction in gbXML is limited to U-value. The same construction can be
assigned to windows, skylights or doors of different sizes. In HAP, however, a window, skylight or door is defined both by its performance data and its size. Therefore, in HAP
a 3x5 window and a 3x6 window are two different window assemblies, where in gbXML the two different sized window openings might use the same gbXML "window type". If
you use one window type in gbXML for multiple window openings of different sizes, HAP will import multiple versions of these as "Window(1)", "Window(2)", etc.. for each
different set of dimensions. If you want to use the "Replace Existing" feature during the course of the project, you will encounter the same sort of problem with these
constructions as described for spaces not having unique names in item #2 above. Therefore, it is important that each unique set of dimensions and performance data for a
window, skylight or door be assigned a separate construction in gbXML and be uniquely named.
Data Which is Imported. Tools that generate gbXML provide varying quantities of information. The amount of building data written to gbXML depends on the tool you are using
and the amount of effort you invest before generating the gbXML. At a minimum most tools export information about building surfaces – the dimensions and orientations of floor,
wall, roof, window, skylight and door surfaces. Some tools add the ability to define and export information about lighting, occupants, electrical equipment, and information about
wall, roof, window, skylight and door constructions. A few tools allow hourly operating schedules to be defined. HAP will import a wide variety of building information from gbXML,
but it is ultimately limited by what is written to gbXML in the first place. HAP is able to import the following types of information.
1. Space Name
2. Surface geometry for spaces – dimensions, gross areas and orientations for:
a. Floors – Above grade, on grade, below grade.
b. Exterior Walls – Above grade, below grade.
c. Roofs
Page 35 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Create New or Replace Existing when Importing gbXML
1.0 Getting Started ›› 1.5 Working with Projects ››
d. Exterior Windows
e. Exterior Skylights
f. Exterior Doors
3. Building Weight – HAP will automatically compute the building weight for the space based on the size and construction of all surfaces associated with a space, including all
types of floors, ceilings, roofs, interior walls and exterior walls. If construction data is not supplied for one or more surfaces, building weight cannot be calculated and HAP will
assign a default building weight.
4. Occupants
a. Quantity of occupants.
b. Sensible and latent heat gain per occupant.
c. Occupant hourly schedule.
5. Overhead Lighting
a. Overhead lighting W/sqft or W/sqm.
b. Overhead lighting hourly schedule.
6. Electrical Equipment
a. Electrical equipment W/sqft or W/sqm.
b. Electrical equipment hourly schedule.
7. Infiltration Airflow
a. A single ACH infiltration airflow can be defined in gbXML and is assigned to design cooling, design heating and typical conditions in HAP.
8. Wall Assembly
a. Exterior surface absorptivity
b. Interior surface resistance.
c. Thermal properties of all material layers in the wall.
d. Items a-c are used to compute the overall U-value, weight and conduction transfer function coefficients for the wall.
9. Roof Assembly
a. Exterior surface absorptivity
b. Interior surface resistance.
c. Thermal properties of all material layers in the wall.
d. Items a-c are used to compute the overall U-value, weight and conduction transfer function coefficients for the roof.
10. Window Assembly
a. Window dimensions
b. Solar heat gain coefficient (SHGF) or Shade Coefficient (SC)
c. U-value.
11. Door Assembly
a. Door dimensions
b. U-value.
12. Fractional Schedules
a. Hourly profile values (percent of full internal heat gain)
b. Assignments of profiles to days of the week and times of year.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Create New or Replace Existing when Importing gbXML
When importing gbXML into a HAP project that already contains data, your intention may be to replace the existing items in HAP with data from gbXML, or to create new items
from the gbXML. This message window allows you to specify which approach should be used when importing data. The message only appears when the project you’re importing
data into contains at least one space, schedule or wall, roof, window, or door assembly.
Example #1: Originally you imported gbXML for a floor plan drawing into a new, untitled project, then saved the project and added further data in HAP to allow you to run load
calculations. Later you receive revised floor plan drawings and wish to generate new gbXML from the drawings and import it into HAP to replace data for the existing spaces.
Therefore, you would use the "Replace Existing" option.
Example #2: You originally created a project and manually entered spaces. Now you wish to add to this project by importing gbXML for a floor plan drawing to create additional
spaces. In this situation you would choose the "Create New" option to create a new set of spaces in the project from the gbXML.
More about "Replace Existing". When the "Replace Existing" option is selected, HAP will try to match each item from gbXML with a corresponding item in your HAP project
using the item name. For example, if gbXML contains a space named "Room A101", the software will search for a space in HAP project of the same name. If a match is found,
data for that HAP space will be replaced with the new gbXML data. Otherwise, a new space will be created. This procedure is used for spaces, schedules, and wall, roof, window,
skylight and door assemblies. By replacing data in this way, rework after the new gbXML data is imported can be minimized.
Notes:
a. For any item that is replaced, all data for the item replaced. For example, suppose you originally imported data for a space and then added or modified the content of the space
afterwards. If you import updated gbXML at a later time using "Replace Existing", all data for that space will be replaced, including the additions or modifications you made.
This is true for spaces as well as any schedules or wall, roof, window, skylight or door assemblies imported from gbXML.
b. If a space, schedule or wall, roof, window, skylight or door assembly in your HAP project was not imported from gbXML, then its content will not be affected by importing
updated gbXML.
c. For air systems in your project which serve spaces imported from gbXML, the air system input data will not be affected. However, you will need to rerun any system design and
energy simulation calculations since revising space data through a gbXML import invalidates prior calculation results.
Possible Pitfalls:
a. If item names in gbXML are not unique, the translation software will not be able to match data from gbXML with existing data in HAP, and therefore cannot replace existing
data. For example, if every space in the CAD tool was named "Engineering Space", then all spaces in gbXML will have this name. HAP will originally import these spaces as
"Engineering Space(1)", "Engineering Space(2)", etc... to differentiate them. However, when you try to update data, the space names from gbXML cannot be matched with the
space names in HAP. Therefore it is critical to supply unique names to all items in the CAD tool before gbXML is exported.
b. A similar problem exists for window, skylight and door assemblies. Unique names must be supplied for each unique combination of opening dimensions and thermal
performance for a window, skylight and door.
c. If item names are modified in HAP after data was imported, the software won’t be able to match item names when "Replace Existing" is used. For example, if the space name
in gbXML is "Room 1100", but the space name is modified in HAP after it is imported to "Room A1100", the "Replace Existing" feature will not be able to match names and
therefore cannot update the space data.
Page 36 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Importing Data From a Building System Optimizer Project
1.0 Getting Started ›› 1.5 Working with Projects ››
1.6 Performing Common Tasks
1.0 Getting Started ››
1.6.1 Performing Common Tasks
1.0 Getting Started ›› 1.6 Performing Common Tasks ››
Performing Common Tasks
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.1 Performing Common Tasks ››
More about "Create New". When the "Create New" option is used the translation software will create a new item in HAP for each item found in gbXML. This is the same mode of
operation used when importing gbXML into a new, empty project.
Possible Pitfall
a. If you use "Create New" when updating an existing project, a second set of imported data will result. For example, if the original import produced spaces "Room A100", "Room
A101", etc... The second import of data for the same building will produce spaces "Room A100(1)", "Room A101(1)", etc... because HAP requires unique item names. This
second set of items may make it inefficient to differentiate items and work with the data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Importing Data From a Building System Optimizer Project
The Import BSO Project Data options on the Project Menu are used to transfer data from a Building System Optimizer (BSO) project of the indicated version into a HAP project.
Building System Optimizer is one of the tools in the Carrier eDesign Suite of software. It is designed for rapid energy modeling and screening of alternatives during the
schematic design phase of projects.
These options have two major applications:
1. Transitioning from Schematic to Detailed Design Phase – If BSO was used to evaluate HVAC design alternatives during the schematic design phase of a project, and you
wish to transfer those alternatives into HAP for further study during the detailed design phase, the import option can be used to accomplish this.
2. Acquiring Data from your Sales Engineer – If your Carrier sales engineer is using BSO to demonstrate HVAC system design or equipment concepts to you, and you want to
study those scenarios in more detail in HAP, the import options can be used to transfer your sales engineer’s BSO project data into your HAP project.
Basic Procedure. Data is imported using the following procedure.
1. Start HAP.
2. If your source data is from BSO v1.6 choose the Import BSO v1.6 Project Data option on the Project Menu.
3. The Import BSO Project Data window will appear. Choose whether you want to import data from a project archive file, or from an active project on your computer.
4. If you selected “Archive File”, a file selection window will appear next. Select the Building System Optimizer archive file you want to import. Then press OK.
5. If you selected “Project”, a Select Project window will appear. It will list available active BSO projects. Select a project and press OK.
6. HAP will then create a new untitled project, data will be read from the archive file or from the active project you selected, and will be written into the untitled HAP project.
7. When the import is complete you can inspect the data and then save the project.
Note: Building System Optimizer input screens are similar to those in the HAP Full Wizard session. They only deal with high level descriptions of weather, the building, HVAC
alternatives and utility rates. When data is imported from BSO into HAP, the data is transformed into the detailed input data that appears in HAP’s detailed interface. The
imported data will not appear in the HAP Wizard screens. This process is similar to the operation of a HAP Full Wizard session – you first enter high level data into the wizard
input screens and then press Finish. HAP transforms the high level inputs from the Wizard screens into a detailed HAP model. This kind of detailed HAP model is what is
produced when importing a BSO project.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks associated with inputting data and generating reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of common tasks coverd in section 1.6 and the basic operating procedure for manipulating data in the program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Performing Common Tasks
While designing and analyzing systems with HAP, a common set of procedures is used to enter data, modify data and generate reports. Using common procedures to operate
the program makes the program easier to learn and simpler to use. Whether you are working with walls, spaces or systems, for example, the same basic procedures are used.
Page 37 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Basic Procedures for Performing Common Tasks
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.1 Performing Common Tasks ››
1.6.2 Working with Input Data
1.0 Getting Started ›› 1.6 Performing Common Tasks ››
Creating a New Item
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
For an explanation of the basic procedures that apply to all common tasks, click here: Basic Procedures. For a discussion of the specific procedures used to perform a common
task, click on any of the following:
Creating a New Item
Editing an Existing Item
Using the On-Line Calculator to Enter Data
Duplicating an Existing Item
Duplicating a Building with all of its Spaces and HVAC Equipment
Deleting Items
Generating Input Reports
Generating Design Reports
Searching and Replacing Space Data
Rotating Space Orientations
Performing LEED (90.1 PRM) Rotations
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basic Procedures for Performing Common Tasks
Common tasks such as entering, editing or deleting data use the same basic procedure which is explained below.
1. Select the Data Category by clicking on the desired item in the tree view panel on the left-hand side of the HAP main window. For example, if you need to work with Space
data, first click on the "Space" item in the tree view panel. This will cause a list of spaces in your project to appear in the list view panel on the right side of the HAP main
window.
2. Select One or More Items from the list view panel on the HAP main window. For example, when working with spaces, select one or more space items from the list of spaces
in your project. There are four ways to select items:
a. Selecting a Single Item - Click once on the name of the item you wish to select. The name will be highlighted indicating is has been selected.
b. Selecting Multiple, Consecutive Items - While pressing the [Shift] key on the keyboard, click on the name of the first and last items in the group you wish to select. The
names of all items in the group will be highlighted to indicate they are selected.
c. Selecting Multiple, Non-Consecutive Items - While pressing the [Ctrl] key on the keyboard, click on the name of each item in the group you wish to select. Each name will
be highlighted to indicate it is selected.
d. Selecting All Items in the Category - Choose the Select All option on the Edit Menu (on the menu bar). The names of all items shown in the list view will be highlighted
indicating they are selected.
3. Perform the Task on the selected items. Particular tasks such as entering or editing data can usually be performed by several different methods. Users are free to choose the
method that is most convenient. These methods include the following. Which methods can be used for each task will be explained in subsequent sections of this appendix.
a. Menu Bar. Often an option on the Edit Menu or Report Menu on the main window menu bar can be used to perform the task.
b. Toolbar. In many cases one of the buttons on the main window toolbar can be used to perform the task.
c. Item Pop-Up Menus. Right-clicking on the group of selected items will display the item pop-up menu which usually will contain an option for performing the task.
d. Category Pop-Up Menus. Right-clicking on the selected category in the tree view panel will display the category pop-up menu. Note that selecting an option on this pop-up
menu will perform the task on ALL items in the category, not just those currently selected. Therefore, category pop-up menus should be used carefully.
e. Direct Use of the Keyboard. In some cases the keyboard keys can be used to directly perform a task.
f. Special Features. There are also cases where special additional methods are provided for performing tasks. These will be explained in the subsequent sections where they
apply.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains common tasks for inputting data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Item
There are three ways to create new items in HAP. The example below deals with wall data, but the procedure can be used for any category of data in HAP. Simply substitute
your category name for "wall" in the following description.
To create a new wall item:
1. Select the Wall category in the tree view pane on the left side of the main window. A list of walls in the project will appear in the right-hand list view pane.
2. Use one of the following three methods to create a new item.
a. Select the "New Default…" item in the list view pane.
b. Right click on the Wall item in the tree view panel to display the category pop-up menu. Then select the "New" option in this pop-up menu.
c. Use a special feature to create a new wall from within one of the program input forms. See details below.
3. After creating the new wall, the input form will appear. Enter data for the wall and then press OK to save the data and return to the HAP main window.
Special Feature. Certain categories of data can be created from within other input forms. For example, while entering space data on the space form, you can create a new wall
as follows:
Page 38 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Editing an Existing Item
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
1. While editing data in the Space Input Form on the "Walls, Windows Doors" tab, choose the "create new wall" item in the wall drop-down list. The wall input form will then
appear.
2. Enter the desired wall data including the wall name.
3. Click the OK button to save the wall and return to the space input form. When you return to the space form, the wall you created will automatically be selected for use in the
space.
Note that this method can only be used to create the following kinds of new items:
While Entering Data
In the Following Form:
You Can Create the Following
Kinds of New Data Items:
Spaces
Schedules (Fractional)
Spaces
Walls
Spaces
Roofs
Spaces
Windows
Spaces
Doors
Spaces
External Shading
Systems
Schedules (Fractional)
Systems
Schedules (Fan/Thermostat)
\*Systems
Cooling Towers
\*Systems
Boilers
\*Plants
Chillers
\*Plants
Cooling Towers
\*Plants
Boilers
\*Electric Rates
Schedules (Time-Of-Day Utility Rate)
\*Fuel Rates
Schedules (Time-Of-Day Utility Rate)
\*Buildings
Schedules (Fractional)
\*Buildings
Electric Rates
\*Buildings
Fuel Rates
\*Items marked with an asterisk are available in HAP but not HAP System Design Load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Item
There are three ways to edit existing items in HAP. The example below deals with editing an existing schedule, but the procedure can be used for any category of data in HAP.
Simply substitute your category name for "schedule" in the following description.
To edit an existing schedule item:
1. Select the Schedule category in the tree view pane on the left side of the main window. A list of schedules in the project will appear in the right-hand list view pane.
2. Use one of the following three methods to edit a schedule item.
a. Double-click on the schedule item in the list view pane.
b. Right-click on a schedule item in the list view pane to display its pop-up menu. Then select the "Properties" item on this menu.
c. Use a special feature to edit an existing schedule from within one of the program input forms. See details below.
3. After displaying the data to edit, make the necessary changes. Then press OK to save the changes and return to the HAP main window.
Special Feature. Certain categories of data can be edited from within other input forms. For example, while entering space data on the space form, you can edit data for any
schedule linked to that space as follows:
1. While editing data in the Space Input Form on the "Internals" tab, press the "Schedule" button next to any one of the Schedule drop-down lists. The input form for the currently
selected schedule will appear and changes can be made to that schedule.
2. Make changes to the schedule.
3. Click the OK button to save the changes and return to the space input form.
Note that this method can only be used to edit the following kinds of data:
While Entering Data
In the Following Form:
You Can Edit the Following
Kinds of Related Data Items:
Spaces
Schedules (Fractional)
Spaces
Walls
Spaces
Roofs
Spaces
Windows
Spaces
Doors
Spaces
External Shading
Systems
Schedules (Fractional)
Systems
Schedules (Fan/Thermostat)
\*Systems
Cooling Towers
\*Systems
Boilers
\*Plants
Boilers
\*Electric Rates
Schedules (Time-Of-Day Utility Rate)
\*Fuel Rates
Schedules (Time-Of-Day Utility Rate)
Page 39 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Using the On-Line Calculator to Enter Data
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
Duplicating an Existing Item
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
Duplicating a Building (with Spaces and HVAC Eqpt)
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
\*Buildings
Schedules (Fractional)
\*Buildings
Electric Rates
\*Buildings
Fuel Rates
\*Items marked with an asterisk are available in HAP but not HAP System Design Load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using the On-Line Calculator to Enter Data
While entering data, you may encounter situations in which you don’t have data for an input item, but you have related information. For example, when entering the space floor
area you may know the length and width of the floor but not its area. Rather than calculate the floor area by hand, you can use an on line calculator to calculate the value and
insert it into the input item.
For HAP users, most numeric inputs in the energy analysis portions of the program (plants, buildings, chillers, cooling towers, boilers, electric rates and fuel rates) provide an
integrated on-line calculator. To use this calculator, simply enter an equation followed by the equal sign. For example, if you want to multiply 20 by 9, type the equation 20\*9=.
When you press the [=] key the equation will be calculated and the result (180) will be inserted into the input item. The calculator recognizes the following mathematical symbols:
a. Multiplication: \* Example: 20\*9=
b. Division: / Example: 100/5=
c. Addition: + Example: 46.1+85.9=
d. Subtraction: Example: 100-84=
In addition, compound equations can be entered if necessary. For example: 100-9\*8+12=
For both HAP and HAP System Design Load users, the system design portions of the program (weather, spaces, systems, walls, roofs, windows, doors, external shades) do not
yet offer this integrated on-line calculator feature. Until these portions can be upgraded to include the integrated calculator, the Windows On-Line Calculator must be used
instead. The following example illustrates how to use the Windows calculator.
Example: You need to enter the floor area for a space, but you only know the floor dimensions are 17 ft by 32 ft. The Windows Calculator can be used to compute the floor area
and then insert it into HAP as follows:
1. Start the Windows Calculator: From the Windows desktop, press Start. On the Start Menu choose Programs. On the Programs Menu choose Accessories. On the Accessories
Menu choose Calculator. If you don’t need the calculator right away, minimize the Calculator window by pressing the minimize button on the Calculator title bar. The calculator
will be available for use whenever you need it.
The Windows Calculator is a program supplied with the Windows operating system. For typical Windows installations it is placed in the Accessories program group.
2. While running HAP and entering space data, display the Calculator by pressing the Calculator button that appears on your taskbar. The Calculator will appear.
3. Calculate the floor area by pressing the calculator keypad buttons for the equation 17 \* 32 = . The result (544) will appear in the calculator display.
4. Copy the result to the clipboard: Choose the Edit option in the Calculator menu bar. Then choose the Copy option on the Edit Menu. This copies the result of your equation
(544) to the Windows clipboard.
5. Return to HAP and place the cursor in the floor area text box by clicking once on this text box so the default floor area is highlighted.
6. Finally, on your keyboard, hold the [Shift] key down and press [Ins]. This inserts the contents of the Windows clipboard into the input field. The value 544 will appear as your
floor area, replacing the previous floor area value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating an Existing Item
While entering data, it is often useful to create new items using defaults from an existing item. For example, a series of spaces in a building might use the same wall and window
constructions and the same lighting levels and schedules. Defining this series of spaces with each new space based on the last space’s data can yield a tremendous increase in
productivity. You only need to change a handful of space inputs for each successive space, rather than specifying every input item for each space.
The Duplicate feature in HAP is used for this purpose. For example, when you duplicate a space, a new space is created using input data from the original space as defaults.
Many readers will be familiar with the Copy and Paste features commonly offered in Windows software. HAP’s Duplicate feature combines Copy and Paste into one function. So
in one step, Duplicate lets you make a copy of an item and paste it into your project.
There are three ways to make a duplicate of an existing item in HAP. The example below deals with duplicating an existing space, but the procedure can be used for any
category of data in HAP. Simply substitute your category name for "space" in the following description.
To duplicate an existing space:
1. Select the Space category in the tree view pane on the left side of the main window. A list of spaces in the project will appear in the list view pane.
2. Select the desired space in the list view pane by clicking on it once.
3. Use one of the following three methods to duplicate a space:
a. Use the "Duplicate" option on the Edit Menu.
b. Press the "Duplicate" button on the Toolbar.
c. Right-click on the selected space item to display its pop-up menu. Then select the "Duplicate" item on this menu.
4. After the space has been duplicated its data will be displayed in the space input form. Edit data as necessary and then press OK to save the changes and return to the HAP
main window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Building (with Spaces and HVAC Eqpt)
When performing an analysis for LEED® Energy and Atmosphere Credit 1 or LEED® Energy and Atmosphere Prerequisite 2 (Whole Building Energy Simulation option), it is
sometimes necessary to make a copy of a HAP building and all the air systems, plants, spaces, chillers, cooling towers and boilers that are linked to the building. An example is
after a Proposed Design has been created and you wish to make a copy of all its data as the basis for assembling the Baseline 0 degree building. The Duplicate Building (with
Spaces and HVAC Eqpt) option is used for this purpose. To use this option:
Page 40 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Copying Items
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
Deleting Items
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
Replacing Space Data
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
1. Select the Building category in the tree view pane on the left side of the main window. A list of buildings in your project will appear in the list view pane on the right.
2. Select the desired Building in the list view pane by clicking on it once.
3. Use one of the following two methods of duplicating the Building:
a. Choose the Duplicate Building (with Spaces and HVAC Eqpt) on the Edit Menu.
=OR=
b. Right-click on the selected Building to display its pop-up menu and then choose the Duplicate Building (with Spaces and HVAC Eqpt) on this menu.
4. A window will appear explaining what this option does and asking whether you are using this option to copy data in preparation for creating a Baseline Building or a Proposed
Design. If you choose Baseline Building, the program will use the prefix [B000] in the name of each entity (system, plant, etc…) it copies so you can easily identify the data. If
you choose Proposed Design, the program will use the prefix [P] in the name of each entity it copies. A third option is provided for directly specifying a custom prefix for the
duplicated data other than [B000] or [P]. After making your selection press OK to duplicate the Building.
5. The program will then make a copy of the original Building and all the spaces, air systems, plants, chillers, cooling towers and boilers linked to the Building. Names of copied
items will be assigned the proper prefix as described above.
6. Once the program is finished, a message will be displayed confirming completion of the work and explaining how to identify the data items that were created.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying Items
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Items
There are five ways to delete existing items in HAP. The example below deals with deleting air systems, but the procedure can be used for any category of data in HAP. Simply
substitute your category name for "system" in the following description. Note: If you ever accidentally delete data, you can often undo the deletion. A paragraph at the end of this
section explains how.
To delete two air systems from a project:
1. Select the System category in the tree view pane on the left side of the main window. A list of systems in the project will appear in the list view pane.
2. In the list view pane select the two air systems to be deleted.
3. Use one of the following five methods to delete the air systems:
a. Press the Delete key on the keyboard.
b. Use the Delete option on the Edit Menu.
c. Use the Delete button on the Toolbar.
d. Right-click on the selected systems in the list view pane to display the item pop-up menu. Then select the "Delete" item on this menu.
e. Right-click on the System category in the tree view pane to display the pop-up menu for the system category. Then select the "Delete" item on this menu. Note that this will
delete ALL systems in the project, so this option should be used carefully.
4. HAP will display a warning message listing the number of systems to be deleted and asking you to confirm the deletion before it erases the data.
How to Undo Accidental Deletion of Data: When data is deleted, it is permanently erased from the working copy of your project. However, if you ever mistakenly delete data
and have not yet saved the project, you can undo the deletion by re-opening the project. Use the Open option on the Project Menu. When you choose the Open option, HAP will
ask if you want to save changes to your current project data. Make sure you DO NOT save the project data at this point. Then reopen the project. Data from your most recent
project/save will be restored. While this will successfully undo your accidental deletion of data, any other changes you made to the project since the last project/save will also be
lost.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Replacing Space Data
During the course of a design project, specifications for the building sometimes change. For example, the wall construction characteristics change or lighting levels are adjusted.
In such a situation, its useful to be able to globally change all space data rather than modifying the spaces one at a time.
The Replace feature in HAP is used for this purpose. For example, the Replace feature can be used to change the overhead lighting wattage for 45 spaces all in one step. This
provides a vast time savings over modifying the 45 spaces one at a time. A Replace can be performed in two ways:
1. The first is using a "search and replace" approach in which you define a "value to replace" and a "replace with" value. For example, if "value to replace" is 2.0 W/sqft of
overhead lighting, and "replace with" is 1.8 W/sqft, the program will search for all occurrences of 2.0 W/sqft of overhead lighting in the spaces you choose, and will replace
these with 1.8 W/sqft.
2. The second is using a "replace all" approach in which you only specify a "replace with" value; the "value to replace" specification is left blank in this case. For example, if the
"value to replace" is blank and the "replace with" value is 1.8 W/sqft of overhead lighting, the program will replace all overhead lighting inputs in the spaces you designate with
1.8 W/sqft, regardless of what the original overhead lighting values are.
There are four methods for globally replacing space data in HAP. The example below deals with changing the overhead lighting W/sqft in a group of spaces from 2.0 to 1.8. The
same general procedure can be used for replacing many other types of space input data.
1. Select the Space category in the tree view pane on the left side of the main window. A list of spaces in the project will appear in the list view pane.
2. In the list view pane select the spaces whose data is to be modified.
3. Use one of the following four methods to replace the data:
a. Use the "Replace" option on the Edit Menu.
b. Press the "Replace" button on the Toolbar.
Page 41 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Rotating Spaces
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
Performing LEED (90.1 PRM) Rotations
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.2 Working with Input Data ››
1.6.3 Using Features of the Main Program Window
1.0 Getting Started ›› 1.6 Performing Common Tasks ››
Selecting Items in the List View
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
c. Right-click on the group of selected spaces to display its pop-up menu. Then select the "Replace" item on this menu.
d. Right-click on the Space category name in the tree view pane on the left side of the main window to display the Space category pop-up menu. Then select the "Replace"
option on this menu. Note that this will apply changes to ALL spaces in the project, so this method should be used carefully.
4. After the Replace option is selected, the Replace Data form will appear.
5. On the Internals tab of this form choose "Overhead Lighting W/sqft" as the category to be changed, specify a "value to replace" of 2.0 and a "replace with" value of 1.8.
6. Then click on the OK button to run the search and replace process. The program will notify you of the number of spaces searched and the number of items replaced before
returning to the HAP main window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Rotating Spaces
During the course of a design project, the orientation of the building is sometimes adjusted by the architect. In such a situation, it is useful to be able to globally change the
orientations of wall exposures and roof exposures in all your spaces rather than modifying the spaces one at a time.
The Rotate feature in HAP is used for this purpose. For example, suppose a building contains 100 spaces. Midway through the design process, the architect changes the building
orientation by shifting it 45 degrees clockwise. The rotate feature can be used to adjust the wall and roof orientations in one step. This provides a vast time savings over
modifying the 100 spaces one at a time.
There are four ways to rotate space data in HAP. The example below deals with rotating the orientation of wall and roof exposures by 45 degrees clockwise. The same general
procedure can be used for rotation by other amounts.
1. Select the Space category in the tree view pane on the left side of the main window. A list of spaces in the project will appear in the list view pane.
2. In the list view pane select the spaces to be rotated.
3. Use one of the following four methods to rotate the spaces:
a. Use the "Rotate" option on the Edit Menu.
b. Press the "Rotate" button on the Toolbar.
c. Right-click on the group of selected spaces to display its pop-up menu. Then select the "Rotate" item on this menu.
d. Right-click on the Space category name in the tree view pane on the left side of the main window to display the Space category pop-up menu. Then select the "Rotate"
option on this menu. Note that this will rotate ALL spaces in the project, so this method should be used carefully.
4. After the Rotate option is selected, the Rotate Data form will appear. On this form specify the amount of rotation (45 degrees in this example). Then press the OK button to
begin the rotation. The program will report the number of wall and roof exposures that were rotated before returning to the HAP main window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Performing LEED (90.1 PRM) Rotations
When performing an analysis for LEED® Energy and Atmosphere Credit 1 or LEED® Energy and Atmosphere Prerequisite 2 (Whole Building Energy Simulation option), it is
necessary to make four copies of the Baseline Building. The first Baseline Building, using an orientation equal to the Proposed Design, is assembled by manually defining the
characteristics of its spaces, systems, plants, chillers, cooling towers, and boilers, as necessary. Then it is necessary to make three further copies of this Baseline Building with
spaces rotated 90 deg, 180 deg and 270 deg, respectively, from the original Baseline Building orientation. The Perform LEED (90.1 PRM) Rotations option is used to quickly
generate these three copies of the Baseline Building. To use this option:
1. Select the Building category in the tree view pane on the left side of the main window. A list of buildings in your project will appear in the list view pane on the right.
2. Select the Baseline Building in the list view pane by clicking on it once.
3. Use one of the following two methods to perform the LEED rotations:
a. Choose the Perform LEED (90.1 PRM) Rotations option on the Edit Menu.
=OR=
b. Right-click on the selected Building to display its pop-up menu and then choose the Perform LEED (90.1 PRM) Rotations option on this menu.
4. A window will appear explaining what this option does. Press OK to start the rotations.
5. The program will produce three copies of the Baseline Building you selected. Copies include the building and all the spaces, air systems, plants, chillers, cooling towers and
boilers linked to the building. The spaces in the first copy will be rotated 90 deg from the original orientation. The spaces in the second copy will be rotated 180 deg. The
spaces in the third copy will be rotated 270 deg. HAP uses prefixes for the copied items so you can easily identify them. [B090] indicates data for the Baseline 90 deg rotation,
[B180] indicates data for the Baseline 180 deg rotation, and [B270] indicates data for the Baseline 270 deg rotation.
6. When the program is finished generating this data it displays a message confirming completion and explaining how to identify the data that was produced.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains common tasks for working with data in the HAP main window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Selecting Items in the List View
In HAP, tasks are performed with project data by selecting the data in the list view of the main program window and then using various toolbar buttons or menu options to do
such things as edit, duplicate, delete and print data. This topic describes the four ways of selecting items in the list view. Before using any of the procedures below, it is assumed
Page 42 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Inverting Selected Items in the List View
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
Changing the List View Format
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
Turning the Toolbar On and Off
you have clicked on the desired category name in the tree view of the main program window. For example, if you want to select spaces, you have clicked on the Space category
name in the tree view to display a list of spaces in your project.
A. Selecting a Single Item
Click once on the name or icon of the item you wish to select. The name will be highlighted indicating it has been selected.
B. Selecting Multiple, Consecutive Items
Holding the [Shift] key on the keyboard down, click on the name or icon of the first and last items in the group you wish to select. The names of all items in the group will be
highlighted indicating they are selected.
C. Selecting Multiple, Non-Consecutive Items
Holding the [Ctrl] key on the keyboard down, click on the name or icon of each item you wish to select. The name of each item you select will be highlighted.
D. To Select All Items in a Category
Choose the Select All option on the Edit Menu (on the menu bar). The names of all items shown in the list view will be highlighted indicating they are selected.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Inverting Selected Items in the List View
The Invert Selection option on the Edit Menu is used to de-select all currently selected items in the list view and then select all unselected options.
Example: The 12 spaces in your project are currently shown in the list view in the main program window. You have selected the first 5 of these spaces, so the first five space
names are highlighted. If you choose the Invert Selection option on the Edit Menu, spaces 1-5 will be de-selected, and spaces 6-12 will be selected automatically.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Changing the List View Format
The list view in the main program window provides a list of items, such as spaces, walls, roofs, etc.., that you have entered and stored in your project. This list of items can be
displayed in four different formats: List, Details, Large Icons, and Small Icons. You can change from one format to another using options on the View Menu and buttons on the
toolbar. Each of the four list view formats is described below.
A. List Format
In List Format each item is shown as a small icon with the item name to the right of the icon. Items are listed in a column format. Once items fill the first column, additional
items are shown in a second column. To switch to this list view format, choose the "List" option on the View Menu, or press the "List" toolbar button.
B. Details Format
In Details Format each item is shown as a small icon with the item name to the right of the icon. Additional descriptive details are listed opposite the item, as shown in the
following table. Items are shown in column format. Once items fill the available display area, the list view must be scrolled to display additional items. To switch to this list view
format, choose the "Details" option on the View Menu, or press the "Details" toolbar button.
Data Category
Details Item #1:
Details Item #2:
Details Item #3:
Weather
Design City
Simulation City
Spaces
Floor Area
Systems
System Type
Sizing Status
Simulation Status
Plants
Plant Type
Sizing Status
Simulation Status
\*Buildings
Simulation Status
Schedules
Schedule Type
Walls
Overall U-Value
Overall Weight
Roofs
Overall U-Value
Overall Weight
Windows
Overall U-Value
Shade Coefficient
Doors
Door U-Value
Glass U-Value
Ext. Shading
(none)
\*Chillers
Chiller Type
Full Load Capacity
\*Cooling Towers
Clg Tower Type
\*Boilers
Boiler Type
Full Load Capacity
\*Electric Rates
(none)
\*Fuel Rates
(none)
\*Items marked with an asterisk are available in HAP but not HAP System Design Load.
C. Large Icons Format
In Large Icon format, each item is shown as a large icon with the name positioned below the icon. Items are listed in rows from left to right across the list view panel. Once
icons fill the available display area, the list view must be scrolled to view additional icons. To switch to Large Icon format, choose the "Large Icons" option on the View Menu,
or press the "Large Icons" toolbar button.
D. Small Icons Format
In Small Icon format, each item is shown as a small icon with the item name to the right of the icon. Items are listed in rows from left to right across the list view panel. Once
icons fill the available display area, the list view must be scrolled to see additional items. To switch to Small Icon format, choose the "Small Icons" option on the View Menu, or
press the "Small Icons" toolbar button.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 43 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
Turning the Status Bar On and Off
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
Setting User Preferences
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.3 Using Features of the Main Program Window ››
Turning the Toolbar On and Off
To toggle the toolbar on or off, click on the "Toolbar" item on the View menu. When the toolbar is included in the main program window, a check mark will appear next to the
"Toolbar" item on the View Menu.
Users sometimes turn the toolbar off to gain extra room for displaying data in the list view and tree view panels. This situation is common when using monitors with 640x480
resolution. In other cases, users find they do not often use the toolbar, and therefore turn it off to simplify the main program window appearance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Turning the Status Bar On and Off
To toggle the status bar on or off, click on the "Status Bar" item on the View menu. When the status bar is included in the main program window, a check mark will appear next to
the "Status Bar" item on the View Menu.
Users sometimes turn the status bar off to gain extra room for displaying data in the list view and tree view panels. This situation is common when using monitors with 640x480
resolution. In other cases, users find they do not often refer to information in the status bar (date, time, messages, maximum and minimum input limits), and therefore turn it off to
simplify the main program window appearance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Setting User Preferences
The Preferences option on the View Menu is used to specify preferences affecting program operation. When this option is selected, the Preferences window appears. This
window contains two tabs.
The General Tab is divided into two parts. The first part contains preferences applying to all Carrier eDesign programs on your computer:
1. Measurement Units - Choose whether program input data and results are displayed using English units or SI Metric units.
2. Email Address for Your Carrier Sales Engineer allows you to specify an e-mail address that is used with the Send Email to Sales Engineer option on the Project Menu. This
option is used when collaborating with your Carrier sales engineer to archive your project data and e-mail it to the sales engineer so equipment selections can be run against
your sizing data.
The second part of the General Tab contains preferences which apply only to HAP:
1. Show Tooltips - Tooltips are the small messages that appear when you position the mouse cursor over toolbar buttons and various other portions of the main program
window, or certain input windows. Tooltips will be shown when this box is checked.
2. Show Date - When this box is checked, the current date will be shown in the right-hand portion of the status bar.
3. Show Time - When this box is checked, the current time will be shown in the right-hand portion of the status bar.
4. Operating Mode allows you to turn Energy Analysis features on and off. This option is only offered when running the full version of HAP. It is not offered when running HAP
System Design Load.
In HAP users have the option of switching the program from full HAP mode to HAP System Design mode and vice versa. Switching to HAP System Design mode turns off all
of the inputs and features for energy analysis. When using the program only for system design work, users may find it more efficient to hide the unneeded energy analysis
features from view. Users can switch between operating modes at any time and for any project. For example, if you created a project while in HAP System Design mode you
can later switch it to full HAP mode. All of the original project data will remain. You will only have to supply the extra energy analysis data to run energy studies.
Page 44 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.6.4 Generating Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ››
Generating Input Data Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
The Project Tab contains preferences related to the current HAP project only. Currently this tab provides options for:
1. LEED® Rating System. Choose whether the LEED® rating system used in this project will be LEED v4, LEED 2009, or LEED NC-2.2. This choice affects how the LEED EA
Credit 1 Summary report is formatted. Formatting is customized to the rating system you select. When you make a selection, HAP will default the Ventilation Standard and
Energy Standard inputs. For example, if you choose LEED v4, HAP will default the Ventilation Standard as ASHRAE 62.1-2010 and the Energy Standard as ASHRAE
90.1-2010. However, you can change these defaults afterwards, if necessary..
2. Ventilation Standards. Choose whether ventilation defaults should be based on one of the ASHRAE Standard 62.1 editions or "User-Defined". Typically this choice is made
at the start of a project since it affects how data is entered for spaces and systems. When you choose one of the ASHRAE Standard options, you will be able to default space
ventilation requirements by selecting a space usage type. In addition, options will be offered in system inputs for calculating ventilation airflow using the Ventilation Rate
Procedure. When you choose "User-Defined", you will always be required to specify space ventilation requirements yourself and the only ventilation calculation option will be
"Sum of Space OA Airflows".
3. Energy Standard. Choose the edition of the ASHRAE 90.1 energy standard used in this project. This choice affects how HAP defaults minimum efficiencies for equipment.
When the "ASHRAE Minimum Eqpt Efficiency" option is selected, instead of directly specifying equipment performance values like kW, EER, COP, SEER or HSPF or average
efficiency (%), the program will default efficiencies based on the ASHRAE 90.1 standard you select. When performing Appendix G Performance Rating Method calculations for
a LEED analysis, the energy standard edition should be synchronized with the version of LEED you're using in the project: 90.1-2010 for LEED v4, 90.1-2007 for LEED 2009,
or 90.1-2004 for LEED NC 2.2. HAP synchronizes the energy standard edition automatically when you select a LEED rating system.
4. Currency Units. Specify the currency symbol or abbreviation to be used in this project. This input will be used for all program inputs and results involving cost. For example, if
you specify "$" as the currency units, all energy and fuel prices will be based on $ and all energy cost reports will display costs in units of $.
Command Buttons. Finally, the form contains three buttons in the lower right-hand corner:
a. Press the OK button to apply any changes you’ve made to the preferences and then exit..
b. Press the Cancel button to exit without applying changes you’ve made to preferences.
c. Press the Help button to display this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes common tasks involved with generating program reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating Input Data Reports
HAP provides four ways to print or view input data for your project. When printing data, it is sent directly to your printer. When viewing data, information appears in the HAP
Report Viewer. The Viewer allows you to quickly browse the data. The Viewer also provides a button for printing the data.
The example below deals with viewing or printing input data for a group of spaces, but the procedure can be used for any category of data in HAP. Simply substitute your
category name for "space" in the following description.
To view or print input data for a group of spaces:
1. Select the Space category in the tree view pane on the left side of the main window. A list of spaces in the project will appear in the list view pane.
2. In the list view pane select the spaces whose input data is to be viewed or printed.
3. Use one of the following four methods to view or print the input data:
a. Choose the "View Input Data" or "Print Input Data" options on the Reports Menu.
b. Press the "View Input Data" button on the Toolbar.
c. Right-click on the selected spaces in the list view pane to display the item pop-up menu. Then select the "View Input Data" or "Print Input Data" option on this menu.
d. Right-click on the Space category in the tree view pane to display the pop-up menu for the space category. Then select the "View Input Data" or "Print Input Data" option on
this menu. Note that this will view or print input data for ALL spaces, so this option should be used carefully.
Page 45 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Generating Weather Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Generating System Design Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Generating Plant Design Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Generating System Simulation Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating Weather Reports
HAP provides four ways to print or view weather data for your project. When printing data, it is sent directly to your printer. When viewing data, information appears in the HAP
Report Viewer. The Viewer allows you to quickly browse the data. The Viewer also provides a button for printing the data.
1. Click on the Weather category name in the tree view panel of the HAP main window.
2. Use one of the following four methods to request weather reports:
a. Choose the Print/View Input Data option on the Reports Menu.
b. Press the View Input Data button on the toolbar.
c. Right-click on the "Weather Properties" item in the list view panel. Then choose the Print/View Input Data item in the pop-up menu that appears.
d. Right-click on the "Weather Properties" item in the tree view panel. Then choose the Print/View Input Data item in the category pop-up menu that appears.
3. All 4 methods above will cause the Weather Reports Selection dialog to appear. Select the desired reports in this dialog.
4. To view the reports, press the Preview button on the Reports Selection dialog. The HAP Report Viewer will appear and will display the reports you selected. The Viewer
contains a Print button that can be used to print the reports if desired.
5. To print the reports without viewing them first, press the Print button on the Report Selection dialog.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating System Design Reports
System design reports provide information about loads and the required sizes of air system components such as coils, fans, and supply terminals. HAP provides four ways to
generate these reports, all utilizing the same basic procedure.
1. Select the System category in the tree view pane on the left side of the main window. A list of systems in the project will appear in the list view pane.
2. In the list view pane select the desired systems.
3. Use one of the following four methods to view or print system design reports:
a. Choose the "Print/View Design Results" option on the Reports Menu.
b. Press the "Print/View Design Results" button on the Toolbar.
c. Right-click on the selected systems in the list view pane to display the item pop-up menu. Then select the "Print/View Design Results" option on this menu.
d. Right-click on the System category in the tree view pane to display the pop-up menu for the system category. Then select the "Print/View Design Results" option on this
menu. Note that this will generate design reports for ALL systems in the project, so this option should be used carefully.
4. The System Design Reports Selection dialog will appear. Select the reports to be generated.
5. To view the reports, press the Preview button on the System Design Reports dialog. If system design calculations must be run before the reports can be generated, HAP will
run these calculations automatically. If no calculations are needed, the reports will be displayed immediately. Reports are displayed in the HAP Report Viewer. After viewing
the reports you can print the reports by pressing the Print button on the Report Viewer. However, you print one report document at a time from the Viewer. If you wish to print
all reports in one batch, it is more efficient to use the Print button on the System Design Reports dialog.
6. To print the reports directly, press the Print button on the System Design Reports dialog. If system design calculations must be run before the reports can be generated, HAP
will run these calculations automatically. If no calculations are needed, the reports will be printed immediately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating Plant Design Reports
Plant design reports provide sizing information for chiller plants and boiler plants. HAP provides four ways to generate these reports, all utilizing the same basic procedure.
1. Select the Plant category in the tree view pane on the left side of the main window. A list of plants in the project will appear in the list view pane.
2. In the list view pane select the desired plants.
3. Use one of the following four methods to view or print plant design reports:
a. Choose the "Print/View Design Results" option on the Reports Menu.
b. Press the "Print/View Design Results" button on the Toolbar.
c. Right-click on the selected plants in the list view pane to display the item pop-up menu. Then select the "Print/View Design Results" option on this menu.
d. Right-click on the Plant category in the tree view pane to display the pop-up menu for the plant category. Then select the "Print/View Design Results" option on this menu.
Note that this will generate design reports for ALL plants in the project, so this option should be used carefully.
4. The Plant Design Reports Selection dialog will appear. Select the reports to be generated.
5. To view the reports, press the Preview button on the Plant Design Reports dialog. If plant or system design calculations must be run before the reports can be generated, HAP
will run these calculations automatically. If no calculations are needed, the reports will be displayed immediately. Reports are displayed in the HAP Report Viewer. After
viewing the reports you can print the reports by pressing the Print button on the Report Viewer. However, you print one report document at a time from the Viewer. If you wish
to print all reports in one batch, it is more efficient to use the Print button on the Plant Design Reports dialog.
6. To print the reports directly, press the Print button on the Plant Design Reports dialog. If plant or system design calculations must be run before the reports can be generated,
HAP will run these calculations automatically. If no calculations are needed, the reports will be printed immediately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 46 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Generating Plant Simulation Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Generating Building Simulation Reports
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
HAP Report Viewer
1.0 Getting Started ›› 1.6 Performing Common Tasks ›› 1.6.4 Generating Reports ››
Generating System Simulation Reports
System simulation reports provide information about system operation and energy use during a typical year. These reports are offered in HAP but not HAP System Design Load.
HAP provides four ways to generate these reports, all utilizing the same basic procedure.
1. Select the System category in the tree view pane on the left side of the main window. A list of systems in the project will appear in the list view pane.
2. In the list view pane select the desired systems.
3. Use one of the following four methods to view or print system simulation reports:
a. Choose the "Print/View Simulation Results" option on the Reports Menu.
b. Press the "Print/View Simulation Results" button on the Toolbar.
c. Right-click on the selected systems in the list view pane to display the item pop-up menu. Then select the "Print/View Simulation Results" option on this menu.
d. Right-click on the System category in the tree view pane to display the pop-up menu for the system category. Then select the "Print/View Simulation Results" option on this
menu. Note that this will generate simulation reports for ALL systems in the project, so this option should be used carefully.
4. The System Simulation Reports Selection dialog will appear. Select the reports to be generated.
5. To view the reports, press the Preview button on the System Simulation Reports dialog. If system calculations must be run before the reports can be generated, HAP will run
these calculations automatically. If no calculations are needed, the reports will be displayed immediately. Reports are displayed in the HAP Report Viewer. After viewing the
reports you can print the reports by pressing the Print button on the Report Viewer. However, you print one report document at a time from the Viewer. If you wish to print all
reports in one batch, it is more efficient to use the Print button on the System Simulation Reports dialog.
6. To print the reports directly, press the Print button on the System Simulation Reports dialog. If system calculations must be run before the reports can be generated, HAP will
run these calculations automatically. If no calculations are needed, the reports will be printed immediately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating Plant Simulation Reports
Plant simulation reports provide information about plant operation and energy use during a typical year. These reports are offered in HAP but not HAP System Design Load. HAP
provides four ways to generate these reports, all utilizing the same basic procedure.
1. Select the Plant category in the tree view pane on the left side of the main window. A list of plants in the project will appear in the list view pane.
2. In the list view pane select the desired plants.
3. Use one of the following four methods to view or print plant simulation reports:
a. Choose the "Print/View Simulation Results" option on the Reports Menu.
b. Press the "Print/View Simulation Results" button on the Toolbar.
c. Right-click on the selected plants in the list view pane to display the item pop-up menu. Then select the "Print/View Simulation Results" option on this menu.
d. Right-click on the Plant category in the tree view pane to display the pop-up menu for the plant category. Then select the "Print/View Simulation Results" option on this
menu. Note that this will generate simulation reports for ALL plants in the project, so this option should be used carefully.
4. The Plant Simulation Reports Selection dialog will appear. Select the reports to be generated.
5. To view the reports, press the Preview button on the Plant Simulation Reports dialog. If plant or system calculations must be run before the reports can be generated, HAP will
run these calculations automatically. If no calculations are needed, the reports will be displayed immediately. Reports are displayed in the HAP Report Viewer. After viewing
the reports you can print the reports by pressing the Print button on the Report Viewer. However, you print one report document at a time from the Viewer. If you wish to print
all reports in one batch, it is more efficient to use the Print button on the Plant Simulation Reports dialog.
6. To print the reports directly, press the Print button on the Plant Simulation Reports dialog. If plant or system calculations must be run before the reports can be generated, HAP
will run these calculations automatically. If no calculations are needed, the reports will be printed immediately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Generating Building Simulation Reports
Building simulation reports provide information about annual energy use and energy cost. These reports are offered in HAP but not HAP System Design Load. HAP provides four
ways to generate these reports, all utilizing the same basic procedure.
1. Select the Building category in the tree view pane on the left side of the main window. A list of buildings in the project will appear in the list view pane.
2. In the list view pane select the desired buildings.
3. Use one of the following four methods to view or print building simulation reports:
a. Choose the "Print/View Simulation Results" option on the Reports Menu.
b. Press the "Print/View Simulation Results" button on the Toolbar.
c. Right-click on the selected buildings in the list view pane to display the item pop-up menu. Then select the "Print/View Simulation Results" option on this menu.
d. Right-click on the Building category in the tree view pane to display the pop-up menu for the building category. Then select the "Print/View Simulation Results" option on this
menu. Note that this will generate simulation reports for ALL buildings in the project, so this option should be used carefully.
4. The Building Simulation Reports Selection dialog will appear. Select the reports to be generated.
5. To view the reports, press the Preview button on the Building Simulation Reports dialog. If building, plant or system calculations must be run before the reports can be
generated, HAP will run these calculations automatically. If no calculations are needed, the reports will be displayed immediately. Reports are displayed in the HAP Report
Viewer. After viewing the reports you can print the reports by pressing the Print button on the Report Viewer. However, you print one report document at a time from the
Viewer. If you wish to print all reports in one batch, it is more efficient to use the Print button on the Building Simulation Reports dialog.
6. To print the reports directly, press the Print button on the Building Simulation Reports dialog. If building, plant or system calculations must be run before the reports can be
generated, HAP will run these calculations automatically. If no calculations are needed, the reports will be printed immediately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 47 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
1.7 Documentation Resources
1.0 Getting Started ››
HAP Report Viewer
The Report Viewer is used to display all HAP reports. This includes input, system design and energy simulation reports as well as calculation error reports and the gbXML
Translation Report. For information on the content a specific report, click on one of the following. For information about features of the Report Viewer itself, continue reading
below the figure.
System Design Reports
Plant Design Reports
System Simulation Reports
Plant Simulation Reports
Building Simulation Reports
Calculation Error Report
gbXML Translation Report
Overview of Layout and Features. The Report Viewer consists of four key components.
1. The Title Bar appears across the top of the Report Viewer window. At the right-hand end of the title bar is a close button which is used to close the viewer and return to the
HAP main window.
2. The Menu Bar appears beneath the title bar. It contains two menus which provide options for performing useful tasks with reports.
The first menu is the File Menu. Options on this menu are as follows:
a. Save Report As is used to save the report as a disk file. Only the report document currently visible in the viewer is saved. The report is saved in Rich Text Format (RTF).
This option is useful for incorporating report material in other documents. RTF files can be read by many popular word processor programs.
b. Print Setup is used to adjust settings for your default printer. This option is typically used prior to printing a report.
c. Print is used to print the report document that is currently visible.
d. Exit is used to close the Report Viewer and return to the HAP main window.
The second menu is the Help Menu. It contains one option:
e. How to Use the Report Viewer displays an overview help topic for the Viewer.
3. The Toolbar appears beneath the menu bar. It contains buttons for performing useful tasks with the reports. Many of these tasks are the same as provided by options on the
Menu Bar. Working from left to right across the toolbar the buttons perform the following functions:
a. The Save Report As button serves the same function as the Save Report As option on the File Menu, described above.
b. The Print button prints the report document that is currently visible in the viewer.
c. The Zoom In and Zoom Out buttons are used to enlarge or reduce the magnification for the currently displayed page. Zoom In increases the magnification for the page.
Zoom Out decreases the magnification for the page.
4. The Report Viewing Area appears below the toolbar. It displays all pages for the current batch of reports. If you select multiple reports, HAP will bundle the reports into a
single document. You must then use the [PgUp], [PgDn], arrow keys or scroll bar to scroll the report to see all of its content.
Key Organizational Principles. In order to effectively use the Report Viewer it helps to understand how the program organizes and displays reports. There are three key
principles:
1. The group of reports you select is placed in a single report document with pages numbered 1 to N. To view the contents of the reports you use the [PgUp], [PgDn], and arrow
keys and the scroll bar to scroll the document.
Example: If you select 3 air systems and then select a set of 4 system design reports, a total of 12 reports will be generated (3 systems x 4 reports). All 12 reports will be
placed in a single document. To view the content of all 12 reports, you scroll through the pages of this document.
2. The "Print" option in the Report Viewer prints the entire report document - whether that document contains a single report or a batch of reports. If you are printing to a PDF
converter, a single PDF will be generated.
3. The "Save Report As" option in the Report Viewer will save the entire report document as a Word RTF file - whether that document contains a single report or a batch of
reports..
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 48 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Using the Documentation Menu
1.0 Getting Started ›› 1.7 Documentation Resources ››
Using the Help Menu
1.0 Getting Started ›› 1.7 Documentation Resources ››
Using the Help System In HAP
1.0 Getting Started ›› 1.7 Documentation Resources ››
This section explains how to use documentation resources on the Help and Documentation Menus.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using the Documentation Menu
HAP provides extensive resources to help users learn about, understand and use the software. These resources found on the Documentation and Help Menus. Options on the
Documentation Menu are described below. Options on the Help Menu are described in a separate topic.
1. Quick Reference Manual - Displays an electronic copy of the HAP Quick Reference Manual. This manual contains a subset of the information in the help system including the
introductory information, tutorials, example problems and application information sections.
2. Example Problem Reports - Displays a document containing calculation results from the example problem (Chapters 3 and 4 of the help system). Some companies require
that calculation results of newly installed software must be validated against a reference set of results. This document provides the reference results for that validation work.
3. ASHRAE 90.1 Energy Cost Budget - Displays a document describing how HAP complies with simulation software requirements in Section 11 (Energy Cost Budget Method)
of ASHRAE Standard 90.1 - Energy Standard for Buildings except Low-Rise Residential Buildings.
4. ASHRAE 140 Test Results - Displays a document describing test results for the current version of HAP generated using software test suites in ASHRAE Standard 140 -
Standard Method of Test for the Evaluation of Building Energy Analysis Computer Programs.
5. ASHRAE 183 (Peak Load Calculations) - Displays a document describing how HAP complies with provisions in ASHRAE Standard 183 - Peak Cooling and Heating Load
Calculations in Buildings Except Low-Rise Buildings..
6. ASHRAE 90.1 Appendix G - Displays a document describing how HAP complies with simulation software requirements in Appendix G (Performance Rating Method) of
ASHRAE Standard 90.1 - Energy Standard for Buildings except Low-Rise Residential Buildings.
7. Using HAP for LEED EA Credit 1 - Displays a document describing how to use HAP for LEED Energy and Atmosphere Credit 1 (Optimize Energy Performance) analyses..
8. US Federal Regulation 10 CFR 434 - Displays a document describing how HAP complies with simulation software requirements in Federal Register 10CFR Part 434
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using the Help Menu
HAP provides extensive resources to help users learn about, understand and use the software. These resources found on the Documentation and Help Menus. Options on the
Help Menu are described below. Options on the Documentation Menu are described in a separate topic.
1. Contents and Index - Launches the help system. The help system contains introductory information, tutorials, examples, application information, and complete explanations
of all program input screens and reports and calculation documentation. In addition you can launch the help system by pressing [F1] at any point during program operation or
by pressing any of the Help buttons that appear on program input screens. Read more.
2. Contact Software Support - Displays telephone and e-mail contact information you can use to contact Carrier software support for assistance with the program.
3. eDesign Support Web Site - Launches your web browser and displays the eDesign Application Support web page. This page provides self-service support materials such as
frequently asked questions and "eHelps", which are short articles on common program topics of interest.
4. Check for Program Updates - Launches your web browser and displays the eDesign Downloads web page where you can check to see if patch updates or major updates for
the program have been released. Note that the patch updates are usable by customers worldwide. Major updates on this web page are only available to customers in the US
and Canada. For other regions of the world, please contact your local Carrier sales office for information about major software updates.
5. Software Newsletter. The "eDesign Newsletter" menu option links you to the EXchange software newsletter web page from which you can subscribe to this quarterly
electronic newsletter containing information about HAP and other Carrier eDesign tools.
6. eDesign Software Training - Launches your web browser and displays the the eDesign Software Training web page which contains class descriptions, a schedule of class
dates and locations, and on-line class registration. These training classes are specifically for the US and Canadian markets.
7. eDesign Software Web Site - Launches your web browser and displays the main eDesign software web page. This page contains information about all eDesign programs in
addition to HAP.
8. Carrier Commercial Web Site - Launches your web browser and displays the Carrier commercial building products web page. Note that this web page is for the North
American market. Please visit www.carrier.com for links to web pages for other regions of the world.
9. About HAP - Displays the currrent program version. This option is useful if you are unsure if you have the latest version. The version displayed via this option can be
compared with the versions shown in the eDesign Downloads web page (item 4 above).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Using the Help System In HAP
HAP Help. HAP provides extensive documentation via its help system to assist users in learning, understanding and using the software. In HAP you can obtain information from
the help system by:
a. Using options on the Help menu in the main program window .
b. Pressing the Help button on any input form.
c. Pressing F1 at any time during program operation.
Each of method of obtaining help is discussed below in greater detail.
Method 1 - Using The Help Menu.
Select the "Contents and Index" option on the Help Menu to display help. The help system displays in a window containing three tabs on the left: Contents, Index, and Search.
1. "Contents" provides a table of contents representation of the help system. Topics represented by page icons are organized into chapters represented by book icons. The
table of contents operates as a tree view. Double-click on a book icon to display the topics in a chapter. Double-click on a page icon to display the help topic in the right-hand
pane of the window.
2. "Index" contains an alphabetical list of subjects that you can browse through. It also permits you to enter a search word or phrase. When the search word or phrase is
entered, the index automatically scrolls to the subject whose title most closely matches your search entry.
3. "Search" allows you to enter a word or phrase. You then click the "List of Topics" button and the help software lists all help topics which include the word or phrase. You can
then display a desired topic by double-clicking the topic name in the left panel.
Page 49 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm
Method 2 - Using The Help Button on Input Forms.
All HAP input forms contain a Help button. When you press this button, a help topic appears which provides an overview of the form and its use. This feature is very useful when
using a form for the first time. The overview help explains the data you are entering, gives a quick orientation of the form and its features, and provides links to all inputs found on
the form. For example, the overview help for the space input form defines the term "space" and explains how it is used in the program, briefly explains the space input form and
its seven tabs, and provides links to information about the 67 types of input items found on the form.
Method 3 - Using F1 Help
Context sensitive help can be obtained at any time by pressing the [F1] key. This launches the help system and displays the topic most closely related to the current position of
the cursor. For example, if you are entering space data and the cursor is in the input field for building weight, pressing F1 will display the help topic for building weight. This
feature is very useful for obtaining explanations and answering questions which arise as you enter data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 50 of 50
1.0 Getting Started
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9AE2.htm