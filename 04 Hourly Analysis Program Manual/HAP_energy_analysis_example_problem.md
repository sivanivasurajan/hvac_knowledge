4.0 Energy Analysis Example Problem
Overview for Energy Analysis Example Problem
4.0 Energy Analysis Example Problem ››
Energy Analysis Example: Defining the Problem
4.0 Energy Analysis Example Problem ››
This chapter provides a detailed example problem for energy modeling.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Energy Analysis Example Problem
The procedure for conducting an energy analysis with HAP involves five steps:
1. Define the Problem.
2. Gather Data.
3. Enter Data Into HAP.
4. Use HAP to Generate Simulation Reports.
5. Evaluate the Results.
The example problem presented in the following topics will demonstrate the first four steps in this process.
Sample printouts of input data and calculation results can be found in the HAP Quick Reference Guide.
Note: The following example problem describes energy analysis performed during the detailed design phase
of a project. A different procedure can often be used when performing energy analysis in the preliminary or
schematic design phase of a project. HAP provides special features to make this type of analysis fast and
easy. Please refer to the energy analysis tutorial for preliminary design applications for further details.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Example: Defining the Problem
The objective of this example problem is to estimate annual energy use and energy cost for a building.
Normally an energy analysis compares energy use and cost for two or more design scenarios. To make this
example practical and efficient, the scope of the example will be limited to estimating energy use and cost for a
single design scenario. This will demonstrate the key steps in the energy analysis process. In a real energy
study, certain of the steps would be repeated to generate the additional design scenarios being evaluated.
The example will analyze the classroom wing of the high school building used in the system design example
problem discussed earlier. The floor plan for this wing of the school building is shown below. It is comprised of
six classrooms, a music room and its associated office, storage and practice rooms, plus two corridors for a
total of 12 rooms.
The rooms in this portion of the school building will be air conditioned by one VAV rooftop unit serving parallel
fan powered mixing box (PFPMBX) terminals. A gas-fired preheat coil in the rooftop unit and electric
resistance heating coils in the mixing box terminals provide heating. HAP will be used to simulate building
loads and equipment operation hour-by-hour for one year in order to determine energy use and energy cost.
Note: The VAV air system serves all of the spaces shown in the figure below except for D105 South Vestibule
and D112 West Vestibule. The two vestibules contain fan coil heaters and would be modeled using a separate
heating-only fan coil air system. For purposes of this example we will focus on the VAV air system and omit
consideration of the vestibule fan coil units.
Page 1 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
Energy Analysis Example: Gathering Data
4.0 Energy Analysis Example Problem ››
Floor Plan for School Building
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Example: Gathering Data
The second step in the analysis process is to gather information necessary to model heat transfer processes
in the building, to analyze operation of the HVAC equipment and to calculate costs for energy and fuel use.
This involves gathering data for the building, its environment, the HVAC equipment and the utility rate
structures. Below, each type of data will be discussed.
Gathering Weather Data
The same design weather conditions used in the system design example problem will be used here: ASHRAE
design weather conditions for Chicago O’Hare International Airport, plus daylight savings time specifications
and cooling design calculation months. Please refer to the HAP Quick Reference Guide for a complete list of
inputs.
For the energy analysis, simulation weather data will also be needed. This is observed weather data for a
typical year spanning all 8,760 hours in the year. We will use the Typical Meteorological Year (TMY2) weather
file for Chicago O’Hare International Airport as the source of this data. This data is provided in the library of
HAP simulation weather data.
Page 2 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
In addition, the operating calendar for the year must be specified. We will use a calendar with January 1st
falling on a Saturday and having the following days designated as holidays:
Calendar of Holidays
Date
Holiday
January 1
New Year’s Day
April 18 – 22
Spring Holiday
May 30
US Memorial Day
June 25 – August 14
Summer Holiday
September 5
US Labor Day
November 24, 25
US Thanksgiving Holiday
December 24 – 31
Christmas/New Year Holiday
Gathering Space Data
Data describing the heat transfer elements of each room in this wing of the building will be the same as
described in the system design example problem. This earlier discussion covered wall, roof, window, external
shade, schedule and space data.
The only adjustment needed for energy analysis will be the assignment of schedule profiles to days of the
week and times of year. The "School\_In\_Session" profiles for each schedule will be assigned to weekdays in
all 12 months. The "Weekend/Holiday" profiles for each schedule will be assigned to Saturday, Sunday and
Holidays in all 12 months. Because we have designated the June 25 to August 14 summer shutdown period
as "holidays" we do not need to create separate profiles representing operation during the shutdown days.
Please refer to the HAP Quick Reference Guide for a complete list of inputs.
Gathering Air System Data
One VAV rooftop unit will provide air-conditioning to the rooms in this wing of the school building. Heating will
be provided by a gas-fired preheat coil in the rooftop unit and electric resistance coils in the parallel fan
powered mixing box terminals. Data defining this air system equipment is the same as described in the system
design example problem.
Because we are performing an energy analysis, performance data for the DX cooling apparatus and the gas-
fired preheat coil will need to be added to this system data.
Performance data associated with the rooftop unit is as follows:
Design outdoor air temperature = 91 F.
Gross cooling capacity = Peak Load + 15% safety factor.
AHRI Performance Rating = 11.0 EER
Outdoor air temperature for start of head pressure control = 55 F
Outdoor air temperature for unit shutoff = 15 F
Preheat Coil Gross heating capacity = Peak Load + 25%
Efficiency for gas-fired heat exchanger = 82%
Gathering Electric Rate Data
The General Service electric rate structure for the local utility company is defined as follows:
Monthly Customer Charge
The Monthly Customer Charge shall be $40.00
Demand Charge
Charge per kilowatt for all kilowatts of Maximum Demand for the month:
For Summer Months........................................$14.50
For Winter Months.......................................... $11.25
Page 3 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
Energy Analysis Example: Entering Data
4.0 Energy Analysis Example Problem ››
For purposes of the demand charge, the Summer Months shall be the customer’s first billing period with an
ending meter reading on or after June 15 and the three succeeding monthly billing periods.
Energy Charge
Charge per kilowatt-hour for kilowatt-hours supplied in the month:
For the first 30,000 kilowatt-hours..................... $0.04247
For the next 470,000 kilowatt-hours................... $0.03167
For all over 500,000 kilowatt-hours.................... $0.03118
Maximum Demand
The Maximum Demand shall be the highest 30-minute demand established at any time during the month.
Minimum Charge
The minimum monthly charge shall be the Monthly Customer Charge.
Gathering Fuel Rate Data
The packaged rooftop unit uses gas heating equipment so a fuel rate for natural gas must be defined. The
General Service natural gas rate structure for the local utility company is defined as follows:
Monthly Customer Charge
The Monthly Customer Charge shall be $22.00
Distribution Charge
Charge per Therm for natural gas supplied in the month:
For the first 100 Therms................................... $0.22360
For the next 4,900 Therms................................ $0.11500
For all over 5000 Therms.................................. $0.05329
Gas Charge
Charge per Therm for natural gas supplied in the month:
For all Therms................................................. $0.39650
Minimum Charge
The minimum monthly charge shall be the Monthly Customer Charge.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Example: Entering Data
Once input data has been gathered, it is entered into HAP. This is the third step in the analysis process. The
procedure for entering data into HAP is presented below in a tutorial format.
1. Program Setup
a. (Optional) If you are running HAP and switched to System Design mode for system design work, you
must switch back to full HAP mode in order to perform energy analysis work. To activate energy analysis
features, choose "Preferences" on the View Menu and then check the "Enable Energy Analysis
Features" check box.
2. Project Setup
a. (Optional) If you only wish to view this example rather than entering all the data yourself, you can use
archive data for the example problem which is provided on the HAP CD. To use this archive file:
Run HAP. Use the New option on the Project Menu to create a new untitled project. The n choose the
Retrieve option on the Project Menu. In the Retrieve window choose the archive file containing the HAP
example problem and click the Optn button. On the next window click the Retrieve button. Finally, after
data has been retrieved, use the Save option on the Project Menu to save the project. Use the project
Page 4 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
name "Example Problem".Copy the Example.E3A file from the \Example folder on the CD to the \E20-
II\Archives folder on your computer.
Skip to step 3 below.
=OR=
b. If you already performed the system design portion of this example problem (Chapter 3), then a project
already exists containing example problem data. In this case use the Open option on the Project Menu to
open the project.
=OR=
c. If you did not work through the system design portion of the example, choose New on the Project menu.
This creates a new project. Then choose Save on the Project Menu. Name the project "Example
Problem". From here on, periodically save the project as you enter data.
3. Enter Weather Data
a. Click the “Weather” item in the tree view panel in the main program window. A “Weather Properties” item
appears in the list view panel.
b. Double click on the “Weather Properties” item in the list view. The Weather input window will appear.
c. On the General tab enter design weather parameters. The HAP Quick Reference Guide provides a list of
these inputs. If you previously worked through the system design example problem, this design weather
data will already exist and does not need to be re-entered.
d. Next click on the Simulation tab to define simulation weather data and operating calendar data.
Press the “Select From HAP Library” button to select simulation weather data. This will display the
“Select City” window listing simulation weather files in the \E20-II\Weather folder. In this folder, choose
the USA\_Illinois\_Chicago\_TMY2.HW1 file. It contains simulation weather data for Chicago.
After returning to the Weather window, specify the day of the week for January 1st as Saturday.The list
of holidays to be specified is found in the HAP Quick Reference Guide.
e. Finally, press the OK button to save the data and return to the HAP main window.
4. Enter Space Data
If you previously worked through the system design example problem, then data for spaces and associated
walls, roofs, windows, external shades and schedules has already been defined. Only modifications to the
schedule data will be required as described in step 5 below.
On the other hand, if you did not work through the system design example problem, enter all the space
data. The system design example problem describes this information. The HAP Quick Reference Guide
provides a list of these inputs. While entering this data press F1 or the Help button if you have questions
about input items or procedures.
5. Modify Schedule Data
The entry of schedule data described in the system design example problem only covered data for system
design applications. For energy analyses, profiles within the schedule must be assigned to the days of the
week and times of year. Repeat the following steps for each of the four schedules in this example problem:
a. Edit the schedule.
b. Click on the assignments tab. Assign the "School\_In\_Session" profile to Monday through Friday for all 12
months. Assign the "Weekend/Holiday" profile to Saturday, Sunday and Holidays for all 12 months. The
HAP Quick Reference Guide provides a list of these inputs. For helpful hints on quickly entering this
data, please refer to the online help system by pressing "Help" or F1 while on the Schedule form.
6. Enter Air System Data
If you previously worked through the system design example problem then you only need to add
equipment performance data for the gas-fired preheat coil and the DX cooling apparatus. To add this data,
edit the Packaged Rooftop AHU and enter the data described below.
Page 5 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
If you did not work through the system design example, enter all data for the system. These inputs are
described in the system design example problem. The HAP Quick Reference Guide provides a list of
these inputs. If you have questions about input data or procedures, press F1 or the Help button on the
System form.
a. Next enter the equipment performance data as described below.
b. Go to the Equipment Tab on the System form.
c. Press the "Edit Equipment Data" button opposite "Preheat Unit". In the Equipment window that appears
enter data for the preheat coil. Refer the HAP Quick Reference Guide for a list of these inputs. Then
press OK to return to the System form.
c. Next press the "Edit Equipment Data" button opposite "Central Cooling Unit". In the Equipment window
that appears enter data for the DX cooling equipment. Refer the HAP Quick Reference Guide for a list of
these inputs. Then press OK to return to the system form.
d. Finally press OK to save the system inputs and return to the HAP main window.
7. Enter Electric Rate Data
a. Click on the "Electric Rate" item in the tree view panel in the main program window. Electric Rate
information will appear in the list view panel.
b. Double-click on the  item in the list view panel. The Electric Rate input form will
appear.
c. Enter data for the electric rate. The HAP Quick Reference Guide provides a list of these inputs. While
entering data press F1 or the Help button if you have questions about input items or procedures.
d. The electric rate described in Gathering Data contains a customer charge and a minimum charge.
Seasonal scheduling is used with a 4-month summer season running from June through September. The
energy charge is a "declining block" type of charge with 3 steps. Modeling of this type of charge is
discussed in the application topic for modeling utility rates. The demand charge is a "flat price" type of
charge with 2 steps, one for each season. This type of charge is also discussed in the application topic
for utility rates. The billing demand is equal to the measured peak demand so there are no demand
determination clauses.
e. After entering the electric rate data, press the OK button to save the data and return to the HAP main
window.
8. Enter Fuel Rate Data
a. Click on the "Fuel Rate" item in the tree view panel in the main program window. Fuel Rate information
will appear in the list view panel.
b. Double-click on the  item in the list view panel. The Fuel Rate input form will
appear.
c. Enter data for the fuel rate. Refer the HAP Quick Reference Guide for a list of these inputs. While
entering data press F1 or the Help button if you have questions about input items or procedures.
The Natural Gas fuel rate described in Gathering Data contains a customer charge and a minimum
charge.
The fuel charge is a "declining block" type of charge with 3 steps. Modeling of this type of charge is
discussed in the application topic for modeling utility rates. One wrinkle in this fuel rate is that separate
"distribution" and "gas" charges are listed. These need to be combined into one set of prices. An easy
way to do this by using the on-line calculator feature of the program. For example, for the first step in the
fuel charge enter the value 0.2236+0.3965=. When you press the "=" key the two values will be added
and the result displayed in the input cell.
Finally, there is no demand charge for this fuel rate and therefore there are also no demand
determination clauses.
d. After entering the fuel rate data, press the OK button to save the data and return to the HAP main
window.
9. Enter Building Data
Page 6 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
Energy Analysis Example: Generating Reports
4.0 Energy Analysis Example Problem ››
The final data entry step involves building data. The building is simply a container for all the system, plant
and non-HVAC energy-consuming equipment for a design alternative. Because we are dealing with a
packaged rooftop unit in this example, we only have system equipment. No chilled water, hot water or
steam plant equipment is involved. Therefore, the building contains only the VAV Rooftop air system and
the electric and fuel rate pricing structures (note that lighting and electric equipment data is calculated as
part of the air system simulation and is automatically included when you include the system in the building).
To enter this data:
a. Click on the "Building" item in the tree view panel in the main program window. Building information will
appear in the list view panel.
b. Double-click on the  item in the list view panel. The Building input form will appear.
c. Enter data for the building. Refer the HAP Quick Reference Guide for a list of these inputs. While entering
data press F1 or the Help button if you have questions about input items or procedures.
On the Plants tab, enter the reference name for the building as "Base Case Design". In many
applications plants would also be included in the building. However, this example problem does not
involve plants so no further inputs are needed on this tab.
On the Systems tab, select the VAV Rooftop air system to include it in the building. A system multiplier of
1 will be used.
The Misc. Energy tab contains inputs for non-HVAC systems which consume energy and have not yet
been accounted for. In the example problem, the only non-HVAC equipment is lighting and it has already
been accounted for in space inputs. Therefore, no data needs to be entered on the Misc. Energy tab.
Finally, on the Meters tab, select the "General Service Electric Rate" you defined earlier for the electric
meter. Select the "General Service Gas Rate" you defined earlier for the natural gas meter. As an
alternative to entering electric and fuel rates prior to entering the building (steps 7 and 8), you could
create these rates at the same time as the building. To do so use the "create new..." options on the drop-
down lists for electric and natural gas rates.
d. After entering the building data, press the OK button to save the data and return to the HAP main
window.
At this point all input data has been entered and we’re ready to generate energy simulation reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Example: Generating Reports
The fourth step in the energy analysis procedure is to use the data entered in step 3 to perform energy
analysis calculations and generate simulation reports. The procedure for doing this is as follows:
1. Click the Building item in the tree view portion of the main program window. Building information will appear
in the list view.
2. Right click the "Base Case Design" item in the list view. On the menu which appears, select the "Print/View
Simulation Results" item. The Building Simulation Reports window will appear.
3. In the Building Simulation Reports window, select the "Annual Component Costs" and "Monthly Energy Use
by by System Component" options. The Annual Component Costs report will list the costs for each system
component such as fans, cooling, heating and lights. The "Monthly Energy Use by System Component"
report will list monthly energy consumption by system component and energy type. These are just two of
the many useful reports offered for building simulations. They were chosen to provide a sample of energy
simulation results. The choice of simulation results depends on the information you are seeking. Some
reports compare final results for multiple buildings. Others provide more detailed information for a single
building and are used when investigating aspects of building performance. Read More.
Page 7 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm
4. After selecting the reports, press the Preview button. The program will determine whether system and
building calculations need to be run before generating the report. Calculations will be required the first time
you generate reports and they will run automatically. A status monitor will help you keep track of the
progress of the calculation. Once the calculation is finished your reports will be generated and displayed in
the Report Viewer.
5. The Report Viewer can be used to browse and print the reports. Use the scroll bar to browse the reports in
the bundle. Samples of these reports are provided in the HAP Quick Reference Guide.
Information about intermediate results in an energy simulation can also be obtained. These reports are useful
for investigating aspects of performance for a particular air system or plant included in the building. For
example, the following steps can be used to generate simulation reports for the VAV Rooftop air system.
1. Click the Air System item in the tree view portion of the main program window. System information will
appear in the list view.
2. Right-click the "VAV Rooftop" item in the list view. On the menu which appears, select the "Print/View
Simulation Results" item. The System Simulation Reports window will appear.
3. In the System Simulation Reports window, place a check in the box in the "Table" column opposite "Monthly
Simulation Results". Then press the Preview button. Because simulation calculations were just run, this
report will be displayed immediately. It shows monthly total loads and energy use for all components in the
air system. A sample of this report is shown in the HAP Quick Reference Guide. Many other report options
are provided in the System Simulation Report windows and can provide useful information when studying
system performance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 8
4.0 Energy Analysis Example Problem
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh55DD.htm