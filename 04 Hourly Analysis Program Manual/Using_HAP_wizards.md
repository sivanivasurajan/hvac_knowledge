8.0 Using HAP Wizards
8.1 Overview
8.0 Using HAP Wizards ››
Overview for HAP Wizards
8.0 Using HAP Wizards ›› 8.1 Overview ››
This chapter explains how to use the Wizard features to rapidly assemble building and energy models.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of the organization and capabilities of the Wizard feature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for HAP Wizards
This topic provides an overview of concepts and procedures for the HAP Wizard features.
A. Alternate Input Approaches.
HAP provides two distinct ways of creating input data:
1. The HAP detailed interface uses a "bottom up" approach for creating a model of the building and its HVAC systems. All data is
directly entered by the user. This approach is best suited to detailed design applications where a high level of detail is necessary.
2. The HAP wizard interface takes a "top down" approach. A user answers a relatively small set subset of questions about the building
location, the building itself, the HVAC system alternatives, and the energy and fuel prices. HAP uses these inputs with intelligent
defaulting assumptions to generate a complete set of detailed input data for the project. This approach is well suited to preliminary or
schematic design studies where you need to quickly screen multiple design alternatives to identify the most promising designs for
detailed study.
B. How Wizards Work
The Wizard interface guides you through a series of input screens which ask high level questions about the building location, the
building, HVAC equipment and utility rates. HAP then automatically applies intelligent defaulting assumptions to convert your Wizard
inputs into a complete set of detailed inputs for the detailed interface. When you return to the HAP main program window you can edit
the detailed data, if desired, and then run the energy simulations to compare energy costs.
Input data that can be configured in a Wizard session in a matter of minutes could take hours or even days to create manually in the
detailed interface. Therefore, Wizard features can greatly increase your productivity when using HAP, especially for preliminary design
and screening studies. Read More.
C. Launching the Wizard Features.
The Wizard features in HAP can be launched using options on the Wizard Menu and the toolbar:
1. The Full Wizard Session option on the Wizard Menu is used to run the Weather, Building, Equipment and Utility Rate Wizards in
tandem to generate 100% of the data needed for an energy study comparing HVAC design alternatives. This option should be used
when you need to rapidly create data for a complete analysis. The Full Wizard Session feature can also be launched via the Wizard
button on the toolbar. Read More.
2. The Weather Wizard option on the Wizard Menu is used to run the Weather Wizard alone. This option can be used to quickly set up
design and simulation weather for a project.
3. The Building Wizard option on the Wizard Menu is used to run the Building Wizard alone. This option is used when you need to
rapidly create spaces for a building and will later apply HVAC equipment to the spaces using the HAP detailed interface.
4. The Equipment Wizard option on the Wizard Menu is used to run the Equipment Wizard alone. This option is used when spaces
have been previously created and you need to quickly apply HVAC equipment to the spaces.
5. The Utility Rate Wizard option on the Wizard Menu is used to run the Utility Rate Wizard alone. This option can be used to rapidly
set up utility rates for electricity, gas, oil, and/or propane.
Note that all wizard features use a "once-thru" design. That is, after you enter data in the Wizards, HAP generates a full set of detailed
input data from your inputs and you return to the HAP main window. Once back in the HAP main window, it is not possible to return to
the Wizards and see you original inputs. Therefore, it is important to use the reporting features in the Wizards to print your Wizard
inputs if you will need to refer to them after returning to the HAP main window.
D. Weather Wizard Overview
Page 1 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
The Weather Wizard consists of one screen which allows the user to select the building location graphically via map images, or via drop
down lists. The city selection is then used go generate a full set of design and simulation weather data for the chosen site.
E. Building Wizard Overview
The Building Wizard is comprised of two input screens.
1. The Building Footprint screen allows you to define the footprint shape, dimensions and zoning, the number of floors and the building
usage type. This screen also displays a building footprint diagram to help you visualize the building you are configuring.
2. The Building Details screen allows you to define outdoor ventilation requirements, internal loads, envelope construction and
infiltration for the building.
With the data from these two input screens, the program generates detailed data for all spaces in the building as well as internal load
schedules and wall, roof and window assemblies.
F. Equipment Wizard Overview
The Equipment Wizard is comprised of a series of 1, 2 or 3 input screens from the following list, depending on the type of equipment
being defined:
1. The System and Equipment screen appears for all equipment types. It is used to define the equipment type, heating type, and the
air-side system and its key features. For DX equipment, cooling and heating performance is also defined on this screen.
2. The Chilled Water Plant screen appears when defining a system type with chilled water cooling is defined: chilled water AHUs,
hydronic fan coils, induction beams or chilled beams. The Chilled Water Plant screen is used to define one of three different kinds of
chilled water plants.
(i) A Chiller Plant provides cooling only and uses chillers.
(ii) A Changeover Plant provides both cooling and heating and uses reversible chillers. When a Changeover Plant is modeled,
make sure to specify air-side changeover controls. These inputs are found on the System and Equipment Details screen either
for central systems for fan coil systems.
(iii) A Heat Recovery Plant is comprised of of interconnected cooling and heating plants in which heat rejected by the chillers in
the cooling plant is captured and used to meet part or all of the heating loads imposed on the heating plant. When this plant
type is selected inputs on this screen will define the cooling portion of the plant and the type of heat recovery used. Inputs on
the Heating Plant screen will define the equipment in the heating portion of the plant.
3. The Heating Plant screen appears for systems using hot water or steam heat. It is used to configure the distribution system and
specify type of boilers or heat pumps, and equipment performance.
4. The WSHP Loop screen appears when defining Water Source Heat Pump or Ground Source Heat Pump systems. It defines water
loop information such as control setpoints, source water temperatures and pump, cooling tower, and auxiliary boiler performance.
These Wizard input screens display simple system diagrams to help you visualize the air-side system or plant equipment you are
configuring. Readers should note that these diagrams are not meant to be exact schematic diagrams of a system. Instead they are only
intended to show the major components and their relationship to one another.
Many of the Equipment Wizard input screens have a "Details" button that allows you to display and modify a second level of more
detailed information about the equipment. Visiting the Details input screens to modify data is optional. Some users may prefer to have
greater control over input data and assumptions and therefore will visit the detailed screens. Others may wish to work only on the top
level screens and accept the program defaulting.
The content, format and number of Equipment Wizard input screens varies widely with the type of equipment being defined. When
working with the Equipment Wizard it sometimes helps to have a mental map of the sequence of input screens. The following flow
diagrams show the sequence of screens for the three most common equipment scenarios.
F-1. DX Equipment - Rooftops, Vertical Packaged Units, Split DX AHUs, DX Fan Coil Units
Page 2 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Read More:
System and Equipment Wizard Screen
System and Equipment Details - Central Systems
System and Equipment Details - Terminal Systems
F-2. CW / HW or Steam - Chilled Water AHUs, 2-Pipe Fan Coils, 4-Pipe Fan Coils, Induction Beams, Chilled Beams
Read More:
System and Equipment Wizard Screen
System and Equipment Details - Central Systems
System and Equipment Details - Terminal Systems
Chilled Water Plant Wizard Screen
Chilled Water Plant Details
Heating Plant Wizard Screen
Heating Plant Details
F-3. WSHP - WSHP Loop or Ground Source Heat Pumps
Read More:
System and Equipment Wizard Screen
System and Equipment Details - Terminal Systems
WSHP Loop Wizard Screen
G. Utility Rate Wizard Overview
The Utility Rate Wizard consists of 1 screen when taking a simple approach to rates, or 3 input screens when using the detailed
approach.
1. The main Utility Rate Input Screen is used for both approaches. It allows flat electricity and fuel prices to be quickly defined if using a
simple approach to modeling prices. It also allows the electric rate to be specified as "detailed" at which point the user can detour
into the additional electric rate screens described below.
Page 3 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Full Wizard Session Overview
8.0 Using HAP Wizards ›› 8.1 Overview ››
2. The Detailed Electric Rate Setup Screen asks high level questions about the rate being configured. These questions involve whether
seasonal or time of day pricing will be used, and whether the energy and demand charges involve flat or stepped prices.
3. The Detailed Electric Rate Prices Screen takes information from the previous screen and automatically configures the energy charge
and demand charge pricing tables. A user only needs to enter individual prices, and block sizes (if applicable). With this two-step
design much of the difficulty in creating detailed electric rates is eliminated.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Wizard Session Overview
The Full Wizard Session option on the Wizards Menu and on the toolbar allows you to run Wizards in tandem to create a complete set
of data for an energy analysis. This option is typically used when you are starting a new project for preliminary design or screening
alternatives and you want to rapidly create a complete set of project data all at once. Read More: Wizard Overview.
When the menu option or toolbar button is clicked, the Full Wizard Session window shown above appears. This window has three key
components:
1. The Button Panel along the left side of the window contains command buttons used to perform key tasks for entering and
generating data:
a. The Weather button is used to launch the Weather Wizard to select the building location which in turn will define weather
conditions.
b. The Building button is used to launch the Building Wizard to define the size, shape, usage, internal loads and envelope for the
building.
c. The Equipment button displays the Equipment Alternatives window from which you can add, edit, copy and delete HVAC
equipment design alternatives using the Equipment Wizard.
d. The Utility Rate button is used to launch the Utility Rate Wizard to define pricing for electric energy and fuels used in the building.
Page 4 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Alternatives Window - Edit Mode
8.0 Using HAP Wizards ›› 8.1 Overview ››
e. The Finish button is used when you are finished inputting data to convert your wizard inputs into a full set of detailed HAP data
and then return you to the HAP main window. In the main window you can edit the detailed data, if desired, and then run energy
simulations.
Note that it is often useful to generate the Wizard input reports before pressing the Finish button. Once you press Finish and
return to the HAP main window, it will not be possible to see your Wizard inputs again as the Wizard inputs are not saved (only
the detailed data that is generated is saved). The input reports serve as a useful reference if you need to review your original
Wizard inputs at a later point in time.
f. The Cancel button is used to exit the Full Wizard Session and return to the HAP main window without generating detailed data.
2. The Display Panel in the right-hand portion of the window displays a concise summary of data you have created thus far in this
wizard session. As you visit each Wizard, a summary of the data you input will appear in these panels.
3. The Menu Bar along the top of the window provides three pull-down menus containing options for manipulating data in the Full
Wizard Session:
a. The Edit Menu contains options for launching each Wizard. These options serve the same purpose as the first four buttons in the
button panel.
b. The Report Menu contains options for generating reports listing data you entered in each Wizard during the current session.
Users are encouraged to use the Report options before pressing Finish to end the Full Wizard Session. The Wizards use a "once-
thru" design. After you press Finish to generate detailed data and return to the HAP main window, it is not possible to return Full
Wizard Session to see your original inputs. The original Wizard inputs are not saved - only the detailed data that is generated is
saved. Therefore, it is often useful to use the Report Menu options to print your Building Wizard and Equipment Wizard inputs so
you can refer to them later.
c. The Help Menu contains one option used to display this help topic.
Application Information. A typical sequence of steps for configuring data in a Full Wizard Session is shown below. Note that users
may actually select the wizards in steps 2 through 5 in any order desired. The order shown is just a typical sequence.
1. When the Full Wizard Session window appears, it will always default data in the display panels for the four Wizards. You always start
a Full Wizard Session with a blank slate.
2. Click the Weather button to launch the Weather Wizard and select a building location.
3. Click the Building button to launch the Building Wizard to define your building characteristics.
4. Click the Equipment button to display the Equipment Alternatives window. In this window press Add to launch the Equipment Wizard
to define your first HVAC equipment design. When finished entering data you are returned to the Equipment Alternatives window
where you can click Add or Copy to add another alternative. When finished defining all your equipment design alternatives, press
Close to return to the Full Wizard Session window.
5. Click the Utility Rate button to launch the Utility Rate Wizard to define prices for electric energy and fuels.
6. At this point if you need to make adjustments to your data, you can click the any of the Wizard buttons in the button panel to edit your
data.
7. When finished entering and editing your data, press Finish in the button panel. At this point HAP will convert your Wizard inputs into
detailed HAP data as follows:
a. Weather Wizard data is used to generate a full set of design and simulation weather data for the selected site.
b. Building Wizard data is used to generate spaces for each "zone" defined in your building, along with the specified schedules and
wall, roof and window assemblies.
c. Equipment Wizard data is used to create air systems, plants and buildings. One HAP "building" entity is created for each HVAC
alternative you defined. To this building are linked the plants and air systems described by your inputs. All related building, plant
and system names start with the alternative identifier you specified (such as "ALT1") so that you can easily identify and associate
the data.
d. Utility Rate Wizard data is used to create an electric rate and one or more fuel rates, and then link these rates to each of the
building entities generated by the Equipment Wizard.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Alternatives Window - Edit Mode
The Equipment Alternatives window appears when you click the Equipment button on the Full Wizard Session window, or choose the
Equipment option on the Edit Menu. This window allows you to create, edit, copy and delete HVAC design alternatives.
Page 5 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Alternatives Window - Report Mode
8.0 Using HAP Wizards ›› 8.1 Overview ››
The window consists of two key components:
1. The Selection List in the center and left portions of the window lists the equipment design alternatives you have created thus far in
this wizard session. You can click on items in this list to highlight them and then click a button in the Button Panel to perform a task
with the data. For example, you can highlight one item and click the Edit button to edit data for the item.
2. The Button Panel on the right side of the window provides six buttons for performing various tasks:
a. The Add button is used to create a new equipment design alternative and add it to the list.
b. The Edit button is used to display input data for the existing design alternative highlighted in the selection list so you can modify
the data.
c. The Copy button is used to create a new design alternative by copying the item highlighted in the selection list and displaying its
data for modification.
d. The Delete button is used to erase the item or items highlighted in the selection list.
e. The Close button is used to close the Equipment Alternatives window and return to the Full Wizard Session window.
f. The Help button is used to display this help topic.
Application Information. A typical sequence of steps for creating data in the Equipment Alternatives window is shown below.
a. The first time you visit the Equipment Alternatives window during a Full Wizard Session, the Selection List will be empty.
b. Click the Add button to launch the Equipment Wizard to create your first design alternative. When you exit the wizard and return to
the Equipment Alternatives window, the design alternative you created will be shown in the Selection list.
c. Click the Add button to create your second design alternative. Or if the second alternative is similar to the first, highlight the first
alternative in the Selection List and then click the Copy button.
d. Repeat step "c" until the desired equipment alternatives have been defined. Then press Close to close the window and return to the
Full Wizard Session window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Alternatives Window - Report Mode
The Equipment Alternatives window appears when you choose the Equipment option on the Report Menu. In report mode this window
is used to generate a report listing Equipment Wizard inputs for one or more equipment design alternatives selected from the list.
Page 6 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
8.2 Weather Wizard
8.0 Using HAP Wizards ››
Weather Wizard - Weather Input Screen
8.0 Using HAP Wizards ›› 8.2 Weather Wizard ››
The window consists of two key components:
1. The Selection List in the center and left portions of the window lists the equipment design alternatives you have created thus far in
this wizard session. Items selected in this list will be included in the input report when you click the View Report button.
2. The Button Panel on the right side of the window provides three buttons for performing various tasks:
a. The View Report button is used to generate the input report. The equipment design alternatives highlighted in the Selection List
will be included in the report. The report is displayed in the standard HAP report viewer. From the viewer you can examine the
report, save it to a disk file or print the report.
b. The Close button is used to close the Equipment Alternatives window and return to the Full Wizard Session window.
c. The Help button is used to display this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes use of the Weather Wizard to rapidly define site weather conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Weather Wizard - Weather Input Screen
The Weather Wizard is used to select the location for the building project. This information will then be used to automatically generate
full sets of design and simulation weather data for the project.
The weather Wizard consists of one input screen, shown below, which is divided into three parts. Features in each part are described
below the screen image.
Page 7 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
1. Map Image Panel. The upper part of the screen contains map images that can be used to graphically select your desired location.
The graphical selection approach requires the following steps to progressively zoom from the world view down to a location view on
which you can select your city.
a. First click the Select Region button below the map panel. The world map will appear. When you hover the mouse cursor over
different portions of the map, the region name will appear. Click your desired geographical region. The selected region will be
highlighted in green.
b. Next click the Select Location button below the map panel. The map view will zoom in to your selected region. For example, if you
selected the United States, the Location map will show the 50 states. Again, you can hover the mouse cursor over different
portions of the map to display state, province or country names on this map. Click the desired location. The state, province or
country will be highlighted in green.
c. Finally, click the Select City button below the map panel. The map view will zoom in to your selected state, province or country.
This new map view will show available cities. To select a city, click the city name or the dot next to the name. The dot will change
colors to indicate it is selected. Note that when running a Full Wizard session, if you select a location in the United States the
program will automatically default electric and natural gas prices based on the Energy Information Administration (EIA) state-
average price for that location.
2. Drop Down List Panel appears toward the bottom of the screen and contains three drop-down lists for region, location and city. As
you use the Map Image Panel to make selections, the items shown as selected in these drop-down lists update automatically. As an
alternative to using the map panel, you can select items directly from the drop down lists.
3. Command Buttons. The lower right corner of the input screen contains command buttons:
a. OK - If running Weather Wizard as part of a Full Wizard Session, the OK button retains your inputs and returns you to the Full
Wizard Session window. If running Weather Wizard alone from the Wizards Menu, the OK button displays the Weather Wizard
input report and then converts your data into a full set of design and simulation weather for the selected location.
b. Cancel - Exits the Weather Wizard without retaining any changes you made.
c. Help - Displays this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
8.3 Building Wizard
8.0 Using HAP Wizards ››
Building Wizard - Building Footprint Screen
8.0 Using HAP Wizards ›› 8.3 Building Wizard ››
This section describes use of the Building Wizard to rapidly assemble a building model.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Building Wizard - Building Footprint Screen
The Building Wizard is used to define the size, shape, usage, envelope and internal loads for a complete building. This Wizard consists
of two input screens:
1. The Building Footprint screen defines the footprint size and shape, the number of floors, building usage type and zoning. This screen
is discussed in further detail in this topic.
2. The Building Details screen defines outdoor ventilation air requirements, internal loads, envelope construction and infiltration for the
building. Read More.
Building Wizard inputs will ultimately be used to generate a complete set of detailed inputs for spaces in the building as well as wall,
roof, and window assemblies and internal load schedules.
The Building Footprint input screen, shown below, contains inputs divided into 4 groups and command buttons in the lower right.
Each of these input screen features will be discussed below.
1. General Information.
a. Building Type and Building Subcategory together define the usage type for the building being created. These inputs will
determine the defaults for outdoor ventilation, internal loads, constructions and infiltration that appear on the Building Details
screen. When you change either input, items on the Building Details screen are automatically reset to the proper defaults.
b. Building Identifier is a short label that will be used to identify all spaces created from the wizard inputs. This label appears as the
prefix in the space name. If you are using the Building Wizard to create multiple building scenarios, this feature helps you manage
your data by identifying which spaces are associated with which building definition.
2. Building Information defines the building footprint shape and the method of zoning. This section also contains a diagram of the
building footprint to help you visualize the building being configured.
The orientation of the building can be controlled using the compass icon located in the upper right-hand corner of the building view
pane. Initially the compass North points to the top of the pane, indicating "up" is north. To change the orientation use your mouse to
drag the compass North pointer clockwise or counterclockwise to the desired point of the compass rosette. For example if you drag
the compass North needle clockwise until the West pointer points up, the face of the building pointing up is facing West. In the figure
above "up" is northeast.
3. Building Dimensions. Items in this section describe the horizontal and vertical dimensions of the building.
a. X and Y Dimensions define the dimensions of the building footprint. The X and Y labels refer to X and Y dimensions shown in the
footprint diagram in the lower left part of the input screen. As you change these values the diagram will adjust to show a scale
representation of the footprint.
b. Perimeter Zone Depth - The horizontal distance from the exterior wall to the interior boundary of the perimeter zone. As you
change this value the footprint diagram will be scaled to show the relative size of the perimeter zone.
c. Number of Floors - The number of floors in the building. Inputs may be limited by the Building Subcategory input. For example if
you specify "Low Rise 1-2 stories" number of floors will be limited to 2.
d. Floor to Floor Height - The vertical distance between floors. This value is used to compute wall surface area.
e. Floor to Ceiling Height - The vertical distance from floor to ceiling level. This distance is used to compute space volume for
converting infiltration air changes into airflow quantities.
f. Window Area - The percentage of gross wall area which is fenestration. For example if 15% is specified, the target for each space
created is a window to wall ratio of 15%. Note the actual window to wall ratio in the generated spaces may not exactly equal the
value you define. Using the dimensions of the window assembly specified on the Building Details input screen, HAP will determine
the number of windows that comes closest to the window to wall ratio you specified. Because HAP will not consider "partial"
windows, the dimensions of your window assembly may result in a window to wall ratio slightly above or below the value you
specified.
g. Typical Intermedigte Floor. When the building contains 4 or more floors, you can choose whether to represent each intermediate
floor separately, or with as one typical floor with a multiplier applied. If you wish to use the typical floor approach, place a check
mark in the box. This feature provides a way to minimize space data created when it is not necessary to model floors above the
first floor and below the top floor separately.
Example: A building has a rectangular footprint with perimeter by exposure zoning so there are 5 zones per floor. The building has
10 floors. If you check the box for "Typical Intermediate Floor", HAP will generate 15 spaces - 5 for the first floor, 5 for one
Page 9 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Building Wizard - Building Details Screen
8.0 Using HAP Wizards ›› 8.3 Building Wizard ››
intermediate floor representing floors 2 to 9, and 5 spaces for the 10th floor. If the "Typical Intermediate Floor" box is not checked,
HAP will generate 50 spaces, 5 for each of the 10 floors.
4. Summary. This section contains display-only information about the building you are creating. Data includes the number of spaces
that will be created and floor, wall and window areas. Sometimes this information is helpful if you are trying to match a particular
building floor area target or wall area target.
5. Command Buttons. The following command buttons are provided.
a. Help - Displays this help topic.
b. Next - Displays the Building Details input screen.
c. Cancel - Exits the Building Wizard without saving any changes you made.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Building Wizard - Building Details Screen
The Building Details input screen is the second of two Building Wizard screens. It allows details regarding ventilation airflow
requirements, internal loads, envelope construction and infiltration to be defined. These inputs will apply uniformly to all spaces
generated for the building.
This input screen contains inputs divided into five groups and command buttons in the lower right. Each of these input screen features
will be discussed below.
1. Ventilation. Ventilation inputs define the outdoor ventilation airflow requirements for spaces in the building. The Space Usage input
allows ventilation requirements to be defaulted based on space usage types listed in ASHRAE Standard 62.1. The ASHRAE
Standard edition currently in effect for the project is shown in the title for this group of inputs (this is changed via the
View/Preferences option in the HAP main window). Items in the space usage list match those listed in the selected standard. When a
Page 10 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
space usage type is selected, outdoor air requirements 1 and 2 are defaulted. If you choose "user defined" as the space usage type,
then the outdoor air requirements can be directly specified.
2. Occupancy defines the density, hourly schedule and activity level for occupants in the spaces. The drop down list for the schedule
contains a series of standard schedules taken from the ASHRAE Standard 90.1 User's Manual and any schedules previously
defined in the HAP project. If you select one of the standard schedules, the Wizard will add it to the HAP project along with the
spaces it creates.
3. Overhead Lighting defines the fixture type, density and hourly schedule for overhead lighting. As with occupants, the drop-down list
for schedule contains standard schedules from the ASHRAE Standard 90.1 User's Manual and any schedules previously defined in
the HAP project. If necessary, the Wizard will add the schedule you choose to your HAP project along with the spaces it creates.
4. Electrical Equipment defines the power density and hourly schedule for electrical equipment in the spaces. Often these are referred
to as "plug loads". As with occupants and overhead lighting, standard schedules from the ASHRAE Standard 90.1 User's Manual
and schedules previously defined in the HAP project are shown in the drop-down list. When necessary, the schedule you choose will
be added to the HAP project along with the spaces created.
5. Building Envelope defines the wall, roof and window construction assemblies and the infiltration rate for the building envelope.
Inputs in this section are divided into four groups:
a. Wall - Select the wall assembly from the drop down list. This list contains a set of default ASHRAE 90.1 assemblies listed by
climate zone plus any wall assemblies you previously defined in the HAP project. ASHRAE 90.1 assemblies listed will be for the
edition of the standard you selected for the project (see View/Preferences option on main HAP window). When you select a wall
assembly, the overall U-value of the assembly and the sequence of material layers from inside to outside will be listed in the
space below.
b. Roof - Select the roof assembly from the drop down list. This list contains a set of default ASHRAE 90.1 assemblies listed by
climate zone plus any roof assemblies you previously defined in the HAP project. ASHRAE 90.1 assemblies listed will be for the
edition of the standard you selected for the project (see View/Preferences option on main HAP window). When you select a roof
assembly, the overall U-value of the assembly and the sequence of material layers from inside to outside will be listed in the
space below.
c. Window - Select the window type from the drop-down list. This list contains a set of default ASHRAE 90.1 window types listed by
climate zone, default common window types (e.g., single, double, triple pane, clear, reflective and tinted glass types), and any
window assemblies you previously defined in the HAP project. ASHRAE 90.1 window types listed will be for the edition of the
standard you selected for the project (see View/Preferences option on main HAP window). When you select a window type the
overall U-value and shade coefficient are listed in the space below. This window type will be applied to all perimeter spaces and
total window area will be calculated according to the window to wall ratio specified on the Building Wizard footprint input screen.
d, Infiltration - This input defines the infiltration air changes per hour for spaces in the building. Infiltration will only apply to spaces
having a perimeter exposure. The same infiltration value will be applied to cooling design, heating design and energy simulation
conditions.
6. Command Buttons. The following command buttons are provided.
a. Help - Displays this help topic.
b. Previous - Returns you to the Building Footprint input screen.
c. Finish - If running the Building Wizard as part of a Full Wizard Session, the Finish button retains your inputs and returns you to the
Full Wizard Session window. If running Building Wizard alone from the Wizards Menu, the Finish button will display the Building
Wizard input report and then convert Building Wizard inputs into a full set of detailed space data.
d. Cancel - Exits the Building Wizard without saving any changes you made.
Page 11 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
8.4 Equipment Wizard
8.0 Using HAP Wizards ››
Zone Wizard - Zone Configuration Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes use of the Equipment Wizard to rapidly create HVAC system alternatives.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Wizard - Zone Configuration Screen
The Equipment Wizard option on the Wizards menu is used to rapidly apply HVAC equipment to spaces that were previously defined in
HAP. When this option is selected the Zone Configuration input screen appears first. The purpose of this screen is to organize spaces
in your project into floors and zones so the Equipment Wizard can properly apply air systems to the spaces. Spaces are organized by
first creating floors and then using drag-and-drop or menu items to assign spaces on the left side of the screen to floor-zone-space tree
diagram on the right side of the screen.
Quick Tip. For preliminary design or screening studies use the following steps to rapidly configure spaces:
a. Specify the number of floors and whether the typical intermediate floor option is used.
b. In the Unassigned Spaces list highlight all spaces on the first floor and then drag and drop the spaces onto the Floor 1 node in the
tree. All spaces will be automatically converted into single space zones.
c. Repeat the previous step for each floor.
d. Press OK to proceed.
Page 12 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
The Zone Configuration input screen is divided into five key sections, each of which is described below:
1. The Number of Floors panel contains the following inputs:
a. Number of Floors - Allows the number of floors in the building to be defined. One floor node for each floor your create will appear
in the tree diagram panel.
b. Use Typical Intermediate Floor - When 4 or more floors are specified, you have the option of modeling the intermediate floors
with one representative floor. For example, if the building has 10 floors, floors 2 through 9 could be modeled with a single
representative floor if they are sufficiently similar. When this option is chosen, the program applies a multiplier of 8 to the floor so
the actual number of floors, floor area, wall area and window area are accounted for. When this option is not selected, all floors
must be separately modeled.
2. The Unassigned Spaces panel on the left lists all spaces currently defined in your project. Using drag-and-drop you can assign
spaces to zones in the tree diagram on the right, or you can highlight spaces in the list and use an the Assign Spaces option on the
Space Menu to accomplish the same result. Details:
a. If you drag and drop spaces onto a zone node in the tree, the spaces will be assigned to that particular zone.
b. If you drag and drop spaces onto a floor node in the tree, the program will automatically create as series of single-space zones for
that floor. Each space will be assigned to one zone. This is a useful shortcut method for assigning spaces. It saves you the step of
creating zones first allowing you to accomplish creation of zones and assignment of spaces in a single step.
c. All spaces to which you want to apply equipment must be assigned.
d. It is not necessary to assign all spaces in the Unassigned Spaces list. If you are modeling only a portion of the building, or only
using a portion of your spaces, these can be assigned to zones. The other spaces can remain on the Unassigned Spaces list.
3. The Floors/Zones/Spaces Tree Diagram panel on the right shows the relationship between floors, zones and spaces in the
building. In this diagram you can highlight nodes in the tree, expand and collapse the tree display and right-click on nodes to display
pop-up menus. Details:
a. Click the plus sign next to a node to expand the tree. For example, if you click the plus sign for a zone node, the tree expands to
show the spaces assigned to that zone.
b. Click the minus sign next to a node to collapse the tree. For example, if you click the minus sign for a zone, that portion of the tree
will collapse so it no longer shows spaces assigned to the zone.
c. Right-click on a floor node to display a pop-up menu containing options for performing tasks with the floor. The menu contains the
same items as appear on the Floor Menu on the Menu Bar (see below).
Page 13 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Systems and Equipment Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
d. Right-click on a zone node to display a pop-up menu containing options for performing tasks with the zone. The menu contains
same items as appear on the Zone Menu on the Menu Bar (see below).
e. Right-click on a space node to display a pop-up menu containing options for performing tasks with the space. The menu contains
same items as appear on the Space Menu on the Menu Bar (see below).
4. The Menu Bar along the top of the window contains three menus providing options which duplicate drag-and-drop and mouse-click
functionality in the Floor/Zone/Space tree diagram panel.
Floor Menu:
a. Add One Zone - Adds one empty zone to the floor node currently highlighted in the tree diagram.
b. Add Multiple Zones - Adds multiply empty zones to the floor currently highlighted in the tree diagram. When you select this option
you will be prompted for the number of zones to add.
Zone Menu:
a. Delete Zone - Erases the zone highlighted in the tree diagram. If the zone contained spaces, they will be moved back to the
Unassigned Spaces list on the left. Deleting a zone does not destroy any spaces.
b. Rename Zone - Allows you to rename the zone currently highlighted in the tree diagram.
Space Menu:
a. Assign to Zone - The space or spaces highlighted in the Unassigned Spaces list on the left will be assigned to the Zone
highlighted in the tree view diagram.
b. Specify Multiplier - Allows you to define a multiplier for the space currently highlighted in the tree diagram.
c. Remove Space - Removes the highlighted space from the tree diagram on the right and moves it to the Unassigned Spaces list on
the left. Note that removing does not erase the space. It merely moves the space.
5. Command Buttons appear in the lower right:
a. OK - Saves your zone configuration information and proceeds to the first screen of the Equipment Wizard. Later when Equipment
Wizard inputs are converted to detailed HAP data, equipment will be applied to spaces as you have configured them.
b. Cancel - Ends the wizard session without saving any data or generating any detailed HAP data.
c. Help - Displays this help topic.
Preliminary Design Applications. When performing preliminary design or screening studies, you will often have a simple model of the
building where each space represents an entire zone. If so you can quickly configure your spaces into zones and floors with the
following steps:
a. First specify the number of floors and whether the typical intermediate floor option is used.
b. In the Unassigned Spaces list highlight all spaces on the first floor and then drag and drop the spaces onto the Floor 1 node in the
tree. All spaces will be automatically converted into single space zones.
c. Repeat the previous step for each floor.
d. Press OK to proceed.
Detailed Design Applications. When performing detailed design work, you will typically have a detailed model of the building which
may involve varying numbers of spaces per zone.. For this application:
a. First specify the number of floors and whether the typical intermediate floor option is used.
b. For each floor add the required number of zones using the Floor Menu on the Menu Bar or the right-click pop-up menu feature in the
tree diagram.
c. Assign spaces to individual zones, as required using drag-and-drop or options on the Zone Menu.
d. Repeat previous two steps for all floors and zones.
e. Press OK to proceed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Wizard - Systems and Equipment Screen
The Equipment Wizard is used to define one HVAC design alternative for a building. The Equipment Wizard consists of 1, 2 or 3 input
screens depending on the type of equipment being configured. Some of these Wizard input screens offer a Details button that can be
used to display and modify a second level of more detailed inputs. More about HAP Wizards.
The Systems and Equipment Wizard screen contains data for air-side equipment. When configuring DX Equipment it also contains
performance data for the DX equipment.
Page 14 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
The content and format of the Systems and Equipment Wizard screen varies depending on the equipment being configured. The figure
above shows the content when configuring chilled water AHU equipment. The screen is divided into up to 5 sections and also provides
command buttons in the lower right. These input screen features are described below.
1. Description.
a. Name - A reference name for the equipment alternative being defined. When data is later converted to detailed HAP inputs, this
name will be used for the HAP "building" representing the design alternative.
b. Identifier - A short unique label which identifies this design alternative. Examples: BASE or ALT1. This identifier will be used as
the prefix for the name of every system, plant, chiller, cooling tower and boiler generated from the equipment wizard inputs. In this
way you can easily recognize which data items belong together with each design alternative.
c. Notes - The Notes button displays a small window that allows you to enter descriptive information about the design alternative.
This information will only appear on the Equipment Wizard Input Report. It is not saved as part of the detailed HAP inputs.
2. Equipment describes the kind of equipment being configured.
a. Equipment Type - Choose the type of equipment being analyzed.
b. Heating Type - Choose the heat source for the equipment.
c. System Type - Choose the type of air-side system.
d. Configuration - Specify how air-side equipment is arranged in the building - one unit for the entire building, one unit per floor, or
one per zone.
e. Operating Schedule - Choose the operating schedule for the equipment. This will be used to create a fan/thermostat schedule in
the detailed HAP data. The drop-down list includes a series of default schedules taken from the ASHRAE 90.1 User's Manual and
also any fan/thermostat schedules previously defined in the current project. When a new equipment alternative is created, the
schedule will default based on the building type selected in the Building Wizard.
3. Performance defines performance for DX equipment. When multiple DX units will be created, these performance values apply to all
DX units created.
a. AHRI Cooling Rating - Specify the AHRI or ISO/AHRI cooling performance rating in EER or SEER as applicable. In English units
EER is W/BTUh and in Metric it is W/W.
b. AHRI Heating Rating - For heat pump equipment specify the AHRI or ISO/AHRI heating performance rating in COP or HSPF as
applicable.
c. Heating Efficiency - For combustion heating equipment, specify the heating efficiency such as a steady state efficiency, an
annual fuel utilization efficiency (AFUE) or a similar standard rating.
Page 15 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - System and Equipment Details - Central Systems
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
4. Key Features provides options for key control or energy conservation features used with the air-side equipment. The number and
type of these options varies with the type of equipment and system specified. These features include:
a. OA Economizer - Offers several types of outdoor air economizer control.
b. DOAS Type - Offers several types of Dedicated Outdoor Air System (DOAS) units. This option applies to terminal type systems
such as DX fan coils, hydronic fan coils, induction beams, active chilled beams, VRF and water source heat pump systems.
c. DCV Control - Demand Controlled Ventilation control.
d. Ventilation Reclaim - Offers several types of ventilation air heat reclaim devices.
e. Indoor Fan - Offers options for fan type and control.
f. Fan Control - Offers options for 1-speed or 2-speed supply fan control. This option is offered for Constant Volume - Single Zone
systems with equipment type "packaged rooftop", "split DX AHU", "air cooled vertical packaged units", or "water-cooled vertical
packaged units".
g. Capacity Control - Offers options for 1-stage or 2-stage cooling. This option is offered for Constant Volume - Single Zone
systems with equipment type "packaged rooftop", "split DX AHU" or "air cooled vertical packaged units".
h. Dehumidification - "Passive" refers to uncontrolled dehumidification at the cooling coil. "Humidistat" refers to active humidity
control using a humidistat and a reheat coil.
i. Humidifier - Offers several options for humidifier equipment.
j. Cooling Tower Fan - Offers several fan control options. This option only appears for water-cooled vertical packaged equipment.
For other tower applications such as WSHP systems and chilled water plants, cooling tower fan control options are provided on
one of the subsequent wizard screens.
5. Air System Diagram. The air system diagram panel depicts the main components of the air-side system you are configuring. As you
input data the diagram changes to adapt to your inputs. Readers should note that these diagrams are not meant to be an exact
"schematic" diagram of a system. Each diagram is instead meant to show the major components of the system and their position
relative to one another.
6. Command Buttons are provided in the lower right:
a. Details - Displays the Details input screen for system and equipment data. If you are defining central equipment such as rooftops
or chilled water AHUs, the details screen for central systems appears. If you are defining terminal equipment such as fan coils or
WSHPs, the details screen for terminal systems appears.
b. Help - Displays this help topic.
c. Next - If further Wizard input screens are needed to define the equipment, this button will be enabled and can be used to proceed
to the next screen.
d. Finish - If the Systems and Equipment screen is the only screen needed to define the equipment, the Finish button will be
enabled. When using the Full Wizard Session feature, the Finish button retains the inputs and returns you to the Equipment
Alternatives screen. When using the Equipment Wizard option on the Wizards Menu, clicking the Finish button displays the
Equipment Wizard Input Report and then the detailed HAP data is generated, before you are returned to the HAP main window.
e. Cancel - Exits the Equipment Wizard without retaining any inputs or changes, and without generating any detailed HAP data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Wizard - System and Equipment Details - Central Systems
This input screen contains detailed inputs for the air-side system that was configured on the Equipment and Systems Wizard screen. As
inputs are modified on the Equipment and Systems Wizard screen, intelligent defaulting is used to set values shown on this Details
screen. Some users prefer to customize these details and therefore visit this screen to edit the data. Other users prefer to accept the
program defaults and do not visit this screen.
Page 16 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
This Details screen contains data for central types of equipment such as rooftops, vertical packaged units, split DX AHUs and chilled
water AHUs. The format and content of this screen varies depending on the type of equipment and type of air-side system being
defined. The screen is divided into as many as 12 sections and also contains command buttons in the lower right. Each feature of this
input screen is described below.
1. Cooling - Describes the central cooling apparatus.
a. Design SAT - The design supply air temperature for cooling operation.
b. AHRI Clg Rating - For DX equipment, the AHRI rating for cooling equipment in EER or SEER as applicable. In English units EER
is W/BTUh. In Metric units EER is W/W.
c. Minimum Airflow - For VAV systems, the minimum airflow for VAV terminals.
d. Oversizing Factor - For DX equipment, the oversizing factor to be applied to the equipment. For example 15% means the gross
cooling capacity is to be set as peak cooling coil load plus 15%.
e. Capacity Control - Offers options for 1-stage or 2-stage cooling. This option is offered for Constant Volume - Single Zone
systems with equipment type "packaged rooftop", "split DX AHU" or "air cooled vertical packaged units"
2. Heating - Describes the central heating apparatus.
a. Design SAT - The design supply air temperature for heating operation. This only applies to systems providing central heating,
such as a single zone CAV system or a VVT system.
b. AHRI Htg Rating - For DX heat pump equipment, the AHRI rating in COP or HSPF as applicable.
c. Efficiency - For combustion heating equipment, the heating efficiency such as a steady state efficiency or an annual fuel
utilization efficiency (AFUE) or similar value.
d. Oversizing Factor - For DX heat pump and combustion equipment, the oversizing factor to be applied to the equipment. For
example, 25% means the gross heating capacity is to be set as peak heating coil load plus 25%.
3. Preheat Coil - Constant Volume Reheat and VAV systems are assumed to have a preheat coil.
a. Setpoint - The setpoint temperature for the coil. The coil is controlled by a duct thermostat located downstream of the coil.
b. Efficiency - For combustion heating equipment, the heating efficiency such as a steady state efficiency or an annual fuel
utilization efficiency (AFUE) or similar value.
c. Oversizing Factor - For combustion equipment, the oversizing factor to be applied to the equipment. For example, 25% means
the gross heating capacity is to be set as peak heating coil load plus 25%.
4. Supply Fan
a. Type - Allows the fan type and constant speed or variable speed to be defined. Also provides an option to use the part-load fan
curve from ASHRAE Standard 90.1-2004 Appendix G. This has application for LEED EA Credit 1 analysis.
Page 17 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - System and Equipment Details - Terminal Systems
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
b. Supply Fan Performance - The performance of the fan in terms of total static, BHP, motor kW, or Watts per unit flow.
c. Terminal Fan Performance - For fan powered mixing box terminals, the fan performance in terms of total static, BHP, motor kW,
or Watts per unit flow.
d. Fan Control - Offers options for 1-speed or 2-speed supply fan control. This option is offered for Constant Volume - Single Zone
systems with equipment type "packaged rooftop", "split DX AHU", "air cooled vertical packaged units", or "water-cooled vertical
packaged units".
e. Low Speed Fan Flow - When 2-speed supply fan control is selected, this input is used to specify the ratio of airflow at low speed
to airflow at high speed. For example, a value of 67% means the low speed airflow is 67% of the high speed airflow.
5. Thermostats
a. Setpoints - The occupied and unoccupied setpoints for cooling and heating.
b. Operating Schedule - The fan/thermostat schedule for system operation. The drop-down list contains default options from the
ASHRAE 90.1 User's Manual and any fan/thermostat schedules currently defined in the HAP project.
6. Air System Changeover - This section only appears for Chilled Water AHU equipment. It is used to specify whether this is a 2-pipe
changeover system and if so, how changeover is controlled. If a changeover system is being modeled, check this box. Inputs in this
section will then be enabled.
a. Changeover Controlled By - Changeover can be controlled in one of two ways. To select an option click the radio button next to
the desired option.
(i) Schedule - With this option availability of cooling or heating is scheduled by month. Next to this option is a row of buttons, one
for each month. If the button has a "pushed in" appearance, usually indicated by a white background, that means heating is
scheduled for the month. If the button has raised appearance, usually indicated by a gray background, that means cooling is
scheduled for the month. In the figure above heating is scheduled ON for January through May and September through
December. Cooling is scheduled ON for June through August.
(ii) OAT Threshold - With this option, the system switches between cooling and heating based on an outdoor air dry-bulb
temperature (OAT) threshold. When the OAT is above the threshold, cooling is ON. When the OAT is below the threshold
heating is ON. When this option is selected, HAP will automatically assign a changeover deadband of 7 F and a minimum
cycle time of 4 hours. Click here for information about these changeover settings.
7. Outdoor Air Economizer
a. Type - The type of economizer control.
b. Upper Cutoff OADB - The upper cutoff above which economizer operation is locked out.
8. Demand Controlled Ventilation (DCV)
a. Base Ventilation Rate - The minimum outdoor ventilation airflow rate.
b. Min and Max CO2 Differentials - The indoor-outdoor CO2 differentials for DCV control. At the maximum CO2 differential the
ventilation airflow is at its design value. At the minimum CO2 differential the ventilation airflow is at the base ventilation rate.
c. Outdoor Air CO2 Level - Carbon dioxide level for outdoor air at the building site.
9. Ventilation Reclaim
a. Type - The type of ventilation heat reclaim device used.
b. Efficiency - The thermal efficiency of the heat reclaim device.
c. Input Power - Input power required by the device. This could represent the motor for a heat or energy wheel or the pump power
for a pump around system.
10. Humidity Control
a. Dehumidification - "Passive" is uncontrolled dehumidification occurring at the cooling coil. "Humidistat" is active humidity control
using a humidistat and a reheat coil.
b. Max RH Setpoint - The maximum RH setpoint for active (humidistat) control.
c. Humidifier - The type of humidifier used.
d. Min. RH Setpoint - The minimum RH setpoint for controlling the humidifier.
11. Cooling Tower - Cooling tower data only appears here for water-cooled vertical packaged equipment. For WSHP and chilled water
plant equipment, cooling tower inputs are found a different input screen.
a. Design OAWB - The design outdoor air wet-bulb temperature for sizing the cooling tower.
b. Fan Control - The method of controlling the fan when holding the minimum return water setpoint.
c. Fan kW/Ton - The design tower fan input power in kW per ton of heat rejection.
d. Condenser Water Flow - The condenser water flow rate for the tower.
e. Condenser Water Pump - Performance for the condenser water pump defined in terms of head, motor kW or Watts per unit flow.
f. Minimum ECWT - The minimum return water setpoint for the tower. When the tower can produce colder return water it modulates
its operation to hold this setpoint. Modulation is accomplished the method specified in Fan Control above.
12. Command Buttons
a. OK - Saves the changes and returns to the System and Equipment Wizard screen
b. Cancel - Returns to the System and Equipment Wizard screen without saving changes.
c. Help - Displays this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Wizard - System and Equipment Details - Terminal Systems
Page 18 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
This input screen contains detailed inputs for the air-side system that was configured on the Equipment and Systems Wizard screen. As
inputs are modified on the Equipment and Systems Wizard screen, intelligent defaulting is used to set values shown on this Details
screen. Some users prefer to customize these details and therefore visit this screen to edit the data. Other users prefer to accept the
program defaults and do not visit this screen.
This Details screen contains data for terminal types of equipment such as fan coils, water source heat pumps, induction beams or
chilled beams. The format and content of this screen varies depending on the type of equipment being defined. The screen is divided
into as many as 13 sections and also contains command buttons in the lower right. Each feature of this input screen is described below.
1. Cooling - Describes the terminal cooling equipment.
a. Design SAT - The design supply air temperature for cooling operation.
b. AHRI Clg Rating - For DX equipment, the AHRI or ISO/AHRI rating for cooling equipment in EER or SEER as applicable. In
English units EER is W/BTUh. In Metric units EER is W/W..
c. Oversizing Factor - For DX equipment, the oversizing factor to be applied to the equipment. For example 15% means the gross
cooling capacity is to be set as peak cooling coil load plus 15%.
2. Heating - Describes the terminal heating equipment.
a. Design SAT - The design supply air temperature for heating operation.
b. AHRI Htg Rating - For DX heat pump equipment, the AHRI or ISO/AHRI rating in COP or HSPF as applicable..
c. Efficiency - For combustion heating equipment, the heating efficiency such as a steady state efficiency or an annual fuel
utilization efficiency (AFUE) or similar value.
d. Oversizing Factor - For DX heat pump and combustion equipment, the oversizing factor to be applied to the equipment. For
example, 25% means the gross heating capacity is to be set as peak heating coil load plus 25%.
3. Features
a. Supply Fan Performance - The performance of the terminal unit supply fan in terms of total static, BHP, motor kW, or Watts per
unit of flow. This input only applies to terminal equipment containing a fan: DX fan coils, hydronic fan coils, VRF indoor units,
water source heat pumps.
b. Airflow Ratio - The ratio of total supply air to primary air delivered by an induction terminal. This input only applies to Induction
Beam and Active Chilled Beam systems. Example: A particular type of Induction Beam terminal has an airflow ratio of 4.0. For a
given zone, the primary supply air to the terminal is 150 CFM. Therefore the total supply air produced by the terminal will be 150
CFM x 4 = 600 CFM, of which 150 CFM is primary air and 450 CFM is induced room air.
4. Thermostats
a. Setpoints - The occupied and unoccupied setpoints for cooling and heating.
Page 19 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
b. Operating Schedule - The fan/thermostat schedule for system operation. The drop-down list contains default options from the
ASHRAE 90.1 User's Manual and any fan/thermostat schedules currently defined in the HAP project.
5. Changeover - This section only appears for 2-Pipe Fan Coil, Induction Beam and Active Chilled Beam equipment. It is used to
specify whether changeover controls are used and if so, how changeover is controlled. If a changeover system is being modeled,
check this box. Inputs in this section will then be enabled.
a. Changeover Controlled By - Changeover can be controlled in one of two ways. To select an option click the radio button next to
the desired option.
(i) Schedule - With this option availability of cooling or heating is scheduled by month. Next to this option is a row of buttons, one
for each month. If the button has a "pushed in" appearance, usually indicated by a white background, that means heating is
scheduled for the month. If the button has raised appearance, usually indicated by a gray background, that means cooling is
scheduled for the month. In the figure above heating is scheduled ON for January through May and September through
December. Cooling is scheduled ON for June through August.
(ii) OAT Threshold - With this option, the system switches between cooling and heating based on an outdoor air dry-bulb
temperature (OAT) threshold. When the OAT is above the threshold, cooling is ON. When the OAT is below the threshold
heating is ON. When this option is selected, HAP will automatically assign a changeover deadband of 7 F and a minimum
cycle time of 4 hours. Click here for information about these changeover settings.
The remaining sections deal with a Dedicated Outdoor Air System (DOAS) unit.
6. DOAS Unit
a. Type - The type of DOAS unit used to supply treated or untreated outdoor air to the intakes of the fan coil or WSHP units, or to the
primary supply air nozzles in Induction Beam or Active Chilled Beam terminals. A DOAS unit must be used for Induction Beam
and Active Chilled Beam systems. For all other terminal equipment type it is optional. When a DOAS unit is not used, the fan coil
or WSHP introduces outdoor ventilation air directly through a wall opening.
7. Cooling Coil
a. Used - Specify whether the DOAS unit contains a cooling coil.
b. Setpoint - Control setpoint for the coil. The coil is controlled by a duct thermostat downstream of the DOAS unit.
c. AHRI Cooling Rating - For DX equipment the AHRI or ISO/AHRI rating for cooling in EER or SEER as applicable. In English
units EER is W/BTUh. In Metric units EER is W/W.
8. Heating Coil
a. Used - Specify whether the DOAS unit contains a heating coil.
b. Setpoint - Control setpoint for the coil. The coil is controlled by a duct thermostat downstream of the DOAS unit.
c. Heating Type - Source of heating for the coil.
d. Efficiency - For combustion heating equipment, the heating efficiency such as a steady state efficiency or an annual fuel
utilization efficiency (AFUE) or similar value.
e. AHRI Htg Rating - For heat pump equipment, the AHRI or ISO/AHRI rating in COP.
9. Fan Performance
a. Ventilation Fan - The performance for the ventilation fan in terms of total static, BHP, motor kW or Watts per unit of flow.
b. Exhaust Fan - The performance for the exhaust fan in terms of total static, BHP, motor kW or Watts per unit of flow.
c. Unocc Damper Position - Whether outdoor air dampers in the ventilation unit are open or closed during unoccupied
fan/thermostat schedule periods. This input is only offered for Induction Beam and Chilled Beam systems. When outdoor air
dampers are closed during the unoccupied period, 100% of primary air is recirculated. With dampers open, 100% of primary air is
outdoor air.
d. Unocc Airflow - Primary airflow during unoccupied fan/thermostat periods as a percentage design primary airflow. Airflow is
specified in increments of 5% from 50% to 100%. This input is only offered for Induction Beam systems. Applications of these
systems often can use reduced primary airflow during unoccupied times to minimize energy use.
10. Demand Controlled Ventilation (DCV)
a. Base Ventilation Rate - The minimum outdoor ventilation airflow rate.
b. Min and Max CO2 Differentials - The indoor-outdoor CO2 differentials for DCV control. At the maximum CO2 differential the
ventilation airflow is at its design value. At the minimum CO2 differential the ventilation airflow is at the base ventilation rate.
c. Outdoor Air CO2 Level - Carbon dioxide level for outdoor air at the building site.
11. Ventilation Reclaim
a. Type - The type of ventilation heat reclaim device used.
b. Efficiency - The thermal efficiency of the heat reclaim device.
c. Input Power - Input power required by the device. This could represent the motor for a heat or energy wheel or the pump power
for a pump around system.
12. Humidity Control
(These inputs are offered only for Induction Beam and Active Chilled Beam systems)
a. Dehumidification - "Humidistat" means active humidity control is used, with a humidistat located in the DOAS unit discharge to
control discharge humidity, and a dehumidification reheat coil. "Passive" means dehumidification cooling coil is not actively
controlled.
b. Max RH Setpoint - Specify the maximum RH setpoint at the ventilation air handler discharge for active (humidistat) control..
13. Command Buttons
a. OK - Saves the changes and returns to the System and Equipment Wizard screen
b. Cancel - Returns to the System and Equipment Wizard screen without saving changes.
c. Help - Displays this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 20 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Chilled Water Plant Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
Equipment Wizard - Chilled Water Plant Screen
The Chilled Water Plant Wizard screen contains data describing a plant with cooling only chillers or reversible chillers. This screen only
appears when configuring equipment for chilled water AHUs, 2-Pipe or 4-Pipe Fan Coils, Induction Beam or Active Chilled Beam
systems.
The Chilled Water Plant Wizard screen is divided into three sections and also provides command buttons in the lower right. These input
screen features are described below.
1. Plant Configuration
a. Plant Type - Specifies whether the plant is a Chiller Plant, a Changeover Plant or a Heat Recovery Plant.
(i) A Chiller Plant provides cooling only and uses chillers.
(ii) A Changeover Plant provides both cooling and heating and uses reversible chillers. When a Changeover Plant is modeled,
make sure to specify air-side changeover controls. These inputs are found on the System and Equipment Details screen either
for central systems for fan coil systems.
(iii) A Heat Recovery Plant is comprised of of interconnected cooling and heating plants in which heat rejected by the chillers in
the cooling plant is captured and used to meet part or all of the heating loads imposed on the heating plant. When this plant
type is selected inputs on this screen will define the cooling portion of the plant and the type of heat recovery used. The next
input screen will define the equipment in the heating portion of the plant.
b. Number of Units - This defines the number of chillers connected in parallel in the plant, and how the plant capacity is shared
between the chillers. For example "2 Chillers - Equally Sized" means the two chillers each are sized for 50% of the plant capacity.
"2 Chillers - 60%/40%" means the first chiller is sized for 60% of the plant capacity and the second chiller is sized for 40%. Note
that when defining a Heat Recovery Plant that uses the "Dedicated heat recovery chiller in parallel with cooling-only chillers" or the
"Dedicated heat recovery chiller in condenser loop" configurations, Number of Units refers only to the cooling-only chillers. The
dedicated heat recovery chiller is automatically added as an extra chiller in these cases.
c. Equipment Type - The type of chiller or reversible chiller used in the plant. All equipment in the plant will have the same type.
Page 21 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Chilled Water Plant Details Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
d. Input Power - The full load input power for each chiller in the plant. For a Changeover Plant separate input power values are
defined for full load cooling and full load heating duty. For a heat recovery plant using air-cooled chillers with heat recovery
condenser, separate input values are defined for full load cooling in air-cooled mode and full load cooling in water-cooled heat
recovery mode.
2. Key Plant Features provides options for key control and energy conservation features used in the plant. These features include:
a. Distribution System - The type of chilled water distribution system used.
b. Temperature Reset Control - The type of supply water temperature reset control used. Choices include constant supply water
temperature, reset based on an outdoor air temperature schedule and reset based on load (holding a constant return water
temperature). For chiller plants this input applies to chilled water temperature control. For changeover plants this input applies to
both chilled water and hot water supply temperature control.
c. Condenser Pump Control - For a chiller plant using water-cooled chillers, how the condenser water loop is controlled. Choices
include constant flow / constant speed and variable flow / variable speed.
d. Source Water Pump Control - For a changeover plant using water-to-water reversible chillers, how the source water loop is
controlled. Choices include constant flow / constant speed and variable flow / variable speed.
e. Heat Rejector Type - Offers a choice of cooling towers, dry coolers, and geo, well or surface water sources as heat rejection
equipment for water cooled chiller plants. Geo, well or surface water is required for water to water changeover plants.
f. Fan Control - For cooling towers, several options are offered for controlling the tower fans when holding hold minimum return
water setpoint. For dry coolers, fan cycling is used to hold minimum setpoint. This input only applies for water-cooled chiller
plants.
g. Auxiliary Heating - For changeover plants, this item specifies whether auxiliary heating capability is included.
h. Water Side Economizer - The type of water sized economizer used. Non-Integrated means the economizer only operates when it
is able to supply 100% of the plant load. Integrated means the economizer can operate in tandem with mechanical cooling to
provide partial free cooling thus increasing the number of economizer operating hours. Applies for water-cooled chiller plants, air-
cooled chiller plants, and water to water changeover plants.
i. DX Free Cooling - For air-cooled chillers, this item specifies whether non-integrated or integrated DX free cooling is used. With
DX free cooling, when outdoor air temperature is lower than leaving chilled water temperature by a sufficient delta-T, the chiller
compressor can be turned off and a refrigerant pump is used to circulate refrigerant between the evaporator and condenser to
operate the refrigerant cycle and provide cooling. With non-integrated free cooling, the chiller switches from 100% compressor
cooling to 100% free cooling when the free cooling capacity equals or exceeds the chiller load. With integrated free cooling, the
chiller has two independent circuits and can operate with one circuit in compressor cooling and one circuit in free cooling to
provide partial free cooling. When free cooling capacity is sufficient to meet all of the chiller load, both circuits operate in DX free
cooling mode to provide 100% free cooling.
j. Heat Recovery Method - For a heat recovery type of plant select the heat recovery method used in the plant from this list. For an
explanation of each method click here: Heat Recovery Plant Overview.
3. Plant Diagram. The plant diagram depicts the components of the plant you are configuring. As you input data the diagram changes
to adapt to your inputs. Readers should note these diagrams are not meant to be exact "schematic" diagrams of a plant. Due to
space limitations, each diagram is instead meant to only show the major components of the system and their position relative to one
another.
Example: The diagram always shows two chiller icons regardless of how many chillers have been specified. For a water-cooled plant
there is one cooling tower icon, even though the equipment will be configured with one tower per chiller on a common water loop.
When defining a chiller plant there is one diagram panel showing the configuration of components. For a changeover plant there are
two tabbed panels, one for the equipment in cooling mode and one for heating mode. To view each panel, click its tab.
4. Command Buttons
a. Details - Displays the Chilled Water Plant Details input screen.
b. Help - Displays this help topic.
c. Previous - Returns you to the System and Equipment Wizard screen.
d. Next - If hot water or steam heating is used, this button will be enabled and can be used to proceed to the Heating Plant Wizard
screen.
e. Finish - If the Chilled Water Plant Wizard screen is the last screen needed to define the equipment, the Finish button will be
enabled. When using the Full Wizard Session feature, the Finish button retains the inputs and returns you to the Equipment
Alternatives screen. When using the Equipment Wizard option on the Wizards Menu, clicking the Finish button displays the
Equipment Wizard Input Report and then the detailed HAP data is generated, before you are returned to the HAP main window.
f. Cancel - Exits the Equipment Wizard without retaining any inputs or changes, and without generating any detailed HAP data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 22 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Chilled Water Plant Details Screen
This input screen contains detailed inputs for the chiller plant or changeover plant configured on the Chilled Water Plant Wizard screen.
As inputs are modified on the Chiller Plant Wizard screen, intelligent defaulting is used to set values shown on this Details screen.
Some users prefer to customize these details and therefore visit this screen to edit the data. Other users prefer to accept the program
defaults and do not visit this screen.
This screen has different content depending on whether you're configuring a Chiller Plant or a Changeover Plant. Figure 1 at the end of
this topic shows the content for a Chiller Plant. Figure 2 shows the content for a Changeover Plant. Items on the screen are grouped in
up to 7 sections with command buttons in the lower right. Features of this input screen are described below.
1. Plant Configuration - This section applies for both chiller plants and changeover plants.
a. Number of Units - This defines the number of chillers or reversible chillers connected in parallel in the plant, and how the plant
capacity is shared. For example "2 Chillers - Equally Sized" means the two chillers each are sized for 50% of the plant capacity.
"2 Chillers - 60%/40%" means the first chiller is sized for 60% of the plant capacity and the second chiller is sized for 40%.
b. Plant Control - Scheme for controlling chillers in the plant. "Sequenced" means individual chillers are added as load increases
and are turned off as load decreases. Those chillers running at any point in time share the load by running at equal part load
ratios. "Equal Unloading" means all chillers share the load running at equal part load ratios for all load conditions.
c. Full Load ECWT, EWT or OAT - For chillers, this input describes the entering condenser water temperature (ECWT) for water-
cooled chillers or the outdoor air temperature (OAT) for air cooled chillers at the full load rating point. For water source reversible
chillers in changeover plants a pair of inputs describes the ECWT for cooling and the entering water temperature (EWT) for
heating at full load. For air source reversible chillers a pair of inputs describes the cooling OAT and heating OAT for the full load
rating point. For heat recovery plants using air-cooled chillers with heat recovery condensers a pair of inputs describes the full
load OAT for air-cooled mode and the full load ECWT for water-cooled heat recovery mode.
d. Full Load LCHWT or HWST - Full Load LCHWT is the design leaving chilled water temperature (LCHWT) for the plant. For
changeover plants the full load hot water supply temperature (HWST) is also required.
e. Temperature Control - The type of supply water reset control used. Choices include constant supply water temperature, reset
based on an outdoor air temperature schedule and reset based on load (holding a constant return water temperature). For a
changeover plant this control will apply to both cooling and heating duty for the plant.
f. Maximum LCHWT - For chiller plants and changeover plants in cooling mode, the maximum leaving chilled water temperature
(LCHWT) is defined when temperature reset is used.
g. OADB for Min LCHWT, OADB for Max LCHWT - When supply water temperature reset is based on an outdoor air dry-bulb
(OADB) schedule, these two inputs define control points for reset in cooling mode.
(i) The full load LCHWT is used when the OADB is equal to or warmer than the "OADB for Min LCHWT".
(ii) The maximum LCHWT is used when the OADB is equal to or colder than the "OADB for Max LCHWT".
(iii) Between the two OADB values, LCHWT is reset along a linear profile.
h. Minimum HWST - For changeover plants in heating mode, the minimum hot water supply temperature is defined when
temperature reset is used.
i. OADB for Min HWST, Max HWST - When supply water temperature reset is based on an outdoor air dry-bulb (OADB) schedule,
these two inputs define control points for reset in heating mode.
(i) The full load HWST is used when the OADB is equal to or colder than the "OADB for Max HWST".
(ii) The minimum HWST is used when the OADB is equal to or warmer than the "OADB for Min LCHWT".
(iii) Between the two OADB values, HWST is reset along a linear profile.
j. Oversizing Factor - The oversizing factor to be applied to the plant. For example 15% means the plant capacity will be determined
as peak plant load plus 15%. In a changeover plant the same factor is used for determining cooling and heating capacity. For
example a 15% factor means cooling capacity is peak plant cooling load plus 15% and peak plant heating capacity is peak plant
heating load plus 15%.
2. Equipment - This section applies for both chiller plants and changeover plants.
a. Type - The type of chiller or reversible chiller used in the plant. All equipment in the plant will have the same type.
b. Input Power - The full load input power for each chiller in the plant. For a changeover plant separate input power values are
defined for full load cooling and full load heating duty. For heat recovery plants using air-cooled chillers with heat recovery
condensers a pair of inputs describes the input power for air-cooled mode and for water-cooled heat recovery mode.
3. Distribution System - This section applies for both chiller plants and changeover plants.
a. Type - The type of supply water distribution system used.
b. Flow - The design supply water flow rate. For changeover plants the chilled and hot water supply flow rates will be equal.
c. Primary Pump Power - Performance for the primary supply water pumps defined in terms of head, pump kW or Watts per unit of
flow. The units of measure defined here also applies to secondary pumps, if they are used.
d. Secondary Pump Power -Performance for the secondary supply water pumps, if used, defined in terms of head, pump kW or
Watts per unit of flow.
e. Control Head - In a variable flow system, the head that is independent of flow.
f. Minimum Flow - In a variable flow system, the minimum flow allowed for both primary and secondary loops.
4. Cooling Towers - This section applies for chiller plants only.
Page 23 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
a. Heat Rejector Type - Offers a choice of cooling towers and dry coolers as heat rejection equipment.
b. Design OAWB - The design outdoor air wet-bulb temperature for sizing a cooling tower.
c. Design OADB - The design outdoor air dry-bulb temperature for sizing a dry cooler.
d. Fan Control - The method of controlling the fan when holding the minimum return water setpoint.
e. Fan kW/Ton - The design tower fan input power in kW per ton of heat rejection.
f. Average Monthly Source Water Temperatures - The average source water temperature is defined for each month of the year to
represent performance of the geo well field, surface water or well water that serves as a heat sink.
5. Water Source Details - This section applies for water-to-water changeover plants only.
a. Average Monthly Source Temperatures - For a changeover plant using water-to-water reversible chillers, the average source
water temperature is defined for each month of the year to represent performance of the geo well field, surface water or well water
that serves as a heat source/sink.
6. Condenser Water Loop or Source Water Loop - For chiller plants this section describes the condenser water loop and pumps. For
a changeover plant this section describes the source water loop and its pumps.
a. Pump Control - How the water loop is controlled, for water-cooled chillers or water-to-water reversible chillers. Choices include
constant flow / constant speed and variable flow / variable speed.
b. Flow - The water flow rate for the tower, dry cooler, or geo/surfece/well source. This value can be specified as flow (gpm or L/s),
delta-T (F or K) or flow per unit of capacity (gpm/ton or L/s/kW). For a changeover system, the same flow is used for both cooling
and heating mode.
c. Pump - Performance for the water pump defined in terms of head, motor kW or Watts per unit of flow.
d. Minimum ECWT - For chiller plants only, the minimum return water setpoint for the tower or dry cooler. When the tower can
produce colder return water it modulates its operation to hold this setpoint. Modulation is accomplished the method specified in
Fan Control specified earlier in the cooling towers section.
e. Static Head - Describes the portion of the condenser pump head due to the vertical rise in the condenser pumping loop. This
input is only enabled when "Variable Flow / Variable Speed" pump control is specified. In an open loop condenser water loop, the
presence of static head causes the zero flow point on the pump system curve to correspond to static head, rather than passing
through the zero flow, zero head point. This has a significant effect on pump performance when operating at reduced pump flow
and speed. If the condenser loop is a closed loop, specify zero for static head.
Note: For chiller plants and for changeover plants using a geothermal / well / surface water source this input is not applicable and
should be specified as zero.
f. Minimum Flow - Specifies the minimum flow setpoint as a percent of design water flow. This input is only enabled when "Variable
Flow / Variable Speed" pump control is specified. In a chiller plant, the water flow varies to hold the delta-T across the condenser
constant down to minimum flow. As load continues to drop, water flow is held constant and the delta-T decreases with load. In a
changeover plant, the source water flow is controlled in the same manner.
7. Waterside Economizer - This section applies for both chiller plants and changeover plants.
a. Type - The type of water sized economizer used. Non-Integrated means the economizer only operates when it is able to supply
100% of the plant cooling load. Integrated means the economizer can operate in tandem with mechanical cooling to provide
partial free cooling thus increasing the number of economizer operating hours. Applies for water-cooled chiller plants, air-cooled
chiller plants, and water-to-water changeover plants.
b. HX Approach - Defines the performance of the plate frame heat exchanger used in a waterside economizer. The approach is the
difference between the temperature of water in the chilled water loop leaving the heat exchanger minus the cold water from the
heat rejection system entering the heat exchanger.
8. Command Buttons
a. OK - Saves the changes and returns to the Chilled Water Plant Wizard screen
b. Cancel - Returns to the Chilled Water Plant Wizard screen without saving changes.
c. Help - Displays this help topic.
Figure 1. Details Screen Content for a Chiller Plant
Page 24 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Figure 2. Details Screen Content for a Changeover Plant
Page 25 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Heating Plant Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Wizard - Heating Plant Screen
The Heating Plant Wizard screen contains data describing a hot water plant using boilers or air-to-water or water-to-water heat pumps.
It is also used to define steam boiler plants. This screen only appears when configuring equipment that uses hot water or steam
heating.
Page 26 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
The Heating Plant Wizard screen is divided into three sections and also provides command buttons in the lower right. These input
screen features are described below.
1. Heating Plant
a. Equipment Type - Specifies whether the plant uses boilers, water-to-water heat pumps or air-to-water heat pumps.
b. Number of Units - This defines the number of boilers or heat pumps connected in parallel in the plant, and how the plant capacity
is shared between the equipment. For example "2 Boilers - Equally Sized" means the two boilers each are sized for 50% of the
plant capacity. "2 Boilers - 60%/40%" means boiler 1 is sized for 60% of the plant capacity and boiler 2 is sized for 40%.
c. Fuel or Energy Type - The energy or fuel source for the boiler. Only applies when equipment type is "Boilers".
d. Boiler Efficiency - The efficiency for the boilers such as a steady state efficiency or an annual fuel utilization efficiency (AFUE) or
similar value.
e. Full Load Input Power - The full load input power for heat pumps used in the plant.
2. Key Plant Features provides options for key control and energy conservation features used in the plant.
a. HW Distribution System - The type of hot water distribution system used.
b. HWST Reset Control - The type of hot water supply temperature (HWST) reset control used.. Choices include constant HWST,
reset based on an outdoor air temperature schedule and reset based on load (holding a constant return water temperature).
c. Service Hot Water - Specifies whether the plant serves service hot water (SHW) loads in addition to space heating loads in the
building.
d. Auxiliary Heating - For heat pump plants, this specifies whether auxiliary heating capability is included in the plant.
3. Plant Diagram. The plant diagram depicts the components in the hot water or steam plant you are configuring. As you input data the
diagram changes to adapt to your inputs.. Readers should note that these diagrams are not meant to be exact "schematic" diagrams
of a plant. Each diagram is instead meant to show the major components of the system and their position relative to one another.
4. Command Buttons
a. Details - Displays the Heating Plant Details input screen.
b. Help - Displays this help topic.
Page 27 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - Heating Plant Details Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
c. Previous - Returns you to the previous Wizard screen.
d. Finish - When using the Full Wizard Session feature, the Finish button retains the inputs and returns you to the Equipment
Alternatives screen. When using the Equipment Wizard option on the Wizards Menu, clicking the Finish button displays the
Equipment Wizard Input Report and then the detailed HAP data is generated, before you are returned to the HAP main window.
e. Cancel - Exits the Equipment Wizard without retaining any inputs or changes, and without generating any detailed HAP data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Wizard - Heating Plant Details Screen
This input screen contains detailed inputs for the plant configured on the Heating Plant Wizard screen. As inputs are modified on the
Heating Plant Wizard screen, intelligent defaulting is used to set values shown on this Details screen. Some users prefer to customize
these details and therefore visit this screen to edit the data. Other users prefer to accept the program defaults and do not visit this
screen.
This screen has different content depending on whether you're configuring a hot water boiler plant, a heat pump hot water plant or a
steam plant. Figure 1 at the end of this topic shows the content for a hot water boiler plant. Figure 2 shows the content for a heat
pump hot water plant. Figure 3 shows the content for a steam plant. Items on this screen are grouped in up to 6 sections with
command buttons in the lower right. Features of this input screen are described below.
1. Heating Plant - This section applies both for boiler plants and heat pump plants.
a. Number of Units - Defines the number of boilers or heat pumps connected in parallel in the plant, and how the plant capacity is
shared between the equipment. For example "2 Boilers - Equally Sized" means the two boilers each are sized for 50% of the plant
capacity. "2 Boilers - 60%/40%" means boiler 1 is sized for 60% of the plant capacity and boiler 2 is sized for 40%.
b. Plant Control - The scheme for controlling boilers or heat pumps in the plant. "Sequenced" means individual units are added as
load increases and are turned off as load decreases. Those units running at any point in time share the load by running at equal
part load ratios. "Equal Unloading" means all boilers or heat pumps share the load running at equal part load ratios for all load
conditions.
c. Full Load HWST - The design hot water supply temperature (HWST) for the plant. Only applies for hot water plants.
d. HWST Reset Control - The type of hot water supply temperature (HWST) reset control used. Choices include constant HWST,
reset based on an outdoor air temperature schedule and reset based on load (holding a constant return water temperature). Only
applies for hot water plants.
e. Minimum HWST - The minimum hot water supply temperature (HWST) for the plant. Only applies when HWST reset control is
used.
f. OADB for Max HWST, OADB for Min HWST - When HWST reset based on an outdoor air dry-bulb (OADB) schedule is used,
these two inputs define control points for the reset.
(i) The full load HWST is used when the OADB is equal to or colder than the "OADB for Max HWST".
(ii) The minimum HWST is used when the OADB is equal to or warmer than the "OADB for Min HWST"
(iii) Between the two OADB values, HWST is reset along a linear profile.
g. Oversizing Factor - The oversizing factor to be applied to the plant. For example 25% means the plant capacity will be
determined as peak heating plant load plus 25%.
2. Equipment Details - This section applies both for boiler plants and heat pump plants.
a. Fuel or Energy Type - The energy or fuel source for the boiler. This input only applies for boiler plants.
b. Boiler Type - The type of hot water boiler equipment used. Choices are condensing and non-condensing boilers. This input only
applies for boiler plants.
c. Efficiency - The efficiency for the boiler such as a steady state efficiency or an annual fuel utilization efficiency (AFUE) or similar
value. This input only applies for boiler plants.
d. Heat Pump Type - The type of heat pump equipment used. This input only applies for heat pump plants.
e. Full Load Input Power - The input power for a heat pump at its full load rating condition. This input only applies for heat pump
plants.
3. Water Source Details - This section applies only for heat pump plants.
a. Average Source Temperatures - For a hot water plant using water-to-water heat pumps the average source water temperature
is defined for each month of the year to represent performance of the geo well field, surface water or well water that serves as the
heat source.
4. Distribution System - This section applies both for boiler plants and heat pump plants, but not for steam plants.
a. Type - The type of hot water distribution system used.
b. HW Flow - The design hot water flow rate for the system.
Page 28 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
c. Primary HW Pumps - Performance for the primary hot water pumps defined in terms of head, pump kW or Watts per unit of flow.
The units of measure defined here also applies to secondary pumps, if they are used.
d. Secondary HW Pumps -Performance for the secondary chilled water pumps, if used, defined in terms of head, pump kW or
Watts per unit of flow.
e. Control Head - In a variable flow system, the head that is independent of flow.
f. Minimum Flow - In a variable flow system, the minimum flow allowed for both primary and secondary loops.
5. Auxiliary Heating - This section applies only for heat pump plants if auxiliary heating is included in the plant on the main wizard
screen.
a. Heating Source - Specify the source of auxiliary heat.
b. Triggers - COP - Check this box if the plant has controls that will turn off the heat pumps when their operating COP drops below a
threshold and then run 100% auxiliary heat below this threshold. For example if the box is checked and a "COP" value of 2.0 is
specified, the heat pumps will turn off when their operating COP falls below 2.0.
c. Triggers: OAT - Check this box if the plant has controls that will turn off the heat pumps when the outdoor air dry-bulb
temperature (OAT) falls below a specified threshold temperature. For example if the box is checked and an "OAT" value of 15 F
is specified, the heat pumps will turn off when the OAT is colder than 15 F and the auxiliary heater will serve 100% of the plant
load.
d. Allow Simultaneous Auxiliary - Check this box if the auxiliary heater is allowed to operate simultaneously with the heat pumps.
Checking the box models a plant in which the heat pumps serve as first stage heat and when they are unable to meet the plant
load, the auxiliary heaters turn on as second stage heat to meet the remainder of the load. The plant runs in this way until the
COP or OAT trigger is reached, if either of these triggers are specified. Once a trigger is reached the plant switches to 100%
auxiliary.
In other plants either the heat pumps run or the auxiliary heater runs, but not both. To model this type of plant leave the box
unchecked. For this control, once the heat pump capacity is insufficient to meet a plant load, the heat pumps turn off and auxiliary
serves 100% of the plant load. The plant controller will also turn the heat pumps off and use auxiliary heat to meet 100% of the
load if the COP or OAT trigger is reached, if either of these triggers are specified
6. Service Hot Water - This section only applies when the plant serves service hot water (SHW) loads.
a. Determine Consumption from Building Occupancy - Check this box if service hot water (SHW) consumption should be
determined from the number of building occupants and a hot water volume per person per day specification. Leave the box
unchecked if you want to specify hot water consumption as a peak flow rate (gpm or L/s).
b. Max Consumption - Defines the maximum SHW demand. If demand is being determined from building occupancy this input has
units of hot water volume per person per day. If demand is being specified directly, this input has units of peak hot water flow in
gpm or L/s.
c. Usage Schedule - When demand is specified as a peak hot water flow, a usage schedule must be selected to define how the hot
water flow varies hour by hour during the days of the year. This drop down list contains default schedules from the ASHRAE 90.1
User's Manual for different building types, and any fractional schedules you previously defined in this project.
d. Storage - Describes the volume of a hot water storage tank. When modeling a tankless or instantaneous water heating system,
specify the volume as zero. When modeling a stored hot water system, specify the volume of the storage tank.
e. Temperatures - This group of inputs defines the inlet, outlet and control temperatures for the system.
(i) Design - Specify the design SHW supply temperature for the system.
(ii) Minimum - Specify the minimum storage tank temperature at which the heating source is activated to heat the tank to the
design supply temperature. If storage volume is zero (i.e tankless system), this input is not used.
(iii) CWS - Specify the average cold water supply temperature. This is the temperature of water entering the system from the
supply main.
f. Pasteurization - Check this box if a hot water storage tank is used and the system has a Pasteurization cycle. Certain local codes
required this cycle which heats tank water to an elevated temperature periodically as a means of sterilizing the SHW supply, in
particular to kill Legionella bacteria.. When this box is checked the two inputs below it will be enabled. If the SHW system does
not use a Pasteurization cycle, uncheck the box.
(i) Period - Defines the time in days between Pasteurization cycles. For example a Period of 7 days means Pasteurization cycles
occur every 7 days during the simulation.
(ii) Duration - Specifies the duration in hours of each Pasteurization cycle. For example, some codes require Pasteurization to
last for 24 hours. This means the equipment will heat the hot water in the tank to the elevated temperature for 24 consecutive
hours and then return to normal tank operation.
Note: When a Pasteurization cycle is selected, the program defaults to a start time of midnight, a pasteurization temperature of
158 F (70 C), and includes an auto-sized supplemental electric heater.
7. Command Buttons
a. OK - Saves the changes and returns to the Heating Plant Wizard screen
b. Cancel - Returns to the Heating Plant Wizard screen without saving changes.
c. Help - Displays this help topic.
Figure 1. Details Screen for Hot Water Boiler Plant
Page 29 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Figure 2. Details Screen for Heat Pump Hot Water Plant
Page 30 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - WSHP Loop Screen
8.0 Using HAP Wizards ›› 8.4 Equipment Wizard ››
Figure 3. Details Screen Content for Steam Plant
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 31 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Equipment Wizard - WSHP Loop Screen
The WSHP Loop Wizard screen contains data describing a WSHP or GSHP loop and associated equipment and controls. The figure
below shows the appearance of the screen when defining a WSHP Loop type of system.
The content of the WSHP Loop Wizard screen changes depending on type of WSHP system being defined. The screen is divided into
up to 5 sections and also provides command buttons in the lower right. These input screen features are described below.
1. Water Loop
a. Loop Water Flow - Defines the design water flow rate for the WSHP or GSHP loop.
b. Loop Pump - Defines the performance of the WSHP or GSHP loop circulation pumps in terms of head, motor kW or Watts per
unit flow.
c. Maximum and Minimum Loop Setpoints - These inputs only appear for WSHP Loop systems and define the maximum and
minimum setpoints for the loop. When the loop temperature reaches maximum setpoint the cooling tower turns on to reject heat
and hold the maximum setpoint. When the loop temperature reaches minimum setpoint the auxiliary boiler turns on to hold
minimum setpoint.
2. Cooling Tower - These inputs only apply for a WSHP Loop system.
a. Design OAWB - The design outdoor air wet-bulb temperature for sizing the cooling tower.
b. Fan Control - The method of controlling the tower fan to hold the maximum loop setpoint.
c. Fan Power - The design tower fan input power in kW per ton of heat rejection.
3. Auxiliary Boiler - These inputs only apply for a WSHP Loop system.
a. Fuel or Energy Type - The energy or fuel source for the auxiliary boiler.
b. Boiler Efficiency - The efficiency for the boiler such as a steady state efficiency or an annual fuel utilization efficiency (AFUE) or
similar value.
4. Source Water Temperatures - These inputs only apply for a Ground Source Heat Pump (GSHP) system.
a. Monthly Average Source Temperatures - The average source water temperature for the heat pump system. One source
temperature is defined for each month.
5. Heat Pump Loop Diagram. The loop diagram depicts the major components of the WSHP or GSHP loop you are configuring.
Readers should note these diagrams are not meant to be exact "schematic" diagrams of a system. Each diagram is instead meant to
show the major components of the system and their position relative to one another.
Page 32 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
8.5 Utility Rate Wizard
8.0 Using HAP Wizards ››
Utility Rate Wizard - Utility Rate Input Screen
8.0 Using HAP Wizards ›› 8.5 Utility Rate Wizard ››
6. Command Buttons
a. Help - Displays this help topic.
b. Previous - Returns you to the System and Equipment Wizard screen.
c. Finish - When using the Full Wizard Session feature, the Finish button retains the inputs and returns you to the Equipment
Alternatives screen. When using the Equipment Wizard option on the Wizards Menu, clicking the Finish button displays the
Equipment Wizard Input Report and then detailed HAP data is generated, before you are returned to the HAP main window.
d. Cancel - Exits the Equipment Wizard without retaining any inputs or changes, and without generating any detailed HAP data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes use of the Utility Rate Wizard to rapidly model energy price structures.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Utility Rate Wizard - Utility Rate Input Screen
The Utility Rate Wizard is used to quickly configure prices for electric energy and fuels. This Wizard consists of one main screen and
two optional input screens. The optional screens are used only when configuring a detailed electric rate. The main Utility Rate Wizard
input screen, shown below, is divided into three parts. Features of each part are described below the screen image.
1. Electric Rate Panel. The upper part of the screen is used to define prices for electric energy. The Wizard provides two approaches
to defining electric rates. The simple approach involves entering the data shown in this panel:
Page 33 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Utility Rate Wizard - Detailed Electric Rate Setup Screen
8.0 Using HAP Wizards ›› 8.5 Utility Rate Wizard ››
a. Rate Name - Specify a descriptive name for the rate. For projects in the United States you can select from a list of state average
prices compiled by the US Energy Information Administration (EIA). When a state is selected from the drop-down list, the state-
average electric price is defaulted and the EIA price is also defaulted for natural gas.
b. Rate Type - Select "Simple"
c. Energy Charge - Specify the flat price which applies to all electrical energy use.
d. Demand Charge - If a demand charge is modeled, specify a flat price for all demand kW.
e. CO2e Emissions - To calculate CO2 equivalent (CO2e) emission data resulting from electric energy consumption, specify the
CO2e emission rate. The default value is an average for the United States. For further information on CO2e emission factors, see
the discussion at the end of this topic.
The second approach to electric rates is the detailed approach. This approach is used when you want to model the electric rate is
more detail than just specifying flat energy and demand prices. To use this approach, select the Rate Type as "Detailed" and then
click the "View / Edit Detailed Inputs" button. This will display the Detailed Electric Rate Setup screen, which is the first of two
screens allowing a detailed rate definition.
2. Fuel Rate Panel. The lower part of the screen is used to define prices for fuel and remote source steam. This panel contains two
tabs. The Fuel Rates tab is divided into three parts for natural gas, fuel oil and propane prices. Check boxes are used to select
which of these fuels apply to your project. The Remote Steam Rate tab is used to define the price of remote source steam and is
typically only used when a chilled water plant using steam absorption chillers is being modeled in this project. The same set of input
items appears for each fuel and for remote source steam:
a. Rate Name - Specify a descriptive name for the rate. For natural gas applications for projects in the United States you can also
select from a list of state average prices compiled by the US Energy Information Administration (EIA). When a state is selected
from the drop-down list, the state-average natural gas price is defaulted and the EIA price is also defaulted for electricity.
b. Units of Measure - This drop-down list contains common units of measure for the fuel. If you select one of these items in the list,
the conversion factor and CO2e emission inputs will be defaulted. You can also directly enter your own units of measure. In this
case, you must specify the appropriate conversion factor and CO2e emission factor yourself.
c. Conversion Factor - This defines the conversion from standard energy units (kBTU in English or kWh in Metric) to your specified
fuel units of measure. For example, when using Therms of gas, the conversion is 100 kBTU per Therm. The energy simulation
produces equipment energy consumption in standard units which must then be converted to your fuel units of measure before fuel
costs can be calculated.
d. Price - Specify the flat price for the fuel that applies to all fuel or remote steam use.
e. CO2e Emissions - To calculate CO2 equivalent (CO2e) emission data resulting from fuel use, specify the CO2e emission rate.
The default value is an average for the United States. For further information on CO2e emission factors, see the discussion at the
end of this topic.
3. Command Buttons. The lower right corner of the input screen contains command buttons:
a. Help - Displays this help topic.
b. Finish - If running Utility Rate Wizard as part of a Full Wizard Session, the Finish button retains your inputs and returns you to the
Full Wizard Session window. If running Utility Rate Wizard alone from the Wizards Menu, the OK button displays the Utility Rate
Wizard input report and then converts your data into detailed electric rate and fuel rate definitions for use in the HAP detailed
interface.
c. Cancel - Exits the Utility Rate Wizard without retaining any changes you made.
Further Information about CO2e Factors. Many different gaseous emissions from the generation of electricity or burning of fossil
fuels contribute to atmospheric greenhouse warming. The CO2 equivalent (CO2e) emission factor represents the equivalent lb or kg of
CO2 per unit of energy or fuel that has the same greenhouse warming effect as all of the different gaseous emissions combined. This
provides a single point of reference for evaluating the greenhouse warming effect of energy consumption.
Emission data for electrical energy is based on assumptions about the type of power plants used to generate the electricity, and the
efficiency of transmitting energy to the building site. For example, a utility that relies heavily on coal-fired power plants will have higher
CO2e emission rates than one that uses hydroelectric power, nuclear plants or gas-fired power plants.
Emissions data for fuel sources will depend on the type and quality of the fuel.
Emission rate data is often available from government reports. For applications in the United States, one useful source of this data is
Source Energy and Emission Factors for Energy Use in Buildings, Deru and Torcellini, National Renewable Energy Laboratory
Technical Report NREL/TP-550-38617, June 2007. This report is available for download from an NREL web site.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Utility Rate Wizard - Detailed Electric Rate Setup Screen
When using the Detailed option for defining an electric rate, you must work through two input screens. The first screen is the Detailed
Electric Rate Setup screen (shown below). It asks high level questions about the nature of the electric rate, such as whether seasonal
or time of day pricing is used and whether flat or stepped prices are used for energy and demand charges. This information is then
Page 34 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
used to automatically configure the energy and demand charge price tables which appear on the Detailed Electric Rate Prices screen
so that only prices and block sizes (if applicable) need to be defined. This top down approach to rate definition, including the automatic
configuration of price tables, greatly simplifies the process of creating an electric rate.
The Detailed Electric Rate Setup screen is divided into three parts. Features of each part are described below the screen image.
1. Electric Rate Setup. The left side of the screen contains high level questions about the content and organization of the electric rate.
Answers to these questions can typically be determined by reviewing the electric rate sheet you obtained from the utility company.
Inputs in this portion of the screen include.
a. Rate Name - Specify a descriptive name for the rate.
b. Customer Charge - A customer charge is a fixed charge, not related to energy use or peak demand, that is imposed each month.
c. Seasonal Pricing - If your electric rate defines different prices based on time of year, check the Seasonal Pricing box. A table will
then appear on the right side of the screen to allow you to define the months included in the Summer and Winter seasons.
d. Time of Day Pricing - If your electric rate defines different prices based on time of day, check the Time of Day Pricing box. At
table will then appear on the right side of the screen to allow you to define the start times for the peak and off peak pricing periods.
e. Energy Charge Type - Select the type of energy charge in your rate. If a single energy price applies to all energy use all year, or
in a particular season or time of day period, choose the "Flat Prices" option. If instead, multiple price steps for blocks of energy are
defined, choose the appropriate "Stepped Prices" option in the list based on whether the units of measure for the blocks are
"kWh", "kWh/kW" or "Hours Use".
f. Energy Charge Steps - When the energy charge type is one of the stepped types, specify the quantity of steps per period you see
in the rate schedule.
g. Demand Charge Type - First, if a demand charge is not used, choose the "Not Used" option in this drop-down list. If a demand
charge is used, then choose the "Flat Prices" option of flat prices are defined for all demand all year, or in each season or time of
day period. Or choose the "Stepped Prices" option if prices for multiple steps of kW demand are specified in the rate schedule.
h. Demand Charge Steps - When the demand charge type is "Stepped Prices", specify the number of steps per period you see in
the rate schedule.
i. CO2e Emissions - To calculate CO2 equivalent (CO2e) emission data resulting from electric energy consumption, specify the
CO2e emission rate. The default value is an average for the United States. For further information on CO2e emission factors, see
the discussion at the end of this topic.
Page 35 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
Utility Rate Wizard - Detailed Electric Rate Prices Screen
8.0 Using HAP Wizards ›› 8.5 Utility Rate Wizard ››
2. Electric Rate Schedules. The right hand side of the screen is used to define seasonal and time of day schedules. These inputs only
appear if you checked the boxes for Seasonal Pricing and/or Time of Day Pricing on the left side of the screen.
a. Seasonal Pricing- When seasonal pricing is selected, you must specify the start and end months for the Summer billing season.
Note that the start and end months are inclusive. Based on your summer inputs, the program automatically sets the start and end
months for the winter billing season.
b. Time of Day Pricing - When time of day pricing is selected, you must specify the start times for the peak and off peak billing
periods. Start times are specified separately for weekday, Saturday and Sunday/Holiday day types. If a day type does not have a
particular period, select "None". If a billing period applies to all 24 hours in a day, select "All".
3. Command Buttons. The lower right corner of the input screen contains command buttons:
a. Help - Displays this help topic.
b. Next - Proceeds to the Detailed Electric Rate Prices screen.
c. Cancel - Exits this screen without retaining any changes you made and returns to the Utility Rate Input Screen.
Further Information about CO2e Factors. Many different gaseous emissions from the generation of electricity or burning of fossil
fuels contribute to atmospheric greenhouse warming. The CO2 equivalent (CO2e) emission factor represents the equivalent lb or kg of
CO2 per unit of energy or fuel that has the same greenhouse warming effect as all of the different gaseous emissions combined. This
provides a single point of reference for evaluating the greenhouse warming effect of energy consumption.
Emission data for electrical energy is based on assumptions about the type of power plants used to generate the electricity, and the
efficiency of transmitting energy to the building site. For example, a utility that relies heavily on coal-fired power plants will have higher
CO2e emission rates than one that uses hydroelectric power, nuclear plants or gas-fired power plants.
Emissions data for fuel sources will depend on the type and quality of the fuel.
Emission rate data is often available from government reports. For applications in the United States, one useful source of this data is
Source Energy and Emission Factors for Energy Use in Buildings, Deru and Torcellini, National Renewable Energy Laboratory
Technical Report NREL/TP-550-38617, June 2007. This report is available for download from an NREL web site.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Utility Rate Wizard - Detailed Electric Rate Prices Screen
The Detailed Electric Rate Prices screen is used to specify energy and demand prices, as well as a ratchet clause and minimum kW
clause for demand, if applicable. The pricing tables on this screen are automatically configured based on inputs from the Detailed
Electric Rate Setup screen to simplify your work.
The Detailed Electric Rate Prices screen is divided into three parts. Features of each part are described below the screen image.
Page 36 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
1. Electric Energy Charge. The left side of the screen contains the pricing table for the electric energy charge. The number of rows
and the specifications for season and time of day period are automatically defaulted based on your inputs from the Setup input
screen. The only portions of the table you must fill out are the energy prices, and the block sizes (if applicable). Pricing and block
size information is typically listed on electric rate schedules. Note: On some electric rate schedules, prices are subdivided into
multiple components and may need to be summed before entering the total price into the table.
2. Electric Demand Charge. The right side of the screen contains the pricing table for the electric demand charge and demand
determination clauses.
a. Demand Charge Prices - This table appears only if you have a demand charge. The number of rows and the specifications for
season and time of day period are automatically defaulted based on your inputs from the Setup input screen. The only portion of
the table you must fill out are the demand prices and the block sizes (if applicable). Pricing and block size information is typically
listed on electric rate schedules.
b. Ratchet Clause - The demand determination section of your electric rate schedule will identify whether a ratchet clause exists. In
this clause the ratchet demand is the peak measured during one portion of the year, such as the summer. Billing demands each
month are determined as the actual monthly demand or a percentage of the ratchet demand, whichever is higher. To define a
ratchet clause, first check the box. Then specify opposite "Peak Months" the start and end of the period over which the ratchet
demand is measured. If the entire year is used, specify January to December. Next, specify the start and end of the period in
which the ratchet penalty applies. If the entire year is used, specify January to December. Finally, specify the ratchet multiplier.
Example: The Ratchet Demand is measured in the summer months June through September. Then for all months of the year the
billing demand is either the actual demand measured or 85% of the Ratchet Demand whichever is higher. The screen image
above shows the inputs for this scenario.
c. Minimum Demand - The demand determination section of your electric rate schedule will also identify whether a minimum
demand clause is used. In this clause, a minimum demand kW is set. The billing demand each month is then the actual measured
demand or the minimum demand, whichever is larger.
3. Command Buttons. The lower right corner of the input screen contains command buttons:
a. Help - Displays this help topic.
b. Previous - Returns to the Detailed Electric Rate Setup screen.
c. Finish - Retains the detailed electric rate inputs and returns to the Utility Rate Input screen.
Page 37 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm
d. Cancel - Exits this screen without retaining any changes and returns to the Utility Rate Input screen.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 38 of 38
8.0 Using HAP Wizards
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh4C4C.htm