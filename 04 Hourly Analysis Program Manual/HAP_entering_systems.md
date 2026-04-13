11.0 Entering Systems
11.1 Overview for Systems and the System Form
11.0 Entering Systems ››
Overview for Systems and the System Form
11.0 Entering Systems ›› 11.1 Overview for Systems and the System Form ››
This chapter explains input data for HVAC air systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of how air system input data is organized.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Systems and the System Form
About Systems. An Air System is the equipment and controls which provide cooling and heating to a region of a building. An air system serves one or more zones; each
zone is a group of one or more spaces having a single thermostatic control. Examples of air systems include central station air handlers, packaged rooftop units,
packaged vertical units, split systems, packaged DX fan coils, hydronic fan coils and water source heat pumps. Components in an air system include fans and coils as
well as the associated ductwork, supply terminals and controls. When performing an energy analysis, the DX cooling, heat pump, electric resistance heating and
combustion heating components are considered part of the air system.
Air system data must be entered and saved in your project before reports containing design load information and system sizing information can be generated. In addition,
when sizing plants such as chillers and boilers, all systems served by the plant must be defined before plant sizing reports can be generated.
The System Form, shown above, is used to define the characteristics of an air system. The System Form contains three key components:
1. The Title Bar appears across the top of the form. It lists the name of the system whose data is displayed in the form. At the right end of the title bar is a button for
closing the form.
2. The Working Area is in the center of the form and contains multiple categories of system information represented as separate tabs in a notebook. For the full HAP
edition there are five tabs for the five categories of system data. For HAP System Design Load only the first four of these categories are used. To move from one tab
to another, simply click on the desired tab. The five tabs are as follows:
a. General contains the system name, its equipment classification and system type, and the number of zones.
b. System Components contains information about centrally located components in the system such as fans and coils, and information about the distribution duct
system.
c. Zone Components contains data describing the spaces in each zone and equipment in the zone such as supply terminals, thermostats and supplemental heating
units.
d. Sizing Data contains criteria for sizing the system. It also contains system sizing values which can be directly entered for retrofit applications rather than being
calculated by the program.
e. Equipment Data contains information about DX cooling, heat pump, and combustion heating components of the system. This information is only relevant when
performing energy analyses. Note that when running the program in System Design Load mode, this tab does not appear.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the system inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the system. If you press Cancel while creating a new system, a new system will not
be added to your project.
c. Press Help to display this overview topic.
System Features. Finally, HAP provides useful features for:
Creating new systems.
Editing an existing system.
Page 1 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.2 General System Data
11.0 Entering Systems ››
General Tab / System Form
11.0 Entering Systems ›› 11.2 General System Data ››
System Name
11.0 Entering Systems ›› 11.2 General System Data ››
Equipment Type
11.0 Entering Systems ›› 11.2 General System Data ››
Printing system data
Deleting a system.
Copying a system.
Duplicating a system.
Printing or viewing system design reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the General tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
General Tab / System Form
The General tab on the system form contains several key values which describe the nature of the system as a whole. Input items on this tab determine the items and
options that appear on the remaining three tabs. Items on this tab include:
System Name
Equipment Type
System Type
Number of Zones
Ventilation Air (for terminal systems only).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Name
This is a reference name used to identify the air system. It appears on the main program window, on system input reports and system design reports. It also appears on
selection lists when linking systems to plants. Therefore, it is useful to make this name as descriptive as possible so you can easily differentiate this system from others in
your project.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Type
This item defines the equipment classification for the HVAC system being analyzed. The choice of an equipment type determines the system types offered in the next
input item, the components and controls which can be included in the system, choices for cooling and heating sources and whether a system can be linked to certain
types of plants. For example, a Chilled Water Air Handling Unit can be connected to a chiller plant for plant sizing calculations, but a Packaged Rooftop Unit cannot.
Users may choose from six equipment classifications:
Page 2 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
System Type
11.0 Entering Systems ›› 11.2 General System Data ››
Number of Zones
11.0 Entering Systems ›› 11.2 General System Data ››
1. Undefined: This option allows you to avoid making an equipment type choice. It is often used for preliminary block load estimates in which equipment type is not yet
relevant. It is also used in detailed system design studies in which the equipment type is not yet known.
When Undefined is selected, cooling and heating sources for coils will default to "any". It will not be possible to choose specific sources such as "chilled water" or "hot
water". Systems using the "undefined" equipment type are, however, allowed to be connected to chiller and boiler plants for plant sizing calculations.
2. Packaged Rooftop Units: Packaged rooftop DX cooling units. The equipment can be cooling only, or can also provide electric, combustion, hot water, steam or heat
pump heating.
3. Packaged Vertical Units: Packaged indoor DX cooling units. The equipment can be cooling only, or can also provide electric, combustion, hot water, or steam
heating.
4. Split Air Handling Units: Packaged or built-up air handling units using a DX cooling coil and a separate condensing unit. Equipment can be cooling only, or can also
provide electric, combustion, hot water, steam or heat pump heating.
5. Chilled Water Air Handling Units: Packaged or built-up air handling units using a chilled water cooling coil. Equipment can be cooling only or can also provide
electric, combustion, hot water or steam heating.
6. Terminal Units: This class of equipment involves separate cooling/heating units located in each zone. Examples include packaged DX fan coil units such as PTACs
or PTHPs, split DX fan coil units, hydronic fan coil units, water source heat pumps, VRF units, induction beams and active chilled beams.
The program offers special features for modeling these systems. In HAP, a terminal unit system can contain multiple zones, each containing a separate terminal unit.
Thus, large quantities of units can be modeled quickly as part of one "system". HAP permits modeling of systems in which outdoor ventilation air is introduced directly
to terminal units, and also systems in which a Dedicated Outdoor Air System (DOAS) unit is used to treat outdoor air and then deliver it to terminal units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Type
This item defines the kind of air system being entered. HAP offers features for analyzing a variety of common air handling systems. Choosing a system type is important
because each type contains different components and operates in different ways.
When performing system design work with HAP, the choice of a system type will influence system sizing calculations because the program tailors sizing procedures to
the system type. This is referred to as "System-Based Design". For example, sizing procedures for constant volume systems differ from those for variable volume
systems. In addition, the program will generate data to size the major components in each system. For example, a Two-Fan Dual Duct VAV system contains two supply
fans which each must be sized, while most other system types contain only one supply fan.
When using HAP to perform operating cost studies, the choice of a system type will influence the system operation and energy consumption levels during the whole year
energy simulation the program performs.
The contents of the drop-down list for system type vary according to the equipment type you chose. System types available within each equipment classification are
shown below.
Undefined
Packaged Rooftop Units
Packaged Vertical Units
CAV - Single Zone
CAV - Single Zone
CAV - Single Zone
CAV - Terminal Reheat
CAV - Terminal Reheat
CAV - Terminal Reheat
VAV
CAV - 2-Deck Multizone
VAV
VVT
CAV - 3-Deck Multizone
VVT
CAV - Dual Duct
CAV - Make Up Air / DOAS
VAV
VAV - 1-Fan Dual Duct
VAV - 2-Fan Dual Duct
VVT
Split AHU
Chilled Water AHU
Terminal Units
CAV - Single Zone
CAV - Single Zone
Packaged DX Fan Coils
CAV - Terminal Reheat
CAV - Terminal Reheat
Split DX Fan Coils
CAV - 2-Deck Multizone
CAV - 2-Deck Multizone
Water Source Heat Pumps
CAV - 3-Deck Multizone
CAV - 3-Deck Multizone
Ground Water Source Heat Pumps
CAV - Dual Duct
CAV - Dual Duct
Ground Source Heat Pumps
CAV - Make Up Air / DOAS
CAV - Make Up Air / DOAS
2-Pipe Fan Coils
VAV
CAV - 4-Pipe Induction
4-Pipe Fan Coils
VAV - 1-Fan Dual Duct
VAV
Induction Beams
VAV - 2-Fan Dual Duct
VAV - 1-Fan Dual Duct
Active Chilled Beams
VVT
VAV - 2-Fan Dual Duct
Variable Refrigerant Flow (VRF)
VVT
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 3 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Air for Terminal Systems
11.0 Entering Systems ›› 11.2 General System Data ››
11.3 System Components Data
11.0 Entering Systems ››
System Components Tab / System Form
11.0 Entering Systems ›› 11.3 System Components Data ››
Number of Zones
This item defines the number of zones served by the air system. A "zone" is a group of one or more spaces having a single thermostatic control. Later, the spaces
included in each zone will be defined along with descriptions of thermostat setpoints and supply terminal equipment.
Zones are often used differently for different applications:
a. In some systems, each room contains a thermostat. Therefore, each zone contains one space representing a single room.
b. In other situations, one thermostat is allocated to a group of rooms. In these cases, the zone includes several spaces.
c. In terminal unit systems (DX fan coils, hydronic fan coils, induction beams, active chilled beams, water source heat pumps), each zone contains a separate terminal
unit with its own thermostat. This feature of the program allows you to define one system encompassing a large number of zones each containing a terminal unit. This
serves as an efficient way for analyzing performance of large numbers of terminal units at one time.
d. For preliminary load estimates, a zone might be used to represent rooms on one exposure of a building or on an entire floor.
e. For preliminary block load estimates, a zone might be defined as the entire building.
The choice of zones affects system operation, the accuracy of your system design and energy analysis calculations, and the effort required to model the system:
1. The Role of Zones in Calculations. HAP calculates loads for each zone separately. It then evaluates how zone thermostats react to these loads, and the subsequent
behavior of air system fans, coils and supply terminals in response to calls for cooling or heating from the zone thermostats. Therefore, zoning has a significant effect
on system performance.
2. How Zone Modeling Affects Accuracy. The most accurate approach is to model one zone per thermostat in your system. This accurately models the system as it is
installed since the program can calculate the cooling and heating demands sensed by each thermostat in the system. However, engineers sometimes combine actual
zones to reduce input effort. When combining zones it is important that only regions with identical or similar patterns of loads be combined. Oversimplifying the system
by combining too many regions or by combining regions with dissimilar load patterns can cause cooling and heating loads to be underestimated. An extreme example
involves combining all rooms on a single floor into one zone. All heat gains and losses on this floor will be mixed to determine the net zone load. At certain times heat
gains from interior rooms will offset heat losses from perimeter zones and cause both cooling and heating loads to be underestimated.
3. How Zone Modeling Affects Modeling Effort. The larger the number of zones the more work will be required to assign spaces, specify thermostat setpoints and
supply terminal equipment. Further, systems with a larger number of zones require more time to calculate than systems with fewer zones. However, the benefit of
careful modeling of zones is greater accuracy in your results. The danger in simplifying the model by combining zones is that accuracy will suffer.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air for Terminal Systems
When "Terminal Units" has been selected as the Equipment Type, the General Tab contains an extra input item that is used to designate how ventilation air is provided
to the terminal units. Users must choose between two options:
1. Direct Ventilation. With this option untempered outdoor ventilation air is introduced directly at the terminal unit. For example a floor-mounted DX fan coil might receive
ventilation air directly through the exterior wall of the building. A ceiling mounted water source heat pump might receive ventilation air directly through a duct
connected to a roof vent.
When this option is selected, the "DOAS Components" tab on the air system form is disabled. Data on this tab is only relevant if a DOAS unit is used. Instead,
ventilation airflow data is specified in the Common Data section of the Zone Components tab.
2. Dedicated Outdoor Air System (DOAS). With this option, unconditioned or preconditioned outdoor ventilation air is provided to terminal units via a centrally located
HVAC unit. Users have the option of cooling and/or heating this ventilation air and can choose to control dry-bulb temperature or dry-bulb and relative humidity. HAP
assumes the ventilation air is ducted to the inlet of each terminal unit in the system.
When this option is selected, the "DOAS Components" tab on the air system properties window is enabled. It contains data describing the outdoor ventilation airflow,
fans, coils and ductwork associated with the DOAS unit.
Note that Induction Beam and Active Chilled Beam systems are required to have a DOAS unit to provide conditioned primary air to the terminals and drive the air
induction process within the terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the System Components tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Components Tab / System Form
About System Components. The System Components tab on the System Form contains information about centrally located components in the system such as fans
and coils, and information about the distribution duct system.
Page 4 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.1 Ventilation Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Ventilation Air Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.1 Ventilation Data ››
The System Components Tab is divided into two panels which occupy the left-hand and right-hand portions of the tab. Features in these two panels are used to enter
system component data.
1. Checklist Panel. The left-hand panel contains a checklist of system-level components which can be included in the system. Components are listed sequentially
starting with outdoor ventilation air and working clockwise through the system circuit, ending with the return fan. A check mark in the box next to each item indicates
whether that component is included in the system. Certain items are required in the system. These items are checked and cannot be unchecked. An example is the
supply fan. Other items are optional and may be included by checking the item, or excluded by unchecking the item. The figure above shows an example for a VAV
system; 11 system components are offered in this type of system.
2. Data Panel. The right-hand panel contains views of data for each component in the system. The data view in this panel changes each time you click on the name of a
system component in the checklist panel. It is important to click only on the name of the item; clicking on the check box for an item displays its data but also includes
or excludes the component.
In the figure above, central cooling data is shown in the right hand panel because the "Central Cooling" item in the checklist panel was the last item clicked on. To
change the display to "Supply Fan" data, you would simply click on the "Supply Fan" item in the checklist panel.
The type of air system being defined determines the system components offered in the checklist panel. In all, seventeen different components can appear in the checklist
of system components:
Outdoor Ventilation Air
Outdoor Air Economizer
Ventilation Reclaim Device
Precool Coil
Cooling Coil for a DOAS Unit
Preheat Coil
Heating Coil for a DOAS Unit
Humidification Controls
Dehumidification Controls
Central Cooling Coil
Central Heating Coil
Supply Fan
Hot Deck Supply Fan
Ventilation Fan
Duct System Data
Return Fan
Exhaust Fan
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains outdoor ventilation air inputs.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Data
Page 5 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Air Data for Proportional Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.1 Ventilation Data ››
The Ventilation Air data view contains information about outdoor ventilation airflow sizing criteria and controls. Nine input items are used to describe ventilation air, but
certain items will be enabled or disabled depending on the type of Airflow Control selected. The four types of airflow control are listed below. For further information on
input items used to define each type of control, click on the desired item below.
1. Proportional Control models the use of uncontrolled or partially controlled ventilation air for variable volume systems. With this control the ventilation airflow rate varies
as the supply airflow varies. Uncontrolled outdoor airflow tends to vary as a constant percentage of supply air. Thus, if the supply fan has throttled to 60% of its design
flow rate, then the outdoor ventilation airflow is at 60% of the design outdoor airflow rate. This control option is offered only for VAV systems
2. Constant Control specifies that outdoor ventilation will be maintained at the design CFM (or L/s) airflow value for all occupied period hours and for unoccupied period
hours when the ventilation dampers are open. For constant volume systems, constant ventilation airflow can be maintained without special controls. For VAV systems,
it is assumed special damper controls or booster fans are used to maintain a constant ventilation airflow rate as the supply airflow varies. If the supply airflow rate in a
VAV system drops below the design ventilation flow rate, the system will operate with 100% outdoor air, but will be below the design ventilation specification.
3. Scheduled Control refers to special equipment and controls used to vary the outdoor ventilation air according to predetermined hourly and daily schedules. When this
option is used, outdoor ventilation air is calculated using the design airflow value and a user-defined schedule.
4. Demand Controlled Ventilation (DCV) models the use of CO2 sensors in each zone to control ventilation air. Since occupants are the primary source of CO2 in most
buildings, measuring CO2 is a means of indirectly measuring the number of occupants present in a zone. Outdoor ventilation air can then be adjusted as CO2 levels
change so the proper ventilation per occupant is maintained, while at the same time minimizing ventilation air and therefore the cooling and heating loads due to
ventilation. With DCV, the user establishes a control profile which relates a zone CO2 levels to ventilation airflow rates. The program performs a CO2 balance
calculation to estimate CO2 levels at all points in the system. The zone CO2 levels and the control profile together determine the amount of ventilation air introduced
into the system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Data for Proportional Control
Proportional Control models the use of uncontrolled or partially controlled ventilation air for variable volume systems. With this control the ventilation airflow rate varies as
the supply airflow varies. Uncontrolled outdoor airflow tends to vary as a constant percentage of supply air. Thus, if the supply fan has throttled to 60% of its design flow
rate, then the outdoor ventilation airflow is at 60% of the design outdoor airflow rate. This control option is only offered only for VAV systems.
When this control is used, five input items are required in addition to "Airflow Control":
1. Ventilation Sizing Method defines the procedure used to calculate the design outdoor ventilation airflow rate for the system. Options which appear in the list include
the following:
a. Sum of Space OA Airflows – This method calculates the design ventilation airflow by summing the space outdoor airflow requirements for all spaces served by the
system. Certain ventilation standards and codes use this approach. This approach is also typically used when the building is not subject to a ventilation standard or
code. This option appears in all cases.
b. ASHRAE Standard 62-2001 – This method calculates required ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard.
When the system serves more than one space the multiple space equation, equation 6-1, is used. For VAV systems the program will calculate ventilation
requirements at two conditions – with all VAV boxes full open, and with all VAV boxes at minimum position – and then choose the larger airflow as the design value
for the system. This option only appears when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the
Preferences option on the View menu.
Page 6 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Air Data for Constant Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.1 Ventilation Data ››
The 2001 Edition of Standard 62 is not specific about how the Standard should be applied to VAV systems. The ASHRAE Standard 62 committee has responded to
a request for interpretation that examining all VAV boxes at minimum position is a valid approach, but that other valid approaches exist as well. Examination of the
boxes full open and boxes at minimum position is a superset of the minimum position approach and is therefore valid as well.
c. ASHRAE Standard 62-2001 (max only) – This option is only offered for VAV systems. It uses the same procedure as the previous item, except that only the
condition with all VAV boxes full open is considered. Because the 2001 edition of Standard 62 is not specific about how the Standard should be applied to VAV
systems (see discussion above), the use of the Standard for VAV systems requires engineering judgment. This option is offered for those who do now feel the
minimum box condition should be considered, and for those who wish to compare sizing data using the max+min and max only scenarios. This option only appears
when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the Preferences option on the View menu.
d. ASHRAE Standard 62.1-2004
e. ASHRAE Standard 62.1-2007
f. ASHRAE Standard 62.1-2010
g. ASHRAE Standard 62.1-2013
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1.
When the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will
appear, depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2013 as the project preference, only 62.1-2013
will appear as an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Note: When using the Standard 62.1 procedure, only ventilation requirements based on CFM/person (L/s/person) and CFM/sqft (L/s/sqm) can be considered. Other
ventilation specifications are out of scope for the standard. Ventilation requirements specified as CFM (L/s) or % of supply air are therefore excluded from the
calculation.
2. Minimum Airflow specifies whether special controls are used to prevent outdoor ventilation airflow from dropping to unacceptably low levels. The minimum airflow
rate is defined as a percentage of the design ventilation airflow.
Example: The minimum is specified as 25% for a system with a design ventilation airflow of 1000 CFM and a supply airflow rate of 5000 CFM. This means the
ventilation airflow rate may not drop below 250 CFM. Without any minimum controls, ventilation airflow would be 200 CFM when the supply airflow rate dropped to
1000 CFM (20% of design). However, because a minimum airflow rate has been specified, the program will assume the necessary equipment and controls are present
to maintain 250 CFM ventilation airflow for this condition.
3. Unoccupied Damper Position. This item specifies whether outdoor air dampers are open during the unoccupied equipment operating period. When the "Open" item
is selected ventilation airflow will be controlled in the same way it is in the occupied period whenever the system runs during unoccupied hours. When the "Closed"
item is selected dampers will be closed and only the specified damper leakage will occur when the system runs during unoccupied hours.
4. Damper Leak Rate defines how much air leaks through dampers when they are closed and the system is running. Leakage is defined as a percentage of the design
outdoor ventilation airflow rate. If dampers are open during the unoccupied period, this input is not used.
5. Outdoor Air CO2 Level defines the average concentration of carbon dioxide in outside air. It is not used in Proportional control calculations. However, the program
performs a CO2 balance calculation for all systems and displays the results on the System Psychrometrics report to allow users to examine CO2 levels in the
occupied zones. The Outdoor Air CO2 Level is required for this calculation and therefore this input is required for all types of ventilation control. 400 parts per million
(ppm) is a rule of thumb default for the outdoor CO2 level. If you do not have actual data for the building site, we recommend using this default.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Data for Constant Control
Constant Control specifies that outdoor ventilation will be maintained at the design CFM (or L/s) airflow value for all occupied period hours and for unoccupied period
hours when the ventilation dampers are open. For constant volume systems, constant ventilation airflow can be maintained without special controls. For VAV systems, it
is assumed special damper controls or booster fans are used to maintain a constant ventilation airflow rate as the supply airflow varies. If the supply airflow rate in a VAV
system drops below the design ventilation flow rate, the system will operate with 100% outdoor air, but will be below the design ventilation specification.
When this control is used, four input items are required in addition to "Airflow Control":
1. Ventilation Sizing Method defines the procedure used to calculate the design outdoor ventilation airflow rate for the system. Options which appear in the list include
the following:
a. Sum of Space OA Airflows – This method calculates the design ventilation airflow by summing the space outdoor airflow requirements for all spaces served by the
system. Certain ventilation standards and codes use this approach. This approach is also typically used when the building is not subject to a ventilation standard or
code. This option appears in all cases.
b. ASHRAE Standard 62-2001 – This method calculates required ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard.
When the system serves more than one space the multiple space equation, equation 6-1, is used. For VAV systems the program will calculate ventilation
requirements at two conditions – with all VAV boxes full open, and with all VAV boxes at minimum position – and then choose the larger airflow as the design value
for the system. This option only appears when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the
Preferences option on the View menu.
The 2001 Edition of Standard 62 is not specific about how the Standard should be applied to VAV systems. The ASHRAE Standard 62 committee has responded to
a request for interpretation that examining all VAV boxes at minimum position is a valid approach, but that other valid approaches exist as well. Examination of the
boxes full open and boxes at minimum position is a superset of the minimum position approach and is therefore valid as well.
c. ASHRAE Standard 62-2001 (max only) – This option is only offered for VAV systems. It uses the same procedure as the previous item, except that only the
condition with all VAV boxes full open is considered. Because the 2001 edition of Standard 62 is not specific about how the Standard should be applied to VAV
Page 7 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Air Data for Scheduled Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.1 Ventilation Data ››
systems (see discussion above), the use of the Standard for VAV systems requires engineering judgment. This option is offered for those who do now feel the
minimum box condition should be considered, and for those who wish to compare sizing data using the max+min and max only scenarios. This option only appears
when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the Preferences option on the View menu.
d. ASHRAE Standard 62.1-2004
e. ASHRAE Standard 62.1-2007
f. ASHRAE Standard 62.1-2010
g. ASHRAE Standard 62.1-2013
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1.
When the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will
appear, depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2013 as the project preference, only 62.1-2013
will appear as an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Note: When using the Standard 62.1 procedure, only ventilation requirements based on CFM/person (L/s/person) and CFM/sqft (L/s/sqm) can be considered. Other
ventilation specifications are out of scope for the standard. Ventilation requirements specified as CFM (L/s) or % of supply air are therefore excluded from the
calculation.
2. Unoccupied Damper Position. This item specifies whether outdoor air dampers are open during the unoccupied equipment operating period. When the "Open" item
is selected ventilation airflow will be controlled in the same way it is in the occupied period whenever the system runs during unoccupied hours. When the "Closed"
item is selected dampers will be closed and only the specified damper leakage will occur when the system runs during unoccupied hours.
3. Damper Leak Rate defines how much air leaks through dampers when they are closed and the system is running. Leakage is defined as a percentage of the design
outdoor ventilation airflow rate. If dampers are open during the unoccupied period, this input is not used.
4. Outdoor Air CO2 Level defines the average concentration of carbon dioxide in outside air. It is not used in Constant control calculations. However, the program
performs a CO2 balance calculation for all systems and displays the results on the System Psychrometrics report to allow users to examine CO2 levels in the
occupied zones. The Outdoor Air CO2 Level is required for this calculation and therefore this input is required for all types of ventilation control. 400 parts per million
(ppm) is a rule of thumb default for the outdoor CO2 level. If you do not have actual data for the building site, we recommend using this default.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Data for Scheduled Control
Scheduled Control refers to special equipment and controls used to vary the outdoor ventilation air according to predetermined hourly and daily schedules. When this
option is used, outdoor ventilation air is calculated using the design airflow value and a user-defined schedule.
When this control is selected, three input items are required in addition to "Airflow Control":
1. Ventilation Sizing Method defines the procedure used to calculate the design outdoor ventilation airflow rate for the system. Options which appear in the list include
the following:
a. Sum of Space OA Airflows – This method calculates the design ventilation airflow by summing the space outdoor airflow requirements for all spaces served by the
system. Certain ventilation standards and codes use this approach. This approach is also typically used when the building is not subject to a ventilation standard or
code. This option appears in all cases.
b. ASHRAE Standard 62-2001 – This method calculates required ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard.
When the system serves more than one space the multiple space equation, equation 6-1, is used. For VAV systems the program will calculate ventilation
requirements at two conditions – with all VAV boxes full open, and with all VAV boxes at minimum position – and then choose the larger airflow as the design value
for the system. This option only appears when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the
Preferences option on the View menu.
The 2001 Edition of Standard 62 is not specific about how the Standard should be applied to VAV systems. The ASHRAE Standard 62 committee has responded to
a request for interpretation that examining all VAV boxes at minimum position is a valid approach, but that other valid approaches exist as well. Examination of the
boxes full open and boxes at minimum position is a superset of the minimum position approach and is therefore valid as well.
c. ASHRAE Standard 62-2001 (max only) – This option is only offered for VAV systems. It uses the same procedure as the previous item, except that only the
condition with all VAV boxes full open is considered. Because the 2001 edition of Standard 62 is not specific about how the Standard should be applied to VAV
systems (see discussion above), the use of the Standard for VAV systems requires engineering judgment. This option is offered for those who do now feel the
minimum box condition should be considered, and for those who wish to compare sizing data using the max+min and max only scenarios. This option only appears
when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the Preferences option on the View menu.
d. ASHRAE Standard 62.1-2004
e. ASHRAE Standard 62.1-2007
f. ASHRAE Standard 62.1-2010
g. ASHRAE Standard 62.1-2013
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1.
When the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will
appear, depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2013 as the project preference, only 62.1-2013
will appear as an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Page 8 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Air Data for DCV Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.1 Ventilation Data ››
Note: When using the Standard 62.1 procedure, only ventilation requirements based on CFM/person (L/s/person) and CFM/sqft (L/s/sqm) can be considered. Other
ventilation specifications are out of scope for the standard. Ventilation requirements specified as CFM (L/s) or % of supply air are therefore excluded from the
calculation.
2. Schedule defines how outdoor ventilation airflow varies on an hourly and a daily basis. The ventilation schedule can be defined in two ways:
a. Creating a New Schedule. If you have not yet created a ventilation schedule, choose the "create new schedule" item in the schedule drop-down list. The Schedule
Form will appear and will allow you to define profiles for the hourly and daily variation of ventilation airflow. Be sure to specify that the type of schedule is
"fractional". This type of schedule contains values defining the percentage of maximum airflow present for each hour. When you press the OK button to exit from the
Schedule Form, your schedule data will be stored and the schedule will be assigned to ventilation for the current system automatically.
b. Selecting an Existing Schedule. If you previously created and stored schedules in your project database, you can simply select the desired schedule from the
drop-down list.
In addition, you can modify schedule data directly from the System Form by pressing the Schedule button to the left of the drop-down list. When you press this button,
the Schedule Form will appear and will display inputs for the currently selected schedule. After modifying the schedule data, press the OK button to return to the
System Form.
3. Damper Leak Rate specifies air leakage through the dampers as a percentage of the design ventilation airflow rate. Damper leakage is only calculated for hours when
the ventilation schedule specifies airflow as 0% of design. Note that the "Unoccupied Damper Position" item is not enabled for this airflow control since the ventilation
schedule is used to specify times when the dampers are open (airflow schedule value > 0%) and closed (airflow schedule value = 0%).
4. Outdoor Air CO2 Level defines the average concentration of carbon dioxide in outside air. It is not used in Constant control calculations. However, the program
performs a CO2 balance calculation for all systems and displays the results on the System Psychrometrics report to allow users to examine CO2 levels in the
occupied zones. The Outdoor Air CO2 Level is required for this calculation and therefore this input is required for all types of ventilation control. 400 parts per million
(ppm) is a rule of thumb default for the outdoor CO2 level. If you do not have actual data for the building site, we recommend using this default.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Air Data for DCV Control
The Demand Controlled Ventilation option models the use of CO2 sensors in each zone to control ventilation air. Since occupants are the primary source of CO2 in most
buildings, measuring CO2 is a means of indirectly measuring the number of occupants present in a zone. Outdoor ventilation air can then be adjusted as CO2 levels
change so the proper ventilation per occupant is maintained, while at the same time minimizing ventilation air and therefore the cooling and heating loads due to
ventilation. With DCV, the user establishes a control profile which relates a zone CO2 levels to ventilation airflow rates. The program performs a CO2 balance calculation
to estimate CO2 levels at all points in the system. The zone CO2 levels and the control profile together determine the amount of ventilation air introduced into the system.
When this control is selected, seven input items are required in addition to "Airflow Control":
1. Ventilation Sizing Method defines the procedure used to calculate the design outdoor ventilation airflow rate for the system. Options which appear in the list include
the following:
a. Sum of Space OA Airflows – This method calculates the design ventilation airflow by summing the space outdoor airflow requirements for all spaces served by the
system. Certain ventilation standards and codes use this approach. This approach is also typically used when the building is not subject to a ventilation standard or
code. This option appears in all cases.
b. ASHRAE Standard 62-2001 – This method calculates required ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard.
When the system serves more than one space the multiple space equation, equation 6-1, is used. For VAV systems the program will calculate ventilation
requirements at two conditions – with all VAV boxes full open, and with all VAV boxes at minimum position – and then choose the larger airflow as the design value
for the system. This option only appears when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the
Preferences option on the View menu.
The 2001 Edition of Standard 62 is not specific about how the Standard should be applied to VAV systems. The ASHRAE Standard 62 committee has responded to
a request for interpretation that examining all VAV boxes at minimum position is a valid approach, but that other valid approaches exist as well. Examination of the
boxes full open and boxes at minimum position is a superset of the minimum position approach and is therefore valid as well.
c. ASHRAE Standard 62-2001 (max only) – This option is only offered for VAV systems. It uses the same procedure as the previous item, except that only the
condition with all VAV boxes full open is considered. Because the 2001 edition of Standard 62 is not specific about how the Standard should be applied to VAV
systems (see discussion above), the use of the Standard for VAV systems requires engineering judgment. This option is offered for those who do now feel the
minimum box condition should be considered, and for those who wish to compare sizing data using the max+min and max only scenarios. This option only appears
when Standard 62-2001 is chosen as the basis for ventilation defaults for your project. This choice can be changed via the Preferences option on the View menu.
d. ASHRAE Standard 62.1-2004
e. ASHRAE Standard 62.1-2007
f. ASHRAE Standard 62.1-2010
g. ASHRAE Standard 62.1-2013
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1.
When the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will
appear, depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2013 as the project preference, only 62.1-2013
will appear as an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Page 9 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.2 Economizer Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Outdoor Air Economizer Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.2 Economizer Data ››
Note: When using the Standard 62.1 procedure, only ventilation requirements based on CFM/person (L/s/person) and CFM/sqft (L/s/sqm) can be considered. Other
ventilation specifications are out of scope for the standard. Ventilation requirements specified as CFM (L/s) or % of supply air are therefore excluded from the
calculation.
2. Base Ventilation Rate defines the minimum ventilation airflow rate for DCV control as a percentage of the design airflow rate. The base ventilation rate accounts for
non-occupant sources of pollutants such as those from materials, carpeting or furnishing. It typically ranges from 15% to 50% depending on the application. Common
rule of thumb values are in the 20% to 30% range.
3. Damper Leak Rate specifies air leakage through the dampers as a percentage of the design ventilation airflow rate.
4. Minimum CO2 Differential is the first of two control settings for DCV control. It defines the CO2 differential corresponding to use of the base ventilation rate. The
differential is the difference between indoor CO2 and outdoor CO2 levels.
Example: Suppose the outdoor CO2 level is 400 ppm and the minimum CO2 differential is 100 ppm. Therefore, when the indoor CO2 level is 500 ppm and lower, the
control will position outdoor dampers to use the base ventilation rate. Above 500 ppm, the control will adjust outdoor ventilation airflow as a linear function of zone
CO2 level. This is shown in the sample DCV control profile below.
5. Maximum CO2 Differential is the second of two control settings for DCV control. It defines the CO2 differential corresponding to use of the design ventilation rate.
Example: Suppose the outdoor CO2 level is 400 ppm and the maximum CO2 differential is 700 ppm. Therefore, when the indoor CO2 level is 1100 ppm and higher,
the control will position outdoor dampers to use the design ventilation rate. Below 1100 ppm, the control will adjust outdoor ventilation airflow as a linear function of
CO2 level. This is shown in the sample DCV control profile below.
6. Outdoor Air CO2 Level defines the average concentration of carbon dioxide in outside air. As described above, it is used with the maximum and minimum CO2
differentials to determine key control points for the DCV control profile. It is also used in calculating the CO2 levels in zones served by the system since outdoor
ventilation air and infiltration air affect indoor CO2 levels. 400 parts per million (ppm) is a rule of thumb default for the outdoor CO2 level. If you do not have actual data
for the building site, we recommend using this default.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains outdoor air economizer input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Outdoor Air Economizer Data
Page 10 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.3 Ventilation Reclaim Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Ventilation Reclaim Device Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.3 Ventilation Reclaim Data ››
The Economizer data view contains information about an outdoor air economizer used with the system. An economizer is used to vary the flow of outdoor air into the
system to reduce or eliminate the need for mechanical cooling. Items in this data view are as follows:
1. Control defines the type of control used. Three options are offered:
a. Integrated Enthalpy - The economizer control is activated when the enthalpy of return air is greater than the enthalpy of outdoor air. Economizer dampers are
modulated to introduce sufficient outdoor air to eliminate the need for mechanical cooling, or 100% outdoor air if mechanical cooling cannot be completely
eliminated.
b. Integrated Dry-Bulb - The economizer control is activated when the return air dry-bulb temperature is greater than the outdoor air dry-bulb temperature.
Economizer dampers are modulated to introduce sufficient outdoor air to eliminate the need for mechanical cooling, or 100% outdoor air if mechanical cooling
cannot be completely eliminated.
c. Non-Integrated Dry-Bulb - The economizer control is activated when the outdoor air temperature falls below the cooling coil outlet temperature. Economizer
dampers are modulated to introduce sufficient outdoor air to eliminate the need for mechanical cooling. Because this control does not activate until the outdoor air
temperature is below the coil outlet temperature, it always achieves 100% free cooling, but misses the opportunity for partial free cooling provided by the integrated
controls.
2. Upper Cutoff, Lower Cutoff. In some situations, economizer operation is only permitted between specific outdoor air temperatures referred to here as "cutoff"
temperatures. If operation is limited, specify the upper cutoff temperature above which economizer operation is not permitted, and the lower cutoff temperature below
which operation is not allowed. If no limitations are imposed, set the cutoff temperatures to extreme values (e.g., 150 F upper, -50 F lower) so economizer operation
will be available at all times.
Example: An integrated enthalpy economizer is used in a hot, dry climate. In such an application there is a danger the economizer control could be activated in
adverse conditions. For example, when the outdoor air enthalpy is slightly less than the return air enthalpy, it is possible the outdoor air dry-bulb temperature is
warmer than the return air temperature. Therefore, using the economizer would tend to reduce or eliminate latent cooling coil loads, but could increase the sensible
cooling coil load. To minimize such situations, an upper cutoff temperature of 70 F might be used. This cutoff means that the economizer will never activate when the
outdoor dry-bulb temperature is above 70 F, even if the return air enthalpy is greater than the outdoor air enthalpy.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains air-to-air ventilation heat recovery input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Reclaim Device Data
Page 11 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.4 Precool Coil Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Precool Coil Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.4 Precool Coil Data ››
The Ventilation Reclaim data view contains information about a ventilation heat reclaim device used with the system. A ventilation reclaim device transfers heat between
the outdoor ventilation and exhaust air streams in order to reduce loads on air system cooling and heating coils. Examples of ventilation reclaim devices include:
a. Air-to-air heat exchangers.
b. Heat pipes.
c. Heat wheels.
d. Desiccant wheels.
e. Pump around systems.
Example: During cold winter weather, the ventilation reclaim unit transfers heat from warm exhaust air to cold outdoor ventilation air. This increases the temperature of air
entering heating coil and reduces the heating coil load.
Items in this data view are as follows:
1. Reclaim defines whether the device reclaims sensible heat only or both sensible and latent heat. The "Sensible Heat" option should be used for devices such as air-
to-air heat exchangers, which transfer only sensible heat between outdoor and exhaust air streams. The "Sensible & Latent Heat" option is used for devices such as
desiccant wheels which transfer both sensible heat and moisture between air streams.
2. Thermal Efficiency specifies the fraction of the total possible heat transfer which occurs using the ventilation reclaim device. Thermal efficiency for sensible heat
transfer devices is often referred to by the alternate term "heat exchanger effectiveness". Values for sensible units typically range between 50% and 80%. Note that
when the reclaim device provides both sensible and latent heat transfer, the thermal efficiency is used to calculate both heat and moisture transfer.
Example: At the winter design condition, exhaust air is at 75 F and the outdoor ventilation air temperature is 0 F. The ventilation reclaim device warms ventilation air
from 0 F to 45 F. Therefore, the thermal efficiency is 60%. Thermal efficiency is (actual heat reclaim) / (total possible heat reclaim), or (45 - 0) / (75 - 0). Total possible
heat reclaim would warm outdoor ventilation air to the temperature of exhaust air, or 75 F.
3. Input kW defines the input power required to drive the reclaim device. The program assumes the ventilation reclaim device draws this power for all hours during which
it operates. Application examples:
a. To-Air Heat Exchanger: No power use.
b. Heat Pipe: No power use.
c. Heat Wheel: Power required to operate wheel motor.
d. Desiccant Wheel: Power required to operate wheel motor and any electric power supplied to regeneration heating coils.
e. Pump-Around System: Input power for pump.
4. Schedule specifies the months of the year in which the reclaim device operates. The schedule is comprised of a series of twelve buttons, one for each month. To turn
reclaim on for a month, the month’s button must be in a down position. In the figure above the reclaim device is scheduled to operate from January through May and
October through December; it is off in the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains precool coil input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Precool Coil Data
Page 12 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.5 Cooling Coil Data for a DOAS Unit
11.0 Entering Systems ›› 11.3 System Components Data ››
Cooling Coil Data for a DOAS Unit
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.5 Cooling Coil Data for a DOAS Unit ››
The Precool Coil data view contains information about a supplemental cooling coil positioned upstream of the main cooling coil. In warm, humid climates where large
amounts of moisture must be removed from outdoor ventilation air, this moisture must sometimes be condensed in two stages. The precool coil serves as the first stage
of cooling and moisture removal. The main cooling coil serves as the second stage. Items in this data view are as follows:
1. Setpoint specifies the cooling setpoint used to control the coil. HAP assumes the coil is controlled by a thermostat located in the air stream immediately downstream
of the precool coil. For example, if the setpoint is 60 F, the precool coil will operate whenever the entering air is warmer than 60 F and will cool the air to 60 F. When
analyzing coil operation the program calculates both sensible and latent coil loads.
2. Coil Bypass Factor is used to evaluate dehumidification occurring at the cooling coil. In general, the bypass factor is a measure of the approach to the apparatus dew
point (ADP) for air flowing through the coil. The smaller the bypass factor, the closer the outlet air approaches the ADP state.
The coil bypass factor can be obtained from product literature when modeling specific equipment. In most system design applications, however, the HVAC equipment
has not yet been selected. In such a situation, specify a bypass factor that is generally representative of the type of equipment you intend to select.
3. Cooling Source defines how cooling is provided to the precool coil. Choices are restricted based on the equipment classification for the current system.
4. Schedule specifies the months of the year in which the precool coil operates. The schedule is comprised of a series of twelve buttons, one for each month. To turn the
coil on for a month, the month’s button must be in a down position. In the figure above the coil is scheduled to operate from April through October; it is off for the
remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses chilled water cooling and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
5. Coil Position. This item specifies the location of the precool coil. The coil can be in the outdoor ventilation air stream upstream of the point where outdoor air mixes
with return air, or it can be downstream of this mixing point. The position of the coil will influence the precool coil entering air temperature and humidity, and therefore
will determine when the coil operates and how much sensible and latent cooling it must produce.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for cooling coils used in a DOAS AHU.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Data for a DOAS Unit
Page 13 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.6 Preheat Coil Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Preheat Coil Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.6 Preheat Coil Data ››
The Cooling Coil data view contains information about a cooling coil located in a Dedicated Outdoor Air System (DOAS) used in a terminal system such as fan coils,
water source heat pumps, VRF, induction beams, or active chilled beams, or in a standalone Make Up Air Unit (MAU). This cooling coil is used to condition outdoor
ventilation before it is introduced into the building. Items in this data view are as follows:
1. Setpoint specifies the cooling setpoint used to control the coil. HAP assumes the coil is controlled by a duct thermostat located in the discharge air downstream of the
DOAS unit. For example, if the setpoint is 75 F, the cooling coil will operate to keep the discharge duct temperature downstream of the unit at 75 F.
For Induction Beam and Active Chilled Beam systems two different setpoints are specified, one for occupied hours in the fan/thermostat schedule and one for
unoccupied hours. Because these systems require the DOAS unit to operate to power the induction terminals, the discharge setpoint is sometimes reset to a warmer
temperature in the unoccupied hours as an energy saving strategy.
2. Coil Bypass Factor is used to evaluate dehumidification occurring at the cooling coil. In general, the bypass factor is a measure of the approach to the apparatus dew
point (ADP) for air flowing through the coil. The smaller the bypass factor, the closer the outlet air approaches the ADP state.
The coil bypass factor can be obtained from product literature when modeling specific equipment. In most system design applications, however, the HVAC equipment
has not yet been selected. In such a situation, specify a bypass factor that is generally representative of the type of equipment you intend to select.
3. Cooling Source defines how cooling is provided to the coil. Choices are restricted based on the equipment and system types for the current system.
4. Schedule specifies the months of the year in which the cooling coil operates. The schedule is comprised of a series of twelve buttons, one for each month. To turn the
coil on for a month, the month’s button must be in a down position. In the figure above the coil is scheduled to operate from April through October.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses chilled water cooling and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for preheat coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Preheat Coil Data
Page 14 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.7 Heating Coil Data for a DOAS Unit
11.0 Entering Systems ›› 11.3 System Components Data ››
Heating Coil Data for a DOAS Unit
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.7 Heating Coil Data for a DOAS Unit ››
The Preheat Coil data view contains information about a supplemental heating coil positioned upstream of the main coils. In climates with cold winter weather, this extra
heating coil is often used to prevent coil freezing, condensation on ductwork and cold drafts in the zones. Items in this data view are as follows:
1. Setpoint specifies the heating setpoint used to control the coil. HAP assumes the coil is controlled by a thermostat located in the air stream immediately downstream
of the preheat coil. For example, if the setpoint is 50 F, the preheat coil will operate whenever the entering air is colder than 50 F and will heat the air to 50 F
2. Heating Source defines how heat is provided to the preheat coil. Choices are electric resistance, natural gas combustion, fuel oil combustion, propane combustion,
hot water and steam. When the Undefined equipment type is used, the heating source will default to "Any".
3. Schedule specifies the months of the year in which the preheat coil operates. The schedule is comprised of a series of twelve buttons, one for each month. To turn the
coil on for a month, the month’s button must be in a down position. In the figure above the coil is scheduled to operate from January through April and November
through December; it is off for the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this
monthly schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12
months. If you specify OFF months the schedule will be used in combination with the temperature threshold control.
4. Coil Position. This item specifies the location of the preheat coil. The coil can be in the outdoor ventilation air stream upstream of the point where outdoor air mixes
with return air, or it can be downstream of this mixing point. The position of the coil will influence the precool coil entering air temperature, and therefore will determine
when the coil operates and how much heat it must produce.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for heating coils used in a DOAS AHU.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Data for a DOAS Unit
Page 15 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.8 Humidification Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Humidification Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.8 Humidification Data ››
The Heating Coil data view contains information about a heating coil located in a Dedicated Outdoor Air System (DOAS) used in a terminal system such as fan coils,
water source heat pumps, VRF, induction beams, or active chilled beams, or in a standalone Make Up Air Unit (MAU). This heating coil is used to condition outdoor
ventilation before it is introduced into the building. Items in this data view are as follows:
1. Setpoint specifies the heating setpoint used to control the coil. HAP assumes the coil is controlled by a discharge duct thermostat located downstream of the DOAS
unit. For example, if the setpoint is 70 F, the preheat coil will operate to keep the duct temperature downstream of the unit at 70 F.
For Induction Beam and Active Chilled Beam systems two different setpoints are specified, one for occupied hours in the fan/thermostat schedule and one for
unoccupied hours. Because these systems require the DOAS unit to operate to power the induction terminals, the discharge setpoint is sometimes reset to a warmer
temperature in the unoccupied hours as an energy saving strategy.
2. Heating Source defines how heat is provided to the preheat coil. Standard choices are electric resistance, natural gas combustion, fuel oil combustion, propane
combustion, hot water and steam. When modeling a dedicated outdoor air system (DOAS) unit used with water source heat pump terminals, a "water source heat
pump" option is also offered.
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this
monthly schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12
months. If you specify OFF months the schedule will be used in combination with the temperature threshold control.
3. Schedule specifies the months of the year in which the heating coil operates. The schedule consists of a series of twelve buttons, one for each month. To turn the coil
on for a month, the month’s button must be in a down position. In the figure above the coil is scheduled to operate from January through May and September through
December; it is off in the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains humidification input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Humidification Data
Page 16 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.9 Dehumidification Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Dehumidification Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.9 Dehumidification Data ››
The Humidification data view contains information about the humidification controls and equipment in the system.
Note that humidification control operates differently in central systems and Dedicated Outdoor Air Systems (DOAS) or Make Up Air (MUA) systems. In a central system,
such as VAV or CAV, a humidistat in the return air stream works together with a humidifier in the main air handling unit to maintain zones at the specified relative
humidity. In an DOAS or MUA system a humidistat in the discharge duct of the unit works with a humidifier to maintain the unit's discharge air at the specified relative
humidity.
1. Minimum RH Setpoint defines the minimum relative humidity level maintained by the control.
In a central system, for example, if the setpoint is 30%, the humidifier will add moisture to the supply air stream when necessary to prevent the return air humidity from
falling below 30%. If the return air RH is above 30%, the control takes no action and allows the humidity to float.
In an MUA or DOAS system, if the setpoint is 30%, the humidifier will add moisture to the air stream when necessary to prevent the discharge air from the unit from
falling below 30%. If the discharge air humidity is above 30%, the control takes no action and allows the humidity to float.
2. Humidifier Type describes the equipment used to humidify the supply air. Six humidifier types are offered:
a. Self-Contained Steam: Electric - An electric resistance heating element heats water in a reservoir to produce steam which is injected into the supply air stream.
b. Self-Contained Steam: Natural Gas - A gas-fired heat exchanger heats water in a reservoir to produce steam which is injected into the supply air stream.
c. Self-Contained Steam: Propane A propane-fired heat exchanger heats water in a reservoir to produce steam which is injected into the supply air stream.
d. Direct Steam Injection - Clean steam obtained directly from the central steam boiler is injected into the supply air stream.
e. Heated Pan: Steam HX - Steam obtained from the central steam boiler flows through a heat exchanger immersed in a water reservoir to produce clean steam
which is injected into the supply air stream.
f. Heated Pan: Hot Water HX - Hot water obtained from the central boiler plant flows through a heat exchanger immersed in a water reservoir to produce clean steam
which is injected into the supply air stream.
For system design purposes, the choice of a humidifier type will affect the calculation of design heating loads for a boiler plant. When an air system uses a "Direct
Steam Injection" or a "Heated Pan: Steam HX" humidifier, humidification loads will be included when sizing a steam boiler which serves the system. When an air
system uses a "Heated Pan: Hot Water HX" humidifier, humidification loads will be included when sizing a hot water boiler which serves the system.
For energy analysis purposes, the choice of a humidifier type determines the energy source for the humidifier and therefore has an effect on energy consumption
calculations for the system. For example, "Self-Contained:Electric" humidifiers add to the electrical energy consumption of the building. "Heated Pan:Steam HX"
humidifiers add to the hourly loads of central steam boilers.
3. Input Power defines the power the humidifier requires to produce one lb or kg of steam each hour. It is only applicable for self-contained humidifier types. Further, it
will only affect energy simulation results. Given hourly humidification loads, the input energy for the humidifier can be determined using this power/lb or power/kg
value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains dehumidification control input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Dehumidification Data
Page 17 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.10 Central Cooling Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Central Cooling Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
The Dehumidification component contains information about active dehumidification controls. Note that dehumidification control works differently in central systems,
such as VAV or CAV, and in Make Up Air (MUA) or Dedicated Outdoor Air Systems (DOAS).
Central Systems. In central systems such as VAV or CAV dehumidification control uses a humidistat in the return air stream. The humidistat works with the central
cooling coil and a central reheat coil to maintain zones at or below a specified relative humidity. This data view only contains one or two items:
1. Maximum RH Setpoint specifies the maximum relative humidity maintained by the control. For example, if the setpoint is 60%, the cooling coil will remove extra
moisture from the supply air stream when necessary to keep the return air humidity from rising above 60%. A central reheat coil also operates to prevent overcooling
of zones served by the system. If the return air humidity is below 60%, the control takes no action and allows the humidity to float.
2. Heating Source only appears when a central heating coil has not been explicitly added to the system. Selection of dehumidification control automatically adds a
central reheat coil. Heating Source defines the type of reheat used with the dehumidification control. Note that when the system does contain a central heating coil for
space heating duty, this coil is used for both space heating duty and dehumidification reheat duty. Therefore, in this case the Heating Source input does not appear. It
instead appears in the Central Heating data view.
MUA or DOAS Systems. In these systems dehumidification control uses a humidistat located in the discharge duct of the unit. The humidistat works with the cooling coil
and dehumidification rehert coil in the unit to maintain discharge air at or below the specified relative humidity. One or two items appear in this data view:
1. Maximum RH Setpoint specifies the discharge air maximum relative humidity maintained by the control. For example, if the setpoint is 60%, the cooling coil will
remove extra moisture from the air stream whenever necessary to keep the unit discharge air from rising above 60%. The heating coil in the unit operates to provide
reheat when necessary to keep the discharge air temperature at the specified dry-bulb setpoint temperature. If the discharge humidity is below 60%, the control takes
no action and allows the humidity to float.
2. Heating Source only appears when a heating coil has not been explicitly added to the system. When dehumidification control is selected the program automatically
adds a coil for reheat duty. The Heating Source defines the type of reheat used with the dehumidification control. Note that when the system does have a heating coil
in the unit, this coil is used for both heating duty and dehumidification reheat duty. Therefore, in this case the Heating Source input does not appear. It instead appears
in the Heating Coil data view.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for central cooling coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Central Cooling Data
Page 18 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Cooling Supply Air Sizing Criteria
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Cooling Coil Bypass Factor
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
The Central Cooling data view contains information about the central cooling coil and related control and sizing characteristics. The content of this data view changes
depending on the equipment and system type which have been selected. Items in this data view are as follows:
Supply Air Sizing Criteria
Coil Bypass Factor
Cooling Source
Cooling Schedule
Capacity Control
Maximum Supply Temperature
Outdoor Air Temperature for Minimum Supply Temperature
Outdoor Air Temperature for Maximum Supply Temperature
Ventilation Sizing Method (4-Pipe Induction Systems Only)
Bypass Airflow (VVT Systems Only)
Changeover Time (VVT Systems Only)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Supply Air Sizing Criteria
This item defines the sizing criteria for cooling supply air. This sizing criteria is defined differently depending on the current system type:
1. Single Duct CAV Systems: Sizing criteria can be specified in the three ways listed below. To enter a sizing criteria, first choose the units of measure in the drop-down
list and then enter the sizing specification.
a. Supply Temperature - Specify the design supply air temperature (SAT) delivered to zone supply terminals. Cooling supply airflow will be calculated based on this
SAT. In systems which maintain a constant supply temperature, your input also designates this constant SAT. In systems which reset supply temperature, your
value defines the minimum cooling supply temperature.
Note that when duct heat gain is considered the temperature of air leaving the central air handling unit must be colder than your specified SAT. Air will be warmed
to the specified SAT by the time it reaches zone supply terminals. When duct heat gain is not considered, the temperature of air leaving the air handling unit and the
temperature at the supply terminal will be equal.
b. Supply CFM or L/s - Specify the airflow rate delivered by the supply fan. This airflow will be divided among zones in a multiple-zone system based on the ratio of
peak zone sensible loads. This airflow is also used to determine the design supply air temperature for the system.
Note that when duct leakage is considered, the quantity of air reaching zone supply terminals will be less than the supply airflow you specify at the fan. Therefore,
your supply airflow input must include allowance for leakage. When leakage is not modeled, the supply airflow at the fan and the zone terminals will be equal.
c. Supply CFM/sqft or L/s/sqm - Specify the airflow rate delivered by the supply fan in terms of airflow per unit floor area. HAP will calculate the total system airflow
by multiplying the CFM/sqft or L/s/sqm by the total floor area in zones served by the system. Zone airflow rates will be determined based on the floor area for each
zone.
As before, when duct leakage is considered, the quantity of air reaching zone supply terminals will be less than the supply airflow you specify at the fan. Therefore,
your supply airflow input must include allowance for leakage. When leakage is not modeled, the supply airflow at the fan and the zone terminals will be equal.
2. CAV Dual Duct, 2-Deck Multizone and 3-Deck Multizone Systems: The cold deck supply temperature must be provided as the sizing criteria. This is the
temperature of cold deck air supplied to the zone supply terminal for the design condition.
3. VAV Systems: The design supply air temperature must be provided as the sizing criteria. This is temperature of air delivered to the zone supply terminal at the design
condition.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 19 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Cooling Coil Source
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Cooling Coil Schedule
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Cooling Coil Capacity Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Cooling Coil Bypass Factor
The Coil Bypass Factor is used to evaluate dehumidification occurring at the cooling coil. In general, the bypass factor is a measure of the approach to the apparatus
dew point (ADP) for air flowing through the coil. The smaller the bypass factor, the closer the outlet air approaches the ADP state.
The coil bypass factor can be obtained from product literature when modeling specific equipment. In most system design applications, however, the HVAC equipment
has not yet been selected. In such a situation, specify a bypass factor that is generally representative of the type of equipment you intend to select (e.g., small, medium
or large rooftop units, central station air handlers of a particular type, etc…).
Note that when a system contains a precool coil or a terminal cooling coil (for induction systems), this bypass factor is also used to perform calculations for each of these
additional cooling coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Source
This item defines how cooling is provided to the coil. Choices are restricted based on the equipment classification for the current system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Schedule
The cooling coil schedule specifies the months of the year in which the cooling coil operates. The schedule is comprised of a series of twelve buttons, one for each
month. To turn the coil on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from May through October; it is
off from November through April.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses chilled water cooling and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Coil Capacity Control
Capacity Control defines how the output of the cooling coil is controlled. Items offered in this drop down list change depending on system type. The full set of control
types is briefly discussed below.
1. Constant Temperature, Fan Cycled - The supply fan is cycled on and off to modulate cooling provided to the zone. While the supply fan is cycled on, air is delivered
to zone terminal at the design supply air temperature. This control option is only offered for Chilled Water AHU CAV Single Zone systems.
2. Constant Temperature, Fan On - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. Air is delivered to zone
terminals at the design supply air temperature. Because this control provides maximum cooling at all times, conditioning provided to zones in the system must be
modulated either by varying the supply airflow, as is done in VAV systems, or by some form of reheat, as is done in CAV Terminal Reheat, Dual Duct and Multizone
systems.
3. Cycled or Staged Capacity, Fan On - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. In a DX unit,
compressors cycle or unload to modulate the cooling provided to zones in the system. In a chilled water unit, water flow or water temperature is modulated to control
cooling coil capacity.
4. Temperature Reset by Greatest Zone Demand - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. The supply
air temperature is reset according to the greatest sensible cooling load among zones served by the system. When this control is selected, you must also specify the
maximum cooling supply temperature allowed. The control algorithm will not reset the supply temperature above this level.
From a control perspective, demand-based reset is achieved in different ways depending on system type. For CAV Terminal Reheat systems, supply temperature is
reset such that one or more terminal reheat coils are off. In CAV Dual Duct and Multizone systems, cold deck supply temperature is reset such that one or more zones
use 100% cold deck air. In VAV systems, supply temperature is reset such that one or more VAV boxes are fully open.
5. Temperature Reset by Outdoor Air Schedule - Supply air temperature (SAT) is reset according to an outdoor air temperature schedule. When this control is used,
the minimum and maximum SATs are defined along with the corresponding outdoor air temperatures (OAT). The minimum SAT is always the design value. The
remaining SAT and OAT values are defined by the user.
Example: The design SAT is 57 F and the maximum SAT is 67 F. The design SAT is used when the OAT is 95 F and warmer. The maximum SAT is used with the
OAT is 50 F and colder. Between 95 F and 50 F, SAT varies as a linear function of outdoor temperature. This control schedule is shown in the figure below. Inputs for
this control scheme would be:
Design supply temperature = 57 F
Maximum supply temperature = 67 F
OAT for minimum supply temperature = 95 F
OAT for maximum supply temperature = 50 F
Page 20 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Ventilation Sizing Method for 4PIND
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Bypass Airflow
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Changeover Time
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.10 Central Cooling Data ››
Supply Temperature Reset by Outdoor Air Schedule
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Ventilation Sizing Method for 4PIND
Ventilation Sizing Method defines the procedure used to calculate the design outdoor ventilation airflow rate for the system. Since primary air in a 4-pipe induction
system is 100% outdoor air, the ventilation sizing calculation also determines the primary supply airflow for each zone. Two sizing method options are offered:
1. Sum of Space OA Airflows – This method calculates the design ventilation airflow by summing the outdoor airflow requirements for all spaces in a zone to determine
the primary zone airflow rate. The system primary flow rate is the sum of zone airflows. Ventilation airflow equals primary supply airflow.
2. ASHRAE Standard 62-2001 – This method calculates design ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard.
3. ASHRAE Standard 62.1-2004
4. ASHRAE Standard 62.1-2007
5. ASHRAE Standard 62.1-2010
6. ASHRAE Standard 62.1-2013
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1. When
the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will appear,
depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2013 as the project preference, only 62.1-2013 will appear as
an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Note: When using the Standard 62.1 procedure, only ventilation requirements based on CFM/person (L/s/person) and CFM/sqft (L/s/sqm) can be considered. Other
ventilation specifications are out of scope for the standard. Ventilation requirements specified as CFM (L/s) or % of supply air are therefore excluded from the
calculation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Bypass Airflow
In a VVT system air is bypassed directly from the supply to the return duct when the supply airflow rate falls below a certain level. This is done to maintain minimum flow
rates through system cooling and heating coils and to maintain acceptable system pressure levels. The bypass airflow is specified as a percentage of the maximum
supply airflow rate.
Example: If the design supply airflow rate is 10000 CFM and the bypass airflow rate is 75%, air will be bypassed whenever the required supply flow rate to zone terminals
drops below 7500 CFM. Air will be bypassed from the supply duct to the return duct to maintain the supply fan flow rate at 7500 CFM.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Changeover Time
This item defines the time required to change from cooling to heating modes in a VVT air system. In the system simulation model used by the program, VVT systems
operate in up to four different modes per hour: cooling, heating, changeover and float. The length of the changeover period will affect the minutes per hour available for
operation in the other three modes. Changeover time is typically known from the control specification for the VVT system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 21 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.11 Central Heating Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Central Heating Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.11 Central Heating Data ››
Heating Design Supply Air Temperature
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.11 Central Heating Data ››
Heating Coil Source
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.11 Central Heating Data ››
This section explains input data for central heating coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Central Heating Data
The Central Heating data view contains information about the central heating coil and related control and sizing characteristics. The content of this data view changes
depending on the equipment and system type which have been selected. Items in this data view are as follows:
Heating Design Supply Air Temperature
Heating Source
Heating Schedule
Capacity Control
Minimum Supply Temperature
Outdoor Air Temperature for Minimum Supply Temperature
Outdoor Air Temperature for Maximum Supply Temperature
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Design Supply Air Temperature
This item defines the maximum heating supply air temperature delivered to zone terminals. The use of this value varies with system type:
1. CAV-Single Zone, Heating Only - The heating design temperature is used to calculate the required supply airflow rate to the zone at the design heating condition. It
also is the maximum supply temperature permitted with reset controls.
2. CAV-Single Zone, Cooling and Heating - In a system which provides both cooling and heating, supply airflow sizing is based on design cooling conditions rather
than design heating conditions. Therefore, the heating design temperature is only used as the maximum supply temperature permitted with reset controls.
3. Dual Duct and Multizone Systems - For these systems, the input refers to the maximum temperature of hot deck air supplied to zone terminals. When reset is used,
it defines the maximum supply temperature permitted.
The distinction that supply temperature is measured at the zone terminal is significant only when considering duct heat loss. The central air handler must produce air
warmer than the design temperature to overcome heat loss in the supply ducts. When duct heat loss is not considered, the air handler leaving temperature and the
supply temperature at the zone terminals will be equal.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Source
This item defines how heating is provided to the coil. Choices are electric resistance, natural gas combustion, fuel oil combustion, propane combustion, hot water, steam
and heat pump. The "heat pump" option is only offered for the DX equipment types (packaged rooftop units, packaged vertical units, split AHU). When the Undefined
equipment type is used, the heating source will default to "Any".
Page 22 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Heating Coil Schedule
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.11 Central Heating Data ››
Heating Coil Capacity Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.11 Central Heating Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Schedule
The heating coil schedule specifies the months of the year in which the central heating coil operates. The schedule consists of a series of twelve buttons, one for each
month. To turn the coil on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from January through April and
from October through December; it is off during the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Coil Capacity Control
Capacity Control defines how the output of the heating coil is controlled. Items offered in this drop down list change depending on system type. The full set of control
types is briefly discussed below.
1. Constant Temperature, Fan Cycled - The supply fan is cycled on and off to modulate heating provided to the zone. While the supply fan is cycled on, air is delivered
to the zone terminal at the design supply air temperature. This control option is only offered for Chilled Water AHU CAV Single Zone systems.
2. Constant Temperature, Fan On - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. Air is delivered to zone
terminals at the design supply air temperature. Because this control provides maximum heating at all times, conditioning provided to zones in the system must be
modulated either by varying the supply airflow as is done in VAV Dual Duct systems, or by some form of cooling as is done in Dual Duct and Multizone systems.
3. Cycled or Staged Capacity, Fan On - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. In a DX heat pump,
compressors cycle or unload to modulate the heating provided to zones in the system. In a hot water unit, water flow or temperature is modulated to control coil
heating capacity.
4. Temperature Reset by Greatest Zone Demand - During "occupied" system operating hours, the supply fan runs continuously to condition and ventilate. The supply
air temperature is reset according to the greatest sensible heating load among zones served by the system. When this control is selected, you must also specify the
minimum heating supply temperature allowed. The control algorithm will not reset the supply temperature below this level.
From a control perspective, demand-based reset is achieved in different ways depending on system type. In CAV Dual Duct and Multizone systems, hot deck supply
temperature is reset such that one or more zones use 100% hot deck air. In Dual Duct VAV systems, supply temperature is reset such that one or more dual duct VAV
boxes are fully open.
5. Temperature Reset by Outdoor Air Schedule - Supply air temperature (SAT) is reset according to an outdoor air temperature schedule. When this control is used,
the minimum and maximum SATs are defined along with the corresponding outdoor air temperatures (OAT). The maximum SAT is always the design value. The
remaining SAT and OAT values are defined by the user.
Example: The design SAT is 120 F and the minimum SAT is 100 F. The design SAT is used when the OAT is 30 F and colder. The minimum SAT is used with the
OAT is 55 F and warmer. Between 30 F and 55 F, SAT varies as a linear function of outdoor temperature. This control schedule is shown in the figure below. Inputs
for this control scheme would be:
Design supply temperature = 120 F
Minimum supply temperature = 100 F
OAT for maximum supply temperature = 30 F
OAT for minimum supply temperature = 55 F
Page 23 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.3.12 Fan Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Fan Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Supply Temperature Reset by Outdoor Air Schedule
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for supply and return fans.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Data
This help topic discusses the data view for central fans. While entering system data, any of five different kinds of fans may need to be defined: Supply Fans, Return Fans,
Hot Deck Supply Fans, Ventilation Fans and Exhaust Fans. All are described using a similar set of input items. Items for a supply fan are shown above. The complete set
of fan input items are:
1. Fan Type : Choose a specific type of fan to display defaults for fan efficiency and part-load performance, or choose "user-defined" to specify your own performance
data.
2. Configuration : Only required for supply fans to specify the position of the coil relative to the fan.
3. Full-Load Fan Performance : May be defined in terms of total static pressure, BHP, motor kW or Watts per unit flow. Affects fan heat gain and energy consumption.
Supply Fan also provides an option for automatically calculating total system fan kW according to the ASHRAE 90.1 Appendix G equation G3.1.2.9. This feature is
useful for LEED EA Credit 1 analyses.
4. Overall Efficiency or Motor Efficiency : When fan performance is specified as total static, the overall fan efficiency is needed to determine fan power. When fan
performance is specified as BHP, the fan motor efficiency is needed to compute fan power.
Page 24 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Fan Type
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Fan Configuration
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Fan Full Load Performance Value
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
5. Part-Load Fan Performance : Relevant only for VAV fans. Defines how input power varies as a function of part-load airflow. Affects fan heat gain and energy use at off-
design conditions.
6. Fan Control: Defines whether one-speed or two-speed fan control is used. When two-speed control is used the percent airflow at low speed is also defined. This
option appears for CAV Single Zone systems with equipment types "packaged rooftop", "vertical packaged units" and "split DX AHU".
7. Fan Schedule: Applicable only for the Ventilation Fan in a standalone Make Up Air Unit / DOAS system. This schedule defines the operating periods for the Make Up
Air Unit or DOAS fans.
8. Unoccupied Fan Airflow: Applicable only for the Ventilation Fan in Induction Beam systems. This input specifies primary airflow in the unoccupied fan/thermostat
period as a percentage of design primary airflow. Values from 50% to 100% in 5% increments are permitted. For example, if a value of 75% is specified, the
ventilation air handler will deliver 75% of design primary airflow during hours in the unoccupied fan/thermostat period.
9. Unoccupied Fan Control: This input only appears for the Ventilation Fan in Induction Beam systems. This input specifies whether the ventilation fan runs
continuously or cycles on demand during the unoccupied fan/thermostat period. If you choose "continuous operation" the ventilation and exhaust fans in the
ventilation unit will run 60 minutes per hour during unoccupied hours to power the induction terminals. If you choose "cycled on demand" the ventilation and exhaust
fans will remain off when all zones are floating in the deadband between cooling and heating setpoints. When one or more zone thermostats call for cooling or
heating, the ventilation and exhaust fans turn on and operate only for the portion of the hour necessary to meet the zone loads, and then the fans turn off again. This
can be a significant energy saving feature for Induction Beam systems. It is typically used when tight control of zone humidity levels is not required during unoccupied
times.
10. Average Zone Temperature: Applicable only for the ventilation fan in a standalone Make Up Air Unit / DOAS system. This value is an estimate of the average
temperature in the zone served by the system. Because this system is not linked to a thermostat in the zone, it does not control zone temperature. Instead the zone
temperature floats and an estimate of the average zone temperature is needed in order to calculate the floating temperature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Type
Users may choose among ten common fan types shown in the table below, or can select the "user-defined" fan.
For constant volume systems, the only significance of choosing a fan type is that it displays a default fan efficiency value. For variable volume systems, both a default fan
efficiency and a default part-load performance curve are assigned based on the chosen fan type. The default part-load curve cannot be modified.
The only significance of choosing the "user-defined" fan type is that it permits the user to edit the fan part-load performance data for VAV fans.
Fan Types
1. Forward Curved
2. Forward Curved with Dampers
3. Forward Curved with Variable Frequency Drive
4. Forward Curved with Variable Speed Drive
5. Forward Curved with Inlet Guide Vanes
6. Backward Inclined or Airfoil (BI/AF)
7. BI/AF with Inlet Guide Vanes
8. BI/AF with Variable Frequency Drive
9. BI/AF with Variable Speed Drive
10. Controlled Pitch Axial
11. ASHRAE Std 90.1 Appendix G Fan Curve (a)
12. User-Defined Fan
(a) Choosing this fan type will set the VAV fan part-load curve to values shown in Table G.3.1.3.15 of ASHRAE Std 90.1 Appendix G. When using HAP to perform
analysis for the LEED Energy and Atmosphere Credit 1, this fan curve will be required for some applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Configuration
This item defines the position of the supply fan with respect to the cooling coil. "Draw-Thru" means the fan is downstream of the cooling coil. "Blow-Thru" means the fan
is upstream of the cooling coil.
The position of the fan influences latent cooling coil loads since it affects the coil entering temperature (for blow-thru fans) or the required coil leaving temperature (for
draw-thru fans). Both affect the apparatus dew point for the coil.
Note that for "CAV-Dual Duct", "CAV-2-Deck Multizone", "CAV-3-Deck Multizone" and "VAV - 2-Fan Dual Duct" systems, the configuration is set to "blow-thru" and may
not be changed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Full Load Performance Value
Full load fan performance must be known in order to calculate fan heat gain and energy use. In VAV systems it is also the basis for calculating part-load fan heat gains
and energy use. Full load performance can be specified in one of five ways listed below. To enter performance data, first select the desired units of measure from the
drop down list and then enter the performance value.
1. Total Static describes the total static pressure across the fan. It is used with the overall fan efficiency to calculate fan motor input power and fan heat gain.
2. BHP defines the fan motor brake horsepower. It is used with the motor efficiency to determine fan motor input power and fan heat gain.
3. Motor kW specifies the input power to the fan motor. It is used to determine fan heat gain.
4. W/CFM (W/L/s) describes the motor input watts per CFM or L/s delivered by the fan at its design condition.
Page 25 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Baseline Fan Adjustment Factor Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
5. 90.1 App G Fan KW specifies the program should automatically determine the fan input kW using the calculation specified in ASHRAE Standard 90.1 Appendix G,
section G3.1.2.9 and Table G3.1.2.9. The particular calculation procedure used depends on the Energy Standard preference set for the current project - either
ASHRAE 90.1-2004, 90.1-2007, or 90.1-2010.
Note that if ASHRAE 90.1-2007 or 90.1-2010 is the current project preference, selection of the "90.1 App G Fan kW" option will cause a button titled "90.1 A Factor
Calculations" to appear next to the drop-down list. Click this button to display the Baseline Fan Power Adjustment Factor input screen. This input screen is used to
specify additional data needed for the 90.1-2007 and 90.1-2010 baseline fan power allowance calculation.
The "90.1 App G Fan kW" option is intended for use when you are modeling air systems for a baseline building in a LEED Energy and Atmosphere Prerequisite 2 or
Credit 1 analysis. Note that this option is only offered for the supply fan. Fan performance inputs for any return or exhaust fans should be set to zero in this case. For
further information on how this option is used in calculations, please refer to the fan calculation documentation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Baseline Fan Adjustment Factor Data
The Baseline Fan Adjustment Factor Calculation window is used to input additional data needed for the baseline fan power allowance calculation under ASHRAE
Standard 90.1. This calculation involves an adjustment factor "A" which is derived by the following steps:
a. Identify qualifying devices in the proposed air system. Note that devices are defined if they exist in the proposed system even though the adjustment factors apply to
the baseline fan power.
b. For each device used, either accept the ASHRAE prescribed pressure drop or specify the actual pressure drop from the proposed system. Again note that pressure
drops existing in the proposed system are used even though the adjustment factors apply to the baseline fan power.
c. The adjustment factor "A" is then calculated automatically by HAP for each device specified and all the A factors are summed to obtain a system total "A" factor which
is used in the calculation of the baseline fan power allowance.
The qualifying devices are listed along the left side of this window. Items vary depending on the edition of ASHRAE 90.1 selected for the project (see Figures 1 - 3
below)..
To specify data, first check the box for each device that exists in the proposed air system (the system corresponding to the baseline system you are defining). When you
check the box, the pressure drop input will be activated. If a pressure drop value is shown with a gray background, this is an ASHRAE-prescribed pressure drop and may
not be changed. If a pressure drop value is shown with a white background, it is a user input and must be entered according to the rules outlined in ASHRAE Standard
90.1 Section 6. In the 2007 and 2010 editions of the Standard, the data is found in Table 6.5.3.1.1B. In the 2013 edition the data is found in Table 6.5.3.1-2. When all
applicable devices have been selected and their pressure drops defined, click the OK button to return to the Air System Properties window.
Further Information. The adjustment factor "A" is intended to lessen or eliminate any fan power penalty for best practices used in the proposed system. Certain devices
used in a proposed system, such as high efficiency filters, heat recovery, or sound attenuation to name a few, have beneficial effects for comfort or energy efficiency, but
also increase the total fan pressure drop and therefore the fan energy use in the proposed system. To lessen or eliminate the penalty for this increased fan energy in the
proposed system, the fan power for the corresponding baseline system is increased via the "A" factor adjustment. This rationale is why you choose the devices based on
what is used in the proposed system and determine pressure drops based on those existing in the proposed system, even though the adjustment factor applies to fan
power in the baseline system.
Figure 1. Adjustment Factor Window for ASHRAE 90.1-2013
Page 26 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Fan Efficiency
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Figure 2. Adjustment Factor Window for ASHRAE 90.1-2010
Figure 3. Adjustment Factor Window for ASHRAE 90.1-2007
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Efficiency
Page 27 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Fan Part-Load Performance
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Fan Control
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
Fan Schedule
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.12 Fan Data ››
11.3.13 Supply Duct, Return Duct & Return Plenum Data
11.0 Entering Systems ›› 11.3 System Components Data ››
Duct System
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.13 Supply Duct, Return Duct & Return Plenum Data ››
When fan performance is defined in terms of total static pressure, the overall fan efficiency must also be defined. The overall efficiency is a combined value of the fan
mechanical, drive and motor efficiencies. The overall efficiency is used together with the total static pressure to calculate fan motor input power and fan heat gain.
When fan performance is defined in terms of BHP, the fan motor efficiency must also be defined. Motor efficiency is used together with BHP to calculate fan motor input
power and fan heat gain.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Part-Load Performance
The fan part load performance table contains eleven cells which specify fan performance from 100% to 0% of full load fan airflow in 10% increments. Fan power at each
airflow condition is defined as a percentage of the motor input power at the full load condition. This data is used in fan calculations for VAV systems where supply fan
airflow varies continuously. It is also used for fans in dedicated outdoor air systems (DOAS) or standalone make up air unit / DOAS systems where airflow varies
because it is scheduled or is modulated by demand controlled ventilation. The fan data can be entered directly when you have chosen the "user-defined" fan type.
Otherwise, performance data is defaulted based on the type of fan selected.
Example: The fan motor input power at 100% airflow is 12 kW. The part-load performance table specifies 72% kW at 80% airflow. Therefore when fan airflow is at 80% of
its design value, fan motor input power is 72% of 12 kW or 8.64 kW.
During calculations, HAP interpolates between these eleven performance points to determine fan input power at any part-load airflow condition. When entering
performance data, always specify 100% kW at 100% airflow. The 0% airflow point is used as an anchor for interpolations between 10% airflow and 0% airflow. Therefore,
the value specified for 0% airflow should represent % fan motor kW as airflow approaches zero or as it approaches the minimum fan airflow. It is important to note that
specifying a non-zero value at 0% airflow does not mean the fan will use energy when it is off. Fan input power is always zero when the fan is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Control
Specify how the supply fan is controlled:
a. 1-speed fan, cooling and heating - The supply fan runs at design airflow for all occupied hours and cycles between design flow and off for unoccupied hours.
b. 2-speed fan cooling, 1-speed fan heating - For occupied hours the supply fan runs at high or low speeds when a cooling demand exists. The supply fan runs at
design airflow when a heating demand exists. It runs at low speed in deadband. For unoccupied hours, the fan cycles between high speed, low speed and off
when a cooling demand exists. It cycles between high speed and off when a heating demand exists.
c. 2-speed fan, cooling and heating - For occupied hours the supply fan runs at high or low speeds when either a cooling or heating demand exists. It runs in low
speed in deadband. For unoccupied hours, the fan cycles between high speed, low speed and off when cooling or heating demands exist.
When 2-speed control is specified the user must also specify the Low Speed Fan Airflow as a percentage of high speed airflow. For example, a 67% value means low
speed airflow is 67% of high speed airflow.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fan Schedule
The Fan Schedule defines the daily "occupied" and "unoccupied" system operating periods. This input is only appears for the standalone Make Up Air Unit / DOAS
system type. During hours in the "occupied" period the ventilation fan runs continuously. During hours in the "unoccupied" period the ventilation fan is off.
The Fan Schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a fan schedule, choose the "create new schedule" item in the schedule drop-down list. The Schedule Form will
appear and will allow you to define profiles for the daily "occupied" and "unoccupied" periods. Be sure to specify that the type of schedule is "fan/thermostat". In this
type of schedule you designate each hour as "occupied" or "unoccupied". When you press the OK button to exit from the Schedule Form, your schedule data will be
stored and the schedule will be assigned to the current system automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database, you can simply select the desired schedule from the drop-
down list. Note that the schedule you select must be a "fan/thermostat" kind of schedule.
In addition, you can modify schedule data directly from the System Form by pressing the Schedule button to the left of the drop-down list. When you press this button, the
Schedule Form will appear and will display inputs for the currently selected schedule. After modifying the schedule data, press the OK button to return to the System
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for supply ducts, return ducts and return plenums.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 28 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Supply Duct Heat Gain
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.13 Supply Duct, Return Duct & Return Plenum Data ››
Supply Duct Leakage
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.13 Supply Duct, Return Duct & Return Plenum Data ››
Return Duct or Plenum Data
11.0 Entering Systems ›› 11.3 System Components Data ›› 11.3.13 Supply Duct, Return Duct & Return Plenum Data ››
Duct System
The Duct System data view contains information about supply duct heat gain or loss, supply duct leakage and return duct or plenum data. Items in this data view are as
follows:
1. Duct Heat Gain : Heat gains or losses in the supply ductwork can be considered with this item. Heat gains and losses will affect system performance and increase
cooling and heating coil loads.
2. Duct Leakage : Air leakage in supply ductwork increases the airflow requirement for the central supply fan, and in turn increases the fan heat gain and power use.
3. Return Air Via : Return air can be ducted, in which case it is assumed no wall, roof or lighting heat gain is removed by return air. Or air can flow through a return
plenum. In this case a portion of wall, roof and lighting heat gains may be removed by the return air, thus reducing the heat gain to the conditioned space.
4. Wall Heat Gain to Plenum : A portion of wall heat gain can be removed by air flowing through the return plenum when the plenum has an exterior wall exposure.
5. Roof Heat Gain to Plenum : A portion of roof heat gain can be removed by air flowing through the return plenum when the plenum is beneath a roof.
6. Lighting Heat Gain to Plenum : A portion of lighting heat gain can be removed as plenum air flows over the upper surface of the lighting troffer, or when return air flows
through the lighting fixture.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supply Duct Heat Gain
This item defines the heat gain or loss due to conduction of heat through supply duct walls. Per ASHRAE recommendations, duct heat gain or loss is defined as a
percentage of the sum of zone sensible loads for the system. This represents a simple model of heat transfer through duct walls. When a heat gain percentage is
specified, it is used for all design cooling and heating calculations, and also in energy simulations. In addition, for dual duct systems, the heat gain factor is applied to
both warm and cold supply ducts.
Example: A duct heat gain of 2% is specified. For a specific hour the sum of zone sensible loads is 120,000 BTU/hr. Therefore, the duct heat gain will be 2% of 120,000
BTU/hr or 2,400 BTU/hr. This heat gain will be used to determine the change in temperature of supply air between the time it leaves the central air handler and the time it
reaches the zone supply terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supply Duct Leakage
This item specifies air leakage from supply ducts as a percentage of the airflow leaving the supply fan. This represents a simple model of duct leakage. When duct
leakage is modeled, it results in larger fan airflow rates being required to provide the necessary airflow at zone terminals. When specified, leakage is used for all design
cooling and heating calculations, and also in energy simulations. For dual duct systems, the leakage factor is used for both warm and cold supply ducts.
Example: A duct leakage value of 3% is specified. For a specific hour, the supply airflow rate required at zone terminals in a system is 10,000 CFM. Therefore, the
required airflow at the supply fan is 10309.3 CFM. With this fan airflow, 3% leakage will result in 10,000 CFM reaching the zone terminals. The 309.3 CFM that leaks
from the supply duct is assumed to flow directly or indirectly into the return air stream.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Return Duct or Plenum Data
Return air can flow through a return duct or a return air plenum. When return air is ducted, HAP assumes no wall, roof or lighting heat gains are removed by the return
air. When a return air plenum is used, portions of the wall, roof and lighting heat gains can be removed by the return air and this reduces the heat gain to the conditioned
space. Four input items are used to model return ducts and plenums:
1. Return Air Via: Specify whether a return air duct or return air plenum is used in the system. When ducted return is chosen, no further inputs will be required.
Page 29 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.4 Zone Components Data
11.0 Entering Systems ››
Zone Components Tab / System Form
11.0 Entering Systems ›› 11.4 Zone Components Data ››
2. Wall Heat Gain to Plenum: A portion of the wall transmission heat gain will be removed by plenum air when the plenum is adjacent to an exterior wall. The fraction of
the wall load reaching the plenum is based on the area of exterior wall adjacent to the plenum relative to the total wall area. To simplify the specification of this fraction,
users only need to specify the wall area adjacent to the plenum as a percentage of the GROSS wall area. Note that this percentage does not define the percentage of
wall load to plenum. Instead, the program will use your percentage to determine the wall area adjacent to the plenum as a fraction of NET wall area and then will use
this fraction to split the wall load between the plenum and the occupied space. The following example illustrates this procedure.
Example: An air system serves rooms on a floor with a 12 ft floor-to-roof height. The top 2 feet is a return air plenum while the remaining 10 feet are in the occupied
space. The gross wall area for all rooms served by the air system is 6000 sqft. Therefore 1000 sqft of wall area is adjacent to the plenum and 5000 sqft is adjacent to
the occupied space. These walls also have 1200 sqft of window area for the occupied space.
To define the wall load to plenum, a value of 1000 sqft / 6000 sqft or 16.7% should be specified in the program.
During program calculations, the program first uses the specified percentage and the gross wall area to determine the area of wall adjacent to the plenum: 6000 x .167
= 1000 sqft. Next, the program determines the net wall area by subtracting window area from gross wall area: 6000 sqft - 1200 sqft = 4800 sqft net wall area. Then the
program determines wall area adjacent to the plenum as a percentage of the net wall area: 1000 sqft / 4800 sqft = 20.8 %. Therefore, the wall load to plenum will be
20.8% of the total wall load. The remaining 79.2% of the wall load will be assigned to the occupied space.
3. Roof Heat Gain to Plenum: When a plenum is used and is adjacent to a roof exposure, a portion of the roof transmission heat gain will be removed by air flowing
through the plenum. During calculations, the program will multiply the roof load for each zone in the system by the "roof heat gain to plenum" percentage to determine
the roof component of the plenum heat gain. The remainder of the roof load is assumed to reach the zone.
Note that you are defining the "effective" percentage of roof load removed by plenum air. While 100% of the heat transmitted through the roof passes through the
plenum, only a portion of this heat is removed by return air in the plenum. This is because the roof transmission heat warms the plenum air and results in heat flow
through the ceiling tiles into the conditioned space. Therefore, some portion of the roof transmission load typically reaches the space. It is normally not correct to
assign 100% of roof load to the plenum.
Roof load to plenum values typically range from 60% to 95%, but depend on the plenum temperature which is influenced by the plenum geometry (height, width), the
airflow rate and the air velocity. A typical rule of thumb value is 70%.
Example: A roof-to-plenum value of 65% is specified. During program calculations, 65% of the roof load will be assigned to the plenum while 35% will be assigned to
the occupied space.
4. Lighting Heat Gain to Plenum: A portion of the heat gain from lighting fixtures may be removed as plenum air flows over the warm surface of the lighting troffer, or
when return air flows through the lighting fixture itself.
Rule of thumb values for lighting heat gain to plenum depend on the lighting fixture type. For recessed unvented fixtures, values of 30% to 40% are typical. For
recessed, vented fixtures, values of 40% to 50% are typical. For free hanging fixtures, use 0% since the lighting fixtures are not adjacent to the plenum.
Example: A light-to-plenum value of 30% is specified. During program calculations, 30% of the lighting heat gain is assigned to the plenum. The remaining 70% of the
heat gain is assigned to the occupied space where it is used in transfer function calculations to determine the rate of conversion to cooling load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Zone Components tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Components Tab / System Form
About Zone Components. The Zone Components tab on the System Form contains information about components located in or adjacent to zones served by the
system. This includes supply terminals, thermostats, supplemental heating units and the spaces included in the zone.
The Zone Components Tab is divided into two panels which occupy the left-hand and right-hand portions of the tab. Features in these two panels are used to enter
zone component data.
1. Checklist Panel. The left-hand panel contains a checklist of zone-level components which can be included in the system. A check mark in the box next to each item
indicates whether one or more zones in the system include that component. Certain items, such as spaces and thermostats, are required in the system. These items
are checked and cannot be unchecked. Other items, such as zone heating units, are optional and may be included by checking the item, or excluded by unchecking
the item. The figure above shows an example for a VAV system; 4 zone components are offered in this type of system.
Page 30 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.4.1 Space Asssignments
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Space Assignments Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.1 Space Asssignments ››
2. Data Panel. The right-hand panel contains views of data for each zone component. The data view in this panel changes each time you click on the name of a zone
component in the checklist panel. It is important to click only on the name of the item; clicking on the check box for an item displays its data but also includes or
excludes the component.
In the figure above, space assignment data is shown in the right hand panel because the "Spaces" item in the checklist panel was the last item clicked on. To change
the display to "Thermostats" data, you would simply click on the "Thermostats" item in the checklist panel.
The type of air system being defined determines the zone components offered in the checklist panel. In all, seven different items can appear in the checklist of zone
components:
1. Spaces: Defines spaces included in each zone in the system. Required for all system types.
2. Thermostats: Settings for zone thermostats. Required for all system types.
3. Supply Terminals: Information about zone supply terminals such as diffusers and VAV boxes. Required for central air system types.
4. Zone Heating Units: Specifications for supplemental baseboard or fan coil heating units used in zones. Optional for central air system types.
5. Supply Terminals (4-Pipe Induction): A special set of information is required to describe 4-pipe induction terminals.
6. Common Terminal Unit Data: Common data that describes the characteristics and sizing criteria for fan coil units, water source heat pump units, induction terminals or
VRF indoor units. One set of data applies to all terminal units in the system.
7. Terminal Unit Data - Fan Coil Terminals: Specific data that describes further characteristics of fan coil, VRF and water source heat pump terminal units. Data can be
defined on a zone-by-zone basis or as one set of specifications for all fan terminals.
8. Terminal Unit Data - Induction Terminals: Specific data that describes further characteristics of induction beam or active chilled beam terminals. Data can be defined
on a zone-by-zone basis or as one set of specifications for all terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains space assignment input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Space Assignments Data
The Space Assignments data view is used to assign spaces to each zone served by the system. It is also used to name zones. Data for one zone is displayed in the data
view at a time. Features are provided for browsing through the full set of zones defined for the system. The data view consists of four key components:
1. Zone Controls appear in the upper right-hand portion of the data view. The zone name appears in this section and can be entered or changed. The zone name is part
of a drop-down list which can be used to switch from data for one zone to another. The previous and next buttons below the zone name input can also be used to step
forward or backward sequentially through your list of zones. The zone number is displayed above the zone name for reference. In the figure above, data for the
seventh of 14 zones in the system is displayed. The zone name is "Music Rooms".
2. The Spaces List appears on the left-hand side of the data view. It contains a list of all spaces currently stored in your project. This list serves as the reservoir for
choosing spaces to assign to various zones in your system.
3. The Spaces in Zone List appears on the right-hand side of the data view. It contains a list of all spaces assigned to the current zone and the multiplier factors for each
space. Multiplier factors are used when a single space represents one of a number of identical rooms included in a zone. To account for the total number of instances
of that room in a zone the multiplier is used. When each space represents a unique room or area of the building, a multiplier of one is used. In the figure above, the
"Music Rooms" zone includes four spaces, each having a multiplier of one.
4. The Add and Remove buttons are found between the "Spaces List" and the "Spaces in Zone List". The Add button is used to assign a space whose name is
highlighted in the Spaces List to the current zone. The Remove button is used to remove a space whose name is highlighted in the Spaces in Zone List from the
current zone.
Tutorial. The following tutorial explains the steps required to assign spaces to zones in a system.
1. Start with zone 1.
Page 31 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.4.2 Thermostat Data
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Thermostat Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
Thermostat Setpoints
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
2. Enter a name for the zone in the zone name box.
3. In the Spaces List on the left-hand side of the data view, highlight the name of the space you wish to include in the current zone by clicking on the space name.
To include multiple spaces listed consecutively in the space list, hold down the [Shift] key and click on the first and last space names in the block of spaces.
To include multiple spaces listed non-consecutively in the space list, hold down the [Ctrl] key and click on the name of each space you wish to assign.
4. Press the Add button. All the spaces you highlighted will be assigned to the current zone. Their names will appear in the "Spaces in Zone" list on the right-hand side of
the data view. Note that the Add button does not remove the name from the "Spaces List"; it simply adds this space name to the "Spaces In Zone" list.
5. In the "Spaces In Zone" list, change the multipliers for any spaces that represent one of a number of identical rooms in the zone. Click on the name of the desired
space to highlight that row in the list. Then press the Delete key to delete the current multiplier. Finally enter the new multiplier factor.
6. Press the Next button that appears below the zone name to move to the next zone in your system.
7. Repeat steps 1-6 for each zone in your system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for zone thermostats.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Thermostat Data
The Thermostats data view contains information about zone thermostat controls, the zone diversity factor and direct exhaust air. Data for one zone is shown at a time.
The upper portion of the data view is used to control the display of zone data:
1. All Zone Tstats Set the Same specifies whether one set of data will apply to all zones in the system, or whether data will be defined on a zone-by-zone basis. When
this box is checked, only one set of thermostat, diversity factor and direct exhaust data will be defined and it will apply to all zones in the system. When this box is not
checked, a separate set of data will appear for each zone in the system.
2. Zone Controls. The Zone Name identifies the zone whose data is currently shown in the data view. In the figure above, data for the D107-Classroom zone is shown.
The zone name is part of a drop-down list which can be used to display data for any other zone in the system. Or, you can press the right and left arrow buttons above
the zone name to step forward or backward sequentially through your list of zones. The zone number is shown above the zone name to provide reference. Note that
when the "All Zone Tstats set the same" box is checked, the zone name will be "All Zones" indicating common data for all zones is shown. Also note that the zone
name cannot be modified in this data view. It can only be modified on the Space Assignments data view.
The remaining items on this screen describe thermostat controls, the diversity factor and direct exhaust air:
1. Thermostat Setpoints define the settings for cooling and heating for both the occupied and unoccupied period. The throttling range for the thermostat is also specified.
2. Diversity Factor defines whether different lighting and occupant load levels should be used for zone sizing and system sizing purposes.
3. Direct Exhaust Air inputs describe air directly exhausted from the zone by devices such as laboratory hoods, kitchen hoods and toilet exhausts.
4. Thermostat Schedule specifies the periods of the day during which occupied and unoccupied thermostat setpoints are used. This item also influences how the system
operates at different times of day.
5. Unoccupied Cooling specifies whether cooling is permitted during "unoccupied" system operation periods.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 32 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Zone Diversity Factor
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
Zone Direct Exhaust Airflow
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
Thermostat Setpoints
Five input items are used to describe thermostat settings for a zone:
a. Cooling setpoint, occupied period.
b. Cooling setpoint, unoccupied period.
c. Heating setpoint, occupied period.
d. Heating setpoint, unoccupied period.
e. Thermostat throttling range.
Thermostat Setpoints describe the thermostat controls for cooling and heating during the "occupied" and "unoccupied" operating periods. During the "occupied" period,
air systems generally operate to ventilate and condition the building. During the "unoccupied" period, air systems generally operate in an on-demand mode to provide
conditioning only as needed. Because temperature levels maintained in the building tend to vary between the "occupied" and "unoccupied" periods, the program allows
separate cooling and heating setpoints to be defined for each period. The times of day when "occupied" and "unoccupied" periods occur will be specified in the
Thermostat Schedule item at the bottom of this data view.
Throttling Range. The setpoints are used in conjunction with the thermostat throttling range to simulate thermostat behavior using a simple proportional model of cooling
and heating control. The size of the throttling range is usually determined by the type of thermostat used.
Example: Consider the following thermostat settings:
Cooling setpoint = 74 F
Heating setpoint = 70 F
Throttling range = 4 F
For cooling the system maintains the zone between 74 F and 78 F. Therefore the cooling setpoint defines the lower limit of the cooling range. Setpoint plus throttling
range defines the upper limit of the range. When the zone air temperature is at 74 F, the thermostat is calling for minimum cooling. When the zone air temperature is 78
F, the thermostat is calling for maximum cooling. Between 74 F and 78F, the call for cooling increases in proportion to zone temperature.
For heating the system maintains the zone between 70 F and 66 F. Therefore the heating setpoint defines the upper limit of the heating range. Setpoint minus throttling
range defines the lower limit of the range. When the zone air temperature is 70 F, the thermostat is calling for minimum heating. When the zone air temperature is 66 F,
the thermostat is calling for maximum heating. Between 70 F and 66 F the call for heating increases in proportion to zone temperature.
When the zone air temperature is between 74 F and 70 F, there is no call for cooling or heating. The zone temperature floats in the deadband between cooling and
heating setpoints.
Application Information. There are two schools of thought concerning how the thermostat throttling range should be used in system design applications.
One school holds that the actual controls which will be used in the system must be considered. Therefore, the actual throttling range of the thermostat is specified. As a
result, zone air temperatures vary within the thermostat throttling range and are not held constant at the setpoint.
The other school of thought holds that controls should be idealized for a system design calculation to produce worst case estimates of cooling and heating. Therefore, no
throttling range should be specified. Because the ASHRAE Transfer Function/Heat Extraction calculations cannot be performed without a finite throttling range, adherents
to this philosophy specify a throttling range of 0.1 F or 0.1 C. With this approach, larger coil loads are produced to keep the zones within close proximity to the cooling
and heating setpoints.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Diversity Factor
The diversity factor is used to change lighting and occupant loads for the two stages of system design calculations. When calculating required zone airflow rates, HAP
will calculate lighting and occupant loads according to the user's original space and schedule specifications. When simulating system operation to determine cooling and
heating coil loads, the program provides the option of adjusting lighting and people loads to lower levels using the diversity factor.
During coil simulation calculations for the design cooling analysis, the occupant and lighting loads will be multiplied by the diversity factor for each zone served by the
system. For example, if the occupant heat gain schedule for spaces in a zone specifies that 90% of maximum occupancy occurs for an hour, and a diversity factor of
60% is used, coil simulations will be performed using 54% occupancy (60% x 90%).
Diversity factors are typically used for zones with highly variable occupancy. For example, a conference room zone varies from being densely occupied to being empty at
various times of day. When calculating the required supply airflow rate for the conference room, the maximum occupancy level should be used. When calculating the coil
loads for an HVAC system serving the entire building, it may not be necessary to use the same occupant level since the conference room occupants have moved
elsewhere in the building. Considering maximum occupancy for these calculations would overestimate the total occupant load on the system.
When entering diversity factors, remember that 100% means that people and lighting loads will be used as originally specified in space inputs. A 0% diversity factor
means that people and lighting loads will be eliminated completely.
When you do not wish to consider diversity in coil calculations, specify a diversity factor of 100%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Direct Exhaust Airflow
Direct Exhaust Air refers to air directly exhausted from zones without first flowing through the return plenum or return duct. Direct exhaust can occur in a number of
ways. Examples of forced direct exhaust include laboratory fume hoods, kitchen exhaust hoods, toilet exhaust and through-the-wall exhaust. Examples of natural direct
exhaust includes exfiltration through open loading dock doors and entry doors. Direct exhaust is a significant detail when modeling building performance because where
air leaves the building affects system thermal performance. Air leaving the zone directly will often be at a temperature different from air exhausted after flowing through a
return plenum or return duct.
Discussion. The program assumes a steady state flow condition for all its system calculations. Therefore, any outdoor ventilation air entering the building will somehow
be exhausted from the building. The question is where that exhaust occurs. If direct exhaust is specified, this airflow will be exhausted directly from the zone. If any
remaining outdoor ventilation air must be exhausted, the program assumes it flows through the return plenum or duct before being exhausted at the air handling unit, or
some other central location. Finally, for the situation in which direct exhaust air is not specified, the program automatically assumes all outdoor ventilation air is exhausted
at the air handling unit after flowing through the return duct or plenum. No user specification of exhaust airflow is needed in this case.
Direct Exhaust Inputs. Two inputs are required to define direct exhaust air:
1. Direct Exhaust Airflow defines the airflow rate for direct exhaust. This flow rate is assumed to occur for any hour in which the central supply fan is ON and the
ventilation dampers are open. Direct exhaust airflow should be less than or equal to the outdoor ventilation rate for the system.
Page 33 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Thermostat Schedule
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
Unoccupied Cooling Available?
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.2 Thermostat Data ››
11.4.3 Supply Terminal Data
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Supply Terminals
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
If direct exhaust airflow does not exist in the system, specify a zero airflow rate. When this is done, the program will assume any outdoor ventilation air is exhausted
after flowing through the return duct or plenum.
During system design calculations, if the direct exhaust airflow rate for zones in a system exceeds the outdoor ventilation airflow, the design ventilation airflow rate will
be increased to equal the direct exhaust airflow rate.
During simulation of system operation using proportional, scheduled or demand controlled ventilation control, it is possible for ventilation airflow to fall below the direct
exhaust airflow for zones in the system. In such a situation, direct exhaust airflow is reduced since total system exhaust cannot exceed ventilation.
2. Direct Exhaust Fan kW specifies the input power for a direct exhaust fan, such as a toilet exhaust fan or a wall exhaust fan. Fan power will be assigned to all hours
during which direct exhaust airflow exists. If a fan is not used for direct exhaust, specify a zero kW value. This input item is only affects energy consumption in
operating cost analyses.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Thermostat Schedule
The Thermostat Schedule defines the daily "occupied" and "unoccupied" system operating periods. Note that this input is shared among all zones in the system. You
specify the thermostat schedule once and it applies to the system as a whole.
During hours in the "occupied" period:
a. The occupied thermostat setpoints are used.
b. The system fan generally operates continuously to provide both ventilation and conditioning to the building.
During hours in the unoccupied period:
a. The unoccupied thermostat setpoints are used.
b. The system fan generally operates only when demands for cooling or heating exist.
In the HVAC industry, these periods are commonly referred to as "occupied" and "unoccupied" since they typically correspond to times when people are present in or
absent from the building. It is important to note that these schedules are independent of the occupant heat gain schedules defined earlier when entering space data.
Consequently the "occupied" and "unoccupied" system operating periods do not determine whether people are present in the building.
The Thermostat Schedule can be defined in two ways:
1. Creating a New Schedule. If you have not yet created a thermostat schedule, choose the "create new schedule" item in the schedule drop-down list. The Schedule
Form will appear and will allow you to define profiles for the daily "occupied" and "unoccupied" periods. Be sure to specify that the type of schedule is "fan/thermostat".
In this type of schedule you designate each hour as "occupied" or "unoccupied". When you press the OK button to exit from the Schedule Form, your schedule data
will be stored and the schedule will be assigned to the current system automatically.
2. Selecting an Existing Schedule. If you previously created and stored schedules in your project database, you can simply select the desired schedule from the drop-
down list. Note that the schedule you select must be a "fan/thermostat" kind of schedule.
In addition, you can modify schedule data directly from the System Form by pressing the Schedule button to the left of the drop-down list. When you press this button, the
Schedule Form will appear and will display inputs for the currently selected schedule. After modifying the schedule data, press the OK button to return to the System
Form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Unoccupied Cooling Available?
In any cooling system, cooling can be made available or unavailable in the unoccupied operating period. Note that this input item is shared among all zones. You choose
whether unoccupied cooling is available or not available once, and that specification applies to the system as a whole.
When you choose "available", the system will respond to calls for cooling from zone thermostats during the unoccupied period. When you choose "not available", the
system will not respond to calls for cooling from zone thermostats during the unoccupied period. As a result heat will accumulate in the building mass during the
unoccupied period and can result in large pulldown loads at the start of the next occupied period.
Typically unoccupied cooling is specified as "not available" when ambient conditions during the unoccupied period are such that heat build-up will not be a problem.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for supply air terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supply Terminals
Page 34 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Terminal Type
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
The Supply Terminals data view contains information about zone supply terminal equipment. Data for one zone is shown at a time. The upper portion of the data view is
used to control the display of zone data:
1. All Zones are the Same specifies whether one set of data will apply to all zones in the system, or whether data will be defined on a zone-by-zone basis. When this
box is checked, only one set of supply terminal data will be defined and it will apply to all zones in the system. When this box is not checked, a separate set of data will
appear for each zone in the system.
2. Zone Inputs. The Zone Name identifies the zone whose data is currently shown in the data view. In the figure above, data for the D104-Classroom zone is shown.
The zone name is part of a drop-down list which can be used to display data for any other zone in the system. Or, you can press the right and left arrow buttons above
the zone name to step forward or backward sequentially through your list of zones. The zone number is shown above the zone name to provide reference. Note that
when the "All Zones are the Same" box is checked, the zone name will be "All Zones" indicating common data for all zones is shown. Also note that the zone name
cannot be modified in this data view. It can only be modified on the Space Assignments data view.
The items in the Supply Terminal Data group describe supply terminal characteristics:
1. Terminal Type defines the kind of supply terminal equipment used for the zone. Examples include VAV boxes and fan powered mixing boxes.
2. Air Distribution defines the location of the supply air discharge and return air grille in the zone.
3. Air Distribution Effectiveness inputs appear when the ventilation sizing method specified for the air system is one of the ASHRAE Standard 62.1 Ventilation Rate
Procedure options. These inputs assist in defining the proper air distribution effectiveness (Ez) factors used for the terminal in the Ventilation Rate Procedure
calculation.
4. Minimum Airflow specifies the minimum supply airflow requirement for the zone. During sizing calculations, HAP will make sure the terminal is sized for at least this
amount of airflow.
5. Terminal Fan Full Load Performance describes the performance of a terminal mixing box fan at its full airflow condition. This data is used to determine fan heat gain
and motor input power.
6. Overall Efficiency defines the efficiency of a terminal mixing box fan. It is used only when fan full load performance is specified in terms of total static pressure.
7. Design Heating Supply Temperature specifies the heating supply temperature for a terminal containing a reheat coil. This value is used in sizing terminal airflow, and
reheat coil capacity.
The items in the Shared Data group define characteristics that are shared and apply to all supply terminals in the system.:
8. Reheat Coil Source defines the source for heating for terminal reheat coils.
9. Reheat Coil Schedule specifies the months of the year during which the reheat coil is permitted to operate.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Type
This item describes the type of supply terminal used for the zone. The type of supply terminal used influences system operation and also determines additional inputs
required to describe the terminal. To select a terminal type, choose the desired item in the drop-down list. The contents of this list vary depending on the type of system
you are defining. A full list of terminal types offered by HAP appears below:
1. Diffuser (no reheat) - A constant volume supply diffuser. Offered for CAV-Single Zone, CAV-Terminal Reheat, 2-Deck Multizone and 3-Deck Multizone systems.
2. Diffuser with Reheat - A constant volume supply diffuser which includes a terminal reheat coil. Offered for CAV-Single Zone, CAV-Terminal Reheat, 2-Deck
Multizone and 3-Deck Multizone systems.
3. CAV Mixing Box (no reheat) - A constant volume mixing box terminal used with CAV-Dual Duct systems.
4. CAV Mixing Box with Reheat - A constant volume mixing box that includes a terminal reheat coil. Used in CAV-Dual Duct systems.
5. VAV Box (no reheat) - A cooling-only variable volume supply terminal. Offered for VAV systems.
6. VAV Box with Reheat - A variable volume supply terminal which includes a terminal reheat coil. Offered for VAV systems.
7. Series FPMBX with Reheat - A series fan powered mixing box terminal. This terminal mixes primary supply air with return plenum air to maintain a constant volume of
supply air to the zone. It includes a terminal fan mounted in series with the primary airflow path as well as a terminal reheat coil. Offered for VAV systems.
8. Parallel FPMBX with Reheat - A parallel fan powered mixing box terminal. This terminal operates in the same fashion as a VAV box with reheat coil when the zone is
in cooling or in deadband. When the zone thermostat calls for heating, a terminal fan mounted out of the primary air stream turns on to mix warm plenum air with
primary air. This serves as the first stage of heating. If further heating is needed a terminal reheat coil is activated as the second stage of heat. Offered for VAV
systems
Page 35 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Air Distribution
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
Air Distribution Effectiveness
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
Minimum Airflow
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
Terminal Fan Inputs
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
9. VAV Mixing Box - A variable volume mixing box. Used in Dual Duct VAV systems to mix cold deck and hot deck air before providing it to the zone.
10. VVT - A Variable Volume / Variable Temperature supply terminal. Offered for VVT systems only.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air Distribution
This item defines the locations of the supply air discharge into the zone and the return grille for air leaving the zone. Items in the drop-list match the options found in the
Zone Air Distribution Effectiveness table in ASHRAE Standard 62.1. In the 2004 through 2010 editions, see Table 6-2. In the 2013 and 2016 editions, see Table 6.2.2.2.
When the ASHRAE Standard 62.1 Ventilation Rate Procedure is used to calculate ventilation airflow requirements for the system, the supply and return locations are
used together with operating mode, type of supply terminal, heating supply temperature, and zone thermostat setpoint to determine the Zone Air Distribution
Effectiveness (Ez) for the zone.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air Distribution Effectiveness
The Air Distribution Effectiveness input appears when the ventilation sizing method specified for the air system is one of the ASHRAE Standard 62.1 Ventilation Rate
Procedure options.
1. If you select the ASHRAE 62.1 option in the drop-down list, HAP will automatically determine Ez based on the mode of operation (cooling or heating), the type of
terminal, the heating supply temperature, the zone thermostat setpoint, and the location of supply discharge and return grille, using data in the Zone Air Distribution
Effectiveness table in Standard 62.1 (Table 6-2 in the 2004 through 2010 editions. Table 6.2.2.2 in the 2013 and 2016 editions).
2. If you select the User Defined option in the drop-down list, you will directly specify the Ez value in the cell to the right. User-defined Ez inputs are limited to the values
permitted in Standard 62.1. This value will then be used in the Ventilation Rate Procedure calculation. No Standard 62.1 provisions governing Ez changing as a
function of supply cooling or heating conditions will be considered. Users should make sure the specified Ez value is appropriate for the system.
Note that when the ventilation sizing method for the system is "Sum of OA Airflows", these input items do not appear.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum Airflow
This item specifies the minimum supply airflow rate required for the zone. During sizing calculations HAP will compare the required zone airflow rate based on peak zone
and space sensible loads with the minimum airflow specified here. The larger value will be assigned to the zone. In VAV systems this item is also used to determine the
minimum damper position for the supply terminal.
Minimum airflow for the zone can be specified in five ways listed below. To change the units of measure for this input item, choose the desired units from the drop-down
list to the right of this input.
1. CFM or L/s - Minimum airflow is specified directly. Note: When you have specified that "all zones are the same", be careful using these units of measure since the
airflow you enter will be used for all zones in the system.
2. CFM/sqft or L/s/sqm- Minimum airflow is calculated by multiplying your input value by the total floor area in the zone.
3. CFM/person or L/s/person - Minimum airflow is calculated based on the maximum number of occupants in the zone.
4. % of Supply Air - Minimum airflow is calculated as a percentage of the supply airflow for the zone.
5. ACH – Minimum airflow is calculated based on the air changes per hour (ACH) specified. The program calculates the volume of spaces in the zone to determine the
CFM or L/s equivalent of the air changes per hour specified.
Airflow Sizing Example: Minimum airflow of 25 CFM/person is specified for a zone. The maximum number of occupants in the zone is 40. Based on the peak zone
sensible load, the required supply airflow rate is 854 CFM. However, the minimum required airflow is 25 CFM/person x 40 people = 1000 CFM. Therefore, the design
supply airflow rate for the zone will be 1000 CFM instead of 854 CFM.
Minimum Damper Position Example: Minimum airflow of 25 CFM/person is specified for a zone which uses a VAV box as its supply terminal. The maximum number of
occupants in the zone is 40. Based on the peak zone sensible load, the required supply airflow rate for the zone is 2500 CFM. Because the minimum required airflow is
1000 CFM (25 x 40), the minimum damper position for the VAV box is 1000 CFM / 2500 CFM or 40%.
Note: Readers should note that there are two cases in which the minimum zone airflow correction is not used. Both cases involve the sizing method in which space
airflow is calculated from individual peak space loads and the zone airflow is the sum of the space airflow rates. If this sizing method is specified and the supply air sizing
criteria is CFM (L/s) or CFM/sqft (L/s/sqft), the minimum zone airflow correction is not made because it would conflict with the supply air sizing criteria. For example, if
supply air of 5000 CFM is specified in conjunction with a minimum zone airflow rate of 5500 CFM, the two specifications are in direct conflict with one another. Such
conflicts must be corrected in the system input data by the user. The minimum zone airflow correction is used for all other combinations of airflow sizing methods and
supply air sizing criteria.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Fan Inputs
When the supply terminal for a zone is a series or parallel fan powered mixing box, the operating characteristics of the terminal fan must be defined. Two separate input
items are required as shown below.
Page 36 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Design Heating Supply Temperature
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
Reheat Coil Heat Source and Schedule
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.3 Supply Terminal Data ››
11.4.4 Zone Heating Unit Data
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Zone Heating Units Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.4 Zone Heating Unit Data ››
1. Full Load Fan Performance - Full load fan performance must be known in order to calculate fan heat gain and energy use. Full load performance can be specified in
one of three ways listed below. To enter performance data, first select the desired units of measure from the drop down list and then enter the performance value.
a. Total Static describes the total static pressure across the fan. It is used with the overall fan efficiency to calculate fan motor input power and fan heat gain.
b. BHP defines the fan motor brake horsepower. It is used with the fan motor efficiency to determine fan motor input power and fan heat gain.
c. Motor kW specifies the input power to the fan motor. It is used to determine fan heat gain.
d. W/CFM (W/L/s) describes the motor input watts per CFM or L/s delivered by the fan at its design condition.
2. Fan Efficiency - If total static is specified as the fan full load performance value, the overall fan efficiency must also be defined. The overall efficiency is a combined
value of the fan mechanical, drive and motor efficiencies. The overall efficiency is used together with the total static pressure to calculate fan motor input power and
fan heat gain. When BHP is specified as the fan performance value, the fan motor efficiency must be defined. It is used with BHP to determine fan motor input power
and heat gain.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Heating Supply Temperature
This input defines the temperature of supply air delivered by the terminal at the design heating condition. It applies for supply terminals such as constant volume reheat,
VAV reheat, series fan powered mixing boxes, parallel fan powered mixing boxes, or constant volume mixing boxes which contain a heating coil.
The supply temperature is use to determine a required supply airflow rate to meet the heating design load in the zone. Depending on the type of terminal, this airflow
rate can play a role in determining the design supply airflow rate and/or minimum supply airflow rate for the terminal.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Reheat Coil Heat Source and Schedule
These input items define the heat source and the monthly schedule of operation for terminal reheat coils. Note that this data is shared among all zones in the system.
One set of specifications for the reheat source and schedule is used for the entire system.
1. Reheat Coil Heat Source specifies how heating is provided to the coil. Choices are electric resistance, hot water, and steam. When the Undefined equipment type is
used, the heating source will default to "Any".
In design calculations, the choice of a heat source determines whether reheat coil loads will be used in sizing a boiler plant. Reheat coils whose source is hot water,
steam and "any" reheat will be included in boiler sizing calculations. Loads for electric reheat coils will not be considered.
In operating cost studies, the heat source affects building energy consumption. Electric resistance coils add to the building’s electric power profile. Loads for hot water
and steam coils are added to the loads of boilers serving these reheat coils.
2. Reheat Coil Schedule defines the months of the year in which the terminal reheat coil operates. The schedule consists of a series of twelve buttons, one for each
month. To turn the coil on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from January through May
and from September through December; it is off during the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this
monthly schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12
months. If you specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for supplemental zone heating units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Heating Units Data
Page 37 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Zone Heating Unit Type
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.4 Zone Heating Unit Data ››
Zone Heating Unit Trip Temperature
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.4 Zone Heating Unit Data ››
The Zone Heating Units data view contains information about supplemental baseboard or fan coil heating units used in zones. Data for one zone is shown at a time. The
upper portion of the data view is used to control the display of zone data:
1. All Zones are the Same specifies whether one set of data will apply to all zones in the system, or whether data will be defined on a zone-by-zone basis. When this
box is checked, only one set of zone heating unit data will be defined and it will apply to all zones in the system. When this box is not checked, a separate set of data
will appear for each zone in the system.
2. Zone Controls. The Zone Name identifies the zone whose data is currently shown in the data view. In the figure above, data for the "South Vestibule" zone is shown.
The zone name is part of a drop-down list which can be used to display data for any other zone in the system. Or, you can press the right and left arrow buttons above
the zone name to step forward or backward sequentially through your list of zones. The zone number is shown above the zone name to provide reference. Note that
when the "All Zones are the Same" box is checked, the zone name will be "All Zones" indicating common data for all zones is shown. Also note that the zone name
cannot be modified in this data view. It can only be modified on the Space Assignments data view.
The remaining items on this screen describe the characteristics of zone heating units:
1. Zone Heating Unit Type specifies whether a heating unit is used and if so, whether it is a baseboard unit or a fan coil and whether it is controlled by an indoor
thermostat or an outdoor thermostat.
2. Trip Temperature defines the outdoor temperature at which heating unit operation begins. Applicable only for heating units controlled by an outdoor thermostat.
3. Design Supply Temperature specifies the heating supply temperature used to size fan coil heating units.
4. Full Load Fan Performance describes the full load performance of the fan in a fan coil heating unit. It is used to calculate fan heat gain and input power.
5. Fan Overall Efficiency is required when full load fan performance is specified in terms of total static pressure. It is used together with the static pressure to determine
fan heat gain and input power.
6. Zone Unit Heat Source specifies the heat source for coils in the zone heating unit.
7. Zone Unit Heat Schedule defines months during which the zone heating unit operates.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Heating Unit Type
This item defines the type of zone heating unit used in a zone and how it is controlled. To choose a unit type, select the desired item from the drop-down list. Five options
are offered in this list:
1. None: Choose this option when a zone does not contain a supplemental zone heating unit.
2. Baseboard - OAT Control: Baseboard heating units controlled by an outdoor thermostat. Heat output from the baseboard varies as a linear function of outdoor
temperature. This control profile starts with zero output at a user-specified "trip temperature" and rises to maximum output at the winter design dry-bulb temperature.
Note that this type of unit does not respond directly to zone heating loads since it is controlled by an outdoor thermostat rather than an indoor thermostat.
3. Fan Coil - OAT Control: Fan coil heating units controlled by an outdoor thermostat. Outdoor thermostat control is the same as described above for baseboard units.
4. Baseboard - Room Tstat Control: Baseboard heating units controlled by an indoor thermostat. Because an indoor thermostat is used, the baseboard unit operates to
meet zone heating loads.
5. Fan Coil - Room Tstat Control: Fan coil heating units controlled by an indoor thermostat. Using an indoor thermostat, the fan coil unit operates to meet zone heating
loads.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Heating Unit Trip Temperature
The Trip Temperature defines one of the control points for zone heating units which are controlled by an outdoor thermostat. The trip temperature is the outdoor air
temperature at which heating unit operation begins. Unit heat output varies as a linear function of outdoor air temperature between zero at the trip temperature and
maximum output at the winter design temperature.
Page 38 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Zone Heating Unit Fan Coil Inputs
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.4 Zone Heating Unit Data ››
Zone Heating Unit Source and Schedule
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.4 Zone Heating Unit Data ››
11.4.5 Supply Terminal Data for 4-Pipe Induction
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Supply Terminal Data for 4-Pipe Induction Systems
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.5 Supply Terminal Data for 4-Pipe Induction ››
Example: For zone heating units in a system the trip temperature is 35 F. The maximum zone heating unit output is 10,000 BTU/h. The winter design temperature for the
building site is 0 F. With these parameters, zone heating unit operation begins when the outdoor air temperature drops below 35 F. As outdoor temperature continues to
drop, heating unit output increases as a linear function of temperature, reaching maximum output of 10,000 BTU/h when the outdoor air temperature reaches 0 F.
Application Information. Because zone heating units controlled by outdoor thermostats do not respond to room heating loads, there is always a danger that zone
heating unit operation can increase cooling loads. This is particularly a problem when the trip temperature specified is too high. A high trip temperature creates more of
an overlap between zone heating unit operation and outdoor temperature conditions at which zone cooling loads are possible. Therefore, trip temperature must be
chosen carefully considering the balance point between cooling and heating for a zone.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Heating Unit Fan Coil Inputs
When a fan coil zone heating unit is specified, the operating characteristics of the fan in the unit must be known. Three separate input items are required as shown
below.
1. Full Load Fan Performance - Full load fan performance must be known in order to calculate fan heat gain and energy use. Full load performance can be specified in
one of three ways listed below. To enter performance data, first select the desired units of measure from the drop down list and then enter the performance value.
a. Total Static describes the total static pressure across the fan. It is used with the overall fan efficiency to calculate fan motor input power and fan heat gain.
b. BHP defines the fan motor brake horsepower. It is used with the fan motor efficiency to determine fan motor input power and fan heat gain.
c. Motor kW specifies the input power to the fan motor. It is used to determine fan heat gain.
d. W/CFM (W/L/s) describes the motor input watts per CFM or L/s delivered by the fan at its design condition.
2. Fan Efficiency - If total static is specified as the fan performance value, the overall fan efficiency must also be defined. The overall efficiency is a combined value of
the fan mechanical, drive and motor efficiencies. The overall efficiency is used together with the total static pressure to calculate fan motor input power and fan heat
gain. When fan performance is specified in terms of BHP, the fan motor efficiency is defined. It is used with BHP to calculate fan motor power and heat gain.
3. Design Supply Temperature. This item specifies the design heating supply temperature for zone fan coil heating units. HAP will determine the fan coil airflow rate
such that air delivered at this heating supply temperature will meet the design heating load for the zone. The design supply temperature also influences fan cycling
behavior in zone heating units, and this affects energy consumption of the heating units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Heating Unit Source and Schedule
These input items define the heat source and the monthly schedule of operation for the zone heating units. Note that this data is shared among all zones in the system.
One set of specifications for the heat source and schedule is used for the entire system.
1. Zone Unit Heat Source specifies how heating is provided to the coil. Choices are electric resistance, hot water, and steam. When the Undefined equipment type is
used, the heating source will default to "Any".
In design calculations, the choice of a heat source determines whether zone heating unit loads will be used in sizing a boiler plant. Heating units whose source is hot
water, steam and "any" will be included in boiler sizing calculations. Loads for electric heating units will not be considered.
In operating cost studies, the heat source affects building energy consumption. Electric resistance coils add to the building’s electric power profile. Loads for hot water
and steam coils are added to the loads of boilers serving these zone heating units coils.
2. Zone Unit Heat Schedule defines the months of the year in which the zone heating units operate. The schedule consists of a series of twelve buttons, one for each
month. To turn the coil on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from January through April
and from November through December; it is off during the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this
monthly schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12
months. If you specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for 4-pipe induction supply terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Supply Terminal Data for 4-Pipe Induction Systems
Page 39 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.4.6 Common Terminal Unit Data
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Common Terminal Unit Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.6 Common Terminal Unit Data ››
The Supply Terminals data view for a 4-Pipe Induction system contains information about the induction units placed in each zone. Five items are used to describe the
terminals, as listed below. This data is common to all zones in the system.
1. Terminal Type is set to 4-Pipe Induction and cannot be changed by the user.
2. Terminal Cooling Source is set to "chilled water" and may not be changed by the user.
3. Terminal Cooling Schedule defines the months during which chilled water is supplied to the induction units. The schedule consists of a series of twelve buttons, one
for each month. Currently cooling is available for all 12 months by default and may not be changed.
4. Terminal Heating Source identifies the heat source for heating coils in the induction units. Users may choose between "hot water" and "steam" options in this drop-
down list. The choice of a heat source influences boiler plant sizing calculations. Hot water heating coil loads will be included in sizing a hot water boiler which serves
the system. Steam heating coil loads will be included in sizing a steam boiler which serves the system.
5. Terminal Heating Schedule specifies the months during which steam or hot water is supplied to the induction units. The schedule consists of a series of twelve
buttons, one for each month. To turn the coil on for a month, the month’s button must be in a down position, usually indicated by a white background. In the figure
above, the terminal heating coil is permitted to operate for all months of the year.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam heating and changeover control, options on the Equipment Tab allow changeover to be controlled either with this
monthly schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12
months. If you specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data shared by all terminal units in a terminal system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Terminal Unit Data
Page 40 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Common Terminal Unit Cooling Coil Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.6 Common Terminal Unit Data ››
The Common Data view contains information about fan coil units, induction beams, active chilled beams, water source heat pump units or VRF indoor units in the system
that is common to all terminal units in the system. Data specific to each zone terminal unit is shown separately on the Terminal Units data view. Information in this data
view has two different formats. One format is used for terminal units containing a fan: fan coils, water source heat pumps and VRF indoor units. The other format is used
for terminal units not containing a fan: induction beams and active chilled beams.
For both content formats, the data view is divided into four parts:
1. Cooling Coil Data describes sizing and operating characteristics of the cooling components in the terminal unit. For Packaged DX Fan Coils, Split DX Fan Coils, 2-Pipe
Fan Coils, Induction Beams, and Active Chilled Beams cooling capability can be included by checking the "cooling coil" box, or can be excluded by unchecking this
box. For 4-Pipe Fan Coils, VRF indoor units and Water Source Heat Pumps the terminal unit must include a cooling coil. When a cooling coil is included, up to four
items must be defined:
a. Design Supply Temperature is used to size the terminal unit airflow rate. It also influences fan cycling and coil capacity control.
b. Coil Bypass Factor defines the latent cooling performance of the coil. Not displayed here for Induction Beams and Active Chilled Beams; this input appears on the
Terminal Units data view.
c. Cooling Source describes how cooling is provided to the coil.
d. Schedule specifies the months of the year when the cooling coil is permitted to operate.
2. Heating Coil Data describes sizing and operating characteristics of the heating components in the terminal unit. For Packaged DX Fan Coils, Split DX Fan Coils,
2-Pipe Fan Coils, VRF indoor units, Induction Beams and Chilled Beams, heating capability can be included by checking the "heating coil" box, or can be excluded by
unchecking this box. For 4-Pipe Fan Coils and Water Source Heat Pumps the terminal unit must include a heating coil. When a heating coils is included, three items
must be defined:
a. Design Supply Temperature is used to size the terminal unit airflow rate in heating-only units. Otherwise it influences fan cycling and coil capacity control..
b. Heat Source specifies how heating is provided to the coil.
c. Schedule defines the months of the year when the heating coil is permitted to operate.
3. Fan Control Data specifies how the cooling and heating capacities of the terminal unit are controlled. The terminal unit fan can be cycled to modulate cooling and
heating output. When the fan is not cycled, output is modulated by cycling the compressor in DX units, or controlling water flow or temperature in hydronic units. This
input is not applicable for Induction Beams and Active Chilled Beams.
4. Outdoor Ventilation Air Data defines the method for sizing ventilation airflow to the terminal units. This item only appears when "direct ventilation" was specified for the
system. When a Dedicated Outdoor Air System (DOAS) unit is used, ventilation sizing method is described separately on the DOAS Components tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Terminal Unit Cooling Coil Data
Cooling Coil Data describes sizing and operating characteristics of the cooling components in the terminal unit. When a cooling coil is included in the unit, up to four
items must be defined:
1. Design Supply Temperature. This is the design cooling supply air temperature delivered by the terminal unit. It is used to calculate the required terminal unit airflow
rate. When fan cycling is used, the terminal unit delivers air at this design temperature while the fan is on. When fan cycling is not used, the design supply temperature
is the minimum supply temperature for the unit.
2. Coil Bypass Factor is used to evaluate dehumidification occurring at the cooling coil. In general, the bypass factor is a measure of the approach to the apparatus dew
point (ADP) for air flowing through the coil. The smaller the bypass factor, the closer the outlet air approaches the ADP state. The coil bypass factor may be known
from product literature when modeling specific equipment. When equipment has not yet been selected, specify a bypass factor that is representative of the type of
equipment you intend to select (e.g., packaged DX fan coil, hydronic fan coil, etc…).
Note: Cooling coil bypass factor is not shown here for Induction Beam and Active Chilled Beam systems. Instead it is defined for these systems on the Terminal Units
data view.
3. Cooling Source describes how cooling is provided to the coil. For DX fan coils and heat pumps, the cooling source must be "DX". For hydronic fan coils, the cooling
source must be "chilled water".
4. Schedule defines the months of the year in which the cooling coil operates. The schedule consists of a series of twelve buttons, one for each month. To turn the coil
on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from April through October; it is off during the
remaining months.
Page 41 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Common Terminal Unit Heating Coil Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.6 Common Terminal Unit Data ››
Common Terminal Unit Fan Control Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.6 Common Terminal Unit Data ››
Common Terminal Unit Ventilation Data
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.6 Common Terminal Unit Data ››
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses chilled water cooling and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Terminal Unit Heating Coil Data
Heating Coil Data describes sizing and operating characteristics of the heating components in the terminal unit. When a heating coil is included in the terminal unit, three
items must be defined:
1. Design Supply Temperature. This is the design heating supply air temperature delivered by the terminal unit. For heating-only units, it is used to calculate the
required terminal unit airflow rate. When fan cycling is used, the terminal unit delivers air at this design temperature while the fan is on. When fan cycling is not used,
the design supply temperature is the maximum heating supply temperature for the unit.
2. Heating Source describes how heating is provided to the coil. Options in this drop-down list vary depending on terminal unit type. The overall list of options includes
electric resistance, natural gas combustion, fuel oil combustion, propane combustion, hot water, steam and heat pump heating. In system design, the heating source
influences sizing calculations for boiler plants. For example, loads for a hot water heating coil are considered when sizing a hot water boiler linked to the air system. In
the energy analysis, heating source influences building energy consumption. For example, loads for electric resistance heating coils are added to the building power
profile.
3. Schedule defines the months of the year in which the heating coil operates. The schedule is comprised of a series of twelve buttons, one for each month. To turn the
coil on for a month, the month’s button must be in a down position. In the figure below the coil is permitted to operate from January through April and from October
through December; it is off during the remaining months.
To change the on/off status for a month, simply click on the month’s button. For example, if the button is in a down position indicating "ON", clicking the button will
change it to an up position indicating "OFF".
Note: If the air system uses hot water or steam and changeover control, options on the Equipment Tab allow changeover to be controlled either with this monthly
schedule or a outdoor air temperature threshold. When outdoor air temperature threshold is selected, the schedule is typically defined as ON for all 12 months. If you
specify OFF months the schedule will be used in combination with the temperature threshold control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Terminal Unit Fan Control Data
This item specifies how the cooling and heating capacities of the terminal units in this system are controlled. Two options are offered:
1. Fan Cycled: The terminal unit fan is cycled to modulate cooling and heating output. During the portion of the hour the fan is on for cooling duty, air is supplied to the
zone at the design cooling supply temperature. During the portion of the hour the fan is on for heating duty, air is supplied to the zone at the design heating supply
temperature.
2. Fan On: During the "occupied" system operating period, the supply fan runs continuously to condition and ventilate the zone. In DX terminal units, the compressor is
cycled or staged to control cooling capacity. In hydronic terminal units the water flow to the coil, or the water supply temperature to the coil is regulated to reset the
supply air temperature to meet the zone load. For electric resistance and combustion heating, the coils are cycled to modulate heating. In the "unoccupied" system
operating period, the terminal unit is cycled to meet cooling and heating demands.
Note: This input is not applicable for Induction Beam and Active Chilled Beam system since terminals in those systems do not contain a fan.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Terminal Unit Ventilation Data
This item defines the method used to size outdoor ventilation airflow to each terminal unit in the system. This item only appears when "direct ventilation" is specified for
the system. When a Dedicated Outdoor Air System (DOAS) unit is used ventilation is described separately on the DOAS Components tab.
Two sizing methods are offered - the "Sum of Space OA Airflows" method and the ASHRAE Standard 62 method previously selected for the project on the
View/Preferences screen. In all cases the ventilation calculation will be performed separately for each fan coil, water source heat pump, VRF indoor unit or induction
terminal since each represents a self-contained air system supplied with its own ventilation air.
1. Sum of Space OA Airflows – This method calculates the design ventilation airflow for a terminal unit zone by summing the outdoor airflow requirements for all spaces
in the zone. Certain ventilation standards and codes use this approach. This approach is also typically used when the building is not subject to a ventilation standard
or code.
2. ASHRAE Standard 62-2001 – This method calculates design ventilation airflow using the Ventilation Rate Procedure documented in section 6.1 of the Standard. When
a fan coil or terminal heat pump unit serves more than one space the multiple space equation, equation 6-1, is used.
3 thru 7. ASHRAE Standard 62.1 editions 2004 through 2016.
These methods calculate required ventilation airflow using the Ventilation Rate Procedure documented in section 6.2 of the indicated version of Standard 62.1. When
the system serves more than one space, material from Appendix A – Multiple-Zone Systems is also used in the calculation. Only one of these options will appear,
depending on the project preference for Ventilation Standard. For example, if you choose Standard 62.1-2016 as the project preference, only 62.1-2016 will appear as
an option for ventilation sizing method. The choice of a Ventilation Standard can be changed via the Preferences option on the View menu.
Page 42 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.4.7 Terminal Unit Data
11.0 Entering Systems ›› 11.4 Zone Components Data ››
Terminal Units Data - Induction Terminals
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.7 Terminal Unit Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for terminal units in a terminal system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Units Data - Induction Terminals
This Terminal Units data view contains information about induction terminals: induction beams or active chilled beams. This is the second of two data views describing
characteristics of the terminal units. The Common Data view contained one set of specifications common to all terminal units in the system. Information in this data view
can be specified either on a zone-by-zone basis or as common to all terminal units in the system. In this data view information for one zone is shown at a time. The upper
portion of the data view is used to control the display of zone data:
1. All Zones are the Same specifies whether one set of data will apply to all zones in the system, or whether data will be defined on a zone-by-zone basis. When this
box is checked, only one set of terminal data will be defined and it will apply to all zones in the system. When this box is not checked, a separate set of data will
appear for each zone in the system.
2. Zone Controls. The Zone Name identifies the zone whose data is currently shown in the data view. In the figure above, data for the D102-Classroom zone is shown.
The zone name is part of a drop-down list which can be used to display data for any other zone in the system. Or, you can press the right and left arrow buttons above
the zone name to step forward or backward sequentially through your list of zones. The zone number is shown above the zone name to provide reference. Note that
when the "All Zones are the Same" box is checked, the zone name will be "All Zones" indicating common data for all zones is shown. Also note that the zone name
cannot be modified in this data view. It can only be modified on the Space Assignments data view.
The remaining items on this screen describe the supply terminal characteristics.
1. Terminal Type defines the kind of terminal used in the zone. This will be set based on the system type to "Induction Beam" or to "Active Chilled Beam".
2. Air Distribution defines the locations of the supply air discharge into the zone and the return grille for air leaving the zone.
3. Air Distribution Effectiveness inputs appear when the ventilation sizing method specified for the air system is one of the ASHRAE Standard 62.1 Ventilation Rate
Procedure options. These inputs assist in defining the proper air distribution effectiveness (Ez) factors used for the terminal in the Ventilation Rate Procedure
calculation.
If you select the ASHRAE 62.1 option in the drop-down list, HAP will automatically determine Ez based on the mode of operation (cooling or heating), the type of
terminal, the heating supply temperature, the zone thermostat setpoint, and the location of supply discharge and return grille, using data in the Zone Air Distribution
Effectiveness table in Standard 62.1 (Table 6-2 in the 2004 through 2010 editions. Table 6.2.2.2 in the 2013 and 2016 editions).
If you select the User Defined option in the drop-down list, you will directly specify the Ez value in the cell to the right of the drop-down list. This value will then be
used in the Ventilation Rate Procedure calculation.
4. Coil Bypass Factor is used to evaluate dehumidification occurring at the cooling coil. In general, the bypass factor is a measure of the approach to the apparatus dew
point (ADP) for air flowing through the coil. The smaller the bypass factor, the closer the outlet air approaches the ADP state. The coil bypass factor may be known
from product literature when modeling specific equipment. When equipment has not yet been selected, specify a bypass factor that is representative of the type of
equipment you intend to select.
Note: This input only applies to Induction Beam terminals. Induction Beams are designed for total cooling (sensible and latent) so dehumidification performance must
be defined. Active Chilled Beam terminals are sensible-only cooling devices so dehumidification performance is not relevant.
5. Airflow Ratio is the ratio of total supply air to primary air delivered by an induction terminal.
Example: A particular type of Induction Beam terminal has an airflow ratio of 4.0. For a given zone, the primary supply air to the terminal is 150 CFM. Therefore the
total supply air discharged from the terminal grille will be 150 CFM x 4 = 600 CFM, of which 150 CFM is primary air and 450 CFM is induced room air.
Note that induction terminal manufacturers tabulate airflow performance in several different ways. Therefore to accurately define performance for the equipment
you're modeling its important to understand how a specific manufacturer defines airflow ratio and supply air. In HAP, airflow ratio performance is total supply air
divided by primary air. Here "supply air" refers to air discharged from the terminal grill. Some manufacturers tabulate supply air considering the additional room air
induced after air discharges from the terminal grille. This airflow should not be included in the airflow ratio defined in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 43 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Terminal Units Data - Fan Coil Terminals
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.7 Terminal Unit Data ››
Terminal Units - Terminal Type
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.7 Terminal Unit Data ››
Terminal Units - Minimum Airflow
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.7 Terminal Unit Data ››
Terminal Units Data - Fan Coil Terminals
This Terminal Units data view contains information for terminals containing a fan: fan coil units, water source heat pump units or VRF indoor units in the system. This is
the second of two data views describing characteristics of the terminal units. The Common Data view contained one set of specifications common to all terminal units in
the system. Information in this data view can be specified either on a zone-by-zone basis or as common to all terminal units in the system.
In this data view the upper portion is used to control the display of zone data:
1. All Zones are the Same specifies whether one set of data will apply to all zones in the system, or whether data will be defined on a zone-by-zone basis. When this
box is checked, only one set of terminal data will be defined and it will apply to all zones in the system. When this box is not checked, a separate set of data will
appear for each zone in the system.
2. Zone Selection. The Zone Name identifies the zone whose data is currently shown in the data view. In the figure above, data for the D102-Classroom zone is shown.
The zone name is part of a drop-down list which can be used to display data for any other zone in the system. Or, you can press the right and left arrow buttons above
the zone name to step forward or backward sequentially through your list of zones. The zone number is shown above the zone name to provide reference. Note that
when the "All Zones are the Same" box is checked, the zone name will be "All Zones" indicating common data for all zones is shown. Also note that the zone name
cannot be modified in this data view. It can only be modified on the Space Assignments data view.
The remaining items on this screen describe supply terminal characteristics:
1. Terminal Type defines the kind of terminal unit used in the zone. In all cases the terminal type is set to "fan coil" meaning a terminal unit containing a fan and a cooling
and/or heating coil.
2. Air Distribution defines the location of the supply air discharge and return air grille in the zone.
3. Air Distribution Effectiveness inputs appear when the ventilation sizing method specified for the air system is one of the ASHRAE Standard 62.1 Ventilation Rate
Procedure options. These inputs assist in defining the proper air distribution effectiveness (Ez) factors used for the terminal in the Ventilation Rate Procedure
calculation.
4. Minimum Airflow specifies the minimum supply airflow requirement for the zone. During sizing calculations, HAP will make sure the terminal is sized for at least this
amount of airflow.
5. Fan Full Load Performance describes the performance of a terminal unit fan at its full airflow condition. This data is used to determine fan heat gain and motor input
power.
6. Efficiency defines the efficiency of a terminal mixing box fan. Overall efficiency is required when total static pressure is specified. Motor efficiency is required when
BHP is defined.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Units - Terminal Type
This item describes the type of terminal used for the zone. In all cases the terminal type is set to "fan coil" meaning a terminal unit containing a fan and a cooling and/or
heating coil.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Units - Minimum Airflow
This item specifies the minimum supply airflow rate required for the zone. During sizing calculations HAP will compare the required zone airflow rate based on peak zone
and space sensible loads with the minimum airflow specified here. The larger value will be assigned to the zone.
Minimum airflow for the zone can be specified in three ways listed below. To change the units of measure for this input item, choose the desired units from the drop-down
list to the right of this input.
Page 44 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Terminal Units - Fan Inputs
11.0 Entering Systems ›› 11.4 Zone Components Data ›› 11.4.7 Terminal Unit Data ››
11.5 Sizing Data
11.0 Entering Systems ››
Sizing Data Tab / System Form
11.0 Entering Systems ›› 11.5 Sizing Data ››
1. CFM or L/s - Minimum airflow is specified directly. Note: When you have specified that "all zones are the same", be careful using these units of measure since the
airflow you enter will be used for all zones in the system.
2. CFM/sqft or L/s/sqm- Minimum airflow is calculated by multiplying your input value by the total floor area in the zone.
3. CFM/person or L/s/person - Minimum airflow is calculated based on the maximum number of occupants in the zone.
Example: Minimum airflow of 25 CFM/person is specified for a zone. The maximum number of occupants in the zone is 40. Based on the peak zone sensible load, the
required supply airflow rate is 854 CFM. However, the minimum required airflow is 25 CFM/person x 40 people = 1000 CFM. Therefore, the design supply airflow rate for
the zone will be 1000 CFM instead of 854 CFM.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Units - Fan Inputs
Operating characteristics for the terminal unit fan are specified with two input items:
1. Full Load Fan Performance - Full load fan performance must be known in order to calculate fan heat gain and energy use. Full load performance can be specified in
one of three ways listed below. To enter performance data, first select the desired units of measure from the drop down list and then enter the performance value.
a. Total Static describes the total static pressure across the fan. It is used with the overall fan efficiency to calculate fan motor input power and fan heat gain.
b. BHP defines the fan motor brake horsepower. It is used with fan motor efficiency to determine fan motor input power and fan heat gain.
c. Motor kW specifies the input power to the fan motor. It is used to determine fan heat gain.
d. W/CFM (W/L/s) describes the motor input watts per CFM or L/s delivered by the fan at its design condition.
e. 90.1 App G Fan KW specifies the program should automatically determine the fan input kW using the calculation specified in ASHRAE Standard 90.1 Appendix G,
section G3.1.2.9 and Table G3.1.2.9. The particular calculation procedure used depends on the Energy Standard preference set for the current project - either
ASHRAE 90.1-2004, 90.1-2007, or 90.1-2010.
The "90.1 App fG Fan kW" option is intended for use when you are modeling air systems for a baseline building in a LEED Energy and Atmosphere Prerequisite 2
or Credit 1 analysis. For further information on how this option is used in calculations, please refer to the fan calculation documentation.
2. Fan Efficiency - If total static is specified as the fan performance value, the overall fan efficiency must also be defined. The overall efficiency is a combined value of
the fan mechanical, drive and motor efficiencies. The overall efficiency is used together with the total static pressure to calculate fan motor input power and fan heat
gain. When fan performance is defined in terms of BHP the fan motor efficiency must be specified. It is used with BHP to calculate fan motor power and heat gain.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Sizing Data tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Sizing Data Tab / System Form
About Sizing Data. The Sizing Data tab on the System Form contains two types of information: (1) specifications for how the system is to be sized and (2) system and
zone sizing data. Sizing specifications are required in all cases, but system and zone sizing data is normally calculated by HAP. However, sizing data can be entered
directly for retrofit applications or situations in which the performance of an existing system is being studied.
The Sizing Data Tab is divided into two panels which occupy the left-hand and right-hand portions of the tab. Features in these two panels are used to enter sizing
specifications and data.
Page 45 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.5.1 System Sizing Data
11.0 Entering Systems ›› 11.5 Sizing Data ››
System Sizing Data
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.1 System Sizing Data ››
System Sizing Values
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.1 System Sizing Data ››
1. Checklist Panel. The left-hand panel contains a checklist for the two types of sizing data: system sizing data and zone sizing data. Systems normally contain both
types of data. To display system sizing data, click on the System Sizing item. To display zone sizing data, click on the Zone Sizing item. In the figure above system
sizing data is displayed.
This panel is also used to specify whether system sizing data is to be calculated by HAP or directly entered by the user. Normally, the "computer-generated" option is
selected so HAP will perform the sizing calculations itself. When "computer-generated" is selected, the system and zone sizing data items on this tab will be disabled
(displayed in gray). However, for retrofit applications and when studying the performance of existing systems, the "user-defined" option can be used to directly enter
sizing data. When "user-defined" is selected system and zone sizing items on the tab will be enabled (displayed with a white background).
2. Data Panel. The right-hand panel contains views of system sizing or zone sizing data, depending on which category was selected in the checklist panel. In the figure
above, system sizing data is displayed.
Further information on each data view offered on this tab can be found in the following help topics:
System Sizing Data.
Zone Sizing Data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for system level sizing.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Sizing Data
The System Sizing Data view contains general system sizing parameters. When directly entering system sizing data, it is also used to specify central fan and ventilation
airflow rates and central supply temperatures. This data view is divided into three sections:
1. Sizing Data contains information about design supply temperatures, the central fan airflow rate and the system ventilation airflow rate. These items are only enabled
when sizing data is to be user-defined. Items are blank if sizing calculations have not yet been performed. Items display values if calculations have been performed
previously or data is being entered by the user.
2. Hydronic Sizing Specifications define the delta-T values used for sizing water flow in hydronic cooling and heating coils in the system.
3. Safety Factors provide separate factors for increasing zone sensible cooling loads, zone latent cooling loads and zone heating loads to provide a margin of safety in
system design.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
System Sizing Values
This section of the system sizing data view contains information about design supply temperatures, fan airflow rates and the system ventilation airflow rate. These items
are only enabled when sizing data is user-defined. Items are blank when sizing calculations have not yet been performed. Items contain values when calculations have
been performed previously, or data is being entered directly by the user.
The following items are found in this section:
1. Cooling Supply Temperature is the design supply air temperature for cooling operation. It refers to the temperature of air delivered to zone terminals. When duct
heat gain is considered in a system, the temperature of air leaving the central air handler will be colder than this design supply temperature.
In 2-Deck Multizone, 3-Deck Multizone, CAV-Dual Duct and VAV-Dual Duct systems this item is titled "Cold Deck Supply Temperature". It refers to the temperature of
cold deck supply air delivered to zone terminals.
Page 46 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Hydronic Sizing Specifications
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.1 System Sizing Data ››
Safety Factors
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.1 System Sizing Data ››
11.5.2 Zone Sizing Data
11.0 Entering Systems ›› 11.5 Sizing Data ››
Zone Sizing Data
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.2 Zone Sizing Data ››
In Terminal Unit systems, this item is the common cooling supply temperature for all fan coil, heat pump or induction terminal units in the system.
2. Supply Airflow Rate is the design airflow rate delivered by the central supply fan. In a 2-Fan Dual Duct system this refers to the design airflow rate for the cooling
supply fan. This item is not applicable for terminal unit systems.
3. Ventilation Airflow Rate is the design outdoor ventilation airflow rate for the system. This item is not applicable for terminal unit systems. Instead, zone-by-zone
ventilation airflow data is displayed on the Zone Sizing Data view for these types of systems.
4. Heating Supply Temperature is the design supply air temperature for heating operation. It refers to the temperature of air delivered to zone terminals. When duct
heat loss is considered in a system, the temperature of air leaving the central air handler will be warmer than this design supply temperature.
In 2-Deck Multizone, 3-Deck Multizone, CAV-Dual Duct and VAV-Dual Duct systems this item is titled "Hot Deck Supply Temperature". It refers to the temperature of
hot deck supply air delivered to zone terminals.
In Terminal Unit systems, this item is the common heating supply temperature for all fan coil, heat pump, or induction terminal units in the system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Hydronic Sizing Specifications
This section of the System Sizing Data view provides specifications for sizing water flow rates in hydronic cooling and heating coils in the system. The section contains
two input items:
1. Chilled Water Delta-T defines the temperature difference between water leaving and entering a cooling coil. It is used together with the peak coil load to determine
the required water flow rate for the coil. Note that this value is used to size water flow rate for all cooling coils whose cooling source is "chilled water". When a system
does not contain hydronic cooling coils, this input is not used.
2. Hot Water Delta-T defines the temperature difference between water entering and leaving a heating coil. It is used together with the peak coil load to determine the
required water flow rate for the coil. Note that this value is used to size water flow rate for all heating coils in the system whose heat source is "hot water". When a
system does not contain hot water heating coils, this input is not used.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Safety Factors
Safety Factors are used in sizing calculations to provide a margin of safety in the design. In HAP, inputs for three different safety factors are provided:
1. Sensible Cooling Factor is used in cooling design calculations to increase zone sensible cooling loads before cooling supply airflow rates and coil loads are
calculated.
2. Latent Cooling Factor is used in cooling design calculations to increase zone latent cooling loads before coil loads are calculated.
3. Heating Factor is used in heating design calculations to increase zone heating loads before heating supply airflow rates and coil loads are calculated.
Example. Safety factors of 15% cooling sensible and 10% cooling latent are specified. Given these safety factors, all space sensible cooling loads are multiplied by 1.15.
All space latent cooling loads are multiplied by 1.10. Because zone airflow and fan airflow rates are determined from room sensible loads, this will inflate system airflow
rates by 15%. It will also inflate the cooling coil sensible since larger zone loads and fan heat gains must be handled. The 10% latent factor will also increase the cooling
coil load because of the increased system moisture levels.
Application Information. There are at least two schools of thought in the industry regarding safety factors:
a. Those supporting one school include the safety factors in the system inputs so a margin of safety is included in the sizing calculation. Equipment is then selected that
has airflow and coil capacity equal to or greater than the calculated values. Since the calculated values already include a safety margin, equipment selected in this
way also includes the margin of safety.
Example: 10% sensible and latent cooling safety factors are specified in system inputs. Therefore zone sensible and latent loads are increased by 10% during HAP
sizing calculations. The resulting peak cooling coil load is 48.7 tons. Because equipment being selected is only manufactured in 45 and 50-ton sizes, the 50-ton unit is
selected since it is the next larger size. Because the 48.7 ton estimate already included safety factors, the 50-ton unit selection includes a sufficient margin of safety.
b. Those supporting the second school of thought incorporate the margin of safety in the equipment selection process rather than the sizing calculation. These designers
prefer to perform sizing calculations without safety factors so calculation results will be "pure". When equipment is selected, it is chosen so that it provides at least a
predetermined margin of safety above the calculated sizing values.
Example: HAP sizing calculations are performed without safety factors. The peak cooling coil load is 43.1 tons. Because the designer wishes to include a 10% margin
of safety in the design, equipment with a capacity of at least 47.4 tons must be selected. Equipment is available in 45 ton and 50 ton capacities. The 50-ton unit is
selected because it is the first size that provides a margin of safety of 10% or more.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for zone level sizing.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Sizing Data
Page 47 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Zone and Space Airflow Sizing Methods
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.2 Zone Sizing Data ››
The Zone Sizing Data view contains information about zone and space airflow sizing procedures for the system. When directly entering sizing data, it is also used to
specify zone airflow rates, reheat coil capacities, zone heating unit capacities and mixing box fan airflow rates. This data view is divided into two sections:
1. Sizing Method. The upper portion of the data view contains items specifying the method used to size zone airflow rates and space airflow rates in the system.
2. Zone Data Table. The remainder of the data view consists of a table of zone sizing parameters. This table is enabled only when sizing data is "user-defined". Cells in
the table will be blank if sizing calculations have not yet been performed for a system. Cells in the table will contain values if sizing calculations have already been
performed, or the sizing data is user-defined.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone and Space Airflow Sizing Methods
The upper portion of the Zone Sizing Data view contains two items specifying the calculation methods used to size zone airflow rates and space airflow rates in the
system. To specify sizing methods, choose the desired options from the drop-down lists. The choice of the zone sizing method determines the choices offered for the
space sizing method. Each possible combination of methods is explained below.
Note: This data is not displayed for induction beam and active chilled beam systems since these two systems size primary air based on ventilation requirements.
Readers should also note the zone sizing methods discussed below only apply if the supply air sizing criteria is "supply temperature". When CFM (L/s) or CFM/sqft
(L/s/sqm) is used as the sizing criteria, zone airflow is calculated from these criteria rather than from zone loads or space airflows.
1. Zone Method = Peak Zone Sensible Load
Space Method = Coincident Space Loads
The design supply airflow rate for each zone is calculated using the peak zone sensible load for the zone. The zone airflow is then divided among spaces in the zone
on the basis of space sensible cooling loads for the month and hour when the zone load peaks.
Example: A zone has a maximum sensible load of 21600 BTU/h and a required airflow rate of 1000 CFM. This maximum zone load occurs at August 1600. Further,
this zone contains two spaces. At August 1600, the spaces have sensible cooling loads of 8000 BTU/h and 13600 BTU/h respectively.
The required airflow for the first space will be:
(1000 CFM) x (8000 BTU/h)/(21600 BTU/h) = 370 CFM.
The required airflow for the second space will be:
(1000 CFM) x (13600 BTU/h)/(21600 BTU/h) = 630 CFM.
It is important to note that space loads at August 1600 are used in this example calculation even if larger space loads exist at other times.
2. Zone Method = Peak Zone Sensible Load
Space Method = Individual Peak Space Loads
The design supply airflow rate for each zone will be calculated using the peak zone sensible load for the zone. Space airflow rates will be calculated based on the
peak sensible load for each individual space.
When peak loads for all spaces occur at the time the zone peak occurs, the sum of the space airflow rates will equal the zone airflow rate. If the spaces experience
peak loads at different times, then the sum of the space airflow rates will exceed the required zone airflow rate. In such a situation, the ductwork between the zone
terminal and the space diffusers will have excess airflow capacity. The example below illustrates such a situation.
Example: A zone has a maximum sensible load occurring at August 1600 which requires an airflow of 1000 CFM. The zone contains two spaces. One space has a
peak sensible load at August 1300 that requires an airflow of 550 CFM. The second space has a peak sensible load at August 1700 that requires an airflow of 600
CFM.
3. Zone Method = Peak Zone Sensible Load
Space Method = Zone CFM/sqft or L/s/sqm
The zone supply airflow rate is calculated from the maximum zone sensible load. This airflow is divided among spaces in the zone on the basis of zone CFM/sqft or
L/s/sqm and space floor area.
Example: Based on the maximum zone sensible load, a zone has a required airflow rate of 1000 CFM. The zone contains two spaces of 600 sqft and 900 sqft floor
area, respectively. Therefore, the overall zone CFM/sqft is 0.67 CFM/sqft.
The required airflow for the first space will be (600 sqft) x (0.67 CFM/sqft) = 400 CFM.
The required airflow for the second space will be (900 sqft) x (0.67 CFM/sqft) = 600 CFM.
4. Zone Method = Sum of Space Airflow Rates
Page 48 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Zone Sizing Data Table
11.0 Entering Systems ›› 11.5 Sizing Data ›› 11.5.2 Zone Sizing Data ››
11.6 Equipment Data
11.0 Entering Systems ››
Equipment Tab / System Form
11.0 Entering Systems ›› 11.6 Equipment Data ››
Space Method = Individual Peak Space Loads
The design supply airflow rate for each space is calculated based on the peak sensible load in the space. The zone supply airflow rate is the sum of design airflow
rates for spaces in the zone.
Example: A zone contains two spaces. One has a peak sensible load at August 1300 that requires an airflow of 550 CFM. The second space has a peak sensible load
at August 1700 that requires an airflow of 600 CFM. Therefore, the required zone airflow rate is 1150 CFM.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Zone Sizing Data Table
The lower portion of the Zone Sizing Data view contains information about zone supply airflow rates, reheat coil capacities, zone heating unit capacities and fan powered
mixing box fan airflows. For terminal units it also includes information about outdoor ventilation air supplied to each zone. Zone sizing data is displayed in a table in which
each row contains data for a different zone and each column contains data for a different sizing attribute.
Cells in the table will be disabled (gray) when sizing data is computer-generated. Cells will be enabled and may be modified when sizing data is user-defined. Cells in the
table will be blank if sizing calculations have not yet been performed. Cells will contain values if sizing calculations have been performed previously, or data was entered
by the user.
The following items are found in this table:
1. Supply Airflow CFM or L/s defines the design supply airflow rate for this zone. In terminal unit systems it defines the design airflow provided by the fan coil or heat
pump terminal unit in the zone. For induction beam and active chilled beam terminals this column is disabled and does not apply.
2. Zone Htg Unit BTU/hr or W specifies the required capacity for a supplemental heating unit located in the zone. These are baseboard or fan coil heating units
controlled either by an outdoor thermostat or a room thermostat. This cell is disabled and shown as blank if the zone does not include a zone heating unit. Also, this
item is not applicable for terminal unit systems.
3. Reheat Coil BTU/hr or W defines the required capacity for a terminal reheat coil in the supply terminal in this zone. This cell is disabled and shown as blank if the
zone does not include a terminal reheat coil. Also, this item is not applicable for terminal unit systems.
4. FPMBX Fan CFM or L/s lists the required airflow rate for a terminal fan in a parallel fan powered mixing box. This cell is disabled and shown as blank for any zone
which does not contain a parallel mixing box terminal.
5. Ventilation CFM or L/s. For terminal unit systems such as fan coils, VRF, induction beam, active chilled beam and water source heat pumps, the "FPMBX Fan"
column is replaced with ventilation air data. Each cell in this column contains the outdoor ventilation airflow assigned to the zone. When direct ventilation is used, this
is the flow rate for outdoor ventilation air introduced at the terminal unit. When a Dedicated Outdoor Air System (DOAS) is used, this is the flow rate of outdoor
ventilation air delivered by the DOAS unit to each zone terminal. For induction beam and chilled beam systems, this is also the primary air supplied to the induction
terminals.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Equipment Data tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Tab / System Form
About Equipment Data. An Air System is defined as the equipment and controls which provide cooling and heating to a region of a building. This definition is tightly
linked to equipment. For example, a Packaged Rooftop air system includes all the components in the packaged unit, plus the ductwork, air terminals and controls.
Therefore, the DX cooling apparatus and any heat pump, combustion or electric resistance heating apparatus in the packaged unit is considered part of the air system.
Performance data for these components is defined in system inputs. Energy use by these components will be calculated during the system simulation phase of an energy
analysis.
The Equipment tab contains information about DX cooling, heat pump, and combustion heating components of an air system. Electric resistance heat is simply specified
as a heating source on an earlier tab and does not require further inputs so it is not included here.. This information is only relevant when performing energy analyses.
When running the program in System Design Load mode, this tab does not appear.
Note that when cooling is provided by chilled water or heating is provided by hot water or steam, the machinery providing the cooling or heating is external to the system.
It is therefore defined as a plant which serves the air system.
Page 49 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Precool Unit - Air-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
The Equipment Tab consists of a series of items on the right and an Edit button opposite each on the left. The number of items which appear on this tab depend on the
type of equipment being described and the cooling and heating sources specified earlier in the system form. The example above shows a packaged rooftop unit which
uses DX cooling and gas combustion heat. Therefore, both cooling and heating apparatus are defined as part of the system and separate line items are provided for
each on this tab.
To enter or edit equipment data, press the Edit Equipment Data button opposite the desired item. A window will appear containing input data for this equipment
component. There are 17 different items that can appear on this tab. No more than 5 appear at one time. In some cases none will appear if all cooling and heating is
supplied by plants. For information on any of these 17 categories of equipment inputs, click on the following:
Precool Unit - Air-Cooled DX Cooling
Ventilation Cooling Unit - Air-Cooled DX Cooling
Ventilation Cooling Unit - Water Cooled DX Cooling
Preheat Unit - Combustion Heating
Ventilation Heating Unit - Combustion Heating
Ventilation Heating Unit - Water Source Heat Pump
Central Cooling Unit - Air-Cooled DX Cooling
Central Cooling Unit - Water-Cooled DX Cooling
Central Heating Unit - Air Source Heat Pump
Central Heating Unit - Combustion Heating
Terminal Cooling Units - Air-Cooled DX Cooling
Terminal Cooling Units - Water-Cooled DX Cooling
Terminal Heating Units - Air Source Heat Pump
Terminal Heating Units - Water Source Heat Pump
Terminal Heating Units - Combustion
Misc. Components for Water-Cooled VPAC Systems
Misc. Components for WSHP Systems
VRF Outdoor Unit
Changeover Controller
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Precool Unit - Air-Cooled DX
This window contains performance data for air-cooled DX cooling equipment serving a precool coil. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
Page 50 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
1. Estimated Maximum Load. This display-only item lists the peak load for the precool coil. The peak load is generated during design calculations for the system. The
load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will be blank
since the data does not yet exist.
2. Design OAT is the outdoor air design temperature at which gross cooling capacity is defined. Typically the best practice is to enter the outdoor air temperature (OAT)
for the time of the peak load. Cooling capacity varies as a function of OAT. Therefore, if you accept a default or define an OAT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the DX cooling unit at its design outdoor air temperature. No deduction for fan heat is considered in this
value. This value is typically obtained from equipment selection software or product catalogs. This capacity value, together with design OAT and input power, serve as
the anchor point for off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing
input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER or SEER value. This EER or SEER includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating conditions. During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this EER,
subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition and the design OAT you specified for equipment capacity.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW is the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is used when
modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is
used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER or SEER based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity, heating type and the Energy Standard preference for the
project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated
equipment EER or SEER will be displayed on the air system input report.
7. Conventional Cutoff OAT is the outdoor air temperature above which the air-cooled DX equipment operates in a conventional fashion. For equipment with special
low ambient (head pressure) controls, the unit operates normally above this cutoff temperature and modulates the outdoor fans to maintain a constant head pressure
below this temperature. For equipment without special low ambient controls, the unit operates normally above this temperature and is off for temperatures colder than
this value.
8. Low Temperature Operation. This input specifies whether special controls are used to allow a DX cooling unit to operate at low ambient temperatures. When this
control is used, the program assumes head pressure is maintained at a constant level below the "conventional cutoff OAT". This is done by varying condenser fan
operation. On the other hand, if low temperature control is not used, the program assumes the unit will not operate below the conventional cutoff OAT. To select low
temperature operation, place a check mark in the box. If low temperature control is not used, leave the check box empty.
9. Low Temperature Cutoff OAT. When low temperature (head pressure) control is used, a low temperature cutoff temperature must be defined. For temperatures
between the "conventional cutoff OAT" and the "low temperature cutoff OAT", the DX unit operates with the special head pressure controls. Below the "low
temperature cutoff OAT" the unit is off.
Page 51 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Vent Cooling Unit - Air-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Vent Cooling Unit - Air-Cooled DX
This window contains performance data for a Dedicated Outdoor Air System (DOAS) unit containing air-cooled DX cooling equipment. Each input item in the wiindow is
described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the DOAS unit cooling coil for reference purposes. The peak load is generated during design
calculations for the system. The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system,
then this item will be blank since the data does not yet exist.
2. Design OAT is the outdoor air design temperature at which gross cooling capacity is defined. Typically the best practice is to enter the outdoor air temperature (OAT)
for the time of the peak load. Cooling capacity varies as a function of OAT. Therefore, if you accept a default or define an OAT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the DX cooling unit at its design outdoor air temperature. No deduction for fan heat is considered in this
value. This value is typically obtained from equipment selection software or product catalogs. This capacity value, together with design OAT and input power, serve as
the anchor point for off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing
input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER or SEER value. This EER or SEER includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating OAT of 95 F (35 C). During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this
EER, subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition of 95 F (35 C) and the design OAT you specified for this
equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER or SEER based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity, heating type and the Energy Standard preference for the
project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated
equipment EER or SEER will be displayed on the air system input report.
Page 52 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Vent Cooling Unit - Water-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
7. Conventional Cutoff OAT is the outdoor air temperature above which the air-cooled DX equipment operates in a conventional fashion. For equipment with special
low ambient (head pressure) controls, the unit operates normally above this cutoff temperature and modulates the outdoor fans to maintain a constant head pressure
below this temperature. For equipment without special low ambient controls, the unit operates normally above this temperature and is off for temperatures colder than
this value.
8. Low Temperature Operation. This input specifies whether special controls are used to allow a DX cooling unit to operate at low ambient temperatures. When this
control is used, the program assumes head pressure is maintained at a constant level below the "conventional cutoff OAT". This is done by varying condenser fan
operation. On the other hand, if low temperature control is not used, the program assumes the unit will not operate below the conventional cutoff OAT. To select low
temperature operation, place a check mark in the box. If low temperature control is not used, leave the check box empty.
9. Low Temperature Cutoff OAT. When low temperature (head pressure) control is used, a low temperature cutoff temperature must be defined. For temperatures
between the "conventional cutoff OAT" and the "low temperature cutoff OAT", the DX unit operates with the special head pressure controls. Below the "low
temperature cutoff OAT" the unit is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Vent Cooling Unit - Water-Cooled DX
This window contains cooling duty performance data for a Dedicated Outdoor Air System (DOAS) unit which is a water source heat pump. Each input item in the window
is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the DOAS unit cooling coil. The peak load is generated during design calculations for the
system. The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will
be blank since the data does not yet exist.
2. Design EWT is the entering water temperature at which gross cooling capacity is defined. Typically the best practice is to enter the entering water temperature (EWT)
for the time of the peak load. Cooling capacity varies as a function of EWT. Therefore, if you accept a default or define an EWT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor kW below, this kW value must correspond to the Design EWT. That is because the Design EWT is the anchor
point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum Efficiency
options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design EWT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the cooling unit at its design EWT. No deduction for fan heat is considered in this value. This value is
typically obtained from equipment selection software or product catalogs. This capacity value, together with design EWT and input power, serve as the anchor point for
off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
Page 53 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Preheat Unit - Combustion
11.0 Entering Systems ›› 11.6 Equipment Data ››
a. Compressor kW requires input of the compressor power at the design EWT specified earlier on this screen. Typically this option is used when modeling a specific
equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is used together with the
design EWT and gross capacity as the anchor point for off-design and part-load performance calculations.
b. ISO/AHRI Performance Rating allows entry of an ISO/AHRI standard EER value. This EER includes compressor power and indoor fan and pump power
allowances, and is determined at a standard rating temperature. During the energy simulation, HAP will automatically derive the compressor kW from this EER,
adjusting for the indoor fan and pump power allowances and adjusting for any difference between the ISO/AHRI rating condition and the design EWT you specified
for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the equipment type, cooling capacity and the Energy Standard preference for the project (90.1-2004,
90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment EER will
be displayed on the air system input report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Preheat Unit - Combustion
This window contains performance data for a gas, propane or oil-fired preheat coil. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the preheat coil, derived from design calculations for the system. This value provides
guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will be blank since the data
does not yet exist.
2. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be displayed on the air system input report. For energy analysis during detailed design where you are modeling a
specific equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
3. Gross Heating Capacity defines the total heating output of the unit. This value is typically obtained from equipment selection software or product catalogs. This
capacity value is used to determine whether the heating unit has sufficient capacity to meet the coil load. When the coil load is larger than the gross heating capacity,
the program will report an unmet load condition.
4. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.25) = 125 MBH (36.6 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
5. Average Efficiency defines the average performance of the unit. Two options are provided for defining this data:
a. Average Efficiency is defined as 100 x (Heating Output) / (Energy Input). Typically this option is used when modeling a specific equipment unit and efficiency ratings
can be obtained from a product catalog. The data might represent a seasonal value such as an AFUE or a steady state or thermal efficiency value at design.
Typically no further information about efficiency at part-load conditions will supplied these types of units so the latter two types of ratings must be used as an
"average" efficiency for all performance calculations. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment efficiency based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the fuel type, gross capacity and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or
90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment efficiency will be
displayed on the air system input report.
Page 54 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Vent Heating Unit - Combustion
11.0 Entering Systems ›› 11.6 Equipment Data ››
6. Misc. Electric defines input power for electrical components in the combustion unit such as combustion blowers and fuel oil pumps. During simulation calculations the
program will calculate energy use by these components as a function of part-load ratio. That is, at 60% load, 60% of the specified miscellaneous electric power will be
consumed. This assumes the electrical components cycle based on the heating load and therefore that energy use is proportional to the part-load ratio.
For those cases where electrical components are not used or you do not wish to consider them, specify a zero value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Vent Heating Unit - Combustion
This window contains performance data for a gas, propane or oil-fired heating coil in a Dedicated Outdoor Air System (DOAS) unit. Each input item in the window is
described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the DOAS unit heating coil, derived from design calculations for the system. This value
provides guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will be blank since the
data does not yet exist.
2. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be displayed on the air system input report. For energy analysis during detailed design where you are modeling a
specific equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
3. Gross Heating Capacity defines the total heating output of the unit. This value is typically obtained from equipment selection software or product catalogs. This
capacity value is used to determine whether the heating unit has sufficient capacity to meet the coil load. When the coil load is larger than the gross heating capacity,
the program will report an unmet load condition.
4. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross heating capacity to 100 x (1.25) = 125 MBH (36.6 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
5. Average Efficiency defines the average performance of the unit. Two options are provided for defining this data:
a. Average Efficiency is defined as 100 x (Heating Output) / (Energy Input). Typically this option is used when modeling a specific equipment unit and efficiency ratings
can be obtained from a product catalog. The data might represent a seasonal value such as an AFUE or a steady state or thermal efficiency value at design.
Typically no further information about efficiency at part-load conditions will supplied these types of units so the latter two types of ratings must be used as an
"average" efficiency for all performance calculations. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment efficiency based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the fuel type, gross capacity and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or
90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment efficiency will be
displayed on the air system input report.
6. Misc. Electric defines input power for electrical components in the combustion unit such as combustion blowers and fuel oil pumps. During simulation calculations the
program will calculate energy use by these components as a function of part-load ratio. That is, at 60% load, 60% of the specified miscellaneous electric power will be
consumed. This assumes the electrical components cycle based on the heating load and therefore that energy use is proportional to the part-load ratio.
For those cases where electrical components are not used or you do not wish to consider them, specify a zero value.
Page 55 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Vent Heating Unit - WSHP
11.0 Entering Systems ›› 11.6 Equipment Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Vent Heating Unit - WSHP
This window contains heating duty performance data for a Dedicated Outdoor Air System (DOAS) unit which is a water source heat pump. Each input item in the window
is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the DOAS unit heating coil. The peak load is generated during design calculations for the
system. The load provides guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will
be blank since the data does not yet exist.
2. Design EWT is the entering water temperature at which gross heating capacity is defined. Typically the best practice is to enter the entering water temperature (EWT)
for the time of the peak load. Heating capacity varies as a function of EWT. Therefore, if you accept a default or define an EWT warmer than the actual design value,
you increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor kW below, this kW value must correspond to the Design EWT. That is because the Design EWT is the anchor
point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum Efficiency
options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design EWT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity is then shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
4. Gross Heating Capacity defines the total heating output of the unit at its design EWT. This value is typically obtained from equipment selection software or product
catalogs. This capacity value, together with design EWT and input power, serve as the anchor point for off-design and part-load performance calculations. This input is
only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.25) = 125 MBH (36.6 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. ISO/AHRI Performance Rating allows entry of an ISO/AHRI standard COP value. This COP includes compressor power and indoor fan and water pump power
allowances, and is determined a standard rating temperature. During the energy simulation, HAP will automatically derive the compressor kW from this COP,
adjusting for the indoor fan and pump power allowances and adjusting for any difference between the ISO/AHRI rating condition and the design EWT you specified
for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor kW requires input of the compressor power at the design EWT specified earlier on this screen. Typically this option is used when modeling a specific
equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is used together with the
design EWT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment COP based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the equipment type and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or 90.1-2010)
to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment COP will be displayed on the air
system input report.
Note: When this heat pump is used in a WSHP system, auxiliary heating is provided by the auxiliary boiler attached to the water loop. When the heat pump is used in a
GWSHP or GSHP system, it is assumed the heat pump contains an electric auxiliary heating coil.
Page 56 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Central Clg Unit - Air-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Central Clg Unit - Air-Cooled DX
This window contains performance data for air-cooled DX cooling equipment serving a central cooling coil. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the central cooling coil. The peak load is generated during design calculations for the system.
The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will be blank
since the data does not yet exist.
2. Design OAT is the outdoor air design temperature at which gross cooling capacity is defined. Typically the best practice is to enter the outdoor air temperature (OAT)
for the time of the peak load. Cooling capacity varies as a function of OAT. Therefore, if you accept a default or define an OAT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the DX cooling unit at its design outdoor air temperature. No deduction for fan heat is considered in this
value. This value is typically obtained from equipment selection software or product catalogs. This capacity value, together with design OAT and input power, serve as
the anchor point for off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing
input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER or SEER value. This EER or SEER includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating OAT of 95 F (35 C). During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this
EER, subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition of 95 F (35 C) and the design OAT you specified for this
equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER or SEER based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity, heating type and the Energy Standard preference for the
Page 57 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Central Clg Unit - Water-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated
equipment EER or SEER will be displayed on the air system input report.
7. DX System Configuration specifies whether the DX unit uses 1-stage cooling or 2-stage cooling. 1-stage cooling cycles the compressor between on and off to match
the cooling load. 2-stage cooling cycles between high stage and low stage, or low stage and off to match the cooling load..
8. Conventional Cutoff OAT is the outdoor air temperature above which the air-cooled DX equipment operates in a conventional fashion. For equipment with special
low ambient (head pressure) controls, the unit operates normally above this cutoff temperature and modulates the outdoor fans to maintain a constant head pressure
below this temperature. For equipment without special low ambient controls, the unit operates normally above this temperature and is off for temperatures colder than
this value.
9. Low Temperature Operation. This input specifies whether special controls are used to allow a DX cooling unit to operate at low ambient temperatures. When this
control is used, the program assumes head pressure is maintained at a constant level below the "conventional cutoff OAT". This is done by varying condenser fan
operation. On the other hand, if low temperature control is not used, the program assumes the unit will not operate below the conventional cutoff OAT. To select low
temperature operation, place a check mark in the box. If low temperature control is not used, leave the check box empty.
10. Low Temperature Cutoff OAT. When low temperature (head pressure) control is used, a low temperature cutoff temperature must be defined. For temperatures
between the "conventional cutoff OAT" and the "low temperature cutoff OAT", the DX unit operates with the special head pressure controls. Below the "low
temperature cutoff OAT" the unit is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Central Clg Unit - Water-Cooled DX
This window contains performance data for water-cooled DX cooling equipment serving a central cooling coil. This apparatus is found in water-cooled vertical packaged
units. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the central cooling coil. The peak load is generated during design calculations for the system.
The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will be blank
since the data does not yet exist.
2. Design EWT is the entering water temperature at which gross cooling capacity is defined. Typically the best practice is to enter the entering water temperature (EWT)
for the time of the peak load. Cooling capacity varies as a function of EWT. Therefore, if you accept a default or define an EWT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor kW below, this kW value must correspond to the Design EWT. That is because the Design EWT is the anchor
point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum Efficiency
options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design EWT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity is then displayed on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the cooling unit at its design EWT. No deduction for fan heat is considered in this value. This value is
typically obtained from equipment selection software or product catalogs. This capacity value, together with design EWT and input power, serve as the anchor point for
off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
Page 58 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Central Htg Unit - ASHP
11.0 Entering Systems ›› 11.6 Equipment Data ››
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER value. This EER includes compressor power and indoor fan, and is determined a standard rating
temperature. During the energy simulation, HAP will automatically derive the compressor kW from this EER, subtracting the indoor fan power and adjusting for any
difference between the AHRI rating condition and the design EWT you specified for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor kW requires input of the compressor power at the design EWT specified earlier on this screen. Typically this option is used when modeling a specific
equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is used together with the
design EWT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the equipment type, cooling capacity and the Energy Standard preference for the project (90.1-2004,
90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment EER will
be displayed on the air system input report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Central Htg Unit - ASHP
This window contains heating duty performance data for an air source heat pump serving the central heating coil. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the central heating coil. The peak load is generated during design calculations for the
system. The load provides guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will
be blank since the data does not yet exist.
2. Design OAT is the outdoor air design temperature at which gross heating capacity is defined. For air source heat pump equipment the practice is to specify a standard
rating condition or the outdoor air temperature (OAT) for the time of the peak load.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT, if it differs from the
standard rating condition.
3. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
4. Gross Heating Capacity defines the total heating output of the unit at its design outdoor air temperature. This value is typically obtained from equipment selection
software or product catalogs. This capacity value, together with design OAT and input power, serve as the anchor point for off-design and part-load performance
calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
Page 59 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Central Htg Unit - Combustion
11.0 Entering Systems ›› 11.6 Equipment Data ››
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.25) = 125 MBH (36.6 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard COP or HSPF value. This COP or HSPF includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating OAT of 47 F (8.3 C). During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this
COP, subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition of 47 F (8.3 C) and the design OAT you specified for this
equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment COP or HSPF based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity of the unit, auxiliary heating type and the Energy Standard
preference for the project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been
run, the calculated equipment COP or HSPF will be displayed on the air system input report.
7. Cutoff OAT is the outdoor air temperature below which the heat pump turns off and the equipment runs with 100% auxiliary heat. This cutoff temperature is dictated
by equipment operating limits, economic considerations and/or performance considerations. For example, in a heat pump using gas auxiliary heat there is often an
economic balance point below which it is more economical to run 100% gas auxiliary heat than the heat pump.
8. Type of Auxiliary Heating. Specify the type of auxiliary heating used. Choices include electric resistance, and gas, propane and oil-fired combustion. If electric
resistance is selected no further inputs will be required for auxiliary heating. If one of the combustion options is selected, the capacity, efficiency and electrical input for
the combustion heater will need to be defined.
9. Gross Heating Capacity defines the total heating output of the auxiliary heater. This value is typically obtained from equipment selection software or product catalogs.
This capacity value is used to determine whether the heating unit has sufficient capacity to meet the auxiliary load. When the heating coil load is larger than the sum of
heat pump and auxiliary heater capacities, the program will report an unmet load condition.
10. Average Efficiency is used to calculate the energy input for the auxiliary heating unit. It is defined as 100 x (Heating Output) / (Energy Input). The full load efficiency
for the combustion unit can be obtained from equipment selection software or product catalogs. Typically no further information about efficiency at part-load conditions
is supplied so this value must be used as an "average" efficiency for all performance calculations. In those situations where additional information about full and part-
load efficiencies is available it should be used to derive an average efficiency and should then be entered here. Quick Reference: ASHRAE Std 90.1 Equipment
Efficiencies
11. Misc. Electric defines input power for electrical components in the auxiliary heater such as combustion blowers and fuel oil pumps. During simulation calculations the
program will calculate energy use by these components as a function of part-load ratio. That is, at 60% load, 60% of the specified miscellaneous electric power will be
consumed. This assumes the electrical components cycle based on the heating load and therefore that energy use is proportional to the part-load ratio.
For those cases where electrical components are not used or you do not wish to consider them, specify a zero value.
12. Auxiliary Heating Upper Cutoff specifies the outdoor air dry-bulb temperature above which auxiliary heating is locked out. For example if the cutoff is 40 F (4.4 C)
and auxiliary heating is required when the OADB is 45 F (7.2 C), auxiliary heating will not turn on.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Central Htg Unit - Combustion
This window contains performance data used when combustion heating is used for the central heating coil. Each input item in the window is described below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
Page 60 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Clg Units - Air-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
1. Estimated Maximum Load. This display-only item lists the peak load for the central heating coil, derived from design calculations for the system. This value provides
guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will be blank since the data
does not yet exist.
2. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity is then displayed on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
3. Gross Heating Capacity defines the total heating output of the unit. This value is typically obtained from equipment selection software or product catalogs. This
capacity value is used to determine whether the heating unit has sufficient capacity to meet the coil load. When the coil load is larger than the gross heating capacity,
the program will report an unmet load condition.
4. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross heating capacity to 100 x (1.25) = 125 MBH (36.6 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected.
5. Average Efficiency defines the average performance of the unit. Two options are provided for defining this data:
a. Average Efficiency is defined as 100 x (Heating Output) / (Energy Input). Typically this option is used when modeling a specific equipment unit and efficiency ratings
can be obtained from a product catalog. The data might represent a seasonal value such as an AFUE or a steady state or thermal efficiency value at design.
Typically no further information about efficiency at part-load conditions will supplied these types of units so the latter two types of ratings must be used as an
"average" efficiency for all performance calculations. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment efficiency based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the fuel type, gross capacity and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or
90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment efficiency will be
displayed on the air system input report.
6. Misc. Electric defines input power for electrical components in the combustion unit such as combustion blowers and fuel oil pumps. During simulation calculations the
program will calculate energy use by these components as a function of part-load ratio. That is, at 60% load, 60% of the specified miscellaneous electric power will be
consumed. This assumes the electrical components cycle based on the heating load and therefore that energy use is proportional to the part-load ratio.
For those cases where electrical components are not used or you do not wish to consider them, specify a zero value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Terminal Clg Units - Air-Cooled DX
This window contains performance data for air-cooled DX cooling in terminal units. This data is used for packaged DX fan coils and split DX fan coils such as PTACs, unit
ventilators, fan coils and ductless splits.
This data can be entered in two ways:
1. All Terminal Units Use Same Settings. When the "all terminal cooling units use same settings" box in the upper left is checked, only one set of performance data
needs to be defined and it applies to all DX fan coil units in the system. Typically this option is used in preliminary or schematic design applications where autosizing
and one general EER value can be applied to all units in the system. This option offers significant time savings when it can be used.
2. Each Terminal Unit Defined Separately. When the "all terminal cooling units use same settings" box in the upper left is not checked, performance data for each DX
fan coil unit in the system must be specified separately. The drop down list and scroll bar in the upper right is used to move forward or backward through the list of
Page 61 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Clg Units - Water-Cooled DX
11.0 Entering Systems ›› 11.6 Equipment Data ››
zone fan coil units. This option is typically used for detailed design applications where specific equipment units are being modeled so each unit's performance must be
directly defined.
Each item describing fan coil performance is discussed below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the DX fan coil unit. The peak load is generated during design calculations for the system.
The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will be blank
since the data does not yet exist. This option is also blank when the "all terminal cooling units use the same settings" option is selected.
2. Design OAT is the outdoor air design temperature at which gross cooling capacity is defined. Typically the best practice is to enter the outdoor air temperature (OAT)
for the time of the peak load. Cooling capacity varies as a function of OAT. Therefore, if you accept a default or define an OAT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the DX cooling unit at its design outdoor air temperature. No deduction for fan heat is considered in this
value. This value is typically obtained from equipment selection software or product catalogs. This capacity value, together with design OAT and input power, serve as
the anchor point for off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing
input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 40 MBH (11.7 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 40 x (1.15) = 46 MBH (13.5 kW). This input is only
enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER or SEER value. This EER or SEER includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating OAT of 95 F (35 C). During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this
EER, subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition of 95 F (35 C) and the design OAT specified for this
equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER or SEER based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity, heating type and the Energy Standard preference for the
project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated
equipment EER or SEER will be displayed on the air system input report.
7. Conventional Cutoff OAT is the outdoor air temperature below which the cooling unit turns off. This value is typically provided in product catalogs.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 62 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Clg Units - Water-Cooled DX
This window contains cooling duty performance data for terminal units which are water source heat pumps.
This data can be entered in two ways:
1. All Terminal Units Use Same Settings. When the "all terminal cooling units use same settings" box in the upper left is checked, only one set of performance data
needs to be defined and it applies to all heat pump units in the system. Typically this option is used in preliminary or schematic design applications where autosizing
and one general EER value can be applied to all heat pumps in the system. This option offers significant time savings when it can be used.
2. Each Terminal Unit Defined Separately. When the "all terminal cooling units use same settings" box in the upper left is not checked, performance data for each
terminal heat pump in the system must be specified separately. The drop down list and scroll bar in the upper right is used to move forward or backward through the
list of zone heat pump units. This option is typically used for detailed design applications where specific equipment units are being modeled so each unit's performance
must be directly defined.
Each item describing fan coil performance is discussed below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the zone heat pump coil. The peak load is generated during design calculations for the
system. The load provides guidance when specifying the gross cooling capacity. If system design calculations have not been run for the air system, then this item will
be blank since the data does not yet exist. In addiition, if the "all terminal cooling units use same setting" option is selected this input will also be blank.
2. Design EWT is the entering water temperature at which gross cooling capacity is defined. Typically the best practice is to enter the entering water temperature (EWT)
for the time of the peak load. Cooling capacity varies as a function of EWT. Therefore, if you accept a default or define an EWT less than the actual design value, you
increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Note: If you choose to directly specify the compressor kW below, this kW value must correspond to the Design EWT. That is because the Design EWT is the anchor
point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum Efficiency
options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design EWT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross cooling capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the cooling capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity is then displayed on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling capacity.
4. Gross Cooling Capacity defines the total cooling output of the cooling unit at its design EWT. No deduction for fan heat is considered in this value. This value is
typically obtained from equipment selection software or product catalogs. This capacity value, together with design EWT and input power, serve as the anchor point for
off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 40 MBH (11.7 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 40 x (1.15) = 46 MBH (13.5 kW). This input is only
enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. ISO/AHRI Performance Rating allows entry of an ISO/AHRI standard EER value. This EER includes compressor power and indoor fan and pump power
allowances, and is determined a standard rating temperature. During the energy simulation, HAP will automatically derive the compressor kW from this EER,
adjusting for the indoor fan and pump power allowances and adjusting for any difference between the ISO/AHRI rating condition and the design EWT you specified
for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor kW requires input of the compressor power at the design EWT specified earlier on this screen. Typically this option is used when modeling a specific
equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is used together with the
design EWT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment EER based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the equipment type, cooling capacity and the Energy Standard preference for the project (90.1-2004,
Page 63 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Htg Units - ASHP
11.0 Entering Systems ›› 11.6 Equipment Data ››
90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment EER will
be displayed on the air system input report.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Terminal Htg Units - ASHP
This window contains performance data for terminal unit air source heat pumps. This data is used for packaged terminal heat pumps (PTHPs) and split DX heat pumps.
This data can be entered in two ways:
1. All Terminal Units Use Same Settings. When the "all terminal heating units use same settings" box in the upper left is checked, only one set of performance data
needs to be defined and it applies to all heat pump units in the system. Typically this option is used in preliminary or schematic design applications where autosizing
and one general COP value can be applied to all heat pumps in the system. This option offers significant time savings when it can be used.
2. Each Terminal Unit Defined Separately. When the "all terminal heating units use same settings" box in the upper left is not checked, performance data for each
terminal heat pump in the system must be specified separately. The drop down list and scroll bar in the upper right is used to move forward or backward through the
list of zone heat pump units. This option is typically used for detailed design applications where specific equipment units are being modeled so each unit's performance
must be directly defined.
Each item describing terminal unit performance is discussed below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the zone terminal heat pump. The peak load is generated during design calculations for the
system. The load provides guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will
be blank since the data does not yet exist. In addition, if the "all heating terminals use same settings" option is selected, this item will also be blank.
2. Design OAT is the outdoor air design temperature at which gross heating capacity is defined. For air source heat pump equipment the practice is to specify a standard
rating condition or the outdoor air temperature (OAT) for the time of the peak load.
Note: If you choose to directly specify the compressor and outdoor fan kW below, this kW value must correspond to the Design OAT. That is because the Design OAT
is the anchor point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum
Efficiency options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design OAT, if it differs from the
standard rating condition.
3. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be displayed on the air system input report. For energy analysis during detailed design where you are modeling a
specific equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
4. Gross Heating Capacity defines the total heating output of the heating unit at its design outdoor air temperature. This value is typically obtained from equipment
selection software or product catalogs. This capacity value, together with design OAT and input power, serve as the anchor point for off-design and part-load
performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 40 MBH (11.7 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross cooling capacity to 40 x (1.25) = 50 MBH (14.6 kW). This input is only
enabled when the "Auto-Size Capacity" option is selected.
Page 64 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Htg Units - WSHP
11.0 Entering Systems ›› 11.6 Equipment Data ››
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard COP or HSPF value. This COP or HSPF includes compressor, indoor fan and outdoor fan power and is
determined at the standard rating OAT of 47 F (8.3 C). During the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from this
COP, subtracting the indoor fan power and adjusting for any difference between the AHRI rating condition of 47 F (8.3 C) and the design OAT you specified for this
equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment COP or HSPF based on ASHRAE Standard 90.1
minimum equipment efficiency requirements. The program uses the equipment type, cooling capacity of the unit, auxiliary heating type and the Energy Standard
preference for the project (90.1-2004, 90.1-2007, or 90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been
run, the calculated equipment COP or HSPF will be displayed on the air system input report.
7. Cutoff OAT is the outdoor air temperature below which the heat pump turns off and the equipment runs with 100% auxiliary heat. This cutoff temperature is usually
dictated by equipment operating limits, economic considerations and/or performance considerations.
8. Type of Auxiliary Heating is a display-only item. The program assumes that electric auxiliary heat is used for all terminal air source heat pumps. This item is
displayed so this assumption is clearly stated.
9. Auxiliary Heating Upper Cutoff specifies the outdoor air dry-bulb temperature above which auxiliary electric heat is locked out. This is a display-only item. The
program assumes the cutoff is 40 F (4.4 C).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Terminal Htg Units - WSHP
This window contains heating duty performance data for terminal water source heat pump (WSHP) units.
This data can be entered in two ways:
1. All Terminal Units Use Same Settings. When the "all terminal heating units use same settings" box in the upper left is checked, only one set of performance data
needs to be defined and it applies to all heat pump units in the system. Typically this option is used in preliminary or schematic design applications where autosizing
and one general COP value can be applied to all heat pumps in the system. This option offers significant time savings when it can be used.
2. Each Terminal Unit Defined Separately. When the "all terminal heating units use same settings" box in the upper left is not checked, performance data for each
terminal heat pump in the system must be specified separately. The drop down list and scroll bar in the upper right is used to move forward or backward through the
list of zone heat pump units. This option is typically used for detailed design applications where specific equipment units are being modeled so each unit's performance
must be directly defined.
Each item describing terminal unit performance is discussed below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
1. Estimated Maximum Load. This display-only item lists the peak load for the zone heat pump. The peak load is generated during design calculations for the system.
The load provides guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will be blank
since the data does not yet exist. In addition if the "all terminal heating units use same settings" option was selected, this item will also be blank.
2. Design EWT is the entering water temperature at which gross heating capacity is defined. Typically the best practice is to enter the entering water temperature (EWT)
for the time of the peak load. Heating capacity varies as a function of EWT. Therefore, if you accept a default or define an EWT warmer than the actual design value,
you increase the risk that the unit will not have sufficient capacity at design conditions and that will generate unmet load hours.
Page 65 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for Terminal Htg Units - Combustion
11.0 Entering Systems ›› 11.6 Equipment Data ››
Note: If you choose to directly specify the compressor kW below, this kW value must correspond to the Design EWT. That is because the Design EWT is the anchor
point for calculating off-design and part-load performance of the equipment. When you use the AHRI Performance Rating or ASHRAE 90.1 Minimum Efficiency
options, those ratings are at standard conditions and the program will later automatically adjust the rating to your specified Design EWT.
3. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity is then shown on the air system input report. For energy analysis during detailed design where you are modeling a specific
equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
4. Gross Heating Capacity defines the total heating output of the unit at its design EWT. This value is typically obtained from equipment selection software or product
catalogs. This capacity value, together with design EWT and input power, serve as the anchor point for off-design and part-load performance calculations. This input is
only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 40 MBH (11.7 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross cooling capacity to 40 x (1.25) = 50 MBH (14.6 kW). This input is only
enabled when the "Auto-Size Capacity" option is selected.
6. Equipment Performance Rating defines the energy performance of the unit at design. Three options are provided for defining this data:
a. ISO/AHRI Performance Rating allows entry of an ISO/AHRI standard COP value. This COP includes compressor power and indoor fan and water pump power
allowances, and is determined a standard rating temperature. During the energy simulation, HAP will automatically derive the compressor kW from this COP,
subtracting the indoor fan and pump power allowances and adjusting for any difference between the ISO/AHRI rating condition and the design EWT you specified
for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor kW requires input of the compressor power at the design EWT specified earlier on this screen. Typically this option is used when modeling a specific
equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The input kW is used together with the
design EWT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment COP based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the equipment type and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or 90.1-2010)
to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment COP will be displayed on the air
system input report.
Note: When this heat pump is used in a WSHP system, auxiliary heating is provided by the auxiliary boiler attached to the water loop. When the heat pump is used in a
GWSHP or GSHP system, it is assumed the heat pump contains an electric auxiliary heating coil.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for Terminal Htg Units - Combustion
This window contains performance data for combustion heating in terminal units. This data is used for packaged DX fan coils and split DX fan coils such as PTACs, unit
ventilators and fan coils.
This data can be entered in two ways:
1. All Terminal Units Use Same Settings. When the "all terminal heating units use same settings" box in the upper left is checked, only one set of performance data
needs to be defined and it applies to all fan coil units in the system. Typically this option is used in preliminary or schematic design applications where autosizing and
one general efficiency value can be applied to all fan coil units in the system. This option offers significant time savings when it can be used.
2. Each Terminal Unit Defined Separately. When the "all terminal heating units use same settings" box in the upper left is not checked, performance data for each fan
coil unit in the system must be specified separately. The drop down list and scroll bar in the upper right is used to move forward or backward through the list of zone
fan coil units. This option is typically used for detailed design applications where specific equipment units are being modeled so each unit's performance must be
directly defined.
Each item describing terminal unit performance is discussed below.
Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
Page 66 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Misc. Components for Water-Cooled VPAC Systems
11.0 Entering Systems ›› 11.6 Equipment Data ››
1. Estimated Maximum Load. This display-only item lists the peak load for the zone fan coil unit, derived from design calculations for the system. This value provides
guidance when specifying the gross heating capacity. If system design calculations have not been run for the air system, then this item will be blank since the data
does not yet exist. In addition, if the "all terminal heating units use same settings" option is selected, this item will also be blank.
2. Equipment Sizing specifies whether the computer will automatically determine the gross heating capacity, or you will directly specify the capacity. For energy analysis
during the preliminary design phase of a project or when performing the LEED Energy and Atmosphere Credit 1 analysis, it is often appropriate and faster to choose
the "Auto-Sized Capacity" option. During the energy simulation the program will set the heating capacity to the estimated maximum load plus the oversizing allowance
specified below. The resulting capacity will then be displayed on the air system input report. For energy analysis during detailed design where you are modeling a
specific equipment unit, choose "User-Defined Capacity" so you can directly enter the heating capacity.
3. Gross Heating Capacity defines the total heating output of the unit. This value is typically obtained from equipment selection software or product catalogs. This
capacity value is used to determine whether the heating unit has sufficient capacity to meet the coil load. When the coil load is larger than the gross heating capacity,
the program will report an unmet load condition.
4. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 40 MBH (11.7 kW) and the oversizing factor is 25%, the Auto-Size feature will set the gross heating capacity to 40 x (1.25) = 50 MBH (14.6 kW). This input is only
enabled when the "Auto-Size Capacity" option is selected.
5. Average Efficiency defines the average performance of the unit. Two options are provided for defining this data:
a. Average Efficiency is defined as 100 x (Heating Output) / (Energy Input). Typically this option is used when modeling a specific equipment unit and efficiency ratings
can be obtained from a product catalog. The data might represent a seasonal value such as an AFUE or a steady state or thermal efficiency value at design.
Typically no further information about efficiency at part-load conditions will supplied these types of units so the latter two types of ratings must be used as an
"average" efficiency for all performance calculations. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment efficiency based on ASHRAE Standard 90.1 minimum
equipment efficiency requirements. The program uses the fuel type, gross capacity and the Energy Standard preference for the project (90.1-2004, 90.1-2007, or
90.1-2010) to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been run, the calculated equipment efficiency will be
displayed on the air system input report.
6. Misc. Electric defines input power for electrical components in the combustion unit such as combustion blowers and fuel oil pumps. During simulation calculations the
program will calculate energy use by these components as a function of part-load ratio. That is, at 60% load, 60% of the specified miscellaneous electric power will be
consumed. This assumes the electrical components cycle based on the heating load and therefore that energy use is proportional to the part-load ratio.
For those cases where electrical components are not used or you do not wish to consider them, specify a zero value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Misc. Components for Water-Cooled VPAC Systems
This window contains data for additional components and controls used with a water-cooled vertical packaged (VPAC) unit. Each item in this window is described below.
Page 67 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Misc. Components for WSHP Systems
11.0 Entering Systems ›› 11.6 Equipment Data ››
1. Cooling Tower. This item is used to link a cooling tower to the VPAC unit. The drop-down list contains a list of cooling towers in the current project. It also contains a
"" item. A cooling tower can be linked to the system in two ways.
a. Selecting an Existing Cooling Tower. If you previously created and stored cooling towers in your project, you can simply select the desired tower from the drop-
down list.
b. Creating a New Cooling Tower. If you have not yet created a cooling tower, choose the "" item in the drop-down list. The Cooling Tower Form
will appear and will allow you to define data for a new tower. When you press the OK button to exit from the Cooling Tower Form, your cooling tower data will be
stored and the tower will be linked to system automatically.
In addition, you can modify existing cooling tower data directly from the System Form by pressing the Cooling Tower button to the left of the drop-down list. When you
press this button, the Cooling Tower Form will appear and will display inputs for the currently selected tower. After modifying the tower data, press the OK button to
return to the System Form.
2. Min. Return Water Temp defines the minimum setpoint temperature for water returning from the cooling tower to the VPAC unit. When conditions permit the cooling
tower to return a colder water temperature, tower will be controlled to maintain the return water at the minimum setpoint. Control can be achieved by water bypass, fan
cycling, 2-speed fan operation or variable speed fan operation. Choice of control is made in the cooling tower inputs.
3. Condenser Pump defines the performance of the pump at design conditions. Pump performance can be input in one of three ways:
a. ft wg or kPa - When pump head is defined the program will automatcially calculate the pump input kW using the head, condenser flow and the mechanical and
electrical efficiencies. Note that this should be the total pump head including frictional loss for flow through the piping plus pressure losses for flow through the
VPAC condensers, valves and any heat exchangers.
b. W/gpm - The program will calculate pump input kW using W/gpm and the condenser flow rate.
c. kW. This option directly defines the pump motor input power.
4. Condenser Pump Mechanical Efficiency defines the efficiency due to mechanical losses. It is typically obtained from pump selection data. When pump performance
is defined in terms of head, this efficiency is used together with flow, head and electrical efficiency to calculate pump input kW.
5. Condenser Pump Electrical Efficiency defines the electrical efficiency of the pump motor. When pump performance is defined in terms of head, this efficiency is
used together with flow, head and electrical efficiency to calculate pump input kW. When pump performance is defined as kW or Watts per unit flow, this efficiency is
used to derive the equivalent head, used in variable speed pumping calculations.
Note: Currently a cooling tower must be linked to each VPAC unit. For situations where a building contains multiple VPAC units which all share a single large cooling
tower, use the following approach to approximate performance of this configuration:
a. Define one cooling tower for each VPAC unit.
b. Specify a condenser water flow rate for the tower equal to the VPAC unit’s required flow. Specify a pump head equal to the actual system head.
c. Specify the design wet-bulb, range and approach for the actual large tower.
d. Specify tower fan power in terms of kW/Ton. If fan kW is entered instead, divide the total kW among each individual tower based on the ratios of flow rate or heat
rejection.
This will correctly calculate condenser pump power and will approximate performance of the actual large tower and its fan. Deviation from actual tower performance will
depend on the amount of load diversity among the VPAC units. For situations with very little diversity, the error will be small.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 68 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Misc. Components for GSHP Systems
11.0 Entering Systems ›› 11.6 Equipment Data ››
Misc. Components for WSHP Systems
This window contains data for additional components and controls used with WSHP systems. Each item in this window is described below.
1. Cooling Tower. This item only appears for WSHP systems and is used to link a cooling tower to water loop. The drop-down list contains a list of cooling towers in the
current project. It also contains a "" item. A cooling tower can be linked to the system in two ways:
a. Selecting an Existing Cooling Tower. If you previously created and stored cooling towers in your project, you can simply select the desired tower from the drop-
down list.
b. Creating a New Cooling Tower. If you have not yet created a cooling tower, choose the "" item in the drop-down list. The Cooling Tower Form
will appear and will allow you to define data for a new tower. When you press the OK button to exit from the Cooling Tower Form, your cooling tower data will be
stored and the tower will be linked to system automatically.
2. Auxiliary Boiler. This item only appears for WSHP systems and is used to link an auxiliary boiler to the water loop. The drop-down list contains a list of boilers in the
current project. It also contains a "" item. A boiler can be linked to the system in two ways:
a. Selecting an Existing Boiler. If you previously created and stored boilers in your project, you can simply select the desired boiler from the drop-down list.
b. Creating a New Boiler. If you have not yet created a boiler, choose the "" item in the drop-down list. The Boiler Form will appear and will allow
you to define data for a new boiler. When you press the OK button to exit from the Boiler Form, your boiler data will be stored and the boiler will be linked to system
automatically.
3. Circulation Pump defines the performance of the pump at design conditions. Pump performance can be input in one of three ways:
a. ft wg or kPa - When pump head is defined the program will automatcially calculate the pump input kW using the head, system flow rate and the mechanical and
electrical efficiencies. Note that this should be the total pump head including frictional loss for flow through the piping plus pressure losses for flow through the
WSHP units, valves and any heat exchangers.
b. W/gpm - The program will calculate pump input kW using W/gpm and the system flow rate.
c. kW. This option directly defines the pump motor input power.
4. Circulation Pump Mechanical Efficiency defines the efficiency due to mechanical losses. It is typically obtained from pump selection data. When pump performance
is defined in terms of head, this efficiency is used together with flow, head and electrical efficiency to calculate pump input kW.
5. Circulation Pump Electrical Efficiency defines the electrical efficiency of the pump motor. When pump performance is defined in terms of head, this efficiency is
used together with flow, head and electrical efficiency to calculate pump input kW. When pump performance is defined as kW or Watts per unit flow, this efficiency is
used to derive the equivalent head, used in variable speed pumping calculations.
6. Loop Maximum Setpoint, Loop Minimum Setpoint. These items defines the maximum and minimum setpoint temperatures for a WSHP water loop. When the loop
contains excess heat, the cooling tower rejects heat to keep the loop water at the maximum setpoint. When there is a deficit in water heat content, the auxiliary boiler
adds heat to keep loop water at the minimum setpoint.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Misc. Components for GSHP Ssytems
This window contains data for additional components and controls used with GWSHP or GSHP systems. Each item in this window is described below.
Page 69 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Equipment Data for VRF Outdoor Unit
11.0 Entering Systems ›› 11.6 Equipment Data ››
1. Source Water. This item is used to link a definition of source water temperatures to the system. For GSHP systems the source water temperature data provides a
simple model of the heat source/sink. The drop-down list contains a list of items in the cooling tower library, including items defined as "geo, well or surface water".
One of these items should be selected, or you can create a new item using the "" item in the drop down list.
2. Type of Auxiliary Heat. This is a display-only item which documents electric auxiliary heat is used for this equipment.
3. Circulation Pump defines the performance of the pump at design conditions. Pump performance can be input in one of three ways:
a. ft wg or kPa - When pump head is defined the program will automatcially calculate the pump input kW using the head, system flow rate and the mechanical and
electrical efficiencies. Note that this should be the total pump head including frictional loss for flow through the piping plus pressure losses for flow through the heat
pump units in the system, valves and any heat exchangers.
b. W/gpm - The program will calculate pump input kW using W/gpm and the system flow rate.
c. kW. This option directly defines the pump motor input power.
4. Circulation Pump Mechanical Efficiency defines the efficiency due to mechanical losses. It is typically obtained from pump selection data. When pump performance
is defined in terms of head, this efficiency is used together with flow, head and electrical efficiency to calculate pump input kW.
5. Circulation Pump Electrical Efficiency defines the electrical efficiency of the pump motor. When pump performance is defined in terms of head, this efficiency is
used together with flow, head and electrical efficiency to calculate pump input kW. When pump performance is defined as kW or Watts per unit flow, this efficiency is
used to derive the equivalent head, used in variable speed pumping calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Data for VRF Outdoor Unit
This window contains equipment performance data for the outdoor VRF unit serving a group of indoor split DX fan coil units. Each input item in the window is described
below.
Page 70 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
1. Equipment Sizing specifies whether the computer will automatically determine the gross capacities for the outdoor unit, or you will directly specify the capacity. For
energy analysis during the preliminary design phase of a project, it is often appropriate and faster to choose the "Auto-Sized Capacity" option. During the energy
simulation the program will set the cooling capacity to the estimated maximum load plus the cooling oversizing factor specified below. The gross heating capacity will
be calculated as peak heating coil load plus the heating oversizing factor specified below. The resulting capacities will then be shown on the air system input report.
For energy analysis during detailed design where you are modeling a specific equipment unit, choose "User-Defined Capacity" so you can directly enter the cooling
and heating capacities.
2. Design OADB are the outdoor air temperatures at which gross cooling capacity and gross heating capacity are defined. Typically the best practice is to enter the
outdoor air temperature (OAT) for the time of the peak cooling load. Design OADB for heating is typically specified as 47 F (8.3 C).
3. Estimated Maximum Load. This display-only item lists the peak equipment loads for cooling and heating. The peak load is generated during design calculations for
the system. The load provides guidance when specifying the gross capacity. If system design calculations have not been run for the air system, then this item will be
blank since the data does not yet exist.
4. Design Capacity defines the gross cooling capacity of the VRF outdoor unit at the cooling design OADB and the gross heating capacity at the heating design OADB.
This value is typically obtained from equipment selection software or product catalogs. This capacity value, together with design OAT and input power, serve as the
anchor point for off-design and part-load performance calculations. This input is only enabled if you selected "User-Defined Capacity" for the Equipment Sizing input.
5. Capacity Oversizing Factor defines the additional capacity added when using the "Auto-Size Capacity" option. For example if the estimated maximum load for a unit
is 100 MBH (29.3 kW) and the oversizing factor is 15%, the Auto-Size feature will set the gross cooling capacity to 100 x (1.15) = 115 MBH (33.7 kW). This input is
only enabled when the "Auto-Size Capacity" option is selected. Separate oversizing factors are specified for cooling and heating.
6. Performance Value defines the energy performance of the unit at design. Separate values are specified for cooling and heating duty. Three options are provided for
defining this data:
a. AHRI Performance Rating allows entry of an AHRI standard EER or SEER value for cooling or an AHRI standard COP or HSPF value for heating. The AHRI rating
includes compressor, indoor fan and outdoor fan power and is determined at the standard rating OAT of 95 F (35 C) for cooling and 47 F (8.3 C) for heating. During
the energy simulation, HAP will automatically derive the compressor and outdoor fan kW from the rating, subtracting the indoor fan power and adjusting for any
difference between the AHRI rating condition and the design OAT you specified for this equipment. Quick Reference: ASHRAE Std 90.1 Equipment Efficiencies
b. Compressor & OD Fan kW requires input of the sum of compressor and outdoor fan power at the design OAT specified earlier on this screen. Typically this option is
used when modeling a specific equipment unit. The data is obtained from a product catalog or performance data generated by electronic catalog software. The
input kW is used together with the design OAT and gross capacity as the anchor point for off-design and part-load performance calculations.
c. ASHRAE 90.1 Minimum Eqpt Efficiency specifies the program should automatically determine the equipment efficiency rating (EER or SEER for cooling; COP or
HSPF for heating) based on ASHRAE Standard 90.1 minimum equipment efficiency requirements. The EER, SEER, COP, HSPF will subsequently be used to
derive compressor and outdoor fan kW at the design rating point for cooling or heating. The program uses the equipment type, cooling capacity, heating type and
the ASHRAE 90.1 Energy Standard preference for the project to determine the proper ASHRAE efficiency to apply to the equipment. After a simulation has been
run, the calculated equipment efficiency values will be displayed on the air system input report.
7. Compressor Type. The HAP VRF performance model contains performance curves for three common types of units - those containing variable speed rotary
compressors, digital scroll compressors, or variable speed scroll compressors. Choose the compressor type which most closely matches the equipment you are
modeling.
8. Minimum Load. Below minimum load the equipment cycles on and off to meet the load. Above minimum load the equipment stages compressors and adjusts
compressor speed to meet the load.
9. Refrigerant Piping Length. For variable speed rotary VRF equipment, specify the physical length of refrigerant piping from the VRF outdoor unit to the most distant
indoor unit. For variable speed or digital scroll VRF equipment specify the equivalent length for refrigerant piping form the VRF outdoor unit to the most distant indoor
unit. The length must consider both horizontal and vertical sections of piping.
When long lines exist, the VRF outdoor unit will have to generate extra cooling or heating output to overcome refrigerant pressure drop in the lines to satisfy loads at
the indoor unit. Capacity correction factors for line loss are reported in charts or tables in manufacturer's literature. For example if the reported capacity correction
Page 71 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Changeover Controller
11.0 Entering Systems ›› 11.6 Equipment Data ››
factor for a given pipe length is 0.9, the outdoor unit will have to provide 100/0.9 or 111 MBH of cooling output in order to meet a load of 100 MBH at the indoor units.
Separate correction factors are calculated for cooling duty and heating duty based on the piping length.
Note that while HAP enforces reasonable general limits for piping length, actual limitations on line length vary with the specific system configuration. Engineers should
always consult manufacturer's product literature for guidance on line length limitations for an application.
10. Refrigerant Piping Vertical Distance. Specify the vertical distance from the outdoor condensing unit to the indoor unit that is at the greatest vertical distance from
the outdoor unit. Specify a positive value if the outdoor unit is above the indoor unit (for example a roof-mounted outdoor unit). Specify a negative value if the outdoor
unit is below the indoor unit (for example a ground-level outdoor unit serving indoor units on upper floors).
Capacity correction factors for line loss due to vertical distance are reported in manufacturer's literature. For example, if the capacity correction factor is 0.95, the
outdoor unit will have to provide 100/0.95 or 105 MBH of cooling output in order to meet a load of 100 MBH at the indoor units. Separate correction factors are
calculated for cooling duty and heating duty based on the vertical distance.
Note that while HAP enforces reasonable general limits for piping vertical distance, actual limitations on vertical distance vary with the specific system configuration.
Engineers should always consult manufacturer's product literature for guidance on vertical distance limitations for an application.
11. Heat Pump Cutoff OADB is the outdoor air temperature below which the heat pump turns off and the equipment runs with 100% auxiliary heat.
12. Heat Recovery Used specifies whether the system has heat recovery controls. With heat recovery hot gas returning from indoor units in cooling can be used to
satisfy part of the demand of other indoor units in heating, or cold liquid refrigerant returning from indoor units in heating can be used to satisfy part of the demand of
other indoor units in cooling.
13. Auxiliary Heating is a display-only item which documents that auxiliary heating for the system is provided by electric resistance heat in the indoor units.
14. Auxiliary Heating Upper Cutoff specifies the outdoor air dry-bulb temperature above which auxiliary heating is locked out. For example if the cutoff is 40 F and
auxiliary heating is required when the OADB is 45 F, auxiliary heating will not turn on.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Changeover Controller
This window contains data describing 2-pipe changeover controls. These inputs only appear for air systems which use chilled water as the cooling source and hot water
as the heating source. For these systems, changeover controls are sometimes used so the system can only provide cooling or heating at one time. Simultaneous
cooling and heating does not occur in a changeover system. Changeover control inputs are described below the figure.
1. Use 2-Pipe Changeover. Check this box if changeover control should be simulated for the system. When you check this box you will have the opportunity to select
the type of changeover trigger in the subsequent input item.
2. Changeover Trigger. Specify the criteria used to determine when the air system switches between heating and cooling modes:
a. Scheduled control uses the monthly on/off schedules defined for individual cooling and heating coils in the system to determine whether the cooling or heating is
available. Therefore the operating mode varies as a function of time of year. When you select this option, the program will require that all monthly on/off schedules
for coils be synchronized so cooling and heating are not both scheduled ON in any one month.
b. OAT Threshold control changes the operating mode based on the outdoor air dry-bulb temperature. In this case operating mode is a function of weather
conditions.
3. OAT Threshold Inputs. When the "OAT Threshold" control is selected, three further inputs are required to define the control.
a. OAT Threshold defines the outdoor air temperature used to control the changeover from cooling to heating and vice versa. This is the center point for the
deadband described in the next input.
b. Deadband. Often a deadband is used for changeover to prevent frequent cycling between cooling and heating modes.
Example: Suppose the OAT Threshold is 55 F (12.8 C) and the Deadband is 5 F (2.8 K), Therefore when the system is in cooling mode, it will switch to heating
mode when the outdoor air temperature falls below 52.5 F (11.4 C) (setpoint minus one-half deadband). When the system is in heating mode it will switch to
cooling mode when the outdoor air temperature rises above 57.5 F (14.2 C).
If your changeover control does not use a deadband, specify a value of zero. For a deadband of zero, the system will switch to cooling mode as soon as the
outdoor temperature rises above the threshold, and will switch to heating mode as soon as the outdoor temperature falls below the threshold.
c. Minimum Cycle Time defines how frequently the system can switch between cooling and heating modes.
Example: Suppose the Minimum Cycle Time is 3 hours and the OAT Threshold and Deadband are as described in the example for 3b. When the system is in
cooling it will switch to heating when the outdoor air temperature falls below 52.5 F (11.4 C). It will remain in heating mode for a minimum of 3 hours, even if the
outdoor air temperature rises above 57.5 F (14.2 C) during that 3 hour period. If the outdoor air temperature is still above 57.5 F (14.2 C) at the end of the 3 hour
period, the system is permitted to switch to cooling mode.
If your changeover control does not use a minimum cycle time, specify a value of zero.
Application Information
1. Changeover control settings should be synchronized between air systems if those systems are served by the same changeover plant.
a. If Scheduled control is used, the same monthly schedules for cooling coils and heating coils should be used in all air systems served by the changeover plant. If
different schedules are used, then the plant will see times of simultaneous cooling and heating and unmet load conditions will result.
Page 72 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
ASHRAE Std 90.1 Equipment Efficiencies
11.0 Entering Systems ›› 11.6 Equipment Data ››
b. If OAT Threshold control is used, the same set of OAT Threshold, Deadband and Minimum Cycle Time values should be used in all air systems served by the
changeover plant. If different values are used between air systems, the plant may see times of simultaneous cooling and heating and unmet load conditions will
result.
2. When OAT Threshold control is used, monthly coil schedules should normally be set with all 12 months ON. While the program permits monthly schedules with ON
and OFF values to be used at the same time OAT Threshold is specified, this is undesirable and often creates conditions where unmet loads will occur.
Example: OAT Threshold control is specified and the cooling coil schedule specifies cooling is not available during April. During the simulation a mix of cooling and
heating demands exist for a single hour in April when the outdoor temperature is above the OAT Threshold value. By OAT Threshold control the system should
operate in cooling, but cannot because the coil schedule indicates cooling is unavailable for April. The system cannot operate in heating mode because the outdoor
temperature is above the OAT Threshold value. As a result the system cannot provide cooling or heating and building loads are not met.
3. Changover Plant Delay - When a plant switches operating mode from heating to cooling or vice-versa, there may be a delay in which no loads can be supplied by the
plant. The length of delay can be specified on the Configuration tab of the Plant Properties window. One result of this delay is that changeover coinciding with times
of relatively high coil loads may lead to unmet loads. In any single hour having both heating and cooling loads, or between two adjacent hours with different loads, the
plant will be forced to changeover. Air system changeover settings can be used to control the frequency of these events.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
ASHRAE Std 90.1 Equipment Efficiencies
This topic provides tables of minimum equipment efficiencies from ASHRAE Standard 90.1 editions 2004, 2007, 2010, and 2013.
Note that all efficiency values are those in effect after January 1, 2016, the latest date of efficiency changes in 90.1-2013.
Air-Conditioners (excerpts from Table 6.8.1A or Table 6.8.1-1)
Equipment Type
Capacity Range
Heating Type
Minimum
Efficiencies
ASHRAE 90.1
2004
Minimum
Efficiencies
ASHRAE 90.1
2007
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
Air Conditioners, Air-Cooled,
<65 MBH
All
12.0 SEER
13.0 SEER
13.0 SEER
13.0 SEER (pkg)
14.0 SEER
(split)
Split System and Packaged.
>=65 MBH and <135 MBH
Electric or None
10.3 EER
11.2 EER
11.2 EER
11.2 EER
>=65 MBH and <135 MBH
All Other
10.1 EER
11.0 EER
11.0 EER
11.0 EER
>=135 MBH and <240 MBH
Electric or None
9.7 EER
11.0 EER
11.0 EER
11.0 EER
>=135 MBH and <240 MBH
All Other
9.5 EER
10.8 EER
10.8 EER
10.8 EER
>=240 MBH and <760 MBH
Electric or None
9.5 EER
10.0 EER
10.0 EER
10.0 EER
>=240 MBH and <760 MBH
All Other
9.3 EER
9.8 EER
9.8 EER
9.8 EER
>=760 MBH
Electric or None
9.2 EER
9.7 EER
9.7 EER
9.7 EER
>=760 MBH
All Other
9.0 EER
9.5 EER
9.5 EER
9.5 EER
Air Conditioners, Water-Cooled
< 65 MBH
All
12.1 EER
12.1 EER
12.1 EER
12.1 EER
Split System and Packaged
>=65 MBH and <135 MBH
Electric or None
11.5 EER
11.5 EER
12.1 EER
12.1 EER
>=65 MBH and <135 MBH
All Other
11.3 EER
11.3 EER
11.9 EER
11.9 EER
>=135 MBH and <240 MBH
Electric or None
11.0 EER
11.0 EER
12.5 EER
12.5 EER
>=135 MBH and <240 MBH
All Other
10.8 EER
10.8 EER
12.3 EER
12.3 EER
>=240 MBH and < 760 MBH
Electric or None
11.0 EER
11.0 EER
12.4 EER
12.4 EER
>= 240 MBH and < 760 MBH
All Other
10.8 EER
10.8 EER
12.2 EER
12.2 EER
>= 760 MBH
Electric or None
11.0 EER
11.0 EER
12.2 EER
12.2 EER
>= 760 MBH
All Other
10.8 EER
10.8 EER
12.0 EER
12.0 EER
Electrically Operated Unitary and Applied Heat Pumps
(excerpts from Table 6.8.1B or Table 6.8.1-2)
Equipment Type
Capacity Range
Heating Type
Minimum
Efficiencies
ASHRAE 90.1
2004
Minimum
Efficiencies
ASHRAE
90.1 2007
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
Air-Cooled (Cooling Mode)
< 65 MBH
All
12.0 SEER
13.0 SEER
13.0 SEER
14.0 SEER
>=65 MBH and <135 MBH
Electric or None
10.1 EER
11.0 EER
11.0 EER
11.0 EER
>=65 MBH and <135 MBH
All Other
9.9 EER
10.8 EER
10.8 EER
10.8 EER
>=135 MBH and <240 MBH
Electric or None
9.3 EER
10.6 EER
10.6 EER
10.6 EER
>=135 MBH and <240 MBH
All Other
9.1 EER
10.4 EER
10.4 EER
10.4 EER
>=240 MBH
Electric or None
9.0 EER
9.5 EER
9.5 EER
9.5 EER
>=240 MBH
All Other
8.8 EER
9.3 EER
9.3 EER
9.3 EER
Water-to-Air, Water Loop (Cooling Mode)
<17 MBHr
All
11.2 EER
11.2 EER
11.2 EER
12.2 EER
Page 73 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
>=17 MBHr and <65 MBHr
All
12.0 EER
12.0 EER
12.0 EER
13.0 EER
>=65 MBH and <135 MBH
All
12.0 EER
12.0 EER
12.0 EER
13.0 EER
Water-to-Air, Groundwater (Cooling Mode)
<135 MBHr
All
16.2 EER
16.2 EER
16.2 EER
18.0 EER
Briner-to-Air, Ground-Source (Cooling Mode)
<135 MBH
All
13.4 EER
13.4 EER
13.4 EER
14.1 EER
Equipment Type
Cooling Capacity Range
Rating Condition
Minimum
Efficiencies
ASHRAE 90.1
2004
Minimum
Efficiencies
ASHRAE 90.1
2007
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
Air-Cooled (Heating Mode)
< 65 MBH
47 F DB, 43 F WB
7.4 HSPF
7.7 HSPF
7.7 HSPF
8.2 HSPF
>=65 MBH and <135 MBH
47 F DB, 43 F WB
3.2 COP
3.3 COP
3.3 COP
3.3 COP
>=135 MBH
47 F DB, 43 F WB
3.1 COP
3.2 COP
3.2 COP
3.2 COP
Water-to-Air, Water Loop (Heating Mode)
<135 MBH Cooling Capacity
68 F EWT
4.2 COP
4.2 COP
4.2 COP
4.3 COP
Water-to-Air, Groundwater (Heating Mode)
<135 MBH Cooling Capacity
50 F EWT
3.6 COP
3.6 COP
3.6 COP
3.7 COP
Brine-to-Air, Ground Source (Heating Mode)
<135 MBH Cooling Capacity
32 F EWT
3.1 COP
3.1 COP
3.1 COP
3.2 COP
Packaged Terminal Air Conditioners and Heat Pumps
(excerpts from Table 6.8.1D or Table 6.8.1-4)
Equipment Type
Size Category
Rating
Condition
Minimum Efficiencies
ASHRAE 90.1 2004
Minimum Efficiencies
ASHRAE 90.1 2007
PTAC (Cooling Mode) New Construction
All Capacities
95 F OADB
12.5 - (0.213xCap/1000) EER
12.5 - (0.213xCap/1000) EER
PTAC (Cooling Mode) Replacement
All Capacities
95 F OADB
10.9 - (0.213xCap/1000) EER
10.9 - (0.213xCap/1000) EER
PTHP (Cooling Mode) New Construction
All Capacities
95 F OADB
12.3 - (0.213xCap/1000) EER
12.3 - (0.213xCap/1000) EER
PTHP (Cooling Mode) Replacement
All Capacities
95 F OADB
10.8 - (0.213xCap/1000) EER
10.8 - (0.213xCap/1000) EER
PTHP (Heating Mode) New Construction
All Capacities
-
3.2 - (0.026xCap/1000) COP
3.2 - (0.026xCap/1000) COP
PTHP (Heating Mode) Replacement
All Capacities
-
2.9 - (0.026xCap/1000) COP
2.9 - (0.026xCap/1000) COP
Equipment Type
Size Category
Rating
Condition
Minimum Efficiencies
ASHRAE 90.1 2010
Minimum Efficiencies
ASHRAE 90.1 2013
PTAC (Cooling Mode) Standard Size
All Capacities
95 F OADB
13.8 - (0.300xCap/1000) EER
14.0 - (0.300xCap/1000) EER
PTAC (Cooling Mode) Non-Standard Size
All Capacities
95 F OADB
10.9 - (0.213xCap/1000) EER
10.9 - (0.213xCap/1000) EER
PTHP (Cooling Mode) Standard Size
All Capacities
95 F OADB
14.0 - (0.300xCap/1000) EER
14.0 - (0.300xCap/1000) EER
PTHP (Cooling Mode) Non-Standard Size
All Capacities
95 F OADB
10.8 - (0.213xCap/1000) EER
10.8 - (0.213xCap/1000) EER
PTHP (Heating Mode) Standard Size
All Capacities
-
3.7 - (0.052xCap/1000) COP
3.7 - (0.052xCap/1000) COP
PTHP (Heating Mode) Non-Standard Size
All Capacities
-
2.9 - (0.026xCap/1000) COP
2.9 - (0.026xCap/1000) COP
"Cap" refers to rated cooling capacity of the unit in BTU/h.
When Cap is less than 7000 BTU/h, use 7000 BTU/h in the equation.
When Cap is greater than 15,000 BTU/h, use 15,000 BTU/h in the equation.
See footnotes in ASHRAE Standard 90.1 for further information.
Warm Air Furnaces (excerpts from Table 6.8.1E or Table 6.8.1-5)
Equipment Type
Size Category
(Input)
Minimum
Efficiencies
ASHRAE 90.1
2004
Minimum
Efficiencies
ASHRAE 90.1
2007
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
Warm Air Furnace, Gas Fired
<225 MBH
78% AFUE or 80%
Et
78% AFUE or 80%
Et
78% AFUE or 80%
Et
78% AFUE or
80% Et
>=225 MBH
80% Ec
80% Ec
80% Et
80% Et
Warm Air Furnace, Oil Fired
<225 MBH
78% AFUE or 80%
Et
78% AFUE or 80%
Et
78% AFUE or 80%
Et
78% AFUE or
80% Et
>=225 MBH
81% Et
81% Et
81% Et
81% Et
Page 74 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
11.7 Common Tasks
11.0 Entering Systems ››
Creating a New System
11.0 Entering Systems ›› 11.7 Common Tasks ››
Warm Air Duct Furnaces, Gas
Fired
All Capacities
80% Ec
80% Ec
80% Ec
80% Ec
Warm Air Unit Heaters, Gas
Fired
All Capacities
80% Ec
80% Ec
80% Ec
80% Ec
Warm Air Unit Heaters, Oil-
Fired
All Capacities
80% Ec
80% Ec
80% Ec
80% Ec
AFUE = Annual Fuel Utilization Efficiency; Et = Thermal Efficiency; Ec = Combustion Efficiency.
See footnotes in ASHRAE Standard 90.1 for further information.
Electrically Operated Variable-Refrigerant-Flow Air Conditioners (Table 6.8.1I or Table 6.8.1-9)
Equipment Type
Size Category
Heating
Section Type
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
VRF air conditioners, air-
cooled
<65 MBH
All
13.0 SEER
13.0 SEER
>=65 MBH and <135
MBH
Electric or
None
11.2 EER
11.2 EER
>=135 MBH and <240
MBH
Electric or
None
11.0 EER
11.0 EER
>=240 MBH
Electric or
None
10.0 EER
10.0 EER
Electrically Operated Variable-Refrigerant-Flow Air-to-Air Heat Pumps (Table 6.8.1J or Table 6.8.1-10)
Equipment Type
Size Category
Heating
Section Type
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
VRF air cooled, (cooling
mode), without heat
recovery
<65 MBH
All
13.0 SEER
13.0 SEER
>=65 MBH and <135
MBH
Electric or
None
11.0 EER
11.0 EER
>=135 MBH and <240
MBH
Electric or
None
10.6 EER
10.6 EER
>=240 MBH
Electric or
None
9.5 EER
9.5 EER
VRF air cooled, (cooling
mode), with heat
recovery
>=65 MBH and <135
MBH
Electric or
None
10.8 EER
10.8 EER
>=135 MBH and <
240 MBH
Electric or
None
10.4 EER
10.4 EER
>=240 MBH
Electric or
None
9.3 EER
9.3 EER
Equipment Type
Cooling Capacity
Size Category
Heating
Section Type
Minimum
Efficiencies
ASHRAE 90.1
2010
Minimum
Efficiencies
ASHRAE 90.1
2013
VRF, air cooled, (heating
mode)
<65 MBH
-
7.7 HSPF
7.7 HSPF
>=65 MBH and <135
MBH
-
3.3 COP
3.3 COP
>=135 MBH
3.2 COP
3.2 COP
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains how to perform common tasks with air system input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 75 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm
Editing an Existing System
11.0 Entering Systems ›› 11.7 Common Tasks ››
Printing System Inputs
11.0 Entering Systems ›› 11.7 Common Tasks ››
Deleting Systems
11.0 Entering Systems ›› 11.7 Common Tasks ››
Copying a System
11.0 Entering Systems ›› 11.7 Common Tasks ››
Duplicating a System
11.0 Entering Systems ›› 11.7 Common Tasks ››
Printing or Viewing System Design Reports
11.0 Entering Systems ›› 11.7 Common Tasks ››
Creating a New System
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing System
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing System Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Systems
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a System
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a System
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing or Viewing System Design Reports
Please see Generating System Design Reports
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 76 of 76
11.0 Entering Systems
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhB000.htm