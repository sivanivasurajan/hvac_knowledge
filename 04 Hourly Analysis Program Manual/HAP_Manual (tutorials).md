2.0 Tutorials
HAP System Design Tutorial
2.0 Tutorials ››
This chapter provides brief tutorials for using HAP for three common applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP System Design Tutorial
This help topic provides a quick tutorial on using HAP to design systems and plants. It is designed for readers
who want a quick description of how to use the program and are already familiar with the design process, and
HAP terminology.
When you start HAP, the main program window appears. At this point the design process involves the
following five steps to design systems and two additional steps to design plants:
1. Create a New Project
a. Choose New on the Project menu. This creates a new project . A project is the container which holds
your data.
b. Choose Save on the Project menu. You’ll be asked to name the project. From here on, save the project
periodically.
2. Enter Weather Data
a. Click on the "Weather" item in the tree view in the main program window. A "Weather Properties" item
appears in the list view.
b. Double click on the "Weather Properties" item in the list view. The Weather input form will appear.
c. Enter weather data.
d. Press the OK button on the Weather input form to save the data and return to the main program window.
3. Enter Space Data
a. Click on the "Space" item in the tree view in the main program window. Space information will appear in
the list view.
b. Double-click on the "" item in the list view. The Space input form will appear.
c. Enter data for your first space. While entering spaces, you may need to create schedules, Enter data for
your first space. While entering spaces, you may need to create schedules, walls, roofs, windows, doors
or external shades. You can do this by choosing the "create new …" item in drop-down selection lists.
For example, when entering overhead lighting data, you must choose a schedule. In the schedule drop-
down list, choose the "create new schedule" item to create a schedule and automatically assign it to
overhead lighting. Similar procedures are used for walls, roofs, windows, doors and external shades. An
alternate approach is to create schedules, walls, roofs, windows, doors and external shading prior to
entering space data.
d. Press the OK button on the Space input form to save your data and return to the main program window.
e. To enter another space, in the list view right-click on the name of the space you just created. The space
pop-up menu appears.
f. Choose the Duplicate option on the pop-up menu. A copy of the original space will be created and its
input form will appear. This is a quick way of generating new spaces based on defaults from the previous
space.
g. Enter data for this new space.
h. Press the OK button on the Space input form to save your data and return to the main program window.
i. Repeat the previous four steps to enter data for as many spaces as you need.
4. Enter Air System Data
a. Click on the "System" item in the tree view in the main program window. System information will appear
in the list view.
Page 1 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm
b. Double-click on the "" item in the list view. The System input form will appear.
c. Enter data for your first system. While entering the system, you will need to create a fan/thermostat
schedule. You can do this by choosing the "create new schedule" item in the fan/thermostat schedule
drop-down list. This will create a schedule and automatically assign it to your system. An alternate
approach is to create this schedule before entering air system data.
d. Press the OK button on the System input form to save your data and return to the main program window.
e. To enter another system, in the list view right-click on the name of the system you just created. The
system pop-up menu appears.
f. Choose the Duplicate option on the pop-up menu. A copy of the original system will be created and its
input form will appear. This is a quick way of generating new systems based on defaults from the
previous system, if successive systems are similar. If they are not, use the "new default system" option to
create each new system.
g. Enter data for this new system.
h. Press the OK button on the System input form to save your data and return to the main program window.
i. Repeat the previous four steps to enter data for as many systems as you need.
5. Generate System Design Reports
a. Click on the "System" item in the tree view in the main program window. System information will appear
in the list view.
b. Select the systems for which you want reports.
c. Choose the "Print/View Design Results" option on the Reports menu.
d. On the System Design Reports form , choose the desired reports.
e. To view the reports before printing, press the Preview button.
f. To print the reports directly, press the Print button.
g. Before generating reports, HAP will check to see if system design calculations have been performed. If
not, HAP automatically runs these calculations before generating the reports.
6. Enter Plant Data (if necessary)
a. Click on the "Plant" item in the tree view in the main program window. Plant information will appear in the
list view.
b. Double-click on the "" item in the list view. The Plant input form will appear.
c. Enter data for your first plant. For plant design purposes users will typically only select from the first six
plant types (one of the "Generic" types). HAP users have additional options for specific types of chilled
water, hot water and steam plants, but these require extra data not relevant to the design calculation.
Therefore it is more efficient to use the Generic plant types for design. Later Generic plants can be
converted into specific plant types without loss of data.
d. Press the OK button on the Plant input form to save your data and return to the main program window.
e. To enter another plant, in the list view right-click on the name of the plant you just created. The plant pop-
up menu appears.
f. Choose the Duplicate option on the pop-up menu. A copy of the original plant will be created and its input
form will appear. This is a quick way of generating new plants based on defaults from the previous plant,
if successive plants are similar. If they are not similar, use the "new default plant" option to create each
new plant.
g. Enter data for this new plant.
h. Press the OK button on the Plant input form to save your data and return to the main program window.
i. Repeat the previous four steps to enter data for as many plants as you need.
7. Generate Plant Design Reports (if necessary)
a. Click on the "Plant" item in the tree view in the main program window. Plant information will appear in the
list view.
b. Select the plants for which you want reports.
c. Choose the "Print/View Design Results" option on the Reports menu in the menu bar.
d. On the Plant Design Reports form , choose the desired reports.
e. To view the reports before printing, press the Preview button.
f. To print the reports directly, press the Print button.
g. Before generating reports, HAP will check to see if plant design calculations have been performed. If not,
HAP automatically runs these calculations before generating the reports.
Page 2 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm
HAP Energy Analysis Tutorial - Preliminary Design
2.0 Tutorials ››
For further information, please refer to the following help topics. For a complete example problem, please refer
to the HAP Quick Reference Guide.
Using HAP to Design Systems and Plants
HAP’s Main Program Window
HAP Input Forms
Project Data Management
Performing Common Tasks
Using the Help System
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP Energy Analysis Tutorial - Preliminary Design
This topic and the next topic provide tutorials explaining how to use HAP to estimate annual energy use and
energy costs. HAP provides features suited to energy analysis in the preliminary or schematic design phase of
a project and for analysis in the detailed design phase of a project.
In preliminary design the goal is often to quickly "screen" prospective HVAC design alternatives to identify the
most promising designs for further study. In this type of analysis extensive details about the building and its
HVAC equipment may not yet be known or may not be relevant for obtaining useful screening results. As a
result a simplified modeling approach can be used and data entry can be made faster. HAP provides a set of
"wizard" features to help users rapidly generate building and HVAC equipment input data for these
applications. This topic provides a tutorial explaining how to use those features.
In detailed design the goal is to investigate energy consumption and energy cost performance of HVAC
designs in greater detail. In this type of analysis complete details about the building envelope, layout and use
are known and HVAC equipment is defined in greater detail. As a result, data entry is more involved, but
results are also more detailed and accurate. The following topic provides a tutorial explaining how to use HAP
for energy analysis in detailed design applications.
Energy Analysis Tutorial for Preliminary Design
When HAP is started, the main program window appears. At this point the energy analysis involves the
following 5 steps.
1. Create a New Project
a. Choose New on the Project menu. This creates a new project. A project is the container which holds your
data.
b. Choose Save on the Project menu. You’ll be asked to name the project. From here on, save the project
periodically.
2. Run a Full Wizard Session to Rapidly Define All Input Data
a. Choose the Full Wizard Session option on the Wizards menu.
b. In the Full Wizard Session window, first click the Weather button. Select the weather data for your
analysis by either clicking on the map images or using the drop-down lists at the bottom of the Weather
Wizard window. Then click OK to exit the Wizard.
c. From the Full Wizard Session window, then click the Building button. Enter data describing your building
on the two Building Wizard input screens. Then press Finish to exit the Wizard.
d. From the Full Wizard Session window, click the Equipment button next. The Equipment Alternatives
window will appear.
e. In the Equipment Alternatives click the Add button to add a new HVAC equipment alternative. Enter data
on the Equipment Wizard screens to describe your air-side equipment and, as applicable, your DX or
plant equipment. Press Finish to exit.
Page 3 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm
HAP Energy Analysis Tutorial - Detailed Design
2.0 Tutorials ››
f. Repeat the previous step for each equipment alternative you wish to include in your study.
g. When finished, click the Close button on the Equipment Alternatives window to return to the Full Wizard
Session window.
h. From the Full Wizard Session window, click the Utility Rate button. Enter data describing your electric
and fuel prices on the Utility Rate Wizard screens. Press Finish to exit.
i. Finally, on the Full Wizard Session window, click the Finish button. At this point HAP automatically takes
your weather, building, equipment and utility rate wizard input data and generates a complete set of
detailed input data for your analysis. When this work is finished you are returned to HAP main window.
3. Obtain Results
a. In the Building list in the right-hand list view panel select one or more buildings you want to include in
your energy cost comparison.
b. Choose the "Print/View Simulation Results" option on the Reports menu.
c. In the Building Simulation Reports window, choose the desired reports.
d. To view the reports, press the Preview button.
e. To print the reports directly, press the Print button.
f. Note that simulation reports can also be generated for systems and plants separately. These reports
provide more detailed information about the energy use of air system and plant equipment. To generate
these reports, use the same procedure described above, but select systems or plants instead of
buildings.
For further information, please refer to the following help topics.
Using HAP to Perform Energy Analyses
HAP’s Main Program Window
HAP Input Forms
Overview of HAP Wizards
Project Data Management
Performing Common Tasks
Using the Help System
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
HAP Energy Analysis Tutorial - Detailed Design
This tutorial explains how to use HAP to estimate annual energy use and energy cost for alternate system
designs. This tutorial is appropriate for energy analysis in the detailed design phase of a project where
extensive information about the building and its HVAC systems is known, and highly accurate results are
needed.
Note that a tutorial for energy analysis in the preliminary or schematic design phase of a project is provided in
a separate topic.
Energy Analysis Tutorial for Detailed Design
When HAP is started, the main program window appears. At this point the energy analysis involves the
following 7 steps. If system design work has already been completed, many of these steps will not be
necessary or will only require minimal work.
1. Create a New Project
a. Choose New on the Project menu. This creates a new project. A project is the container which holds your
data.
b. Choose Save on the Project menu. You’ll be asked to name the project. From here on, save the project
periodically.
Page 4 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm
=OR=
c. If system design work was done previously, then the project will already exist. In this case use the Open
option on the Project menu to open the project.
2. Enter Weather Data
a. Click on the "Weather" item in the tree view in the main program window. A "Weather Properties" item
appears in the list view.
b. Double click on the "Weather Properties" item in the list view. The Weather input form will appear.
c. Enter weather data. Be sure to enter data on the Simulation tab of the Weather form. Inputs on this tab
link simulation weather data to the project and define the holiday calendar for the year.
d. Press the OK button on the Weather input form to save the data and return to the main program window.
3. Enter Space Data
This step is the same as in the System Design Tutorial , but with the following exceptions:
a. Make sure that schedules for internal loads include profiles assigned for all 7 days of the week and for
holidays. Data originally used for system design work may only have defined profiles for the design day.
b. Make sure infiltration rates for energy analysis days are specified. For design work infiltration rates may
only have been specified for design cooling and design heating conditions.
4. Enter Air System Data
This step is the same as in the System Design Tutorial, but with the following exceptions:
Systems used in an energy analysis may not use the "Undefined" equipment class. Any "Undefined" system
must be converted to one of the specific equipment classes before it can be used in energy simulations. To
convert a system, edit its data and change the "Equipment Class" input from "Undefined" to one of the other
choices. This will change the cooling and heating sources for coils in the system, but will retain the other
input data. Review your input data, particularly the cooling coil and heating coil source items before saving
the system.
a. When defining data for packaged rooftop, packaged vertical units, split DX air handlers, packaged or split
DX fan coils or water source heat pumps, you must enter data on the Equipment tab of the Air System
form. This tab provides inputs describing the full load capacity, full load efficiency and operating controls
for these types of equipment.
b. When entering data for water-cooled vertical packaged units, you will need to create a cooling tower.
When entering data for a water source heat pump system you will need to create a cooling tower and an
auxiliary boiler. You can create both from within the air system form by choose the "create new cooling
tower" and "create new boiler" options on the drop-down lists used to select towers and boilers. An
alternate approach is to create towers and boilers prior to entering the air system.
5. Enter Plant Data (if necessary)
If your study includes chilled water, hot water or steam plants, define each as follows:
a. Click on the "Plant" item in the tree view in the main program window. Plant information will appear in the
list view.
b. Double-click on the "" item in the list view. The Plant input form will appear.
c. Enter data for your plant.
d. While entering plant data it may be necessary to create chillers, reversible chillers, boilers, air-to-water
heat pumps, water-to-water heat pumps, cooling towers and/or dry coolers to link to the plant. This can
be done without leaving the plant form by using the "create new ..." options which appear in the drop-
down lists used to select these plant components. An alternate approach is to define the chillers, heat
pumps, towers, and boilers prior to entering plant data.
e. Press the OK button on the Plant input form to save your data and return to the main program window.
f. If more than one plant is required for your analysis, repeat the previous steps to define each plant.
6. Enter Building Data
a. Click on the "Building" item in the tree view in the main program window. Building information will appear
in the list view.
b. Double-click on the "" item in the list view. The Building input form will appear.
c. Enter data for your building.
Page 5 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm
d. While entering building data it may be necessary to create electric and fuel rates to link to the building.
This can be done without leaving the building form by using the "create new electric rate" and "create
new fuel rate" options which appear on the drop-down lists used to select utility rates. An alternate
approach is to define the electric and fuel rates prior to entering the building.
e. Press the OK button on the Building input form to save your data and return to the main program window.
f. Repeat the previous steps to define each building in your analysis. Typically an energy analysis contains
at least two buildings containing equipment for alternate HVAC designs.
7. Generate Simulation Reports
a. Click on the "Building" item in the tree view in the main program window. Building information will appear
in the list view.
b. To study energy use and cost data for one building, select a single building. If you wish to compare
energy use and costs for a group of buildings, select all buildings in the group.
c. Choose the "Print/View Simulation Results" option on the Reports menu in the menu bar.
d. In the Building Simulation Reports window, choose the desired reports.
e. To view the reports, press the Preview button.
f. To print the reports directly, press the Print button.
g. Before generating reports, HAP will determine whether system, plant and building calculations are
necessary to generate data for your reports. If so, HAP will automatically run the calculations before
generating your reports. If no calculations are necessary, reports will be generated immediately.
Note that simulation reports can also be generated for systems and plants. These reports provide more
detailed information about the energy use of these equipment components. To generate these reports, use
the same procedure described above, but use systems or plants instead of buildings.
For further information, please refer to the following help topics. For a complete example problem, please refer
to the HAP Quick Reference Guide.
Using HAP to Perform Energy Analyses
HAP’s Main Program Window
HAP Input Forms
Project Data Management
Performing Common Tasks
Using the Help System
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 6
2.0 Tutorials
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh9550.htm