3.0 System Design Example Problem
Overview for System Design Example Problem
3.0 System Design Example Problem ››
System Design Example: Defining the Problem
3.0 System Design Example Problem ››
This chapter provides a detailed example problem for peak load calculation and system design.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for System Design Example Problem
The procedure for designing HVAC systems in HAP involves five steps:
1. Define the Problem.
2. Gather Data.
3. Enter Data Into HAP.
4. Use HAP to Generate Design Reports.
5. Select Equipment.
The example problem presented in the following topics will demonstrate each step in this process. Sample
printouts of input data and calculation results can be found in the HAP Quick Reference Guide.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Design Example: Defining the Problem
The objective of this example problem is to design an HVAC system which serves one wing of a high school
building located in Chicago, Illinois. The floor plan for this portion of the school building is shown in below. It is
comprised of six classrooms, a music room and its associated office, storage and practice rooms, plus two
corridors for a total of 12 rooms. In the figure below, classrooms D101 through D104 face due east. East, south
and west walls are exposed to ambient. The north walls adjoin other air-conditioned areas of the building; we will
assume there is no heat transfer across this northern boundary.
The rooms in this portion of the school building will be air conditioned by one VAV rooftop unit serving parallel fan
powered mixing box (PFPMBX) terminals. A gas-fired preheat coil in the rooftop unit and electric resistance heating
coils in the mixing box terminals provide heating. HAP will be used to model the heat transfer processes in the
building in order to determine the following nine equipment sizing values:
a. Rooftop unit required cooling capacity.
b. Rooftop unit required fan airflow
c. Rooftop unit required preheat coil capacity.
d. Rooftop unit required outdoor airflow rate.
e. PFPMBX terminal design airflow rates.
f. PFPMBX terminal minimum airflow rates.
g. PFPMBX terminal fan design airflow rates.
h. PFPMBX terminal reheat coil capacities.
i. Space required supply airflow rates.
Note: The VAV air system serves all of the spaces shown in the figure below except for D105 South Vestibule and
D112 West Vestibule. The two vestibules contain fan coil heaters and would be modeled using a separate heating-
only fan coil air system. For purposes of this example we will focus on the VAV air system and omit consideration
of the vestibule fan coil units.
Page 1 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
System Design Example: Gathering Data
3.0 System Design Example Problem ››
Floor Plan for School Building
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Design Example: Gathering Data
The second step in the design process is to gather information necessary to model heat transfer processes in the
building and to analyze operation of the HVAC equipment which heats and cools the building. This involves
gathering data for the building, its environment and its HVAC equipment. Below, gathering of weather data, data for
spaces in the building and data for the HVAC system will be discussed.
Gathering Weather Data
ASHRAE design weather conditions for Chicago O’Hare International Airport (Chicago IAP) will be used for this
analysis. These design parameters are shown in Figure 3.2. In addition to the ASHRAE data, we will:
1. Specify daylight savings time from April 7 through October 26.
2. Use the period May through November as the design cooling months. This means cooling sizing calculations
will only be performed for this range of months. We could use January through December as the calculation
period. However, design weather conditions in Chicago are such that peak loads are most likely to occur during
the summer or fall months. So we can reduce the set of calculation months to May through November to save
calculation time without sacrificing reliability.
Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Page 2 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
Gathering Space Data
In this example problem we will model the heat transfer of each room separately so peak loads and required airflow
rates can be determined for each room. In this portion of the school building there are 12 rooms, but three (D101,
D102 and D103) are identical. Therefore we will define one of these classrooms as a space and reuse it three
times. This reduces the total number of spaces needed for the analysis from 12 to 10. Characteristics of these
spaces were derived from architectural plans and from information about the use of the building and are described
below.
Walls. One common wall construction is used for all exterior walls. The construction consists of 4-inch face brick,
R-7 board insulation, 8-inch lightweight concrete block, an air space and gypsum board finish. The exterior surface
absorption is in the “dark” category. The overall U-value is 0.084 BTU/(hr-sqft-F). The overall weight is 69.8
lb/sqft. Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Roofs. One uniform horizontal roof construction is used for this portion of the school building. The roof
construction consists of built-up roofing, board insulation with R-21, 22 gauge steel deck, a plenum air space and
acoustic ceiling tiles. The exterior surface absorption is in the “dark” category. The overall U-value is 0.040 BTU/
(hr-sqft-F). The overall weight is 5.8 lb/sqft. Note that in HAP the roof assembly must include all material layers
from the exterior surface to the interior surface adjacent to the conditioned space. Thus, the ceiling plenum is
considered part of the overall roof assembly. Please refer to the HAP Quick Reference Guide for a complete list of
inputs.
Windows & External Shading. One type of fixed window unit is used for all windows in this portion of the school
building. The window units measure 6 feet in height by 4 feet in width, are double glazed, and use an aluminum
frame with thermal breaks. No internal shades are used. Manufacturer’s NFRC ratings indicate the window has a
U-value of 0.550 BTU/(hr-sqft-F) and a shading coefficient of 0.40. All windows have a 4-inch reveal depth.
Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Lighting. Recessed, unvented fluorescent lighting fixtures are used for all rooms in this portion of the school
building. A lighting density of 1.00 W/sqft is used.
For classrooms, offices, storage rooms and practice rooms we will use design day lighting levels of 100% from
0700 through 1700, the standard occupancy period for the school, and 5% from 1800 through 2100 when lighting is
reduced or operated intermittently for custodial work. This lighting profile applies for the days the school is in
session. For weekends and holidays lighting levels of 0% are used. The holiday period includes a summer
shutdown period from late June to early August. Therefore the Weekend/Holiday lighting profile will be used for
July for design calculations.
For the corridors and vestibules we will use design day lighting levels of 100% for 0700 through 2100. Security
lighting levels of 5% will be used for all other hours. This lighting profile applies for days the school is in session.
For weekends and holidays lighting remains at 5% security levels for all hours.
Please refer to the HAP Quick Reference Guide for a complete list of lighting and schedule inputs.
Occupants. The maximum number of occupants varies by space and will be discussed later in this section. For
all rooms except the music room, a “seated at rest” activity level will be used (230 BTU/hr/person sensible, 120
BTU/hr/person latent). For the music room the “office work” activity level will be used due to the higher level of
activity in this room (245 BTU/hr/person sensible, 205 BTU/hr/person latent).
For all rooms we will use design day occupancy levels of 100% for 0700 through 1700, the normal hours of
operation for the school. Occupancy during the period 1800 through 2100 is very infrequent and will be ignored.
Thus, occupancy levels of 0% will be used for all other hours of the day. This occupancy profile applies for days
the school is in session. For weekends and holidays 0% occupancy is used for all hours. For the summer
shutdown period from late June to early August these 0% occupancy values will be used.
Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Spaces. A total of 10 spaces will be defined. Details:
1. Floor areas are shown in the table below.
2. The average ceiling height is 8 feet for all spaces.
3. The building weight is 70 lb/sqft (medium category).
4. Ventilation airflow rates will be defaulted by choosing the appropriate ASHRAE Standard 62.1-2013 space usage
type.
Page 3 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
5. One type of lighting fixture is used in all spaces. Lighting fixture characteristics and schedules were discussed
earlier in this subsection.
6. Occupants per space are listed in the table below. Occupant heat gains and schedules were discussed earlier in
this subsection.
7. One set of common wall, door, window and external shading constructions are used for the building. Wall
orientations, wall areas, and window and door quantities for each space are summarized in the table below.
8. One common roof construction is used for the building. Roof areas are shown in the table below.
9. This wing of the school building uses slab on grade floor construction. The floor slab is constructed of 6-inch of
heavy weight concrete with an overall U-value of 1.2 BTU/(hr-sqft-F). R-7 edge insulation is used for the slab.
Slab floor areas and exposed perimeters are shown in the table below. Note that slab floors are not modeled
for the corridor spaces since neither has an exposed slab perimeter.
Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Space Name
Floor
Area
(sqft)
People
Wall, Window, Door
Data
Roof Data
Slab
Floor
Area
(sqft)
Slab
Exposed
Perimeter
(ft)
D101 - Typical Classroom
907.5
25
E: 275 sqft, 3 windows
H: 907.5 sqft
907.5
27.5
D104 – Classroom
907.5
25
E: 275 sqft, 3 windows
S: 330 sqft, 0 windows
H: 907.5 sqft
907.5
60.5
D106 – Classroom
907.5
25
W: 275 sqft, 3 windows
S: 330 sqft, 0 windows
E: 110 sqft, 0 windows
H: 907.5 sqft
907.5
71.5
D107 - Classroom
907.5
25
W: 275 sqft, 3 windows
H: 907.5 sqft
907.5
27.5
D108 - Music Room
1781.0
50
S: 242 sqft, 2 windows
H: 1781.0 sqft
1781.0
24.2
D109 - Practice Room
65.0
1
W: 66 sqft, 0 windows
S: 99 sqft, 0 windows
H: 65.0 sqft
65.0
16.5
D110 - Storage Room
120.0
0
W: 121 sqft, 0 windows
H: 120.0 sqft
120.0
12.1
D111 - Office
174.0
1
W: 132 sqft, 1 window
H: 174.0 sqft
174.0
13.2
D113 - West Corridor
1054.0
0
None
H: 1054.0 sqft
0.0
0.0
D114 - South Corridor
920.0
0
None
H: 920.0 sqft
0.0
0.0
Gathering Air System Data
One air handling system will provide cooling and heating to the rooms in this wing of the school building.
Therefore, we will define one HAP air system to represent this equipment. Please refer to the HAP Quick
Reference Guide for a complete list of inputs. Details:
1. Equipment Type. A VAV rooftop unit will be used.
2. Ventilation. Outdoor ventilation airflow will be calculated using the ASHRAE Standard 62.1-2007 method.
“Constant” control for ventilation will be used so the system uses the design flow of outdoor air at all times.
Ventilation dampers are closed during the unoccupied period and the damper leak rate is 5%.
3. Cooling Coil. The system provides a constant 55 F supply air temperature to zone terminals. The DX cooling
coil is permitted to operate in all months. The bypass factor for the cooling coil is 0.038 which is representative
of the type of equipment we expect to select.
4. Preheat Coil. The rooftop unit contains a preheat coil to maintain minimum supply duct temperatures during the
winter. The preheat coil is located downstream of the point where return air and outdoor ventilation air mix. The
preheat setpoint is 52 F. The gas-fired heat exchanger in the rooftop unit is used for this purpose. The coil is
permitted to operate in all months.
Page 4 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
System Design Example: Entering Data
3.0 System Design Example Problem ››
5. Supply Fan. The supply fan in the rooftop unit will be forward curved with variable frequency drive. The total
static pressure for the system is estimated to be 3 in wg. The overall fan efficiency is 48%. The coil
configuration is draw-thru.
6. Return Air Plenum. The system uses a return air plenum. It is estimated that 70% of the roof load, 20% of the
wall load and 30% of the lighting load is removed by plenum air.
7. Zoning. A zone is a region of the building with one thermostatic control. One zone will be created for each
classroom. The music room and its adjacent office, storage room and practice room will all be part of a single
zone. Each corridor will also be zone. Therefore, a total of 9 zones will be created: one each for the six
classrooms, one for the music room and two for the corridors.
8. Thermostats. Thermostat settings of 75 F occupied cooling, 80 F unoccupied cooling, 70 F occupied heating
and 65 F unoccupied heating will be used in all zones. The throttling range will be 1.5 F. The schedule for fan
and thermostat operation for the design day will designate 0700 through 2100 as “occupied” hours. This covers
both the 0700-1700 operating hours for the school and the 1800-2100 period when custodial staff is present. All
other hours will be “unoccupied”. This profile applies for the school year which runs from August through June.
During the shutdown month of July all hours will be designated as “unoccupied”. Schedule data is shown in
Figure 3.5.
9. Supply Terminals. All zones use parallel fan powered mixing box terminals with 0.5 in wg total fan static, 50%
overall fan efficiency and a 95 F heating supply temperature. Minimum supply airflow for the terminals is based
on ASHRAE Standard 62.1-2007 requirements. We will specify minimum zone airflow as zero so the program
will automatically use the Standard 62.1-2007 requirement to set the minimum damper position. The heat
source for the reheat coils is electric resistance.
10. Sizing Criteria. Required zone airflow rates will be based on the peak sensible load in each zone. Required
space airflow rates will be based on peak space loads for the individual spaces. Safety factors will be specified
as zero. A margin of safety will be applied later during equipment selection.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Design Example: Entering Data
After weather, space and HVAC system data has been gathered, it is entered into HAP. This is the third step in the
design process. The procedure for entering data into HAP is presented below in a tutorial format.
1. Program Setup
a. (Optional) If you are running HAP, it may be helpful to switch to System Design mode before entering data.
This hides energy analysis inputs from view and simplifies the user interface. To switch to System Design
Mode, choose "Preferences" on the View Menu and then uncheck the "Enable Energy Analysis Features"
check box. This feature is only available in HAP and not in HAP System Design Load.
2. Create a New Project
a. (Optional) If you only wish to view this example rather than entering all the data yourself, you can use archive
data for the example problem which is provided on the HAP CD. To use this archive file:
Run HAP. Use the New option on the Project Menu to create a new untitled project. The n choose the
Retrieve option on the Project Menu. In the Retrieve window choose the archive file containing the HAP
example problem and click the Optn button. On the next window click the Retrieve button. Finally, after data
has been retrieved, use the Save option on the Project Menu to save the project. Use the project name
"Example Problem".
Skip to step 3 below.
=OR=
b. If you will be entering example problem data yourself, choose New on the Project menu. This creates a new
project. A project is the container which holds your data. The new project you create will contain data for the
example problem.
Page 5 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
c. Then choose Save on the Project menu. Because you are saving the project for the first time, you will be
asked to specify a name for the project. Use "Example Problem" as the project name. From here on, save the
project periodically.
3. Enter Weather Data
a. Click the "Weather" item in the tree view in the main program window. A "Weather Properties" item appears in
the list view.
b. Double click on the "Weather Properties" item in the list view. The Weather input form will appear.
c. From the drop-down lists on the Weather form, choose data for United States / Illinois / Chicago IAP. Also
select design cooling months of May through November, and specify daylight savings time from April 7
through October 26. Please refer to the HAP Quick Reference Guide for a complete listing of the inputs.
d. When finished entering this data, press the OK button on the Weather input form to save the data and return
to the main program window.
4. Enter Space Data
Entering space data is the most labor-intensive phase of data entry. By using the program’s "duplicate" feature
input effort can be minimized. First enter data for the "D101- Typical Classroom" space:
a. Click the "Space" item in the tree view in the main program window. Space information will appear in the list
view.
b. Double-click on the "" item in the list view. The Space input form will appear.
c. Enter data on the General tab of the space input form. For this and subsequent tabs, a complete listing of
input data can be found in the HAP Quick Reference Guide.
d. Switch to the Internals tab on the space input form and enter data. As you enter internal load data it will be
necessary to create a lighting schedule and an occupant schedule. This can be done "on-the-fly" without
leaving the space input form. Simply choose the "" item in the schedule drop-down list.
This will launch the schedule input form. Enter data for the appropriate schedule. If you are new to the
Schedule form, make frequent use of the help features on this form to learn about the many ways in which
schedule data can be entered. When finished, press the OK button to save the schedule and return to the
space form. When you do this, the schedule you created will be assigned to the space automatically. For
example, if you chose "" from the drop down list for overhead lighting schedule, the
schedule you create will be assigned to overhead lighting automatically.
e. Switch to the Walls, Windows, Doors tab on the space input form and enter data. As you enter this data it will
be necessary to create wall, window, door and external shade constructions. For example, while the desired
exposure line in the table is highlighted, you can create the wall construction for that exposure by choosing
the "" item in the wall drop-down list. Similar procedures are used for creating window and
external shade constructions. Wall, window, door and shade construction data is also
f. Switch to the Roofs, Skylights tab on the space input form and enter data. As you enter this data it will be
necessary to create a roof construction. With the desired exposure row in the table highlighted, you can
create a roof construction for that exposure by choosing the "" item in the roof drop-down
list.
g. Switch to the Floors tab on the space input form and enter data.
h. At this point, press the OK button to save data for space D101 and return to the main program window.
D102 and D103 are identical to D101, so the next space we enter will be "D104 - Classroom". The "duplicate"
feature can be used to minimize input effort:
a. Right-click the "D101 - Typical Classroom" space item in the list view portion of the main program window. On
the pop-up menu that appears, select the "duplicate" option. A duplicate of "D101 - Typical Classroom" will be
created, the space input form will be launched and data for the new space will be displayed. Because this
new space is a copy of D101, we will only need to modify items which differ from D101.
b. On the General tab of the space input form change the space name to "D104 - Classroom" and specify its
floor area. Input data for this tab and the subsequent tabs is provided in the HAP Quick Reference Guide.
c. Switch to each of the other tabs on the space input form in succession and enter data. Note that many of the
default values for this space will not need to be changed since much of the space data is common among
spaces. By making duplicates of successive spaces, the number of items which need to be modified will be
minimized.
Page 6 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
System Design Example: Generating Reports
3.0 System Design Example Problem ››
System Design Example: Selecting Equipment
3.0 System Design Example Problem ››
d. When finished modifying data for space D104, press the OK button to save data for space D104 and return to
the main program window.
Enter data for the remaining spaces using a procedure similar to that used for D104: Use the "duplicate" feature
to create successive copies of spaces and modify the data for each new space you create in this manner. As
you enter data for the remaining spaces, use a strategy of entering similar spaces consecutively. The
recommended order for the remaining spaces in this example is D106, D107, D108, D109, D110, D111, D113,
and D114 Input data for the remaining spaces is provided in the HAP Quick Reference Guide.
5. Enter Air System Data
a. Click on the “System” item in the tree view in the main program window. System information will appear in the
list view.
b. Double-click on the “” item in the list view. The System input window will appear.
c. Enter data for the “VAV Rooftop” air system. A complete list of inputs is provided in the HAP Quick Reference
Guide. If you are new to the air system window, make frequent use of the help button or the on-line help
features (F1 key) to learn about operation of this window.
d. As you enter data you will need to create a fan/thermostat schedule for the air system. This is done in a
manner similar to creating schedules “on-the-fly” for spaces. In the Thermostats data view on the Zone
Components tab, choose the “” item in the schedule drop-down list. This will launch
the Schedule input window. Be sure to specify the schedule type as “fan/thermostat” instead of “fractional”.
When finished, press the OK button to save the schedule and return to the air system window. The schedule
will be assigned to the air system automatically.
e. When finished entering air system data, press the OK button on the System window to save your data and
return to the main program window.
At this point all input data has been entered and we’re ready to design the system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Design Example: Generating Reports
The fourth step in the design process is to use the data entered in step 3 to perform system design calculations
and generate system design reports. The procedure for doing this is as follows:
1. Click the Systems item in the tree view portion of the main program window. Systems information will appear in
the list view.
2. Right click the "VAV Rooftop" item in the list view. On the menu which appears, select the "Print/View Design
Results" item. The System Design Reports window will appear.
3. In the System Design Reports window, select the "System Sizing Summary", "Zone Sizing Summary" and
"System Load Summary" report options. Then press the Preview button.
4. When you press the Preview button, the program will determine whether system design data exists for the air
system. Since design data has not yet been calculated, the program will run design calculations automatically. A
status monitor will appear to help you track the progress of the calculation. Once the calculation is finished, the
reports you requested will appear in the HAP Report Viewer.
5. The Report Viewer can be used to browse and print the reports. Use the scroll bar to browse the bundle of
reports. Samples of the system design reports are provided in the HAP Quick Reference Guide. Information in
these reports can be used to size the various components of the HVAC system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm
System Design Example: Selecting Equipment
The final step in the design process is to use system design reports to select HVAC equipment. At the beginning of
this example, nine equipment sizing objectives were listed. Data provided on the System Sizing Summary report
and the Zone Sizing Summary report can be used to meet all nine of these objectives. The Air System Design Load
Summary provides supplemental information about component loads. The table below lists the nine sizing
objectives and the report and table which contains data needed to meet each objective.
The System Sizing Summary report contains data used to select the packaged rooftop unit. The Central Cooling
Coil Sizing Data table lists the peak coil capacities, coil entering and leaving conditions and a number of useful
check figures. The Preheat Coil Sizing Data table lists the peak load for this coil as well as entering and leaving
conditions. The Supply Fan Sizing Data table provides the required airflow rates and motor data for the supply fan.
The Outdoor Ventilation Air Data section lists the total outdoor air requirement for the system. Together this data
can be used in packaged rooftop unit selection software offered by Carrier and other manufacturers to select a
rooftop unit which meets the sizing requirements.
The Zone Sizing Summary report contains data used to select terminal equipment. The Zone Sizing Data table lists
the required airflow rate for each zone terminal. It also lists the minimum airflow rate which can be used to set
minimum damper positions for the mixing boxes. The Zone Terminal Sizing Data table lists the required sizes for
the parallel mixing box fans, the reheat coils and the zone heating unit coils. The Space Loads and Airflows table
lists the required airflows for each space served by the system. Because 10 of the 11 zones contain a single space,
space and zone airflows for these zones will match. For the Music Room zone which contains four spaces, the
airflow rates can be used to size ductwork and supply diffusers for the four rooms in this zone. Together this data
can be used in air terminal selection software offered by Carrier and other manufacturers to select terminal
components which meet the sizing requirements. This data can also be used in duct design calculations to size
ductwork for the system.
Table 3.2. Location of System Sizing Data on Design Reports
Objective:
Table
Report: Air System Sizing Summary
1. Rooftop Cooling Capacities
Central Cooling Coil Sizing Data
2. Rooftop Supply Fan Airflow
Supply Fan Sizing Data
3. Rooftop Preheat Coil Capacity
Preheat Coil Sizing Data
4. Rooftop Outdoor Ventilation Airflow
Outdoor Ventilation Air Data
Report: Zone Sizing Summary
5. Supply Terminal Airflow Rate
Zone Sizing Data (see "Design Air Flow")
6. Supply Terminal Minimum Airflow Rates
Zone Sizing Data (see "Minimum Air Flow")
7. Supply Airflow Rates for Mixing Box Fans
Zone Terminal Sizing Data (see "Mixing Box Fan Airflow")
8. Terminal Reheat Coil Capacities
Zone Terminal Sizing Data (see "Reheat Coil Load")
9. Space Airflow Rates
Space Loads and Airflows (see "Air Flow")
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 8
3.0 System Design Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF940.htm