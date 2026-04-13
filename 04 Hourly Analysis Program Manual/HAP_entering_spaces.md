10.0 Entering Spaces
10.1 Overview for Spaces and the Space Form
10.0 Entering Spaces ››
Overview for Spaces and the Space Form
10.0 Entering Spaces ›› 10.1 Overview for Spaces and the Space Form ››
This chapter explains input data for spaces.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of how space input data is organized.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Spaces and the Space Form
About Spaces. A building is divided into units referred to as "spaces" when analyzing its thermal behavior. In
its simplest sense a space represents a single room. A space consists of a number of "elements" such as
walls, roofs, windows, and internal heat gains which influence heat transfer into and out of the space. In
addition, a space is served by one or more air distribution terminals.
The definition of a space is actually flexible. A space does not always have to represent a single room. In
some applications it is more appropriate for a space to represent a group of rooms, a floor or even an entire
building.
All spaces for the portion of the building being analyzed must be defined so system design calculations or
energy simulations can be performed. Later, when air system data is entered you will link spaces to zones
served by the air system. When system design calculations or energy simulations are performed for an air
system, data for all spaces linked to the air system will be used in these calculations.
Page 1 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
The Space Form, shown above, is used to define the characteristics of all heat flow elements in a space. The
Space Form contains three key components:
1. The Title Bar appears across the top of the form. It lists the name of the space whose data is displayed in
the form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains multiple categories of information for the space
represented as separate tabs in a notebook. There are seven tabs for the seven categories of space data.
To move from one tab to another, simply click on the desired tab name. The seven tabs are as follows:
a. General contains the space name, total floor area, average floor to ceiling height and the building weight.
b. Internals contains information about internal heat gains from overhead lighting, task lighting, electrical
equipment, occupants, and miscellaneous sources.
c. Walls, Windows, Doors contains data for vertical wall exposures and the windows, external shading
devices and doors which are part of these exposures.
d. Roofs, Skylights contains information about horizontal or sloped roofs any skylights which are part of
these roof exposures.
e. Infiltration contains infiltration specifications for cooling design, heating design and energy simulation
conditions.
f. Floors contains information about heat transfer through slab floors, basement floors or floors above an
unconditioned region.
g. Partitions contains data about heat flow through walls or ceilings adjacent to unconditioned regions.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the space inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the space. If you press
Cancel while creating a new space, a new space will not be added to your project.
c. Press Help to display this overview topic.
Space Features. Finally, HAP provides useful features for:
Creating new spaces .
Page 2 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.2 General Space Data
10.0 Entering Spaces ››
General Tab / Space Form
10.0 Entering Spaces ›› 10.2 General Space Data ››
Editing an existing space .
Printing space data
Deleting spaces.
Copying a space .
Duplicating a space .
Searching and replacing space data .
Rotating spaces.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the General tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
General Tab / Space Form
The General tab on the space form is used to define several key values which describe the space as a whole
and the ventilation requirements for the space:
Space name
Total floor area
Average floor-to-ceiling height
Building weight
Outdoor Air Ventilation Requirments
Page 3 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Space Name
10.0 Entering Spaces ›› 10.2 General Space Data ››
Space Floor Area
10.0 Entering Spaces ›› 10.2 General Space Data ››
Average Ceiling Height
10.0 Entering Spaces ›› 10.2 General Space Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Name
The Space Name is a reference name used to identify the space. It appears on reports and on selection lists
when linking spaces to an air system. The name should be descriptive so you can recognize what it represents
when it appears later on selection lists.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Floor Area
Enter the total floor area for the space. Floor area is used to compute internal heat gains from such sources as
lighting and occupants, when these heat gains are defined on a per sqft or per sqm basis. Floor area is also
used in conjunction with the average ceiling height to calculate infiltration air changes per hour.
Note that a separate input is provided for specifying the area of slab or basement floors. In applications in
which a space represents an area larger than a single room, it is possible only a portion of the space floor area
has ground contact. In these cases the slab floor area is different from the total space floor area.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 4 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Building Weight
10.0 Entering Spaces ›› 10.2 General Space Data ››
Outdoor Air Ventilation Requirements
10.0 Entering Spaces ›› 10.2 General Space Data ››
Average Ceiling Height
Average ceiling height defines the average floor-to-ceiling height for the space. It is used in conjunction with
the total space floor area to compute the space air volume, which in turn is used when calculating infiltration
air changes per hour.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Building Weight
Building weight defines the overall weight of the interior walls, floors, ceilings and contents of the building. This
value plays a key role in influencing how heat gains are converted into loads. In general terms, heavy
buildings tend to absorb and store heat for longer periods than light buildings. As a result, there is more of a
lag between the time a heat gain occurs and the time it becomes an air-conditioning load.
Building weight can be entered directly as a weight per unit of floor area. Or, you may use the slider control to
the right of the building weight input to specify the weight as Light (30 lb/sqft or 146.5 kg/sqm), Medium (70
lb/sqft or 341.8 kg/sqm), or Heavy (130 lb/sqft or 634.7 kg/sqm) or any value in between these standard
weights.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Outdoor Air Ventilation Requirements
The OA Ventilation Requirements frame contains three inputs which together define the outdoor ventilation
requirements for the space:
1. Space Usage. In this drop-down list choose "User-Defined" to enter your own ventilation requirements, or
choose one of the space usage options to default the requirements. Space usage options are taken from
ASHRAE Standard 62-2001, or ASHRAE Standard 62.1 2004, 2007, 2010, 2013, or 2016 according to your
prior specification in the View/Preferences option. A note below the ventilation inputs indicates which source
of defaults is used.
When complying with Standard 62-2001 or with one of the Standard 62.1 editions, you can select one of the
space usage types in the drop-down list and the corresponding ventilation requirements will be defaulted
automatically. In this situation the ventilation requirements cannot be changed directly. They can only be
changed by selecting a different space usage type.
The list of space usage types is arranged alphabetically by category and then space usage type. Example:
"EDUCATION: Classroom (9+)". To move quickly to a desired category type the first letter in the category.
For example, typing "E" moves you to the first entry for "EDUCATION" category of space usage types.
Page 5 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.3 Internal Loads
10.0 Entering Spaces ››
Internals Tab / Space Form
10.0 Entering Spaces ›› 10.3 Internal Loads ››
If you are instead complying with a different ventilation standard or code or entering your own values,
choose the "User-Defined" usage type. When this option is selected, you will be permitted to directly enter
the ventilation requirements and units of measure.
2. OA Requirement 1 and 2. One or two outdoor air requirements can be defined for the space. For each you
define a value and the units of measure. Example: 20 CFM/person. Units of measure options in English are
CFM, CFM/sqft, CFM/person and % of supply air. In SI Metric the options are L/s, L/s/sqm, L/s/person and
% of supply air.
If the ventilation standard or code you are using only defines one outdoor requirement, specify it and leave
the second outdoor air requirement value as zero.
When values are specified for both outdoor air requirements they will be additive. Some standards or codes
define two requirements per occupied space. One is typically on a per person basis to address CO2 and
people-generated pollutants or odors. The second is typically on a per floor area basis to address pollutants
generated by materials in the space such as carpeting and furnishings. During sizing calculations the
program will sum the two ventilation requirements to obtain the total requirement for the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This tab describes input data on the Internal Loads tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Internals Tab / Space Form
The Internals tab on the Space Form contains information about internal sources of heat gain for the space. As
shown in the figure below, data is divided into five groups, each dealing with a different type of internal heat
gain. The five categories and the input items in each are described below.
Page 6 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
1. Overhead Lighting items describe the characteristics of overhead lighting fixtures. Because lighting fixtures
produce both convective and radiative heat gains, the total fixture wattage as well as the type of the fixture
must be known in order to calculate lighting loads. The lighting schedule is used to describe how lighting
use varies on an hourly and daily basis.
Fixture Type
Wattage
Ballast Multiplier
Schedule
2. Task Lighting items permit a second type of lighting fixture in the space to be modeled. Task lighting is
assumed to consist of free-hanging fixtures or fixtures mounted on walls or furniture. Wattage defines the
fixture peak power use, while the schedule describes how lighting use varies on an hourly and a daily basis.
Wattage
Schedule
3. Electrical Equipment items permit heat gain from electrical appliances or equipment in the space to be
modeled. Common types of equipment modeled in this way include copy machines, desktop computers,
computer printers, cash registers, kitchen equipment, and factory machinery. Wattage defines the maximum
equipment power use while the schedule describes how this power use varies on an hourly and a daily
basis.
Wattage
Schedule
4. People items permit sensible and latent heat gain from occupants of the space to be modeled. The number
of occupants or the occupant density together with the per-person sensible and latent heat gains define the
total occupant heat gain for the space. To simplify the process of determining occupant heat gains,
Page 7 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Overhead Lighting Fixture Type
10.0 Entering Spaces ›› 10.3 Internal Loads ››
standard values for seven common activity levels are provided, or users may enter their own values. The
people schedule defines how the quantity of the occupants in the space varies on an hourly and a daily
basis.
Occupancy
Activity Level
Sensible and Latent Heat Gains
Schedule
5. Miscellaneous Load items describe sensible and latent heat gains from miscellaneous, non-electrical
sources in the space. Examples include gas ovens or steam cookers in kitchens, or refrigeration cases in
supermarkets. Sensible and latent heat gains are described separately. For each, the maximum heat gain is
defined along with a schedule describing the hourly and daily variation of these heat gains.
Miscellaneous Sensible Heat Gain
Miscellaneous Sensible Schedule
Miscellaneous Latent Heat Gain
Miscellaneous Latent Schedule
Special Features. This form provides three important productivity-enhancing features for entering internal
load data:
1. Optional Heat Gain Units. Lighting and equipment wattages can be entered as a total quantity (Watts) or
as a quantity per unit floor area (W/sqft or W/sqm). Occupancy can be defined as a total number of people,
or sqft/person (sqm/person). Use the drop-down list to the right of these heat gain inputs to change to the
desired units of measure.
2. Schedule Creation. Normally, users specify the heat gain schedule by choosing a schedule from the drop
down list provided for each heat gain category. This lists contains the names of all schedules previously
entered and stored in the current project. However, the list also contains a "create new schedule" item
which can be used to create new schedules "on the fly". When this item is selected, the Schedule Form
appears. After you enter schedule data and press OK, the schedule data will be stored, and the schedule
will be assigned to the current heat gain category automatically.
3. Schedule Editing. After a schedule has been selected for a heat gain category, its data can be edited by
pressing the Schedule button, immediately to the left of the schedule drop down list. When you press this
button, the Schedule Form will appear and will display data for the currently selected schedule. You can
modify the schedule’s data and then return to the space form by pressing the OK button on the schedule
form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overhead Lighting Fixture Type
This item defines the type of overhead lighting fixture used in the space. Three choices are offered: recessed
unvented, recessed vented and free hanging.
Lighting fixtures produce both convective and radiative heat gain. The type of lighting fixture used influences
the relative sizes of the convective and radiative components and the way in which radiative heat gains are
distributed. For example, recessed fixtures only radiate to the walls and floor in a space. A free-hanging fixture
radiates to the ceiling as well as the walls and floor. Further, a vented fixture tends to have a higher proportion
of convective heat gain than an unvented fixture.
Please refer to lighting load calculations for further information on this subject.
Page 8 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Overhead Lighting Wattage
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Overhead Lighting Ballast Multiplier
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Overhead Lighting Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overhead Lighting Wattage
This item defines the lamp wattage for the overhead lighting fixture. This is the total of bulb wattages when all
lights in the space are on. Fixture power can be entered in W/sqft (W/sqm) or in total watts. To switch between
these units, use the drop-down list to the right of the lighting input.
Note that when fluorescent lighting fixtures are used, the lamp wattage is increased by the ballast multiplier to
account for power consumption by the ballast starter device. When incandescent lighting fixtures are used the
total wattage is equal to the lamp wattage.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overhead Lighting Ballast Multiplier
For fluorescent lights, power is used to drive both the bulb and a ballast starter device. The program computes
the total power draw for the lighting fixture by multiplying lamp wattage by the ballast multiplier. Ballast
multipliers values from 0.1 to 2.00 are permitted.
Note that when incandescent lighting fixtures are used, the ballast multiplier should be specified as 1.00.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overhead Lighting Schedule
The overhead lighting schedule defines how lighting use varies on an hourly and a daily basis. The lighting
schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a lighting schedule, choose the "create new
schedule" item in the schedule drop-down list. The Schedule Form will appear and will allow you to define
profiles for the hourly and daily variation of lighting use. Be sure to specify that the type of schedule is
"fractional". This type of schedule contains values defining the percentage of maximum heat gain present
for each hour. When you press the OK button to exit from the Schedule Form, your schedule data will be
stored and the schedule will be assigned to overhead lighting for the current space automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Task Lighting Wattage
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Task Lighting Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Electrical Equipment Wattage
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Task Lighting Wattage
The second type of lighting considered in the space is task lighting. Task lighting is assumed to consist of free-
hanging fixtures or fixtures mounted on walls or furniture. Either the W/sqft (W/sqm) or total watts for task
lighting can be defined. To switch between these units, use the drop-down list to the right of the wattage input.
For incandescent lighting, enter the total bulb wattage. For fluorescent lighting, enter the total wattage
including power used by ballast starter devices. The specified lighting wattage will exist when all task lights in
the space are on. A schedule will be defined separately to specify the hourly and daily variation of lighting use.
If task lighting is not used, specify a zero wattage.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Task Lighting Schedule
The task lighting schedule defines how lighting use varies on an hourly and a daily basis. The lighting
schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a lighting schedule, choose the "create new
schedule" item in the schedule drop-down list. The Schedule Form will appear and will allow you to define
profiles for the hourly and daily variation of lighting use. Be sure to specify that the type of schedule is
"fractional". This type of schedule contains values defining the percentage of maximum heat gain present
for each hour. When you press the OK button to exit from the Schedule Form, your schedule data will be
stored and the schedule will be assigned to task lighting for the current space automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Electrical Equipment Wattage
This item is used to model heat gain from electrical appliances or equipment in the space. Common types of
equipment modeled in this way include copy machines, desktop computers, computer printers, cash registers,
kitchen equipment, and factory machinery.
The electrical equipment wattage defines the input power for electrical equipment in the space in either W/sqft
(W/sqm) or in total watts. To switch between these units, use the drop-down list to the right of the wattage
input.
The total wattage entered represents the input power when all electrical equipment in the space is fully
operating. A schedule will be specified separately to define the hourly and daily variation in equipment heat
gains.
Page 10 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Electrical Equipment Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Occupancy
10.0 Entering Spaces ›› 10.3 Internal Loads ››
People Activity Level
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Electrical Equipment Schedule
The electrical equipment schedule defines how equipment heat gain varies on an hourly and a daily basis. The
equipment schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created an equipment schedule, choose the "create new
schedule" item in the schedule drop-down list. The Schedule Form will appear and will allow you to define
profiles for the hourly and daily variation of equipment heat gain. Be sure to specify that the type of
schedule is "fractional". This type of schedule contains values defining the percentage of maximum heat
gain present for each hour. When you press the OK button to exit from the Schedule Form, your schedule
data will be stored and the schedule will be assigned to electrical equipment for the current space
automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Occupancy
This item defines the maximum quantity of people present in the space. Occupancy can be entered either in
terms of sqft/person (sqm/person) or total people. To switch between these units use the drop-down list to the
left of the occupancy input.
The total occupant heat gains for a space are determined by multiplying the number of occupants by the per-
person sensible and latent heat gain values. Hourly and daily variations in occupancy are defined via a
schedule, specified separately.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
People Activity Level
Heat gain from people varies depending on the activity being performed in the space. The program offers the
seven standard activity levels listed in the table below plus a "user-defined" option. Choose the desired activity
level from the drop-down list.
When one of the standard activity levels is chosen, the corresponding sensible and latent heat gains shown in
the table below are used automatically. In order to directly specify sensible and latent heat gains for people,
choose the "User-Defined" activity level option.
Page 11 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
People Sensible and Latent Heat Gain
10.0 Entering Spaces ›› 10.3 Internal Loads ››
People Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Miscellaneous Sensible Heat Gains
Activity Level
Sensible
Heat Gain
(BTU/h
person)
Latent
Heat Gain
(BTU/h
person)
Sensible
Heat Gain
(W person)
Latent
Heat Gain
(W/person)
Seated At Rest
230
120
67.4
35.2
Office Work
245
205
71.8
60.1
Sedentary
Work
280
270
82.1
79.1
Medium Work
295
455
86.5
133.4
Heavy Work
525
925
153.9
271.1
Dancing
305
545
89.4
159.7
Athletics
710
1090
208.1
319.4
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
People Sensible and Latent Heat Gain
People sensible and latent heat gains can be entered directly when using the "user-defined" activity level. The
sensible and latent gains specified will be used to determine the maximum occupant heat gain for the space.
The hourly and daily variations of these heat gains is determined using the people schedule
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
People Schedule
The people schedule defines how occupancy varies on an hourly and a daily basis. The people schedule can
be defined in two ways:
1. Creating a New Schedule. If you have not yet created a people schedule, choose the "create new
schedule" item in the schedule drop-down list. The Schedule Form will appear and will allow you to define
profiles for the hourly and daily variation of occupancy. Be sure to specify that the type of schedule is
"fractional". This type of schedule contains values defining the percentage of maximum occupants present
for each hour. When you press the OK button to exit from the Schedule Form, your schedule data will be
stored and the schedule will be assigned to occupants for the current space automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 12 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Miscellaneous Sensible Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Miscellaneous Latent Heat Gain
10.0 Entering Spaces ›› 10.3 Internal Loads ››
Miscellaneous Sensible Heat Gains
This item can be used to model sensible heat gain or loss from non-electrical heat sources in the space.
Examples include gas ovens or steam cookers in kitchens, and refrigeration cases in supermarkets. The value
you enter represents the maximum sensible heat gain expected. Positive values represent heat gains while
negative values indicate heat loss. A schedule will be specified separately to define the hourly and daily
variations of this heat gain.
Note that this input only results in heat gain or loss being evaluated during load calculations. If the heat source
involves the consumption of fuel, such as natural gas for a cooking oven, and you are performing an energy
analysis with HAP, fuel consumption for this heat source should be specified in the Building portion of the
energy analysis so it can be included in operating cost calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Miscellaneous Sensible Schedule
This schedule defines how miscellaneous sensible heat gains vary on an hourly and a daily basis. The
schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a schedule, choose the "create new schedule" item
in the schedule drop-down list. The Schedule Form will appear and will allow you to define profiles for the
hourly and daily variation of sensible heat gains. Be sure to specify that the type of schedule is "fractional".
This type of schedule contains values defining the percentage of maximum heat gain present for each hour.
When you press the OK button to exit from the Schedule Form, your schedule data will be stored and the
schedule will be assigned to miscellaneous sensible heat gains for the current space automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Miscellaneous Latent Heat Gain
This item can be used to model latent heat gain or loss from non-electrical heat sources in the space.
Examples include steam cookers in kitchens and refrigeration cases in supermarkets. The value you enter
represents the maximum latent heat gain or loss expected. Positive values represent latent heat gains while
negative values indicate latent heat loss. A schedule will be specified separately to define the hourly and daily
variations of this heat gain.
Note that this input only results in heat gain or loss being evaluated during load calculations. If the heat source
involves the consumption of fuel or energy, such as steam for a kitchen appliance, and you are performing an
energy analysis with HAP, fuel consumption for this heat source should be specified in the Building portion of
the energy analysis so it can be included in operating cost calculations.
Page 13 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Miscellaneous Latent Schedule
10.0 Entering Spaces ›› 10.3 Internal Loads ››
10.4 Walls, Windows and Doors
10.0 Entering Spaces ››
Walls, Windows, Doors Tab / Space Form
10.0 Entering Spaces ›› 10.4 Walls, Windows and Doors ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Miscellaneous Latent Schedule
This schedule defines how miscellaneous latent heat gains vary on an hourly and a daily basis. The schedule
can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a schedule, choose the "create new schedule" item
in the schedule drop-down list. The Schedule Form will appear and will allow you to define profiles for the
hourly and daily variation of latent heat gains. Be sure to specify that the type of schedule is "fractional".
This type of schedule contains values defining the percentage of maximum heat gain present for each hour.
When you press the OK button to exit from the Schedule Form, your schedule data will be stored and the
schedule will be assigned to miscellaneous latent heat gains for the current space automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database,
you can simply select the desired schedule from the drop-down list.
In addition, you can modify schedule data directly from the Space Form by pressing the Schedule button to the
left of the drop-down list. When you press this button, the Schedule Form will appear and will display inputs for
the currently selected schedule. After modifying the schedule data, press the OK button to return to the Space
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Walls, Windows and Doors tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Walls, Windows, Doors Tab / Space Form
About Walls, Windows & Doors. The Walls, Windows, Doors tab on the Space Form contains information
about vertical wall exposures and the windows, external shading devices and doors contained in these
exposures. This data is used to calculate the following envelope loads for a space: wall transmission, window
transmission, window solar, door transmission and door solar loads.
Page 14 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
The Walls, Windows, Doors Tab is divided into two panels which occupy the left-hand and right-hand halves
of the tab:
• Wall Exposure Table. The left-hand panel contains a table of wall exposure data. Each row in this
table contains data for one wall exposure. Columns contain different attributes of the exposure. Up to 8
exposures can be defined for each space. The figure above shows a space with three wall exposures:
West, South and East.
• Construction Types. The right-hand panel contains construction information for the current exposure:
wall type, window types, external shade types and door type. Constructions are chosen from drop-down
lists that contain walls, windows, shades, and doors you previously created and stored in your project
database. Features are also provided for creating new constructions or editing existing constructions
without leaving the space form.
As you move from one row to the next in the wall table in the left panel, the information displayed in the
right-hand panel changes to show constructions selected for that exposure. In the figure above, the current
exposure in the left-hand panel is exposure #1. The current exposure is indicated by which row number at
the left end of the row is highlighted. Therefore, construction types for exposure #1 are shown in the right-
hand panel. The current exposure is also listed at the top of the right-hand panel.
Further information about input items in each panel is provided below.1.
Wall Exposure Table / Left-Hand Panel
1. Wall Exposure defines the direction the exterior surface of the wall faces. Any of 16 principal orientations
can be chosen from the drop-down list in this column. To add a wall exposure, change its orientation from
"not used" to one of the 16 principal orientations. When you do this, data items for the exposure will be
enabled. To delete a wall exposure, change its orientation to "not used". When you do this, data items for
the exposure will be disabled.
Page 15 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
2. Wall Gross Area refers to the total surface area of this exposure including wall surface, window apertures
and doors. Later, during load calculations, the program will calculate the net wall area by subtracting the
window and door areas from the gross exposure area.
3. Window 1 Quantity is used to specify the quantity of windows of a particular construction on this exposure.
For example, if the window 1 type specified in the right-hand panel of this tab is a 4ft by 6ft double-glazed
window unit, the window quantity defines the number of these 4x6 window units used in the exposure. The
window quantity can be entered directly, or you can use the spin buttons to increment or decrement the
window quantity.
In some applications, users define the window construction as a unit area section of glass (1 ft by 1 ft or 1 m
by 1 m) so the window quantity defines the total glass area. This is typically done only in preliminary block
load estimates in which detailed window modeling is not necessary, or when an exposure contains a large
number of windows having widely varying dimensions.
Finally, if the wall exposure does not contain windows, specify a quantity of zero.
4. Window 2 Quantity is used to specify the quantity of a second type of window construction used on the
exposure. In some applications different types of windows or windows having different dimensions are used
on the same exposure for a space. HAP permits up to two different window constructions to be specified for
each exposure in a space. The quantity specified here defines the number of window units for the Window 2
construction specified in the right-hand panel of this tab.
If an exposure contains more than two window types, a special technique is required to enter the exposure
data. One approach is to split the gross wall area into two or more sections, defining each section as a
separate wall exposure. Two window types can be assigned to each section of the wall defined in this
manner. Another approach is used when the glazing for all windows is the same, but the window
dimensions vary widely. This approach involves defining the window construction using a unit area
approach. Instead of defining the actual window dimensions, dimensions of 1 ft by 1 ft or 1 m by 1 m (or
some alternate unit size) are used. Then the window quantity is used as a multiplier for this unit area to
account for the total glass area on the exposure.
Finally, if a second window type is not needed for the exposure, specify a Window 2 Quantity of zero.
5. Door Quantity defines the quantity of doors on the exposure. The door construction used for the exposure
is specified separately in the right-hand panel of this tab.
Example: A foyer space in an office building contains a bank of 8 rail and stile entry doors. The door
construction defines the characteristics of one of these doors. A door quantity of 8 would be specified so the
total door area and door heat transmission will be accounted for in the space.
If the exposure does not contain any doors, specify a quantity of zero.
Constructions / Right-Hand Panel
The right-hand panel of the Walls, Windows, Doors tab contains input items for six constructions associated
with the current exposure. Only those constructions used for the current exposure need to be defined. Unused
constructions can be specified as "none". The six constructions defined in this panel are:
1. Wall: The wall assembly used for this exposure. A wall type must be defined for each exposure used by the
space.
2. Window 1: The window construction used for window type #1. Only required if a Window 1 Quantity has
been specified.
3. Shade 1: The external shade geometry used for window type #1. Only required if a Window 1 Quantity has
been specified, and Window 1 uses external shading. If external shading is not used, specify "none".
4. Window 2: The window construction for window type #2. Only required if a Window 2 Quantity has been
specified.
5. Shade 2: The external shade geometry used for window type #2. Only required if a Window 2 Quantity has
been specified and Window 2 uses external shading. If external shading is not used, specify "none".
6. Door: The door construction used for this exposure. Only required if a Door Quantity has been specified.
Each of these constructions can be defined in two ways. The discussion below uses the wall construction as
an example, but the same procedures can be used for windows, external shades and doors.
Page 16 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.5 Roofs and Skylights
10.0 Entering Spaces ››
Roof, Skylights Tab / Space Form
10.0 Entering Spaces ›› 10.5 Roofs and Skylights ››
1. Creating a New Wall Construction. If you have not yet created a wall construction, choose the "create
new wall" item in the wall drop-down list. The Wall Construction Form will appear and will allow you to
define the properties of material layers comprising the wall. When you press the OK button to exit from the
Wall Construction Form, your wall data will be stored and the wall will be assigned to the current wall
exposure automatically.
2. Selecting an Existing Wall Construction. If you previously created and stored walls in your project
database, you can simply select the desired wall from the drop-down list.
In addition, you can modify wall, window, shade or door construction data directly from the Space Form by
pressing the button to the left of the construction drop-down list. When you press this button, the input form for
the appropriate construction type will appear and will display inputs for the currently selected construction.
After modifying the data, press the OK button to return to the Space Form.
Application Information
For many applications, the same set of constructions is used for all exposures in a space. In such a case, you
can save time entering data by making use of HAP’s automatic defaulting feature for constructions. The
constructions for a newly added exposure are defaulted using the constructions specified for the previous
exposure (e.g. exposure #4 uses defaults from exposure #3). Taking advantage of this feature requires
specifying a complete set of constructions for one exposure before you add the next exposure To illustrate this
procedure the following example is used.
Example: A space contains three wall exposures: West, South and East. The same wall and window
constructions are used for all three exposures.
Procedure:
1. In the left-hand panel, specify the orientation, gross area and window quantity for the first (West) exposure.
2. While the first exposure is still the current exposure, use the right-hand panel to create or choose the wall
and window constructions for this exposure.
3. Return to the left-hand panel and specify the orientation, gross area and window quantity for the second
(South) exposure. When you add this exposure by changing its orientation from "not used" to "South", HAP
will automatically default its wall and window constructions to the constructions used for the first exposure.
This saves you the time of selecting wall and window constructions from the drop down lists for this second
exposure.
4. In the left-hand panel specify the orientation, gross area and window quantity for the third (East) exposure.
When you add this exposure by changing its orientation from "not used" to "East", HAP will automatically
default its wall and window constructions to the constructions used in the second exposure. Again you save
the time required to select wall and window constructions yourself.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Roof and Skylights tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Roof, Skylights Tab / Space Form
Page 17 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
About Roofs & Skylights. The Roofs, Skylights tab on the Space Form contains information about horizontal
and sloped roof exposures and the skylights contained in these exposures. This data is used to calculate the
following envelope loads for a space: roof transmission, skylight transmission, and skylight solar loads.
The Roofs, Skylights Tab is divided into two panels which occupy the left-hand and right-hand halves of the
tab:
1. Roof Exposure Table. The left-hand panel contains a table of roof exposure data. Each row in this table
contains data for one roof exposure. Columns contain different attributes of the exposure. Up to 4
exposures can be defined for each space. The figure above shows a space with one horizontal roof
exposure.
2. Construction Types. The right-hand panel contains construction information for the current exposure: roof
type and skylight type. Constructions are chosen from drop-down lists that contain roof and window
constructions you previously created and stored in your project database. Features are also provided for
creating new constructions or editing existing constructions without leaving the space form.
As you move from one row to the next in the roof table in the left panel, the information displayed in the
right-hand panel changes to show constructions selected for that exposure. In the figure above, the current
exposure in the left-hand panel is exposure #1. The current exposure is indicated by which row number at
the left end of the row is highlighted. Therefore, construction types for exposure #1 are shown in the right-
hand panel. The current exposure is also listed at the top of the right-hand panel.
Further information about input items in each panel are provided below.
Roof Exposure Table / Left-Hand Panel
1. Roof Exposure defines the direction the exterior surface of the roof faces. For horizontal roofs, choose "H"
for horizontal from the drop-down list. For a sloped roof, choose any of 16 principal orientations from the
drop-down list. To add a roof exposure, change its orientation from "not used" to horizontal or one of the 16
principal orientations. When you do this, data items for the exposure will be enabled. To delete a roof
Page 18 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
exposure, change its orientation to "not used". When you do this, data items for the exposure will be
disabled.
2. Roof Gross Area refers to the total surface area of this exposure including roof surface and skylight areas.
Later, during load calculations, the program will calculate the net roof area by subtracting the skylight area
from the gross exposure area.
3. Roof Slope. When a roof exposure other than horizontal is specified, the user is asked to define the slope
of the roof in degrees. Roof slope is measured from horizontal. Thus a 60 degree roof slope is steeper than
a 30 degree roof slope.
In some cases building plans specify roof slope in terms of pitch rather than degrees. The following table is
provided to assist you in converting common pitch specifications to degrees.
Pitch
(rise:run)
Slope in
degrees
from Horiz
Pitch
(rise:run)
Slope in
degrees
from Horiz
1:12
5º
1:10
6º
2:12
9º
1:9
6º
3:12
14º
1:8
7º
4:12
18º
1:7
8º
5:12
23º
1:6
9º
6:12
27º
1:5
11º
7:12
30º
1:4
14º
8:12
34º
1:3
18º
9:12
37º
1:2.5
22º
10:12
40º
1:2
27º
11:12
43º
1:1.5
34º
12:12
45º
1:1
45º
3. Skylight Quantity is used to specify the quantity of skylights of a particular construction on this exposure.
For example, if the skylight type specified in the right-hand panel of this tab is a 3 ft by 8 ft double-glazed
skylight unit, the skylight quantity defines the number of these 3x8 skylight units used in the exposure. The
skylight quantity can be entered directly, or you can use the spin buttons to increment or decrement the
skylight quantity.
In some applications, users define the skylight construction as a unit area section of glass (1 ft by 1 ft or 1 m
by 1 m) so the window quantity defines the total glass area. This is typically done only in preliminary block
load estimates in which detailed skylight modeling is not necessary, or when an exposure contains a large
number of skylights having widely varying dimensions.
Finally, if the roof exposure does not contain skylights, specify a quantity of zero.
Constructions / Right-Hand Panel
The right-hand panel of the Roofs, Skylights tab contains input items for two constructions associated with the
current exposure. Only those constructions used for the current exposure need to be defined. Unused
constructions can be specified as "none". The constructions defined in this panel are:
1. Roof: The roof assembly used for this exposure. A roof type must be defined for each exposure used by the
space.
2. Skylight: The window construction used for the skylights in this roof exposure. Only required if a Skylight
Quantity has been specified.
Page 19 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.6 Infiltration
10.0 Entering Spaces ››
Infiltration Tab / Space Form
10.0 Entering Spaces ›› 10.6 Infiltration ››
Each of these constructions can be defined in two ways. The discussion below uses the roof construction as
an example, but the same procedures can be used for skylights.
1. Creating a New Roof Construction. If you have not yet created a roof construction, choose the "create
new roof" item in the roof drop-down list. The Roof Construction Form will appear and will allow you to
define the properties of material layers comprising the roof. When you press the OK button to exit from the
Roof Construction Form, your roof data will be stored and the roof will be assigned to the current roof
exposure automatically.
2. Selecting an Existing Roof Construction. If you previously created and stored roofs in your project
database, you can simply select the desired roof from the drop-down list.
In addition, you can modify roof and skylight construction data directly from the Space Form by pressing the
button to the left of the construction drop-down list. When you press this button, the input form for the
appropriate construction type will appear and will display inputs for the currently selected construction. After
modifying the data, press the OK button to return to the Space Form.
Application Information
For many applications, the same set of constructions is used for all roof exposures in a space. In such a case,
you can save time entering data by making use of HAP’s automatic defaulting feature for constructions. The
constructions for a newly added exposure are defaulted using the constructions specified for the previous
exposure (e.g. exposure #4 uses defaults from exposure #3). Taking advantage of this feature requires
specifying a complete set of constructions for one exposure before you add the next exposure To illustrate this
procedure the following example is used.
Example: A space contains a sloped roof divided into four sections which face North, South, East and West.
Therefore, four roof exposures will be entered for the space.
Procedure:
1. In the left-hand panel, specify the orientation, gross area and slope for the first (North) exposure.
2. While the first exposure is still the current exposure, use the right-hand panel to create or choose the roof
constructions for this exposure.
3. Return to the left-hand panel and specify the orientation, gross area and slope for the second (East)
exposure. When you add this exposure by changing its orientation from "not used" to "East", HAP will
automatically default its roof construction to the construction used for the first exposure. This saves you the
time of selecting a roof construction from the drop down list for this second exposure.
4. Repeat step 3 for the third (South) exposure. Its construction data will be defaulted using data from
exposure 2.
5. Repeat step 3 for the fourth (West) exposure. Its construction data will be defaulted using data from
exposure 3.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes input data on the Infiltration tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 20 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Infiltration Tab / Space Form
About Infiltration. The Infiltration tab on the Space Form contains information about infiltration airflow for the
space for design cooling, design heating and energy simulation calculations. Infiltration results from the
leakage of outdoor air into the space. This typically occurs because of leakage around windows and doors,
and leakage from the opening and closing of doors in the space. Infiltration data is used to calculate the
sensible and latent infiltration loads for the space.
The Infiltration Tab. The central portion of the infiltration tab contains a table of infiltration specifications.
Rows in the table contain infiltration data for design cooling, design heating and energy analysis conditions.
Columns in the table contain infiltration specifications in three different units of measure. When you enter an
infiltration rate in one column, values for the other two columns in the row are calculated automatically. In each
row, the infiltration rate that you entered is indicated by a white border. In the figure above, CFM/sqft was
entered for design cooling, ACH was entered for design heating and CFM/sqft was entered for energy
analysis. Details concerning rows and columns in this table are provided below.
1. Items in the Design Cooling row define infiltration rates used for load calculations on design cooling days.
These load calculations only affect sizing of cooling equipment.
2. Items in the Design Heating row define infiltration rates used for design heating load calculations. These
calculations only affect sizing of heating equipment.
3. Items in the Energy Analysis row define infiltration rates used only in the annual energy simulations.
Therefore, these values only affect the calculation of annual energy use and operating cost.
4. Items in the CFM or L/s column define the infiltration rate as a gross airflow. This value is entered when the
total infiltration airflow for a space is known. It is used directly in calculations.
5. Items in the CFM/sqft or L/s/sqm column define infiltration in terms of airflow per unit of exterior wall area.
Because infiltration occurs through exterior walls - especially through windows and doors in these walls -
rule of thumb infiltration rates are sometimes tabulated in this CFM/sqft or L/s/sqm format. When infiltration
Page 21 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.7 Floors
10.0 Entering Spaces ››
Floors Tab / Space Form
10.0 Entering Spaces ›› 10.7 Floors ››
is entered as CFM/sqft (L/s/sqm), the program calculates the total infiltration airflow by multiplying CFM/sqft
or L/s/sqm by the gross wall area for the space.
6. Items in the ACH column define infiltration in terms of air changes per hour. When infiltration is entered as
ACH, the program uses this ACH value plus the space volume to calculate the total infiltration airflow.
Space volume is derived from the total space floor area and the average floor to ceiling height defined on
the General data tab.
The infiltration tab contains one additional input describing how infiltration occurs. The Infiltration Occurs
item offers two choices for modeling hourly variation of infiltration airflow:
1. Only When Fan Off. This option will limit infiltration load calculations to those hours during which the
fan/thermostat schedule for the system serving the space has been scheduled for the "unoccupied" mode.
This option is used to model situations in which the building is positively pressurized during "occupied"
hours when the system is running continuously. Therefore, infiltration will only occur during the
"unoccupied" hours when the system is off.
Note: If you select the "only when fan off" option, infiltration load will not be calculated for the design heating
condition. This is because the design heating conditions is assumed to be a fan ON hour, with the room
temperature at the occupied heating setpoint, the outdoor air dampers open, and the HVAC fan operating to
circulate air.
2. All Hours. With this option, infiltration loads will be calculated for all hours of the day, regardless of whether
the system is in "occupied" or "unoccupied" mode. This option is used to model situations in which the
building is not pressurized or the pressurization is negligible when the system is on. As a result infiltration
occurs for all hours of the day.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Floors tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Floors Tab / Space Form
About Floors. The Floors tab on the Space Form contains information about heat transfer through floors.
Items on the Floors tab only involve floor types through which heat flow is analyzed: floors above
unconditioned or partially conditioned regions, slab-on-grade floors and basement floors. HAP assumes that
heat transfer through floors above conditioned regions is negligible. Data on the Floors tab is used to calculate
floor transmission loads. When modeling basement floors, inputs are also used to determine transmission
loads for the below-grade portion of basement walls.
Page 22 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
The Floors Tab is divided into two panels which occupy the upper and lower halves of the tab:
1. Floor Type Selection. The upper panel permits selection of the floor type. In the figure above, a Slab Floor
On Grade has been selected.
2. Floor Data. The lower panel contains items describing the heat transmission characteristics of the chosen
floor type.
Because construction characteristics and the heat transfer mechanisms vary significantly between the different
floor types, the list of floor input items in the lower panel changes depending on the floor type selected. Each
floor type and its associated input items are described below:
1. Floor Above Conditioned Space. HAP assumes heat transfer through floors above conditioned spaces is
negligible. Therefore no further input data is required when this floor type is selected.
2. Floor Above Unconditioned Space. Heat transfer between the space and an unconditioned or partially
conditioned region below it is analyzed because of the difference between the space air temperature and
the air temperature in the unconditioned region. Examples: The space is above an unconditioned or partially
conditioned warehouse, a refrigerated storeroom, a mechanical equipment room or a parking garage. Heat
transmission inputs for this type of floor area:
Floor Area
Total Floor U-value
Unconditioned Space Maximum Temperature
Ambient at Maximum Space Temperature
Unconditioned Space Minimum Temperature
Ambient at Minimum Space Temperature
Page 23 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Floor Area Above Unconditioned Space
10.0 Entering Spaces ›› 10.7 Floors ››
Floor Above Unconditioned Space Total U-Value
10.0 Entering Spaces ›› 10.7 Floors ››
Floor Above Unconditioned Space Temperatures
10.0 Entering Spaces ›› 10.7 Floors ››
3. Slab-On-Grade Floor. Heat transfer through the floor to the soil below, and heat transfer through the
exposed perimeter of the floor are analyzed for this floor type. Heat transmission inputs for this type of floor
are:
Floor Area
Total Floor U-value
Exposed Perimeter
Edge Insulation R-Value
4. Slab-Below-Grade Floor. With this floor type, heat transfer through the basement floor and the exposed
perimeter of the floor to adjacent soil is analyzed. Heat transfer through the below-grade portion of
basement walls is also included in these calculations. Heat transmission inputs for this type of floor are:
Floor Area
Exposed Perimeter
Total Floor U-Value
Floor Depth
Basement Wall U-Value
Wall Insulation R-Value
Depth of Wall Insulation
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Floor Area Above Unconditioned Space
Specify the total floor area which is above the unconditioned or partially conditioned region. Floor area is used
to calculate the floor transmission load.
Typically this floor area equals the total space floor area, specified earlier. However, if only a portion of the
space is above the unconditioned region, then only the floor area for that portion of the space should be
specified here.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Floor Above Unconditioned Space Total U-Value
Specify the overall U-value for the floor. It should be based on the total resistance for the floor including both
the resistance of the floor material such as wood or concrete, and any floor covering such as carpeting or tile.
The Floor U-value is used to compute heat transfer through the floor.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 24 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Floor Above Unconditioned Space Temperatures
When calculating transmission loads for floors above unconditioned regions, the temperature of the
unconditioned region must be known. Temperature behavior in the unconditioned region is estimated with a
simple linear model which defines the unconditioned space temperature as a function of the outdoor air
temperature. The model is defined by specifying two pairs of temperatures:
1. The Unconditioned Space Maximum Temperature and the corresponding Ambient Temperature at
Maximum Space Temperature.
2. The Unconditioned Space Minimum Temperature and the corresponding Ambient Temperature at Minimum
Space Temperature.
Together these four temperature inputs define the three sections of the space temperature profile:
1. When the outdoor air temperature is warmer than the "Ambient at Maximum Space Temperature", the
unconditioned space temperature is equal to the "Unconditioned Space Maximum Temperature."
2. When the outdoor air temperature is between the "Ambient at Maximum Space Temperature" and "Ambient
at Minimum Space Temperature", the unconditioned space temperature varies linearly with outdoor
temperature.
3. When the outdoor air temperature is colder than the "Ambient at Minimum Space Temperature", the
unconditioned space temperature is equal to the "Unconditioned Space Minimum Temperature."
Example: A partially conditioned warehouse is below the conditioned space. The warehouse is heated to
maintain a 50 F air temperature in winter and is cooled to maintain a 95 F air temperature in the summer.
Otherwise, the warehouse temperature floats between 95 F and 50 F. Based on engineering judgment, it is
assumed the warehouse reaches 50 F when it is 30 F outdoors. The warehouse reaches 95 F when it is 90 F
outdoors. Inputs used to model this situation are as follows:
Unconditioned Space Maximum Temperature = 95 F.
Ambient at Maximum Space Temperature = 90 F.
Unconditioned Space Minimum Temperature = 50 F
Ambient at Minimum Space Temperature = 30 F
Page 25 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Slab Floor Area
10.0 Entering Spaces ›› 10.7 Floors ››
Slab Floor Total U-Value
10.0 Entering Spaces ›› 10.7 Floors ››
Slab Floor Exposed Perimeter
10.0 Entering Spaces ›› 10.7 Floors ››
Slab Floor Edge Insulation R-Value
10.0 Entering Spaces ›› 10.7 Floors ››
The figure above shows the unconditioned space temperature profile resulting from these inputs. When the
outdoor temperature is above 90 F, the space temperature remains constant at 95 F. Between outdoor
temperatures of 90 F and 30 F, the unconditioned space temperature varies linearly as a function of outdoor
temperature. Below 30 F, the unconditioned space temperature remains constant at 50 F.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Slab Floor Area
Specify the total area of the slab-on-grade floor. The slab floor area is used together with the slab exposed
perimeter to determine heat transfer through the slab and the soil beneath it.
Typically this floor area equals the total space floor area, specified earlier. However, if only a portion of the
space is slab-on-grade, then only the floor area for that portion of the space should be specified here.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Slab Floor Total U-Value
Specify the overall U-value for the slab floor. This U-value should be include the resistance of the concrete
floor plus any floor covering such as carpeting or tile, and the inside surface convection coefficient. The Floor
U-value is used to compute heat transfer through the floor.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Slab Floor Exposed Perimeter
This item defines the perimeter of the slab floor exposed to the ambient for this space only. Do not enter the
perimeter for the entire building slab or the perimeter for the entire room when one or more sides of the room
are not exposed to ambient. This value is used together with the slab floor area to determine heat transfer
through the floor and the soil beneath.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Slab Floor Edge Insulation R-Value
Page 26 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Basement Floor Area
10.0 Entering Spaces ›› 10.7 Floors ››
Basement Floor Exposed Perimeter
10.0 Entering Spaces ›› 10.7 Floors ››
Basement Floor Total U-Value
This item defines the thermal resistance of insulation used along the inner edge of the slab footer (see figure
below). In cold climates, insulation is often used to reduce slab heat loss. The program assumes insulation
with this thermal resistance is present along the entire perimeter of the slab footer for this space. If edge
insulation is not used, specify an R-value of zero.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basement Floor Area
Specify the total area of the slab-below-grade floor. The slab floor area is used together with the slab exposed
perimeter to determine heat transfer through the slab and the soil adjacent to it.
Typically this floor area equals the total space floor area, specified earlier. However, if only a portion of the
space is slab-below-grade, then only the floor area for that portion of the space should be specified here.
For further information on basement floor heat transmission calculations, please refer to the load calculation
topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basement Floor Exposed Perimeter
This item defines the perimeter of the basement floor exposed to contact with soil for this space only. Do not
enter the perimeter for the entire building slab or the perimeter for the entire room when one or more sides of
the room are not exposed to direct soil contact. This value is used together with the slab floor area to
determine heat transfer through the floor and the soil adjacent to it. It is also used with the floor depth to
compute the area of below-grade basement walls for the space. When heat transmission is calculated, heat
flow through the basement floor and the below-grade basement walls will be determined.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 27 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.0 Entering Spaces ›› 10.7 Floors ››
Basement Floor Depth
10.0 Entering Spaces ›› 10.7 Floors ››
Basement Wall Construction Data
10.0 Entering Spaces ›› 10.7 Floors ››
Basement Floor Total U-Value
Specify the overall U-value for the below-grade slab floor. This U-value should be include the resistance of the
concrete floor plus any floor covering such as carpeting or tile, and the inside surface convection coefficient.
The Floor U-value is used to compute heat transfer through the floor.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basement Floor Depth
This item defines the distance between grade level and the top of the slab floor. It is used to compute the area
of the below-grade basement wall. It is also used to calculate heat transfer through the slab floor and the
basement walls since heat flow varies with depth below grade.
For further information on slab floor heat transmission calculations, please refer to the load calculation topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basement Wall Construction Data
When modeling a below-grade slab floor, HAP also calculates heat flow through the below-grade portion of
basement walls. Three inputs are used to describe the construction of the basement wall.
1. Basement Wall U-Value. Specify the overall U-value for the basement wall. Include the resistance of the
wall itself, any framing and finishing layers, and the inside surface convection coefficient. The resistance of
any exterior insulation layers should not be included if it is modeled separately with the next two inputs.
2. Basement Wall Insulation R-Value defines the total thermal resistance of insulation used on the outer
surface of the basement walls (see figure below). In cold climates, this insulation is often used to reduce
heat loss for the portion of the wall just below grade. Wall insulation having this R-value is assumed along
the entire exposed perimeter of the basement wall for this space.
3. Depth of Wall Insulation defines the depth below grade to which exterior wall insulation is used. Insulation
is often not applied over the entire exterior surface of the basement wall. Rather it is applied over the
portion nearest the grade level through which the greatest heat losses occur.
If wall insulation is not used, specify a zero depth.
Page 28 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.8 Partitions
10.0 Entering Spaces ››
Partition Tab / Space Form
10.0 Entering Spaces ›› 10.8 Partitions ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes input data on the Partitions tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition Tab / Space Form
About Partitions. The Partitions tab on the Space Form contains information about heat transfer through
walls and ceilings which are adjacent to unconditioned or partially conditioned regions, or adjacent to regions
at significantly different temperatures. Examples: A wall adjacent to an unconditioned warehouse, a
refrigerated storeroom, or an unconditioned mechanical room. Heat flow through these walls and ceilings
depends upon the heat transmission properties of the wall or ceiling and the temperature behavior in the
adjacent region which are both specified by the user.
Page 29 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Partition Type
10.0 Entering Spaces ›› 10.8 Partitions ››
The Partitions Tab. Each space can contain up to two partition elements. The Partitions tab divided into two
panels which allow the characteristics of each wall or ceiling partition to be defined:
Partition Type
Area
U-Value
Unconditioned Space Maximum Temperature
Ambient at Space Maximum Temperature
Unconditioned Space Minimum Temperature
Ambient at Space Minimum Temperature
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition Type
This item defines whether partition data is for a ceiling or a wall adjacent to an unconditioned region. This input
determines how loads for the partition are reported on design load calculation reports. These reports contain
separate line items for ceilings and partitions (walls). Readers should note that the same procedure is used to
calculate loads whether it is designated as a ceiling partition or a wall partition. This input only affects where
the load is reported.
Page 30 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Partition Area
10.0 Entering Spaces ›› 10.8 Partitions ››
Partition U-Value
10.0 Entering Spaces ›› 10.8 Partitions ››
Partition Unconditioned Space Temperatures
10.0 Entering Spaces ›› 10.8 Partitions ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition Area
Specify the gross surface area of the wall or ceiling partition which is adjacent to the unconditioned region.
Gross area is used when computing the heat gain or loss through the partition.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition U-Value
Specify the overall U-value for the wall or ceiling partition. This U-value is used when computing heat transfer
through the ceiling or wall partition.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition Unconditioned Space Temperatures
When calculating transmission loads for wall or ceiling partitions adjacent to unconditioned regions, the
temperature of the unconditioned region must be known. Temperature behavior in the unconditioned region is
estimated with a simple linear model which defines the unconditioned space temperature as a function of the
outdoor air temperature. The model is defined by specifying two pairs of temperatures:
1. The Unconditioned Space Maximum Temperature and the corresponding Ambient Temperature at
Maximum Space Temperature.
2. The Unconditioned Space Minimum Temperature and the corresponding Ambient Temperature at Minimum
Space Temperature.
Together these four temperature inputs define the three sections of the space temperature profile:
1. When the outdoor air temperature is warmer than the "Ambient at Maximum Space Temperature", the
unconditioned space temperature is equal to the "Unconditioned Space Maximum Temperature."
2. When the outdoor air temperature is between the "Ambient at Maximum Space Temperature" and "Ambient
at Minimum Space Temperature", the unconditioned space temperature varies linearly with outdoor
temperature.
3. When the outdoor air temperature is colder than the "Ambient at Minimum Space Temperature", the
unconditioned space temperature is equal to the "Unconditioned Space Minimum Temperature."
Page 31 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
10.9 Common Tasks
10.0 Entering Spaces ››
Overview for Replace Space Data Form
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Example: A partially conditioned warehouse is adjacent to the conditioned space. The warehouse is heated to
maintain a 50 F air temperature in winter and is cooled to maintain a 95 F air temperature in the summer.
Otherwise, the warehouse temperature floats between 95 F and 50 F. Based on engineering judgment, it is
assumed the warehouse reaches 50 F when it is 30 F outdoors. The warehouse reaches 95 F when it is 90 F
outdoors. Inputs used to model such a situation are as follows:
Unconditioned Space Maximum Temperature = 95 F.
Ambient at Maximum Space Temperature = 90 F.
Unconditioned Space Minimum Temperature = 50 F
Ambient at Minimum Space Temperature = 30 F
The figure above shows the unconditioned space temperature profile resulting from these inputs. When the
outdoor temperature is above 90 F, the space temperature remains constant at 95 F. Between outdoor
temperatures of 90 F and 30 F, the unconditioned space temperature varies linearly as a function of outdoor
temperature. Below 30 F, the unconditioned space temperature remains constant at 50 F.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with space input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Replace Space Data Form
Page 32 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Replacing Space Data. The Replace Space Data feature in HAP is used to change space data quickly.
Rather than modifying space data one space at a time, this option allows you to choose a category of data and
a group of spaces, and then make changes automatically for all spaces in the group. This feature is useful
when building specifications change after space data has been entered. For example if lighting fixture
specifications are changed in 45 spaces that have already been defined, the Replace Space Data feature can
be used globally change the lighting data for all 45 spaces in one step rather than changing the data one
space at a time. In HAP the this global replace task can be performed in two ways:
1. Search & Replace. With this approach you define a "value to replace" and a "replace with" value. For
example if "value to replace" is 2.0 W/sqft of overhead lighting and "replace with" is 1.8 W/sqft, the program
will replace all overhead lighting values of 2.0 W/sqft in spaces you designate with 1.8 W/sqft.
2. Replace All. With this approach you only define a "replace with value" which is then used to replace all
items in the designated spaces, regardless of each item’s original value. The "value to replace" item is left
blank in this case. For example, if the "replace with" value is 1.8 W/sqft of overhead lighting and the "value
to replace" is blank, HAP will replace all overhead lighting values in the designated spaces with 1.8 W/sqft,
regardless of the original lighting values for each space.
The Replace Space Data Form, shown above, is used to control the global replacement of space data.
Before this form appears, you must select the spaces you wish to include in the global replace procedure and
then choose the "Replace Data" option. There are four different ways to do this, as described in the Replacing
Space Data help topic.
The Replace Data form consists of three key components:
1. The Title Bar appears across the top of the form. It lists the spaces which have been selected for inclusion
in the global replacement procedure. In the figure above, three spaces have been selected. When the list of
spaces selected is too large to display, the initial spaces will be listed along with a "…" to indicate that
additional spaces are included. Finally, at the right end of the title bar is a button for closing the form.
2. The Working Area in the center of the form is used to specify what data is to be replaced and how it is to
be replaced. The working area is divided into seven tabs - one for each of the principal categories of space
Page 33 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Overview for Rotate Space Data Form
10.0 Entering Spaces ›› 10.9 Common Tasks ››
data. To switch between tabs, simply click on the desired tab name. Each tab contains the same three input
items used to control global replacement of data:
a. Type of Data to Replace. Choose the type of space data to be changed by selecting the desired item
from this drop-down list. The contents of this list change depending on the current tab. For example,
when you are on the Internals tab, only space inputs related to internal loads will be offered in the list.
b. Specific Value to Replace. If you wish to use the "search and replace" approach described earlier in this
topic, specify the value you wish to replace. In the figure above, all overhead lighting wattage values of
2.0 W/sqft will be replaced. When you wish to use the "replace all" approach to changing data, leave this
input item blank. This tells HAP to replace all values of a particular type, regardless of the original value
of that item.
c. Replace With Value. Specify the new value which will replace the current value. In the figure above,
overhead lighting fixture wattages will be changed to 1.8 W/sqft.
3. Command Buttons appear along the bottom of the form. Four buttons are provided for controlling the
global replacement process:
a. Press OK to perform the global change using the data shown in the working area of the form, and then
return to the Main Program Window. Use this button when you only want to perform one global change
for a set of spaces, or for the last in a sequence of global changes. If no changes have been specified,
this button simply closes the window.
b. Press Cancel to return to the Main Program Window without changing space data. Changes you have
entered, but not yet applied, will be lost.
c. Press Apply to perform the global change using data shown in the working area of the form. When the
global replacement is complete, HAP returns to the Replace Data form so you can specify another global
change. This button is useful when you need to perform global changes for several different space input
items one after the other.
d. Press Help to display this overview help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Rotate Space Data Form
Rotating Spaces. The Rotate Space Data feature in HAP is used to quickly change the orientation of walls
and sloped roofs in a space. Instead of modifying spaces one at a time, the Rotate feature allows you to
choose a group of spaces and change the orientations for all spaces in the group in one simple step. This
feature is useful when building specifications change after the space data has been entered.
Page 34 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Creating a New Space
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Editing an Existing Space
10.0 Entering Spaces ›› 10.9 Common Tasks ››
The Rotate Data Form, shown above, is used to control how the space orientation is changed. Before this
form appears, you must select the spaces you wish to rotate and then choose the "Rotate Data" option. There
are four different ways to do this, as described in the Rotating Space Data help topic.
The Rotate Data form consists of three key components:
1. The Title Bar appears across the top of the form. It lists the spaces which have been selected for rotation.
In the figure above, several spaces have been selected, but there is only room in the title bar to display
names for the first two. The "…" after the second name indicates that additional spaces are included.
Finally, at the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form. It contains a dial that is used to specify the amount and
direction by which spaces will be rotated. To specify rotation, use the mouse to drag the needle to the
desired position. The arrow keys can also be used to move the needle. As you move the needle, the
amount of clockwise rotation will be listed beneath the dial. In the figure above, the needle has been moved
45 degrees in a clockwise direction. Therefore all selected spaces will be rotated in this manner. For
example, the orientation of a north-facing wall will be change to northeast.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to rotate the selected spaces by the amount currently specified in the working area. The
orientation of all wall exposures and any sloped roof exposures will be rotated in all spaces you’ve
selected. When the rotation is complete, a message box will appear listing the total number of walls and
roofs that were rotated. Finally you will be returned to the Main Program Window.
b. Press Cancel to exit from the Rotate Data form without rotating spaces.
c. Press Help to display this overview help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Space
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 35 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm
Printing Space Inputs
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Deleting Spaces
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Copying a Space
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Duplicating a Space
10.0 Entering Spaces ›› 10.9 Common Tasks ››
Editing an Existing Space
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Space Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Spaces
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Space
Please see Duplicating An Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Space
Please see Duplicating An Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 36 of 36
10.0 Entering Spaces
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhEC91.htm