12.0 Entering Plants
12.1 Overview for Plants and the Plant Form
12.0 Entering Plants ››
Overview for Plants and the Plant Form
12.0 Entering Plants ›› 12.1 Overview for Plants and the Plant Form ››
This chapter explains input data for HVAC cooling and heating plants.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of the organization of plant data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Plants and the Plant Form
About Plants. A Plant is the equipment and controls which provide chilled water to cooling coils, hot water or steam to heating coils, or
chilled and hot water to coils in one or more air systems. Examples include chiller plants, reversible changeover plants, heat recovery
plants, hot water plants and steam boiler plants. Plant data must be entered and saved in your project before reports containing plant
sizing and energy use information can be generated.
The Plant Properties window, shown above, is used to define the characteristics of a plant required for sizing calculations and energy
simulations. The Plant Properties window contains three key components:
Page 1 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.2 General Plant Data
12.0 Entering Plants ››
General Tab / Plant Form
12.0 Entering Plants ›› 12.2 General Plant Data ››
1. The Title Bar appears across the top of the form. It lists the name of the plant whose data is displayed in the form. At the right end of
the title bar is a button for closing the form.
2. The Working Area is in the center of the window and contains multiple categories of plant information represented as separate tabs in
a notebook. There are seven tabs for the seven possible categories of plant data. The number of tabs which are enabled depend on
the type of plant being entered. Certain plants only use data on the first two tabs. Others use all seven tabs. To move from one tab to
another, simply click on the desired tab. The seven tabs are as follows:
a. General Tab contains the plant name and plant type.
b. Systems Tab is used to specify the air systems served by the plant.
c. Service Hot Water Tab is used to define characteristics of equipment providing service hot water (SHW) for the building.
c. Configuration Tab is used for chiller, changeover, heat recovery and hot water plants to define the organization of components in
the plant.
d. Schedule of Equipment Tab is used for chiller plants to link chillers and cooling towers to the plant, for changeover plants to link
reversible chillers and heat sink/sources to the plant, for heat recovery plants to link chillers, boilers and heat recovery equipment to
the plnt, and for hot water plants to link boilers or heat pumps to the plant.
e. Distribution Tab is used to define the hydronic distribution system and controls for chilled water and hot water plants. For steam
plants it defines the pipe heat loss factor.
f. Condenser Water Tab is used for chiller plants to define condenser pump performance and condenser loop controls.
g. Source Water Tab is used for hot water, changeover and heat recovery plants to define source water pump performance and
controls.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the plant inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the plant. If you press Cancel while creating a new
plant, a new plant will not be added to your project.
c. Press Help to display this overview topic.
Application Data. The following topics summarize how tabs in the Plant Properties window are used to define specific types of plants:
Defining Generic Plants
Defining a Chiller Plant
Defining a Changeover Plant
Defining a Heat Recovery Plant
Defining a Hot Water Plant
Defining a Service Hot Water Plant
Defining Remote Source Plants
Plant Features. Finally, HAP provides useful features for:
Creating new plants.
Editing an existing plant.
Printing plant data.
Deleting a plant.
Copying a plant.
Duplicating a plant.
Printing or viewing plant design reports.
Printing or viewing plant simulation reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the General tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 2 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Plant Name
12.0 Entering Plants ›› 12.2 General Plant Data ››
Plant Type
12.0 Entering Plants ›› 12.2 General Plant Data ››
General Tab / Plant Form
The General tab on the Plant Properties window contains two input items which describe the general nature of the plant being defined:
Plant Name
Plant Type
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Plant Name
This is a reference name used to identify the plant. It will appear elsewhere in the program on selection lists and reports. The reference
name appears:
a. In the list of available plants on the HAP main window.
b. In the list of available plants when linking plants to a building.
c. On input data reports for plants
d. On plant design reports.
e. On plant simulation reports.
Therefore, it is important to use a descriptive name. Typically the name includes information about the type of plant, its components or its
capacity.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Plant Type
This item defines the kind of plant being defined. The choice of a plant type will determine the type and quantity of data required on
subsequent tabs.
HAP offers features for analyzing a variety of common types of chilled water, hot water and steam plants:
1. Generic Plants - A "generic" plant is used only for sizing calculations. It does not require information about specific components or
controls. It only requires information about the systems served by a plant. Therefore it is quick and easy to define for sizing purposes.
Note that a "generic" plant cannot be used in energy simulations. However, after completing your design work if you wish to use the
plant for energy calculations, simply change its plant type. For example, if the plant was "generic chilled water", you can change the
type to "chiller plant" or "remote source cooling". System selections will be preserved. You will only need to supply information about
specific components such as chillers, cooling towers, controls and distribution system.
Five types of "generic" plants are offered:
a. Generic Chilled Water is used for sizing chilled water plants.
b. Generic Changeover is used for sizing a reversible changeover plant that provides both chilled and hot water.
c. Generic Heat Recovery is used to size cooling and heating equipment in this type of plant.
c. Generic Hot Water is used for sizing hot water plants.
d. Generic Service Hot Water is used for sizing standalone service hot water plants.
e. Generic Steam is used for sizing steam plants.
Click here for further information.
Page 3 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Defining Generic Plants
12.0 Entering Plants ›› 12.2 General Plant Data ››
Defining a Chiller Plant
12.0 Entering Plants ›› 12.2 General Plant Data ››
2. Chilled Water Plants provide chilled water to cooling coils in air systems. A Chilled Water Plant defines the specific components and
controls in the plant and can be used both for sizing calculations and energy simulations. Two types of chilled water plants are
offered.
a. Chiller Plant consists of one or more chillers connected in parallel serving a common chilled water loop. Further Information.
b. Remote Source Chilled Water Plant is used for district or campus cooling applications. In this plant, chilled water is supplied from
an external source. This plant only analyzes the chilled water distribution system portion of the system, not the operation of the
central chiller plant. Further Information.
3. Changeover Plants use reversible air-to-water or water-to-water heat pumps to provide chilled water and hot water to coils in a 2-pipe
system. Further Information.
4. Heat Recovery Plant is a special type of plant that combines all the equipment and controls for a chilled water cooling system and a
hot water heating system, and the equipment to recover heat from the cooling system for use in meeting hot water heating loads.
Further information.
5. Hot Water Plants provide hot water to heating coils in air systems and/or provide heat to service hot water systems. A Hot Water
Plant defines the specific components and controls in the plant and can be used both for sizing calculations and energy simulations.
Three types of hot water plants are offered.
a. Hot Water Plant consists of one or more boilers, air-to-water heat pumps or water-to-water heat pumps connected in parallel
serving common hot water loop. Further Information.
b. Remote Source Hot Water Plant is used for district or campus heating applications. In this plant, hot water is supplied from an
external source. The plant only analyzes the hot water distribution system and not the performance of the central boilers or heat
pumps. Further Information.
c. Service Hot Water Plant - This option is used to model a standalone service hot water (SHW) system. This type of plant uses
boilers and/or air-to-water or water-to-water heat pumps to serve SHW demands in the building. Further Information.
5. Steam Plants provide steam to heating coils in air systems and optionally can provide heat to service hot water systems. A Steam
Plant defines the specific components and controls in the plant and can be used both for sizing calculations and energy simulations.
Two types of steam water plants are offered.
a. Steam Boiler Plant consists of one or more boilers connected in parallel providing steam. Further Information.
b. Remote Source Steam Plant is used for district, campus or waste heat heating applications. In this plant, steam is supplied from
an external source. The plant only analyzes the steam distribution portion of the system and not the performance of the central
boilers which generate the steam. Further Information.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining Generic Plants
A "generic" plant is used only for sizing calculations. It does not require information about specific components or controls. It only
requires information about the systems served by a plant. Therefore it is quick and easy to define for sizing purposes.
Five types of "generic" plants are offered:
a. Generic Chilled Water is used for sizing chilled water plants.
b. Generic Changeover is used for sizing a reversible changeover plant that provides both chilled and hot water.
c. Generic Heat Recovery is used for sizing the chilled water cooling and hot water heating equipment in a heat recovery plant.
c. Generic Hot Water is used for sizing hot water plants.
d. Generic Service Hot Water is used for sizing standalone service hot water plants.
e. Generic Steam is used for sizing steam plants.
To define a "generic" plant data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select the type of generic plant being defined.
2. Systems Tab - Select the air systems served by the generic plant.
3. Service Hot Water Tab - For a Generic Service Hot Water plant, data on this tab defines the service hot water (SHW) demand and
equipment in the SHW distribution system. For Generic Hot Water, Steam and Changeover plants, an option is offered to define SHW
data so the plant serve both space heating and SHW heating demands.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining a Chiller Plant
Page 4 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Defining a Changeover Plant
12.0 Entering Plants ›› 12.2 General Plant Data ››
Defining a Heat Recovery Plant
12.0 Entering Plants ›› 12.2 General Plant Data ››
A Chiller Plant consists of one or more chillers connected in parallel providing chilled water to cooling coils in air systems. To define a
Chiller Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Chiller Plant" as the plant type.
2. Systems Tab - Select the air systems served by the plant.
3. Configuration Tab - Define the number of chillers, plant control and chilled water supply temperature control, heat rejector configuration
and waterside economizer.
4. Schedule of Equipment Tab - Link chillers and heat rejectors to the plant.
5. Distribution Tab - Specify characteristics of the chilled water distribution system and pumps.
6. Condenser Water Tab - Specify characteristics of the condenser water system and pumps. This tab is only applicable when water-
cooled chillers are used in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining a Changeover Plant
A Changeover Plant uses reversible air-to-water or water-to-water chillers to provide chilled water and hot water to coils in a 2-pipe
system. The plant will automatically determine when heating mode or cooling mode is required based on plant loads and specified
changeover controls. Optionally the plant can also supply heat to serve service hot water (SHW) demands.
To define a Changeover Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Changeover Plant" as the plant type.
2. Systems Tab - Select the air systems served by the plant.
3. Service Hot Water Tab - If the plant also serves SHW demands, this tab is used to define the service hot water consumption and the
equipment in the SHW distribution system.
4. Configuration Tab - Define the number of reversible chillers, plant control, supply water temperature control, and auxiliary heating for
the plant.
5. Schedule of Equipment Tab - Link reversible chillers and, if applicable, the source of auxiliary heating, and source water for the plant.
6. Distribution Tab - Specify characteristics of the supply water distribution system and pumps.
7. Source Water Tab - Specify characteristics of the source water system and pumps. This is only applicable when water-to-water
reversible chillers are used in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining a Heat Recovery Plant
A Heat Recovery Plant is a special type of plant in HAP which is equivalent to one chiller plant plus one hot water boiler plant plus
additional equipment to recover heat from the chilled water plant to use in meeting hot water plant loads. This plant consists of one or
more chillers connected in parallel providing chilled water to cooling coils in air systems, one or more hot water boilers in parallel
providing hot water to heating coils in air systems and/or to meet service water heating loads, and additional heat recovery equipment.
To define a Heat Recovery Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Heat Recovery Plant" as the plant type.
2. Systems Tab - Select the air systems served by the plant.
3. Service Hot Water Tab - Specify the service hot water (SHW) load profile and the water heating controls, if the plant provides SHW.
4. Configuration Tab - Define the number of chillers, the cooling system controls, the number of boilers, the heating system controls, and
the method of heat recovery. HAP offers models for six different types of heat recovery systems.
5. Schedule of Equipment Tab - This tab is used to link chillers and heat rejectors to the chilled water part of the plant and to link boilers
to the hot water part of the plant. For heat recovery plants using a dedicated heat recovery chiller (DHRC), this additional water-to-
water heat pump equipment is also specified on this tab..
6. Distribution Tab - Specify characteristics of the chilled water and hot water distribution systems and pumps.
7. Source Water Tab - Specify characteristics of the condenser water system and pumps for the cooling system. This tab is only
applicable when water-cooled chillers are used in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 5 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Defining a Hot Water Plant
12.0 Entering Plants ›› 12.2 General Plant Data ››
Defining a Service Hot Water Plant
12.0 Entering Plants ›› 12.2 General Plant Data ››
Defining Remote Source Plants
12.0 Entering Plants ›› 12.2 General Plant Data ››
Defining a Hot Water Plant
A Hot Water Plant consists of one or more boilers, air-to-water heat pumps or water-to-water heat pumps connected in parallel serving
common hot water loop. The plant can serve heating coils in air systems and optionally also provide heat to a service hot water (SHW)
system. To define a Hot Water Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Hot Water Plant" as the plant type.
2. Systems Tab - Select the air systems served by the plant.
3. Service Hot Water Tab - If the plant also serves SHW demands, this tab is used to define the service hot water consumption and the
equipment in the SHW distribution system.
4. Configuration Tab - Define the number of boilers or heat pumps, and the plant and hot water supply temperature control. When heat
pumps are used, auxiliary heating for the plant is also defined on this tab..
5. Schedule of Equipment Tab - Link boilers or heat pumps to the plant. When water-to-water heat pumps are used, source water is also
linked on this tab.
6. Distribution Tab - Specify characteristics of the hot water supply distribution system and pumps.
7. Source Water Tab - Specify characteristics of the source water system and pumps. This tab is only applicable when water-to-water
heat pumps are used in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining a Service Hot Water Plant
This plant is used to model a standalone service hot water (SHW) system. This type of plant uses boilers, air-to-water and/or water-to-
water heat pumps to serve SHW demands in the building.
To define a Service Hot Water Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Service Hot Water" as the plant type.
2. Systems Tab - This tab is only activated when you choose to define SHW demand in terms of hot water volume per person per day. In
that case air systems are linked to the plant as a means of defining the spaces whose occupants are served by the SHW system.
3. Service Hot Water Tab - This tab defines the service hot water consumption and the equipment in the SHW distribution system.
4. Configuration Tab - Define the number of boilers or heat pumps used to supply heat to the SHW system, and the plant and hot water
supply temperature control. When heat pumps are used, auxiliary heating options for the plant is also defined on this tab.
5. Schedule of Equipment Tab - Link boilers or heat pumps to the plant. When water-to-water heat pumps are used, source water is also
linked on this tab. If auxiliary heating is enabled, the source of auxiliary heat can be defined as a boiler or remote source hot water.
6. Distribution Tab - Specify characteristics of the hot water supply distribution system and pumps which deliver heat to the SHW storage
tank heat exchanger or in direct SHW systems to the demand heat exchanger.
7. Source Water Tab - Specify characteristics of the source water system and pumps. This tab is only applicable when water-to-water
heat pumps are used in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining Remote Source Plants
Remote Source plants are used to model district cooling or heating applications where chilled water, hot water or steam is delivered to
the building from an external system. In Remote Source plants only the distribution system in the building is modeled. The primary
equipment generating the chilled water, hot water or steam is not modeled. Energy cost for these plants is the cost of energy for the
distribution system and the purchased cooling or heating supplied from the external source.
For a Remote Source Chilled Water Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Remote Source Chilled Water" as the plant type.
2. Systems Tab - Select the air systems supplied with chilled water by this plant.
Page 6 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Defining Steam Boiler Plants
12.0 Entering Plants ›› 12.2 General Plant Data ››
3. Distribution Tab - Specify characteristics of the chilled water supply distribution system and pumps.
For a Remote Source Hot Water Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Remote Source Hot Water" as the plant type.
2. Systems Tab - Select the air systems supplied with hot water by this plant.
3. Service Hot Water Tab - Optionally, the plant can also serve service hot water (SHW) demands. This tab defines the service hot water
consumption and the equipment in the SHW distribution system.
4. Distribution Tab - Specify characteristics of the hot water supply distribution system and pumps.
For a Remote Source Steam Plant, data on the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Remote Source Steam" as the plant type.
2. Systems Tab - Select the air systems supplied with steam by this plant.
3. Service Hot Water Tab - Optionally, the plant can also serve service hot water (SHW) demands. This tab defines the service hot water
consumption and the equipment in the SHW distribution system.
4. Distribution Tab - Specify the pipe heat loss for the steam distribution system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Defining Steam Boiler Plants
A Steam Boiler Plant consists of one or more boilers connected in parallel serving common steam system. The plant can serve heating
coils in air systems and optionally can also provide heat to a service hot water (SHW) system. To define a Steam Boiler Plant, data on
the following tabs of the Plant Properties window is required:
1. General Tab - Name the plant and select "Steam Boiler Plant" as the plant type.
2. Systems Tab - Select the air systems served by the plant.
3. Service Hot Water Tab - If the plant also serves SHW demands, this tab is used to define the service hot water consumption and the
equipment in the SHW distribution system.
4. Configuration Tab - Define the number of boilers and the plant control.
5. Schedule of Equipment Tab - Link boilers to the plant.
6. Distribution Tab - Specify pipe heat loss for the distribution system.
Page 7 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.3 System Selection Data
12.0 Entering Plants ››
Systems Tab / Plant Form
12.0 Entering Plants ›› 12.3 System Selection Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the System Selection tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Systems Tab / Plant Form
The Systems tab is used to link air systems to the plant. This determines the loads imposed on the plant both for plant design and energy
analysis applications. This tab contains four key components, described below the figure.
Page 8 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.4 Service Hot Water Data
12.0 Entering Plants ››
1. The Systems List appears on the left-hand side of the tab. It contains a list of all systems in your project which can be linked to a plant
you are defining. A note at the top of this list describes how this list was constructed. For example, in the figure above a chiller plant is
being defined, so the list only contains air systems which contain chilled water cooling coils.
2. The Linked Systems List appears on the right-hand side of the tab. It contains a list of the systems you have linked to the plant.
When performing calculations for the plant, only loads for these systems will be considered. The Linked Systems List also allows
system multipliers to be defined. For example if an air system represents one of a number of identical systems in a building, the
system can be entered and sized once. Then a multiplier is specified to account for the total number of these systems which the plant
serves. The figure above shows a situation where an air system represents an air handler used on one of three identical intermediate
floors. Therefore, a multiplier of 3 is applied to this air system.
3. The Add Button appears between the Systems and Linked Systems lists. To add systems to the linked list, first highlight one or more
systems in the Systems List on the left and then press the Add button. The names of the systems you selected will be copied to the
Linked Systems List. The add button can also be used to increment a system multiplier.
Note that the Add button does not remove items from the Systems List.
4. The Remove Button appears below the Add button. To remove systems from the Linked Systems List, first highlight one or more
systems in the Linked List on the right-hand side of the tab. Then press the Remove button. The systems you selected will be erased
from the Linked List.
Note for Service Hot Water (SHW) plants. For SHW plants, the Systems tab is only activated when SHW consumption is defined in
terms of hot water volume per person per day. In this case air systems linked to the plant are not used to define a space load on the
plant. Instead, linked systems define the occupant population served by the SHW system. Occupants in all spaces served by linked air
systems are assumed to be consumers of the service hot water.
In a SHW plant which defines SHW demand in other terms such as hourly hot water demand (gpm or L/s), or as energy consumption per
day, the Systems tab is disabled and no inputs are required.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Service Hot Water Tab / Plant Form
12.0 Entering Plants ›› 12.4 Service Hot Water Data ››
This section explains input data on the Service Hot Water tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Service Hot Water Tab / Plant Form
Service hot water is hot water generated for uses such as bathing, laundry, dishwashing, or industrial process uses. The Service Hot
Water tab contains information about the service hot water (SHW) consumption, and the SHW distribution and storage systems. The tab,
shown in Figure 1 below, is divided into four parts:
1. This Plant Supplies Service Hot Water - This checkbox in the upper left corner of the tab appears when defining a hot water,
changeover, steam boiler, remote source hot water or remote source steam plant. These plant types serve space heating loads but
can additionally serve SHW loads by checking this box. When this box is checked inputs on the tab are enabled. When defining a
standalone Service Hot Water plant, this input does not appear because the sole purpose of the plant is to serve SHW demands.
Therefore, inputs on the tab are always enabled in this case.
2. Consumption - The Consumption group of inputs in the upper left defines the service hot water demand profile and the supply and
source water temperatures for the system. This inputs are always specified.
3. Supply to Points of Use - The Supply to Points of Use group of inputs in the lower left defines the equipment and controls used to
deliver hot water to its point of use. When a pump is required to deliver SHW to its points of use, these inputs describe the pumping
system. When municipal water supply pressure is sufficient to deliver SHW to its points of use in the building, this group of inputs is
not used.
4. Stored Hot Water - The Stored Hot Water inputs on the right side of the tab defines characteristics and control of a hot water storage
tank, if one is used. For Tankless, On-Demand or Instantaneous SHW systems, inputs in this group are not used.
Application Data - The inputs on this tab allow a wide variety of configurations of SHW plants to be configured. Use of the inputs for
three common SHW applications is described below.
1. Tankless, On-Demand or Instantaneous Water Heater - This type of system produces hot water as SHW demands occur. There is
no storage tank. Figure 2 below shows sample inputs for a system of this type. The Consumption group of inputs is always needed to
define demand. If the pressure provided by the municipal water supply system is sufficient to deliver SHW to its point of use, then no
inputs in the Distribution group are needed other than a pipe loss factor, if desired. When a distribution pump is needed, inputs in the
Distribution group would be used.
Then inputs on the Configuration, Schedule of Equipment and Distribution tabs would also be used to describe the equipment that
supplies heat to generate the SHW.
2. Storage Tank Heater, No Pumping - This type of system generates hot water and stores it in a tank. Water from the storage tank is
supplied to the SHW points of use as demands occur. The equipment defined on the Configuration, Schedule of Equipment and
Distribution tabs delivers heat to the tank to keep it at its setpoint temperature. When the pressure provided by the municipal supply
system is sufficient to deliver the SHW to its points of use, a distribution pump is not needed. Sample inputs for this scenario are
shown in Figure 3.
3. Storage Tank Heater, With Distribution Pump - This system is the same as #2 but requires a distribution pump to deliver the SHW
to its points of use within the building. Figure 3 shows sample inputs for this type of system.
Page 10 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Figure 1. Service Hot Water Tab (all options enabled)
Page 11 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Figure 2. SHW Inputs for Instantaneous (Tankless) Water Heating System
Page 12 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Figure 3. SHW Inputs for Storage Hot Water System (No Pumping)
Page 13 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
SHW Consumption Data
12.0 Entering Plants ›› 12.4 Service Hot Water Data ››
Figure 4. SHW Inputs for Storage Hot Water System (with Supply Pump)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
SHW Consumption Data
The Consumption group of inputs defines the service hot water demand profile and the supply and source water temperatures for the
system. These inputs are always required. Inputs in this group are as follows:
1. Max Rate supplies information to define the maximum SHW use rate and allow an hourly demand profile to be calculated. Max Rate
can be defined in three ways:
Flow rate (gpm or L/s) - This option directly defines the peak SHW usage rate as gpm or L/s of hot water delivered to points of use.
This input will be used together with the Usage Schedule to determine hour-by-hour SHW use during the year. Each hourly demand
is the Max Rate in gpm or L/s multiplied by the hourly schedule factor.
Page 14 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
SHW Supply to Points of Use
12.0 Entering Plants ›› 12.4 Service Hot Water Data ››
Consumption per Person per Day (gal/person/day, L/person/day) - This option defines peak SHW demand in terms of daily
consumption per person. This input is used together with the occupant quantities and occupant schedules specified for spaces served
by air systems linked to the plant to determine hourly SHW demand:
a. In a plant serving combined space and SHW loads, air systems are already linked to the plant to define the space heating loads.
These systems will also be used to compile occupant and occupant schedule data for SHW calculations. For a standalone SHW
plant, the Systems tab is enabled when you select this option and you must select air systems serving the area where the occupant
population exists using SHW from this plant. In this latter case any air system defined in the project may be selected.
b. HAP then uses occupant counts and occupant schedule data for all the spaces served by these air systems to construct hour-by-
hour profiles of total occupants for each day of the simulation.
c. The peak use value specified on the Service Hot Water tab is assumed to correspond to the day with the greatest total occupancy.
This peak day is determined by consulting the hourly occupancy profiles.
d. An hourly usage factor calculated as (gal/person/day) x (integrated 24-hour occupants) / 24 hours
or (L/person/day) x (integrated 24-hour total occupants) / 24 hours.
e. Hourly SHW demands are calculated as (number of occupants for current hour) x (hourly usage factor).
Load per Day (kBTU/day, kWh/day) - Rather than defining the hot water flow rate, this option defines the maximum daily SHW load
in terms of kBTU/day or kWH/day. This input is used together with the Usage Schedule to determine hour-by-hour SHW demands
during the year as follows:
a. The peak usage value specified on the Service Hot water tab is assumed to correspond to the greatest total scheduled daily SHW
usage.
b. Maximum hourly usage factor is calculated as
(kBTU/day) / (maximum 24-hour integrated use from usage schedule profiles)
or
(kWh/day) / maximum 24-hour integrated use from usage schedule profiles)
For consistency the Usage Schedule should use the same profile for Design Days and at least one of the simulation day types.
2. Usage Schedule - When Max Rate is defined as flow (gpm or L/s), the Usage Schedule defines the hour-by-hour variation of SHW
water use.
When Max Rate is defined as load per day (kBTU/day or kWh/day), the Usage Schedule defines the hour by hour variation of the
SHW load.
When Max Rate is defined as consumption per day per person, this input is not used. The demand profile is derived from occupant
schedules instead.
3. Design Temperature defines the SHW supply temperature at the point of use such as a faucet, laundry machine or dishwasher. It is
used with the hourly SHW demand and the cold water supply temperature to determine SHW load. This input is only used when SHW
usage is defined as flow (gpm or L/s) or as consumption per person per day. When SHW usage is defined as load per day, this input
is not needed since the SHW load is directly defined.
4. Average Cold Water Supply defines the temperature of cold supply water ("make-up" water) from the municipal water system
entering the SHW system. It is used with hourly SHW demand and the design temperature above to calculate SHW load. This input is
only used when SHW usage is defined as flow (gpm or L/s) or as consumption per person per day. When SHW usage is defined as
load per day, this input is not needed since the SHW load is directly defined.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
SHW Supply to Points of Use
Page 15 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
SHW Stored Hot Water Data
12.0 Entering Plants ›› 12.4 Service Hot Water Data ››
The Supply to Points of Use group of inputs defines the equipment and controls used to deliver hot water to its point of use, such as hot
water taps in sinks, showers, laundry equipment, or other hot water fixtures. When a pump is required to deliver SHW to its points of
use, these inputs describe the pumping system. When municipal water supply pressure is sufficient to deliver SHW to its points of use in
the building, this group of inputs is not used, except to define a pipe loss factor. Inputs in this section are as follows:
1. Pipe Heat Loss Factor defines heat loss in the piping between the storage tank in a storage hot water system, or the SHW heat
exchanger in a tankless system and the SHW points of use. Heat loss is specified as a percentage of the SHW demand, where
demand is defined as the energy in the volume of SHW water consumed for the hour.
2. Use Supply Pump - If a pump is used to distribute hot water from the storage tank or the SHW heat exchanger in a tankless system to
the SHW points of use, check this box. The remaining inputs in this section will then be enabled. If municipal supply pressure is
sufficient to distribute SHW to points of use so a pump is not needed, then uncheck this box. In this case no further inputs in this
section will be required.
In a non-recirculating system the supply pump is assumed to cycled with the demand. For example, in an hour with 100% of peak
SHW flow, the pump will run at 100% of full power. For an hour with 60% of peak SHW flow, the pump will cycle at 60% of full power.
In a recirculating system (see item 6 below), the pump will either run continuously 24 hours a day, or will cycle off when no demand
exists according to the Pump Cycling input (see item 7 below).
3. Input Power defines the pump performance in terms of head (ft wg or kPa), pump power per unit flow (W/gpm or W/L/s) or as pump
input kW. When performance is defined as head, the program calculates pump input power from this input plus the peak SHW flow
rate and pump efficiencies. When performance is defined as power per unit flow, pump power is calculated from this input and the
peak SHW flow. When pump kW is directly specified, no calculation of input power is needed.
4. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is used to calculate pump motor kW
at design when pump head is specified.
5. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. It is used to calculate pump motor kW
at the design condition when pump head is specified. Electrical efficiency is also involved in determining pump heat gain to the water
loop.
6. Use as Recirculation Pump - If the SHW system is a recirculating system, check this box. In this case the supply pump continuously
circulates the hot water in a loop, so hot water at the desired supply temperature is always available at the point of use. Recirculating
systems are often used in hospitals or hotels where maintaining point of use supply temperature is important. If the system is non-
recirculating and the supply pump is only used to pressurize the system, uncheck this box. In that case, the remaining inputs in this
section will be disabled.
7. Pump Cycling - In a recirculation system, if the supply pump runs continuously, uncheck this box. The supply pump will then run 24
hours a day regardless of demand levels. If instead the supply pump cycles on demand, check this box. In this case the supply pump
will be OFF for any hour with zero SHW demand and will be ON otherwise.
8. Delta-T defines the temperature drop in a recirculation system between the start and end of the recirculation loop due to pipe heat
loss.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
SHW Stored Hot Water Data
Page 16 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
The Stored Hot Water inputs define characteristics and control of a hot water storage tank. Inputs in this section are as follows:
1. Stored Hot Water - If the SHW system uses a hot water storage tank, check this box. Inputs in this section will then be enabled. If
the SHW system does not use a storage tank, uncheck this box. In this case, all remaining inputs in this section will be disabled.
2. Storage Tank Volume - Specify the volume of the storage tank in gallons or liters.
3. Minimum Temperature - Specify the minimum tank setpoint. When the tank temperature reaches this minimum setpoint, the heating
equipment will supply heat to the tank to raise it to the hot water supply temperature.
4. Loss Factor - Specify the hourly tank heat loss to the surroundings. Heat loss can be specified as a percent of total stored heat in the
tank per hour, or in terms of BTU/(hr-gal-F) or W/(L-K). Heat loss is based on the volume of the tank and the delta-T between the hot
water supply temperature and the cold water inlet temperaure.
5. Pasteurization - Check this box if the hot water storage tank uses a Pasteurization cycle. Certain local codes required this cycle
which heats tank water to an elevated temperature periodically as a means of sterilizing the SHW supply, in particular to kill Legionella
bacteria. When this box is checked the sub group of inputs below it will be enabled. If the SHW system does not use a Pasteurization
cycle, uncheck the box.
a. Period defines the time in days between Pasteurization cycles. For example a Period of 7 days means Pasteurization cycles occur
every 7 days during the simulation. The first Pasteurization cycle will occur on January 7 in the simulation.
b. Duration specifies the duration in hours of each Pasteurization cycle. For example, some codes require Pasteurization to last for
24 hours. This means the equipment will heat the hot water in the tank to the elevated temperature for 24 consecutive hours and
then return to normal tank operation.
c. Start At defines the start time for each Pasteurization cycle. Often Pasteurization cycles are scheduled to start at times of off peak
energy prices so the cost of the cycle is smaller. For example, if "Start At" is specified for 12:00am with a "Duration" of 8 hours, the
cycle will begin at 12:00am and run for the following 8 hours.
d. Temperature specifies the elevated temperature to maintain in the tank during the Pasteurization cycle. Typically this will be
specified in codes that mandate Pasteurization cycles.
e. Auto-Size Heater - Check this box if you want HAP to automatically determine the size of the Pasteurization heater. When
Pasteurization cycles are required, the system typically includes supplemental electric heating element. The primary heating
equipment such as a gas boiler or an air-to-water heat pump provides first stage heat to the SHW tank. If this heat input is not
sufficient to reach the Pasteurization temperature, the supplemental electric heater serves as second stage heat to elevate the tank
to the prescribed temperature. If you want to directly specify the capacity for the supplemental electric heater, uncheck the box.
f. Heater Capacity defines the capacity of the supplemental electric heater used for Pasteurization cycles. This input is only enabled if
the Auto-Size Heater box is unchecked. When directly specifying heater capacity note that care must be used to specify an
appropriate capacity. If the capacity is too small, the system may not be able to hold the tank at the required temperature during
Pasteurization cycles.
6. Prioritize Service Hot Water Resupply - This input only appears when SHW is part of a combined space heating and service water
heating plant. In that type of plant, capacity is sometimes limited for economic reasons so it may not always be possible to
simultaneously meet both space heating and service water heating demands.
Page 17 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.5 Configuration Data (Chiller Plants)
12.0 Entering Plants ››
Configuration Tab (Chillers) / Plant Form
12.0 Entering Plants ›› 12.5 Configuration Data (Chiller Plants) ››
Check this box to specify criteria for prioritizing space heating and service water heating demands. If you uncheck the box, the plant
will attempt to simultaneously meet space heating and service water heating demands at all times. The box is typically left unchecked
when a plant is sized to be able to meet the peak simultaneous space heating and SHW load.
If prioritization is selected it only influences the order in which loads are served if capacity is insufficient to meet both space and SHW
loads. For example, if SHW has priority, the plant will meet the SHW load first, and will use any excess capacity to serve space
heating loads. If capacity is sufficient, all loads will be met. If capacity is insufficient, a part of the space heating load will not be met
and an unmet load will be recorded.
Priorization can be done by schedule or by outdoor air dry-bulb temperature threshold:
a. By Schedule - Select this option to control prioritization by time of day. With this control the philosophy is to give first priority to
space heating loads during the "occupied" fan/thermostat period for HVAC systems, and give priority to service water heating loads
or the charging of the storage tank during "unoccupied" fan/thermostat periods.
When "By Schedule" is chosen, you are asked to select a fan/thermostat schedule which defines the occupied and unoccupied
periods. It is important that this schedule is the same one used for air systems served by the plant or reflects a similar pattern of
occupied and unoccupied periods as the air systems use so space heating demands will be synchronized with the prioritization
control.
b. When OAT Above - Select this option to control prioritization by outdoor air dry-bulb temperature. When this option is selected you
are asked to specify an outdoor air dry-bulb (OAT) threshold temperature. With this control, space heating will have priority when
the OAT is colder than the threshold temperature. SHW loads will have priority when the OAT is warmer than the threshold
temperature. The philosophy is that at times of cold OAT, space heating loads are larger and therefore should have priority.
c. When OAT Below - For Changeover plants which serve combined space heating and SHW loads, this third option is offered. The
challenge with this type of plant is that during the summer cooling season, the plant must change from cooling mode to heating
mode to satisfy SHW loads. When this option is selected, a threshold OAT temperature must be specified. The plant will give
priority to space cooling loads when the OAT is warmer than this threshold temperature. The plant will give priority to SHW loads
and any space heating loads when the OAT is colder than this threshold temperature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Configuration Data tab when defining a chiller plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Configuration Tab (Chillers) / Plant Form
For Chiller Plants the Configuration tab contains information about the size, configuration and control of the plant.
This tab contains inputs grouped into the following four categories:
1. Equipment defines the number of chillers linked in parallel to form the plant and information about how the plant and the chillers will be
sized.
2. Cooling Controls allows the user to choose one of several different schemes for controlling chillers in the plant and to define the
method of controlling leaving chilled water temperature.
3. Free Cooling describes whether hydronic free cooling controls and equipment such as a strainer cycle or a waterside economizer are
used in the plant. These inputs are only relevant if the plant contains one or more water-cooled chillers.
4. Cooling Tower Configuration specifies how chillers and cooling towers are configured in the plant. This input is only relevant if the plant
will contain one or more water-cooled chillers.
Page 18 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Equipment Configuration (Chiller Plant)
12.0 Entering Plants ›› 12.5 Configuration Data (Chiller Plants) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Configuration (Chiller Plant)
The Equipment Configuration group of inputs defines the number of chillers linked in parallel to form the plant and contains information
about how the plant and the chillers will be sized. This group contains four inputs:
1. Chiller Sizing. The plant and its chillers can be sized in one of two ways.
a. Auto-Sized Chiller Capacities - For preliminary design or LEED applications where it is necessary to have the capacity
automatically determined, choose the "Auto-Sized Chiller Capacities" option. With this option the program will automatically
determine the plant design capacity using the peak plant load plus the Capacity Oversizing Factor (see below). Once the total plant
capacity is known, the program automatically divides the capacity among the chillers in the plant according to your specification of
chiller sizing splits (also see below).
b. User-Defined Capacity - When you want to directly specify capacities of chillers in the plant, choose the "User-Defined Chiller
Capacities" option.
Note that when you choose "Auto-Sized Chiller Capacities" you will only be able to link chillers to the plant which have the "Auto-Size
Capacity" option turned on. Likewise, if you choose "User-Defined Chiller Capacities" you will only be able to link chillers which have
the "Auto-Sized Capacity" option turned off. This is because the plant and its chillers must be synchronized in this regard. As a result,
on the Schedule of Equipment tab you will see different lists of available chillers in the chiller drop-down list depending on whether you
specified "Auto-Sized" or "User-Defined" capacities for the plant.
Page 19 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Cooling Controls (Chiller Plant)
12.0 Entering Plants ›› 12.5 Configuration Data (Chiller Plants) ››
2. Number of Chillers. This item defines the number of chillers in the plant. The program will evaluate a chiller plant comprised of up to
12 chillers connected in parallel. To change the value, press the up or down arrow next to the input value. The up arrow increases the
number. The down arrow decreases the number.
3. Chiller Sizing Splits. When you specify "Auto-Sized Chiller Capacities" you must also define how the plant capacity will be divided
among chillers in the plant. For example, if the plant contains two chillers, you are offered options such as "Equally Sized", "60%/40%",
"75%/25%" and so on. In these options the first percentage corresponds to CH-1 and the second percentage corresponds to CH-2
shown on the Schedule of Equipment tab. Note: When you specify "User-Defined Chiller Capacities" this input is not relevant and is
therefore disabled.
4. Capacity Oversizing Factor. When you specify "Auto-Sized Chiller Capacities" you must also define the oversizing factor for plant
capacity. For example, if you specify 15%, the program will automatically determine the plant capacity as peak coincident coil load for
air systems served by the plant plus 15%. Note: When you specify "User-Defined Chiller Capacities" this input is not relevant and is
therefore disabled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Controls (Chiller Plant)
The "Cooling Controls" group of inputs allows the user to choose one of several different schemes for controlling chillers in the plant and
to define the method of controlling leaving chilled water temperature. Plant control and chilled water temperature control inputs are
discussed separately below.
Plant Control. Three types of chiller plant control are offered by the program:
1. Sequenced. All chillers in the system are sequenced in the order they are defined on the Schedule of Equipment tab. Chiller 1 turns
on first. If its capacity is not sufficient to meet the load, chiller 2 turns on, and so forth. Chillers are turned on until the total capacity is
sufficient to meet the building load. While running, chillers share the building load by running at the same part-load ratio. The following
example illustrates sequenced control for a system comprised of three 500-ton chillers serving a building whose peak load is 1500
tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
1500
500
500
500
1250
417
417
417
1000
500
500
Off
750
375
375
Off
500
500
Off
Off
250
250
Off
Off
2. Part-Load Chiller: High+Low Loads. With this control, all chillers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load chiller acting as the last chiller to turn on. However, when the capacity of the part-load chiller
alone is sufficient to meet the building load, all other chillers turn off and the part-load chiller runs alone to serve the load. Therefore,
the part-load chiller runs for high and low load conditions and is off for intermediate load conditions. The following example illustrates
"part-load chiller: high+low loads" control for a system comprised of two 500-ton chillers and one 200-ton part-load chiller serving a
building whose peak load is 1200 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Part Load Tons
Page 20 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
1200
500
500
200
1000
500
500
Off
800
400
400
Off
600
300
300
Off
500
500
Off
Off
400
400
Off
Off
300
300
Off
Off
200
Off
Off
200
100
Off
Off
100
3. Equal Unloading. With this control, all chillers in the plant operate for all loads. There is no sequencing of chillers as occurs in the
other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 100-ton chillers
serving a building whose peak load is 300 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
300
100
100
100
240
80
80
80
180
60
60
60
120
40
40
40
60
20
20
20
LCHWT Control. The remaining inputs in this group describe how leaving chilled water temperature (LCHWT) is controlled:
1. LCHWT Control. The program offers three options for controlling plant LCHWT:
a. Constant LCHWT. With this control the design LCHWT (see below) is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant LCHWT is adjusted according to a reset schedule based on outdoor air dry-
bulb temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant LCHWT is adjusted based on plant load. LCHWT is adjusted to maintain the
return water temperature (RWT) at a constant value.
2. Design LCHWT defines the LCHWT set point for the design condition. This is the minimum LCHWT when reset controls are used.
3. … used when OAT greater than. This input specifies the outdoor air temperature (OAT) at and above which the design LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
4. Maximum LCHWT defines the warmest LCHWT allowed when reset controls are used.
5. … used when OAT less than. This input specifies the outdoor air temperature (OAT) at and below which the maximum LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
Example for Reset by OAT Schedule
Design LCHWT = 44 F
...used when OAT greater than = 65 F
Maximum LCHWT = 54 F
...used when OAT less than = 35 F
As shown in the figure, when the outdoor air temperature is 65 F or warmer, the plant controls the LCHWT to the design value of 44 F.
When the outdoor air temperature is 35 F or colder, the plant controls the LCHWT to the maximum value of 54 F. When the outdoor air
temperature is between 65 F and 35 F, the LCHWT varies between 44 F and 54 F along a linear control profile.
Page 21 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Free Cooling (Chiller Plant)
12.0 Entering Plants ›› 12.5 Configuration Data (Chiller Plants) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Free Cooling (Chiller Plant)
This group of inputs on the Configuration tab describe free cooling controls and equipment. Items in this section are as follows:
1. Use Free Cooling. Mark this check box if your system uses hydronic free cooling. Leave the check box blank if free cooling is not
used.
2. Type of Free Cooling. The program offers three types of free cooling:
a. Strainer Cycle. When return water from the cooling tower is sufficiently cold, return water is diverted into the chilled water loop to
serve AHU cooling coils and all chillers are turned off. Because fouling of the chilled water piping and heat exchangers is a concern,
a strainer device is used to filter the water as it flows from the condenser loop into the chilled water loop. Hence the name "Strainer
Cycle".
Example: The operating LCHWT for a system is 44 F. For a certain set of operating conditions, the cooling tower is able to produce
41 F return water. The chillers in the system are all turned off. Cooling tower water is diverted into the chilled water loop and is
blended to provide 44 F water to AHU cooling coils.
b. Non-Integrated Waterside Economizer. A plate-frame heat exchanger is positioned in parallel with chillers in the plant (see Figure
1). When return water from the cooling tower is sufficiently cold, it is diverted through the plate-frame heat exchanger where it cools
water in the chilled water loop, and all chillers in the system are turned off. "Non-Integrated" refers to the fact that the economizer
only operates when it can meet the full plant load. With this control either the economizer meets 100% of the load or the chillers
meet 100% of the load, but economizer and chillers do not operate simultaneously.
Example: The operating LCHWT for a system is 44 F. A Plate-Frame Heat Exchanger is used and provides an approach of 3.0 F.
For a certain set of operating conditions, the cooling tower is able to produce 41 F return water. With the 3 F heat exchanger
approach, cooling tower water can be used to produce 44 F water in the chilled water loop. Therefore the plate frame heat
exchanger can be used to supply cooling to the building. All chillers can be turned off.
c. Integrated Waterside Economizer. A plate-frame heat exchanger is positioned off the return water pipe upstream of the point
where return chilled water mixes with water from the common pipe (see Figure 2). When return water from the cooling tower is
sufficiently cold, it is diverted through the plate-frame heat exchanger where it precools return water and thereby reduces the load
on the chillers. As the return cooling tower water temperature drops, the plate frame heat exchanger will be able to handle
progressively more of the plant load until the point where all chillers are off and the heat exchanger handles 100% of the load.
"Integrated" refers to the fact that the economizer can operate simultaneously with the chillers. It can therefore provide partial as
well as full free cooling and therefore yields greater energy savings potential than the non-integrated type of waterside economizer.
Example: The operating LCHWT for a system is 44 F. An Integrated Waterside Economizer is used and provides an approach of
3.0 F. For a certain set of operating conditions, return water temperature in the chilled water loop is 51 F and the cooling tower
return water temperature is 46 F. The plate-frame heat exchanger can therefore precool return chilled water from 51 F to 49 F. This
reduces the entering water temperature for chillers and therefore reduces the chiller load.
Page 22 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Cooling Tower Configuration (Chiller Plant)
12.0 Entering Plants ›› 12.5 Configuration Data (Chiller Plants) ››
3. Heat Exchanger Approach defines the performance of the plate frame heat exchanger used in a waterside economizer. The
approach is the difference between the temperature of water entering the heat exchanger minus the temperature of water in the chilled
water loop leaving the heat exchanger.
Example: For a given set of flow conditions, 41 F return water from the tower entering the plate-frame heat exchanger will produce
chilled water leaving the heat exchanger at a temperature of 44 F. Therefore the heat exchanger approach is 3 F.
Note for Plants Containing Air-Cooled Chillers. Free cooling inputs only apply for plants containing one or more water-cooled chillers.
If you are entering a plant with all air-cooled chillers, ignore this input. It will not have any effect on system calculations.
Figure 1. Non-Integrated Waterside Economizer - Configuration of Components
(This example shows components for a primary-only constant speed distribution system)
Figure 2. Integrated Waterside Economizer - Configuration of Components
(This example shows components for a primary-only constant speed distribution system)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Tower Configuration (Chiller Plant)
This item defines how cooling towers and chillers in the plant are configured. The program offers two configuration options:
Page 23 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.6 Configuration Data (Changeover Plants)
12.0 Entering Plants ››
Configuration Tab (Changeover) / Plant Form
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
1. One Tower for Each W/C Chiller. With this configuration a separate cooling tower or dry cooler is paired with each water-cooled
chiller in the plant. There is a single condenser water loop with manifolded pumps. The cooling tower or dry cooler and its condenser
pump stage on and off with the corresponding chiller. On the Schedule of Equipment tab you will specify one cooling tower or dry
cooler for each water-cooled chiller in the plant.
2. One Tower Shared by All W/C Chillers in System. With this configuration one large cooling tower or dry cooler is shared by all
water-cooled chillers in the plant. Condenser water flow for all water-cooled chillers is combined and piped to and from the cooling
tower or dry cooler. One condenser water pump drives flow through the plant.
When used in a plant where chillers are sequenced on and off, enhanced performance can be achieved when several chillers have
been sequenced off since a larger heat transfer area is available for a remaining number of chillers to use. However, that gain in heat
transfer efficiency is sometimes offset by the increased condenser water pump power.
Note:
a. Plants Consisting of Air-Cooled Chillers. The Cooling Tower Configuration input typically only applies to systems containing one or
more water-cooled chillers. For a plant consisting of air-cooled chillers, waterside economizer can be modeled by specifying "one
tower shared by all W/C chillers in system" and then specifying a shared cooling tower. This cooling tower will serve to precool return
water in the chilled water loop to reduce or eliminate the chiller load, when conditions allow free cooling. On the other hand, if you are
modeling a plant of air-cooled chillers without waterside economizer, this cooling tower configuration input item is not used and has no
effect on plant calculations..
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Configuration Data tab when defining a changeover plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Configuration Tab (Changeover) / Plant Form
For Changeover Plants the Configuration tab contains information about the size, configuration and control of the plant.
This tab contains inputs grouped into the following six categories:
1. Equipment defines the number of reversible chillers linked in parallel to form the plant and information about how the plant and the
chillers will be sized.
2. Cooling Controls allows the user to choose one of several different schemes for controlling the chillers in cooling mode in the plant and
to define the method of controlling chilled water supply temperature.
3. Heating Controls allows the user to choose one of several different schemes for controlling the chillers in heating mode in the plant and
to define the method of controlling hot water supply temperature.
4. Free Cooling describes whether hydronic free cooling controls and equipment such as a strainer cycle or a waterside economizer are
used in the plant. These inputs are only relevant if the plant contains one or more water-cooled chillers and only pertain to cooling
mode.
5. Auxiliary Heating specifies whether auxiliary heating capability exists and, if so, how it is controlled. This only pertains to heating
mode.
Page 24 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Equipment Configuration (Changeover)
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Configuration (Changeover)
The Equipment Configuration group of inputs defines the number of reversible chillers linked in parallel to form the plant and contains
information about how the plant and the chillers will be sized. This group contains four inputs:
1. Equipment Sizing. The plant and its chillers can be sized in one of three ways.
For preliminary design or LEED applications where it is necessary to have the capacity automatically determined, choose one of the
"Auto-Sized Capacities" options. Once the total plant capacity is known, the program automatically divides the capacity among the
chillers in the plant according to your specification of the chiller sizing splits (also see below). For detailed design scenarios where
specific equipment capacities are known, use the "User-Defined Capacity" option.
a. Auto-Sized Capacities (Based on Cooling Loads) - With this option the program will automatically determine the plant design
capacity using the peak plant cooling load plus the Capacity Oversizing Factor (see below).
b. Auto-Sized Capacities (Based on Heating Loads) - With this option the program will automatically determine the plant design
capacity using the peak plant heating load plus the Capacity Oversizing Factor (see below).
c. User-Defined Capacity - When you want to directly specify capacities of reversible chillers in the plant, choose the "User-Defined
Capacities" option.
Page 25 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Cooling Controls (Changeover)
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
Note that when you choose one of the "Auto-Sized Capacities" options you will only be able to link chillers to the plant which have the
"Auto-Size Capacity" option turned on. Likewise, if you choose "User-Defined Capacities" you will only be able to link chillers which
have the "Auto-Sized Capacity" option turned off. This is because the plant and its chillers must be synchronized in this regard. As a
result, on the Schedule of Equipment tab you will see different lists of available chillers in the equipment drop-down list depending on
whether you specified "Auto-Sized" or "User-Defined" capacities for the plant.
2. Number of Units. This item defines the number of chillers in the plant. The program will evaluate a plant comprised of up to 12 chillers
connected in parallel. To change the value, press the up or down arrow next to the input value. The up arrow increases the number.
The down arrow decreases the number.
3. Sizing Splits. When you specify one of the "Auto-Sized Capacities" options you must also define how the plant capacity will be divided
among chillers in the plant. For example, if the plant contains two chillers, you are offered options such as "Equally Sized", "60%/40%",
"75%/25%" and so on. In these options the first percentage corresponds to chillers 1 and the second percentage corresponds to
chillers 2 shown on the Schedule of Equipment tab. Note: When you specify "User-Defined Capacities" this input is not relevant and is
therefore disabled.
4. Capacity Oversizing Factor. When you specify one of the "Auto-Sized Capacities" options you must also define the oversizing factor
for plant capacity. For example, if you specify 15%, the program will automatically determine the plant capacity as peak coincident coil
load for air systems served by the plant plus 15%. Note: When you specify "User-Defined Capacities" this input is not relevant and is
therefore disabled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Controls (Changeover)
The "Cooling Controls" group of inputs allows the user to choose one of several different schemes for controlling the reversible chillers
when in cooling mode. These inputs also define the method of controlling leaving chilled water temperature when the plant is in cooling
mode. Inputs are described below.
Plant Control. Three types of chiller controls are offered by the program:
1. Sequenced. All chillers in the system are sequenced in the order they are defined on the Schedule of Equipment tab. Chiller 1 turns
on first. If its capacity is not sufficient to meet the load, chiller 2 turns on, and so forth. Chillers are turned on until the total capacity is
sufficient to meet the building load. While running, chillers share the building load by running at the same part-load ratio. The following
example illustrates sequenced control for a system comprised of three 100-ton chillers serving a building whose peak load is 300 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
300
100
100
100
250
83
83
83
200
100
100
Off
150
75
75
Off
100
100
Off
Off
50
50
Off
Off
2. Part-Load Chiller: High+Low Loads. With this control, all chillers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load chiller acting as the last chiller to turn on. However, when the capacity of the part-load chiller
alone is sufficient to meet the building load, all other chillers turn off and the part-load chiller runs alone to serve the load. Therefore,
Page 26 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
the part-load chiller runs for high and low load conditions and is off for intermediate load conditions. The following example illustrates
"part-load chiller: high+low loads" control for a system comprised of two 100-ton chillers and one 50-ton part-load chiller serving a
building whose peak load is 250 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Part Load Tons
250
100
100
50
200
100
100
Off
150
75
75
Off
100
50
50
Off
50
Off
Off
50
25
Off
Off
25
3. Equal Unloading. With this control, all chillers in the plant operate for all loads. There is no sequencing of chillers as occurs in the
other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 100-ton chillers
serving a building whose peak load is 300 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
300
100
100
100
240
80
80
80
180
60
60
60
120
40
40
40
60
20
20
20
LCHWT Control. The remaining inputs in this group describe how leaving chilled water temperature (LCHWT) is controlled:
1. LCHWT Control. The program offers three options for controlling plant LCHWT:
a. Constant LCHWT. With this control the design LCHWT (see below) is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant LCHWT is adjusted according to a reset schedule based on outdoor air dry-
bulb temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant LCHWT is adjusted based on plant load. LCHWT is adjusted to maintain the
return water temperature (RWT) at a constant value.
2. Design LCHWT defines the LCHWT set point for the design condition. This is the minimum LCHWT when reset controls are used.
3. … used when OAT greater than. This input specifies the outdoor air temperature (OAT) at and above which the design LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
4. Maximum LCHWT defines the warmest LCHWT allowed when reset controls are used.
5. … used when OAT less than. This input specifies the outdoor air temperature (OAT) at and below which the maximum LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
Example for Reset by OAT Schedule
Design LCHWT = 44 F
...used when OAT greater than = 65 F
Maximum LCHWT = 54 F
...used when OAT less than = 35 F
As shown in the figure, when the outdoor air temperature is 65 F or warmer, the plant controls the LCHWT to the design value of 44 F.
When the outdoor air temperature is 35 F or colder, the plant controls the LCHWT to the maximum value of 54 F. When the outdoor air
temperature is between 65 F and 35 F, the LCHWT varies between 44 F and 54 F along a linear control profile.
Page 27 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Heating Controls (Changeover)
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
5. Changeover Delay - This input specifies the delay imposed when the plant changes from heating mode into cooling mode. This delay
may be required because of physical limitations of the equipment or control rules. For example, an interval of time may be required to
allow supply water loop temperatures to fall from heating mode levels to neutral levels to avoid introducing unusually hot water into the
chiller's evaporator. During the delay period the plant will not operate so plant loads will not be served and no energy will be
consumed by the plant equipment.
If a delay exists for this changeover plant, specify it in minutes. If no delay is required, or you want to model the idealized plant
operation where no delay exists, specify zero minutes.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Controls (Changeover)
Figure Title
The "Heating Controls" group of inputs allows the user to choose one of several different schemes for controlling reversible chillers when
in heating mode. This section also provides options for defining the method of controlling hot water supply temperature (HWST).
Plant Control. Three types of plant control are offered by the program:
1. Sequenced. All reversible chillers in the system are sequenced for heating mode in the order they are defined on the Schedule of
Equipment tab. For example, chiller 1 turns on first. If its capacity is not sufficient to meet the load, chiller 2 turns on, and so forth.
Chillers are turned on until the total capacity is sufficient to meet the building load. While running, chillers share the building load by
running at the same part-load ratio. The following example illustrates sequenced control for a system comprised of three 1000 MBH
heating capacity reversible chillers serving a building whose peak heating load is 3000 MBH.
Building Load
Chiller 1 (MBH)
Chiller 2 (MBH)
Chiller 3 (MBH)
3000
1000
1000
1000
2500
833
833
833
2000
1000
1000
Off
Page 28 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
1500
750
750
Off
1000
1000
Off
Off
500
500
Off
Off
2. Part-Load Unit: High+Low Loads. With this control, all chillers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load chiller acting as the last unit to turn on. However, when the capacity of the part-load reversible
chiller alone is sufficient to meet the building load, all other chillers turn off and the part-load unit runs alone to serve the load.
Therefore, the part-load chiller runs for high and low load conditions and is off for intermediate load conditions. The following example
illustrates "part-load unit: high+low loads" control for a system comprised of two 1000 MBH heating capacity reversible chillers and one
250 MBH part-load reversible chiller serving a building whose peak heating load is 1250 MBH.
Building Load
Chiller 1 (MBH)
Chiller 2 (MBH)
Part Load (MBH)
2250
1000
1000
250
2000
1000
1000
Off
1500
750
750
Off
1000
500
500
Off
500
250
250
Off
250
Off
Off
250
125
Off
Off
125
3. Equal Unloading. With this control, reversible chillers in the plant operate for all loads. There is no sequencing of equipment as
occurs in the other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 1000
MBH heating capacity reversible chillers serving a building whose peak heating load is 3000 MBH.
Building Load
Chiller 1 (MBH)
Chiller 2 (MBH)
Chiller 3 (MBH)
3000
1000
1000
1000
2500
833
833
833
2000
667
667
667
1500
500
500
500
1000
333
333
333
Hot Water Supply Temperature (HWST) Control. The remaining inputs in this group describe how hot water supply temperature
(HWST) is controlled.
1. HWST Control. The program offers three options for controlling plant HWST:
a. Constant HWST. With this control the design HWST is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant HWST is adjusted according to a reset schedule based on outdoor air dry-bulb
temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant HWST is adjusted based on plant load. HWST is adjusted to maintain the return
water temperature (RWT) at a constant value.
2. Design HWST defines the HWST set point for the design condition. This is the maximum HWST when reset controls are used.
3. … used when OAT less than. This input defines the outdoor air temperature (OAT) at and below which the design HWST is used.
This input is only enabled when the "Reset by OAT Schedule" option is selected.
4. Minimum HWST defines the coolest HWST allowed when reset controls are used.
5. … used when OAT greater than. This input defines the outdoor air temperature (OAT) at and above which the minimum HWST is
used. This input is only enabled when the "Reset by OAT Schedule" option is selected.
Reset by OAT Schedule Example:
Design HWST = 180 F
…used when OAT less than = 20 F
Minimum HWST = 130 F
…used when OAT greater than = 50 F
As shown in the figure, when the outdoor air temperature is 20 F or colder, the plant controls the HWST to the design value of 180 F.
When the outdoor air temperature is 50 F or warmer, the plant controls the HWST to the minimum value of 130 F. When the outdoor
air temperature is between 20 F and 50 F, the HWST varies between 180 F and 130 F along a linear control profile.
Page 29 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Free Cooling (Changeover)
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
6. Changeover Delay - This input specifies the delay imposed when the plant changes from cooling mode into heating mode. This delay
may be required because of physical limitations of the equipment or control rules. For example, an interval of time may be required to
allow supply water loop temperatures to rise from cooling mode levels to neutral levels to avoid introducing unusually cold into the
chiller's condenser. During the delay period the plant will not operate so plant loads will not be served and no energy will be
consumed by the plant equipment.
If a delay exists for this changeover plant, specify it in minutes. If no delay is required, or you want to model the idealized plant
operation where no delay exists, specify zero minutes.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Free Cooling (Changeover)
This group of inputs on the Configuration tab describe free cooling controls and equipment for cooling mode. Items in this section are as
follows:
1. Use Free Cooling. Mark this check box if your system uses hydronic free cooling. Leave the check box blank if free cooling is not
used.
2. Type of Free Cooling. The program offers three types of free cooling:
a. Strainer Cycle. When source water is sufficiently cold, source water is diverted into the chilled water loop to serve AHU cooling
coils and all chillers are turned off. Because fouling of the chilled water piping and heat exchangers is a concern, a strainer device is
used to filter the water as it flows from the source loop into the chilled water loop. Hence the name "Strainer Cycle".
Example: The operating LCHWT for a system is 44 F. For a certain set of operating conditions, the geo well field is able to produce
41 F return water. The chillers in the system are all turned off. Source water is diverted into the chilled water loop and is blended to
provide 44 F water to AHU cooling coils.
b. Non-Integrated Waterside Economizer. A plate-frame heat exchanger is positioned in parallel with chillers in the plant (see Figure
1). When return water from the geo well field is sufficiently cold, it is diverted through the plate-frame heat exchanger where it cools
water in the chilled water loop, and all chillers in the system are turned off. "Non-Integrated" refers to the fact that the economizer
only operates when it can meet the full plant load. With this control either the economizer meets 100% of the load or the chillers
meet 100% of the load, but economizer and chillers do not operate simultaneously.
Example: The operating LCHWT for a system is 44 F. A Plate-Frame Heat Exchanger is used and provides an approach of 3.0 F.
For a certain set of operating conditions, the cooling tower is able to produce 41 F return water. With the 3 F heat exchanger
Page 30 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
approach, source water can be used to produce 44 F water in the chilled water loop. Therefore the plate frame heat exchanger can
be used to supply cooling to the building. All chillers can be turned off.
c. Integrated Waterside Economizer. A plate-frame heat exchanger is positioned off the return water pipe upstream of the point
where return chilled water mixes with water from the common pipe (see Figure 2). When source water from the geo well field is
sufficiently cold, it is diverted through the plate-frame heat exchanger where it precools return water and thereby reduces the load
on the chillers. As the return cooling tower water temperature drops, the plate frame heat exchanger will be able to handle
progressively more of the plant load until the point where all heat pumps are off and the heat exchanger handles 100% of the load.
"Integrated" refers to the fact that the economizer can operate simultaneously with the chillers. It can therefore provide partial as
well as full free cooling and therefore yields greater energy savings potential than the non-integrated type of waterside economizer.
Example: The operating LCHWT for a system is 44 F. An Integrated Waterside Economizer is used and provides an approach of
3.0 F. For a certain set of operating conditions, return water temperature in the chilled water loop is 51 F and the geo well field
source water temperature is 46 F. The plate-frame heat exchanger can therefore precool return chilled water from 51 F to 49 F. This
reduces the entering water temperature for chiller and therefore reduces the chiller cooling load.
3. Heat Exchanger Approach defines the performance of the plate frame heat exchanger used in a waterside economizer. The
approach is the difference between the temperature of water entering the heat exchanger minus the temperature of water in the chilled
water loop leaving the heat exchanger.
Example: For a given set of flow conditions, 41 F source water from the geo well field entering the plate-frame heat exchanger will
produce chilled water leaving the heat exchanger at a temperature of 44 F. Therefore the heat exchanger approach is 3 F.
Note for Plants Containing Air-to-Water Reversible Chillers. Free cooling inputs only apply for plants containing one or more water-
to-water reversible chillers. If you are entering a plant with all air-to-water reversible chillers, ignore this input. It will not have any effect on
system calculations.
Figure 1. Non-Integrated Waterside Economizer - Configuration of Components
(This example shows components for a primary-only constant speed distribution system)
Figure 2. Integrated Waterside Economizer - Configuration of Components
(This example shows components for a primary-only constant speed distribution system)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 31 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Auxiliary Heating (Changeover)
12.0 Entering Plants ›› 12.6 Configuration Data (Changeover Plants) ››
12.7 Configuration Data (Heat Recovery)
12.0 Entering Plants ››
Configuration Tab (Heat Recovery) / Plant Form
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
Auxiliary Heating (Changeover)
This group of inputs defines whether auxiliary heating is available for the plant and, if so, defines controls for the heater. This section
consists of 5 inputs:
1. Auxiliary Heating. Check this box if the plant has an auxiliary heater. Inputs in this section will then be enabled. Auxiliary heaters
are typically used for changeover plants with air-to-water reverisible chillers. As outdoor air temperature decreases, capacity and
efficiency of the chiller can decline to a point where either the reversible chillers cannot meet the plant heating load and/or operating
the chiller becomes too inefficient in heating mode. In both situations an auxiliary heater can be used to supplement plant heating
capacity to meet the plant demand, or to handle the full plant load and allow the chiller to be turned off. When auxiliary heating is
selected, the auxiliary heating device will be specified on the Schedule of Equipment tab.
If the plant contains water-to-water reversible chillers, this equipment may or may not require auxiliary heating capability.
2. Allow Simultaneous Auxiliary. Check this box if the auxiliary heater is allowed to operate simultaneously with the chillers. Checking
the box models a plant in which the chillers serve as first stage heat and when they are unable to meet the plant load, the auxiliary
heaters turn on as second stage heat to meet the remainder of the load. The plant runs in this way until the COP or OAT trigger is
reached, if either of these triggers are specified. Once a trigger is reached the plant switches to 100% auxiliary.
In other plants either the chillers run or the auxiliary heater runs, but not both. To model this type of plant leave the box unchecked.
For this control once the chiller heating capacity is insufficient to meet a plant load, the chillers turn off and auxiliary serves 100% of
the plant load. The plant controller will also turn the reversible chillers off and use auxiliary heat to meet 100% of the load if the COP
or OAT trigger is reached, if either of these triggers are specified.
3. H/X Approach. If the auxiliary heater is a boiler or remote source and heat is transferred to the hot water supply loop via a heat
exchanger, check this box and specify the approach for the heat exchanger. If the auxiliary is an electric sleeve heater or is a boiler
which supplies hot water directly into the hot water supply loop, leave the box unchecked.
4. Trigger: COP Below. Check this box if the plant has controls that will turn off the reversible chillers when their operating COP drops
below a threshold and runs 100% auxiliary heat below this threshold. For example if the box is checked and a "COP Below" value of
2.5 is specified, the reversible chillers will turn off when their operating COP falls below 2.5.
5. Trigger: OAT Below. Check this box if the plant has controls that will turn off the air source reversible chillers when the outdoor air
dry-bulb temperature (OAT) falls below a specified threshold temperature. For example if the box is checked and the "OAT Below"
value of 15 F is specified, the air source reversible chillers will turn off when the OAT is colder than 15 F and the auxiliary heater will
serve 100% of the plant load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Configuration Data tab when defining a heat recovery plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Configuration Tab (Heat Recovery) / Plant Form
For Heat Recovery Plants the Configuration tab contains information about the size, configuration and control of the plant.
This tab contains inputs grouped into the following six categories:
1. Equipment Configuration defines the number of chillers and boilers in the plant and how the equipment will be sized.
2. Cooling Controls allows the user to choose a scheme for controlling the chillers and the method of controlling chilled water supply
temperature.
3. Heating Controls allows the user to choose a scheme for controlling the boilers and the method of controlling hot water supply
temperature.
Page 32 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Equipment Configuration (Heat Recovery)
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
4. Cooling Tower Configuration specifies how chillers and cooling towers are configured in the plant. This input is only relevant if the plant
will contain one or more water-cooled chillers.
5. Heat Recovery Configuration specifies the method used to recover heat from the chilled water system and apply it to loads in the hot
water system.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Configuration (Heat Recovery)
The Equipment Configuration group of inputs defines the number of chillers and boilers in the plant. Inputs are divided into three groups.
1. Equipment Sizing. The plant components can be sized in one of two ways.
a. Auto-Sized Capacities - For preliminary design where it is necessary to have the capacity automatically determined, choose the
"Auto-Sized Capacities" option. With this option the program will automatically determine the plant design capacities using the peak
plant loads plus the Capacity Oversizing Factors (see below). Once the total plant capacities are known, the program automatically
divides the cooling capacity among the chillers in the plant and the heating capacity among the boilers in the plant according to your
specification of sizing splits (also see below).
Page 33 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Cooling Controls (Heat Recovery)
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
b. User-Defined Capacity - For detailed design applications when you want to directly specify chiller and boiler capacities, choose the
"User-Defined Capacities" option.
Note that when you choose "Auto-Sized Capacities" you will only be able to link chillers and boilers to the plant which have the "Auto-
Size Capacity" option turned on. Likewise, if you choose "User-Defined Capacities" you will only be able to link chillers and boilers
which have the "Auto-Sized Capacity" option turned off. This is because the plant and its equipment must be synchronized in this
regard. As a result, on the Schedule of Equipment tab you will see different lists of available chillers and boilers in the drop-down lists
depending on whether you specified "Auto-Sized" or "User-Defined" capacities for the plant.
2. Chillers. Specify the following data for chillers in the plant:.
a. Quantity - Specify the number of chillers connected in parallel in the plant. To change the value, press the up or down arrow next
to the input value. The up arrow increases the quantity. The down arrow decreases the quantity.
Note: For heat recovery plants using the "Dedicated heat recovery chiller in parallel with cooling-only chillers" or "Dedicated heat
recovery chiller in condenser loop" schemes, the chiller quantity does not include the dedicated heat recovery chiller (DHRC). The
DHRC is automatically added as a separate equipment on the schedule of equipment. For example, if the inputs shown above are
for a DHRC heat recovery plant, there will be two cooling-only chillers and an additional dedicated heat recovery chiller in the plant.
b. Chiller Sizing Splits - When you specify "Auto-Sized Capacities" you must also define how the plant cooling capacity will be
divided among chillers in the plant. For example, if the plant contains two chillers, you are offered options such as "Equally Sized",
"60%/40%", "75%/25%" and so on. In these options the first percentage corresponds to CH-1 and the second percentage
corresponds to CH-2 shown on the Schedule of Equipment tab. Note: When you specify "User-Defined Capacities" this input is not
relevant and is therefore disabled.
c. Capacity Oversizing Factor - When you specify "Auto-Sized Capacities" you must also define the oversizing factor for plant
heating capacity. For example, if you specify 15%, the program will automatically determine the plant cooling capacity as peak
coincident cooling coil load for air systems served by the plant plus 15%. Note: When you specify "User-Defined Capacities" this
input is not relevant and is therefore disabled.
3. Boilers. Specify the following data for boilers in the plant:.
a. Quantity - Specify the number of boilers connected in parallel in the plant. To change the value, press the up or down arrow next to
the input value. The up arrow increases the quantity. The down arrow decreases the quantity.
b. Boiler Sizing Splits - When you specify "Auto-Sized Capacities" you must also define how the plant heating capacity will be divided
among boilers in the plant. For example, if the plant contains two boilers, you are offered options such as "Equally Sized",
"60%/40%", "75%/25%" and so on. In these options the first percentage corresponds to B-1 and the second percentage
corresponds to B-2 shown on the Schedule of Equipment tab. Note: When you specify "User-Defined Capacities" this input is not
relevant and is therefore disabled.
c. Capacity Oversizing Factor - When you specify "Auto-Sized Capacities" you must also define the oversizing factor for plant
cooling capacity. For example, if you specify 25%, the program will automatically determine the plant heating capacity as peak
coincident heating coil load for air systems served by the plant plus 25%. Note: When you specify "User-Defined Capacities" this
input is not relevant and is therefore disabled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Controls (Heat Recovery)
The "Cooling Controls" group of inputs allows the user to choose one of several different schemes for controlling the chillers in the plant.
These inputs also define the method of controlling leaving chilled water temperature. Inputs are described below.
Plant Control. Three types of chiller controls are offered by the program:
Note: For the "Dedicated heat recovery chiller in parallel with cooling only chillers" type of heat recovery plant, the dedicated heat
recovery chiller (DHRC) functions as "Chiller 1" in the sequencing schemes below. However, there are special conditions where the
DHRC is off (no heat recovery demand) or has limited cooling capacity (limited heat recovery demand, or low source water
Page 34 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
temperature cutoff). In these cases the cooling contributed by the DHRC as "Chiller 1" is reduced or eliminated and the remaining
chillers in the sequence handle the remaining cooling load.
1. Sequenced. All chillers in the system are sequenced in the order they are defined on the Schedule of Equipment tab. Chiller 1 turns
on first. If its capacity is not sufficient to meet the load, chiller 2 turns on, and so forth. Chillers are turned on until the total capacity
is sufficient to meet the building load. While running, chillers share the building load by running at the same part-load ratio. The
following example illustrates sequenced control for a system comprised of three 100-ton chillers serving a building whose peak load
is 300 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
300
100
100
100
250
83
83
83
200
100
100
Off
150
75
75
Off
100
100
Off
Off
50
50
Off
Off
2. Part-Load Chiller: High+Low Loads. With this control, all chillers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load chiller acting as the last chiller to turn on. However, when the capacity of the part-load
chiller alone is sufficient to meet the building load, all other chillers turn off and the part-load chiller runs alone to serve the load.
Therefore, the part-load chiller runs for high and low load conditions and is off for intermediate load conditions. The following
example illustrates "part-load chiller: high+low loads" control for a system comprised of two 100-ton chillers and one 50-ton part-
load chiller serving a building whose peak load is 250 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Part Load Tons
250
100
100
50
200
100
100
Off
150
75
75
Off
100
50
50
Off
50
Off
Off
50
25
Off
Off
25
3. Equal Unloading. With this control, all chillers in the plant operate for all loads. There is no sequencing of chillers as occurs in the
other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 100-ton chillers
serving a building whose peak load is 300 tons.
Building Load
Chiller 1 Tons
Chiller 2 Tons
Chiller 3 Tons
300
100
100
100
240
80
80
80
180
60
60
60
120
40
40
40
60
20
20
20
LCHWT Control. The remaining inputs in this group describe how leaving chilled water temperature (LCHWT) is controlled:
1. LCHWT Control. The program offers three options for controlling plant LCHWT:
a. Constant LCHWT. With this control the design LCHWT (see below) is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant LCHWT is adjusted according to a reset schedule based on outdoor air dry-
bulb temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant LCHWT is adjusted based on plant load. LCHWT is adjusted to maintain the
return water temperature (RWT) at a constant value.
2. Design LCHWT defines the LCHWT set point for the design condition. This is the minimum LCHWT when reset controls are used.
3. … used when OAT greater than. This input specifies the outdoor air temperature (OAT) at and above which the design LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
4. Maximum LCHWT defines the warmest LCHWT allowed when reset controls are used.
5. … used when OAT less than. This input specifies the outdoor air temperature (OAT) at and below which the maximum LCHWT is
used. This input is only enabled when using "Reset by OAT Schedule".
Page 35 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Heating Controls (Heat Recovery)
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
Example for "Reset by OAT Schedule":
Design LCHWT = 44 F
...used when OAT greater than = 65 F
Maximum LCHWT = 54 F
...used when OAT less than = 35 F
As shown in the figure, when the outdoor air temperature is 65 F or warmer, the plant controls the LCHWT to the design value of 44 F.
When the outdoor air temperature is 35 F or colder, the plant controls the LCHWT to the maximum value of 54 F. When the outdoor air
temperature is between 65 F and 35 F, the LCHWT varies between 44 F and 54 F along a linear control profile.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Controls (Heat Recovery)
The "Heating Controls" group of inputs allows the user to choose one of several different schemes for controlling boilers in the plant.
This section also provides options for defining the method of controlling hot water supply temperature (HWST).
Plant Control. Three types of plant control are offered by the program:
1. Sequenced. All boilers in the system are sequenced in the order they are defined on the Schedule of Equipment tab. For example,
boiler 1 turns on first. If its capacity is not sufficient to meet the load, boiler 2 turns on, and so forth. boilers are turned on until the
total capacity is sufficient to meet the plant heating load. While running, boilers share the plant load by running at the same part-
load ratio. The following example illustrates sequenced control for a system comprised of three 1000 MBH boilers serving a building
whose peak heating load is 3000 MBH.
Building Load
Boiler 1 (MBH)
Boiler 2 (MBH)
Boiler 3 (MBH)
3000
1000
1000
1000
2500
833
833
833
2000
1000
1000
Off
Page 36 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
1500
750
750
Off
1000
1000
Off
Off
500
500
Off
Off
2. Part-Load Unit: High+Low Loads. With this control, all boilers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load boiler acting as the last unit to turn on. However, when the capacity of the part-load boiler
alone is sufficient to meet the building load, all other boilers turn off and the part-load unit runs alone to serve the load. Therefore,
the part-load boilers runs for high and low load conditions and is off for intermediate load conditions. The following example
illustrates "part-load unit: high+low loads" control for a system comprised of two 1000 MBH boilers and one 250 MBH part-load
boilers serving a building whose peak heating load is 1250 MBH.
Building Load
Boiler 1 (MBH)
Boiler 2 (MBH)
Part Load (MBH)
2250
1000
1000
250
2000
1000
1000
Off
1500
750
750
Off
1000
500
500
Off
500
250
250
Off
250
Off
Off
250
125
Off
Off
125
3. Equal Unloading. With this control, boilers in the plant operate for all loads. There is no sequencing of equipment as occurs in the
other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 1000 MBH
boilers serving a building whose peak heating load is 3000 MBH.
Building Load
Boiler 1 (MBH)
Boiler 2 (MBH)
Boiler 3 (MBH)
3000
1000
1000
1000
2500
833
833
833
2000
667
667
667
1500
500
500
500
1000
333
333
333
Hot Water Supply Temperature (HWST) Control. The remaining inputs in this group describe how hot water supply temperature
(HWST) is controlled.
1. HWST Control. The program offers three options for controlling plant HWST:
a. Constant HWST. With this control the design HWST is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant HWST is adjusted according to a reset schedule based on outdoor air dry-
bulb temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant HWST is adjusted based on plant load. HWST is adjusted to maintain the
return water temperature (RWT) at a constant value.
2. Design HWST defines the HWST set point for the design condition. This is the maximum HWST when reset controls are used.
3. … used when OAT less than. This input defines the outdoor air temperature (OAT) at and below which the design HWST is used.
This input is only enabled when the "Reset by OAT Schedule" option is selected.
4. Minimum HWST defines the coolest HWST allowed when reset controls are used.
5. … used when OAT greater than. This input defines the outdoor air temperature (OAT) at and above which the minimum HWST is
used. This input is only enabled when the "Reset by OAT Schedule" option is selected.
Reset by OAT Schedule Example:
Design HWST = 180 F
…used when OAT less than = 20 F
Minimum HWST = 130 F
…used when OAT greater than = 50 F
As shown in the figure, when the outdoor air temperature is 20 F or colder, the plant controls the HWST to the design value of 180 F.
When the outdoor air temperature is 50 F or warmer, the plant controls the HWST to the minimum value of 130 F. When the outdoor
air temperature is between 20 F and 50 F, the HWST varies between 180 F and 130 F along a linear control profile.
Page 37 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Cooling Tower Configuration (Heat Recovery)
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
Heat Recovery Configuration (Heat Recovery)
12.0 Entering Plants ›› 12.7 Configuration Data (Heat Recovery) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Tower Configuration (Heat Recovery)
This item defines how cooling towers and chillers in the plant are configured. The program offers two configuration options:
1. One Tower for Each W/C Chiller. With this configuration a separate cooling tower or dry cooler is paired with each water-cooled
chiller in the plant. There is a single condenser water loop with manifolded pumps. The cooling tower or dry cooler and its condenser
pump stage on and off with the corresponding chiller. On the Schedule of Equipment tab you will specify one cooling tower or dry
cooler for each water-cooled chiller in the plant.
2. One Tower Shared by All W/C Chillers in System. With this configuration one large cooling tower or dry cooler is shared by all
water-cooled chillers in the plant. Condenser water flow for all water-cooled chillers is combined and piped to and from the cooling
tower or dry cooler. One condenser water pump drives flow through the plant.
When used in a plant where chillers are sequenced on and off, enhanced performance can be achieved when several chillers have
been sequenced off since a larger heat transfer area is available for a remaining number of chillers to use. However, that gain in heat
transfer efficiency is sometimes offset by the increased condenser water pump power.
Note:
a. Plants Consisting of Air-Cooled Chillers. The Cooling Tower Configuration is not relevant for heat recovery plants consisting of air-
cooled chillers. This input has no effect on plant performance calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heat Recovery Configuration (Heat Recovery)
This item defines the heat recovery method used in the plant. HAP offers six options::
Page 38 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.8 Configuration Data (Hot Water Plants)
12.0 Entering Plants ››
Configuration Tab (Hot Water) / Plant Form
12.0 Entering Plants ›› 12.8 Configuration Data (Hot Water Plants) ››
1. Dedicated Heat Recovery Chiller in Parallel with Cooling Only Chillers. This plant consists of one or more air-cooled or water
cooled cooling-only chillers in parallel. A dedicated heat recovery chiller (DHRC) is positioned in parallel with the cooling chillers and
acts as the lead chiller. The DHRC condenser is connected to the return water pipe in the hot water system. The DHRC is controlled
to operate when heating demands exist in the hot water system. When operating it contributes cooling to the chilled water system and
simultaneously rejects heat to the hot water system, to reduce the load on the heating system's boilers, thereby reducing boiler energy
use.
2. Heat Exchanger in Condenser Loop. This plant consists of one or more water cooled chillers in parallel rejecting heat to a condenser
water loop using cooling towers or dry coolers.A heat exchanger is connected to the condenser water pipe downstream of the chiller
condenser water outlet and upstream of the cooling tower inlet. This heat exchanger is also connected to the return pipe of the hot
water supply system. The heat exchanger therefore transfer heat from the condenser water loop to the hot water system. In order to
successfully recovery heat by this method, the condenser water temperature entering the heat exchanger must be higher than the
temperature of return water in the hot water system. This requires the chillers to be operated at high entering condenser water
temperatures which result in higher chiller energy use. This heat recovery approach is only viable when the heating savings generated
by heat recovery exceeds the additional energy cost for operating the chillers at high condenser water temperatures.
3. Dedicated Heat Recovery Chiller in Condenser Loop. This plant consists of one or more water-cooled chillers in parallel rejecting
heat to a condenser water loop using cooling towers or dry coolers. A dedicated heat recovery chiller (DHRC) is positioned with its
evaporator in the condenser water pipe downstream of the chiller condenser outlet and upstream of the cooling tower inlet. The
DHRC condenser is in the return water pipe of the hot water system. Therefore, this DHRC acts as a water-to-water heat pump to
transfer heat from the condenser water loop to the hot water loop.
4. Chillers with Desuperheaters. This plant contains air-cooled or water-cooled chillers, one or more of which are equipped with
desuperheaters. A desuperheater is a refrigerant gas to water heat exchanger that is upstream of the condenser. Hot discharge gas
from the compressor flows through the desuperheater and transfers its heat to incoming water. The desuperheater is designed and
operated so it will not cool the refrigerant gas to the saturation point. While the desuperheater can generate high temperature hot
water, it can only capture sensible heat from the refrigerant so the amount of heat recovery is limited to the amount by which
refrigerant gas has been superheated above saturation. Once the refrigerant gas leaves the desuperheater, it passes through an air-
cooled or water-cooled condenser and rejects the remainder of its heat as it would in a conventional chiller.
5. Chillers with Double-Bundle Chillers. This plant contains water-cooled chillers, one or more of which have a double bundle
condenser. This is a condenser with two separate water circuits. One circuit is connected to the cooling tower heat rejection loop.
One circuit is a heat recovery circuit connected to the hot water system. When a heating plant load exists water flows through the
heat recovery circuit and heat is rejected to the hot water system. When no heating plant load exists, water flows through the heat
rejection circuit and heat is rejected to the cooling tower loop.
6. Chillers with Heat Recovery Condensers. This plant contains air-cooled chillers. One or more of the chillers are heat recovery
chillers and have dual condensers - a refrigerant-to-air condenser for normal heat rejection, and a refrigerant-to-water heat exchanger
for heat recovery. When a heating plant load exists, and hot water supply temperature requirements can be met, the heat recovery
chiller uses the refrigerant-to-water condenser to reject heat to the hot water loop. When no heating plant load exists or sufficiently hot
water cannot be generated, the heat recovery chiller uses the refrigerant-to-air condenser to reject heat to the atmosphere.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Configuration Data tab when defining a hot water plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Configuration Tab (Hot Water) / Plant Form
For Hot Water Plants the Configuration tab contains information about the size, configuration and control of the plant.
This tab contains inputs grouped into the following four categories:
1. Equipment defines the number of boilers or heat pumps linked in parallel to form the plant and information about how the plant and the
boilers or heat pumps will be sized.
2. Heating Controls allows the user to choose one of several different schemes for controlling the equipment in the plant and to define the
method of controlling hot water supply temperature.
3. Auxiliary Heating specifies whether auxiliary heating capability exists and, if so, how it is controlled.
Page 39 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Equipment Configuration (Hot Water Plant)
12.0 Entering Plants ›› 12.8 Configuration Data (Hot Water Plants) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Configuration (Hot Water Plant)
The Equipment Configuration group of inputs defines the number of boilers and/or heat pumps linked in parallel to form the plant and
contains information about how the plant and the boilers or heat pumps will be sized. This group contains four inputs:
1. Equipment Sizing. The plant and its boilers or heat pumps can be sized in one of two ways.
a. Auto-Sized Capacities - For preliminary design or LEED applications where it is necessary to have the capacity automatically
determined, choose the "Auto-Sized Capacities" option. With this option the program will automatically determine the plant design
capacity using the peak plant load plus the Capacity Oversizing Factor (see below). Once the total plant capacity is known, the
program automatically divides the capacity among the boilers or heat pumps in the plant according to your specification of sizing
splits (also see below).
b. User-Defined Capacity - When you want to directly specify capacities of boilers or heat pumps in the plant, choose the "User-
Defined Capacities" option.
Page 40 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Heating Controls (Hot Water Plant)
12.0 Entering Plants ›› 12.8 Configuration Data (Hot Water Plants) ››
Note that when you choose "Auto-Sized Capacities" you will only be able to link boilers or heat pumps to the plant which have the
"Auto-Size Capacity" option turned on. Likewise, if you choose "User-Defined Capacities" you will only be able to link boilers or heat
pumps which have the "Auto-Sized Capacity" option turned off. This is because the plant and its equipment must be synchronized in
this regard. As a result, on the Schedule of Equipment tab you will see different lists of available boilers and heat pumps in the
equipment drop-down list depending on whether you specified "Auto-Sized" or "User-Defined" capacities for the plant.
2. Number of Units. This item defines the number of boilers or heat pumps in the plant. The program will evaluate a plant comprised of
up to 12 boilers or heat pumps connected in parallel. To change the value, press the up or down arrow next to the input value. The up
arrow increases the number. The down arrow decreases the number.
3. Sizing Splits. When you specify "Auto-Sized Capacities" you must also define how the plant capacity will be divided among boilers
and heat pumps in the plant. For example, if the plant contains two boilers, you are offered options such as "Equally Sized",
"60%/40%", "75%/25%" and so on. In these options the first percentage corresponds to boiler 1 and the second percentage
corresponds to boiler 2 shown on the Schedule of Equipment tab. Note: When you specify "User-Defined Capacities" this input is not
relevant and is therefore disabled.
4. Capacity Oversizing Factor. When you specify "Auto-Sized Capacities" you must also define the oversizing factor for plant capacity.
For example, if you specify 25%, the program will automatically determine the plant capacity as peak coincident coil load for air
systems served by the plant plus 25%. Note: When you specify "User-Defined Capacities" this input is not relevant and is therefore
disabled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Controls (Hot Water Plant)
The "Heating Controls" group of inputs allows the user to choose one of several different schemes for controlling boilers or heat pumps in
a hot water plant. This section also provides options for defining the method of controlling hot water supply temperature (HWST).
Plant Control. Three types of plant control are offered by the program:
1. Sequenced. All boilers or heat pumps in the system are sequenced in the order they are defined on the Schedule of Equipment tab.
For example, boiler 1 turns on first. If its capacity is not sufficient to meet the load, boiler 2 turns on, and so forth. Boilers or heat
pumps are turned on until the total capacity is sufficient to meet the building load. While running, boilers or heat pumps share the
building load by running at the same part-load ratio. The following example illustrates sequenced control for a system comprised of
three 1000 MBH boilers serving a building whose peak load is 3000 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Boiler 3 MBH
3000
1000
1000
1000
2500
833
833
833
2000
1000
1000
Off
1500
750
750
Off
1000
1000
Off
Off
500
500
Off
Off
2. Part-Load Unit: High+Low Loads. With this control, all boilers or heat pumps are sequenced in a conventional manner described
above for "Sequenced" control, with the Part-Load boiler or heat pump acting as the last unit to turn on. However, when the capacity of
the part-load unit alone is sufficient to meet the building load, all other units turn off and the part-load unit runs alone to serve the load.
Therefore, the part-load boiler or heat pump runs for high and low load conditions and is off for intermediate load conditions. The
following example illustrates "part-load unit: high+low loads" control for a system comprised of two 1000 MBH boilers and one 250
MBH part-load boiler serving a building whose peak load is 1250 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Part Load MBH
Page 41 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
2250
1000
1000
250
2000
1000
1000
Off
1500
750
750
Off
1000
500
500
Off
500
250
250
Off
250
Off
Off
250
125
Off
Off
125
3. Equal Unloading. With this control, all boilers or heat pumps in the plant operate for all loads. There is no sequencing of equipment as
occurs in the other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 1000
MBH boilers serving a building whose peak load is 3000 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Boiler 3 MBH
3000
1000
1000
1000
2500
833
833
833
2000
667
667
667
1500
500
500
500
1000
333
333
333
Hot Water Supply Temperature (HWST) Control. The remaining inputs in this group describe how hot water supply temperature
(HWST) is controlled.
1. HWST Control. The program offers three options for controlling plant HWST:
a. Constant HWST. With this control the design HWST (see below) is held constant for all plant operating hours.
b. Reset by OAT Schedule. With this control the plant HWST is adjusted according to a reset schedule based on outdoor air dry-bulb
temperature. Control points for this schedule are defined by the remaining inputs in this section.
c. Reset by Load (RWT). With this control the plant HWST is adjusted based on plant load. HWST is adjusted to maintain the return
water temperature (RWT) at a constant value.
2. Design HWST defines the HWST set point for the design condition. This is the maximum HWST when reset controls are used.
3. … used when OAT less than. This input defines the outdoor air temperature (OAT) at and below which the design HWST is used.
This input is only enabled when the "Reset by OAT Schedule" option is selected.
4. Minimum HWST defines the coolest HWST allowed when reset controls are used.
5. … used when OAT greater than. This input defines the outdoor air temperature (OAT) at and above which the minimum HWST is
used. This input is only enabled when the "Reset by OAT Schedule" option is selected.
Reset by OAT Schedule Example:
Design HWST = 180 F
...used when OAT less than = 20 F
Minimum HWST = 130 F
…used when OAT greater than = 50 F
As shown in the figure, when the outdoor air temperature is 20 F or colder, the plant controls the HWST to the design value of 180 F.
When the outdoor air temperature is 50 F or warmer, the plant controls the HWST to the minimum value of 130 F. When the outdoor
air temperature is between 20 F and 50 F, the HWST varies between 180 F and 130 F along a linear control profile.
Page 42 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Auxiliary Heating (Hot Water Plant)
12.0 Entering Plants ›› 12.8 Configuration Data (Hot Water Plants) ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Auxiliary Heating (Hot Water Plant)
This group of inputs defines whether auxiliary heating is available for the plant and, if so, defines controls for the heater. This section
consists of 5 inputs:
1. Auxiliary Heating. Check this box if the plant has an auxiliary heater. Inputs in this section will then be enabled. Auxiliary heaters
are typically used for hot water plants with air-to-water heat pumps. As outdoor air temperature decreases, capacity and efficiency of
the heat pump can decline to a point where either the heat pumps cannot meet the plant heating load and/or operating the heat pump
becomes too inefficient. In both situations an auxiliary heater can be used to supplement plant heating capacity to meet the plant
demand, or to handle the full plant load and allow the heat pump to be turned off. When auxiliary heating is selected, the auxiliary
heating device will be specified on the Schedule of Equipment tab.
If this plant contains only boilers, auxiliary heating is not needed and the box can be left unchecked. If the plant contains water-to-
water heat pumps, this equipment may or may not require auxiliary heating capability.
2. Allow Simultaneous Auxiliary. Check this box if the auxiliary heater is allowed to operate simultaneously with the heat pumps.
Checking the box models a plant in which the heat pumps serve as first stage heat and when they are unable to meet the plant load,
the auxiliary heaters turn on as second stage heat to meet the remainder of the load. The plant runs in this way until the COP or OAT
trigger is reached, if either of these triggers are specified. Once a trigger is reached the plant switches to 100% auxiliary.
In other plants either the heat pumps run or the auxiliary heater runs, but not both. To model this type of plant leave the box
unchecked. For this control once the heat pump capacity is insufficient to meet a plant load, the heat pumps turn off and auxiliary
serves 100% of the plant load. The plant controller will also turn the heat pumps off and use auxiliary heat to meet 100% of the load if
the COP or OAT trigger is reached, if either of these triggers are specified.
3. H/X Approach. If the auxiliary heater is a boiler and heat is transferred to the hot water supply loop via a heat exchanger, check this
box and specify the approach for the heat exchanger. If the auxiliary is an electric sleeve heater or is a boiler which supplies hot water
directly into the hot water supply loop, leave the box unchecked.
4. Trigger: COP Below. Check this box if the plant has controls that will turn off the heat pumps when their operating COP drops below
a threshold and runs 100% auxiliary heat below this threshold. For example if the box is checked and a "COP Below" value of 2.5 is
specified, the heat pumps will turn off when their operating COP falls below 2.5.
5. Trigger: OAT Below. Check this box if the plant has controls that will turn off the heat pumps when the outdoor air dry-bulb
temperature (OAT) falls below a specified threshold temperature. For example if the box is checked and the "OAT Below" value of 15
F is specified, the heat pumps will turn off when the OAT is colder than 15 F and the auxiliary heater will serve 100% of the plant load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 43 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.9 Configuration Data (Steam Plant)
12.0 Entering Plants ››
Configuration Tab (Steam) / Plant Form
12.0 Entering Plants ›› 12.9 Configuration Data (Steam Plant) ››
Equipment Configuration (Steam Plant)
12.0 Entering Plants ›› 12.9 Configuration Data (Steam Plant) ››
This section explains input data on the Configuration Data tab when defining a steam plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Configuration Tab (Steam) / Plant Form
For Steam Boiler Plants the Configuration tab contains information about the size, configuration and control of the plant.
This tab contains inputs grouped into the following four categories:
1. Equipment defines the number of boilers or heat pumps linked in parallel to form the plant and information about how the plant and the
boilers or heat pumps will be sized.
2. Heating Controls allows the user to choose one of several different schemes for controlling the equipment in the plant and to define the
method of controlling hot water supply temperature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 44 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Heating Controls (Steam Plant)
12.0 Entering Plants ›› 12.9 Configuration Data (Steam Plant) ››
Equipment Configuration (Steam Plant)
The Equipment Configuration group of inputs defines the number of steam boilers linked in parallel to form the plant and contains
information about how the plant and the boilers will be sized. This group contains four inputs:
1. Equipment Sizing. The plant and its boilers can be sized in one of two ways.
a. Auto-Sized Capacities - For preliminary design or LEED applications where it is necessary to have the capacity automatically
determined, choose the "Auto-Sized Capacities" option. With this option the program will automatically determine the plant design
capacity using the peak plant load plus the Capacity Oversizing Factor (see below). Once the total plant capacity is known, the
program automatically divides the capacity among the boilers in the plant according to your specification of sizing splits (also see
below).
b. User-Defined Capacity - When you want to directly specify capacities of boilers in the plant, choose the "User-Defined Capacities"
option.
Note that when you choose "Auto-Sized Capacities" you will only be able to link boilers to the plant which have the "Auto-Size
Capacity" option turned on. Likewise, if you choose "User-Defined Capacities" you will only be able to link boilers which have the
"Auto-Sized Capacity" option turned off. This is because the plant and its equipment must be synchronized in this regard. As a result,
on the Schedule of Equipment tab you will see different lists of available boilers in the equipment drop-down list depending on whether
you specified "Auto-Sized" or "User-Defined" capacities for the plant.
2. Number of Units. This item defines the number of boilers in the plant. The program will evaluate a plant comprised of up to 12 boilers
connected in parallel. To change the value, press the up or down arrow next to the input value. The up arrow increases the number.
The down arrow decreases the number.
3. Sizing Splits. When you specify "Auto-Sized Capacities" you must also define how the plant capacity will be divided among boilers in
the plant. For example, if the plant contains two boilers, you are offered options such as "Equally Sized", "60%/40%", "75%/25%" and
so on. In these options the first percentage corresponds to boiler 1 and the second percentage corresponds to boiler 2 shown on the
Schedule of Equipment tab. Note: When you specify "User-Defined Capacities" this input is not relevant and is therefore disabled.
4. Capacity Oversizing Factor. When you specify "Auto-Sized Capacities" you must also define the oversizing factor for plant capacity.
For example, if you specify 25%, the program will automatically determine the plant capacity as peak coincident coil load for air
systems served by the plant plus 25%. Note: When you specify "User-Defined Capacities" this input is not relevant and is therefore
disabled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Controls (Steam Plant)
The "Heating Controls" group of inputs allows the user to choose one of several different schemes for controlling boilers in a steam plant.
Plant Control. Three types of plant control are offered by the program:
1. Sequenced. All boilers in the system are sequenced in the order they are defined on the Schedule of Equipment tab. For example,
boiler 1 turns on first. If its capacity is not sufficient to meet the load, boiler 2 turns on, and so forth. Boilers are turned on until the total
capacity is sufficient to meet the building load. While running, boilers share the building load by running at the same part-load ratio.
The following example illustrates sequenced control for a system comprised of three 1000 MBH boilers serving a building whose peak
load is 3000 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Boiler 3 MBH
3000
1000
1000
1000
2500
833
833
833
2000
1000
1000
Off
1500
750
750
Off
Page 45 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.10 Schedule of Equipment Data
12.0 Entering Plants ››
Schedule of Equipment Tab (Chillers) / Plant Form
12.0 Entering Plants ›› 12.10 Schedule of Equipment Data ››
1000
1000
Off
Off
500
500
Off
Off
2. Part-Load Unit: High+Low Loads. With this control, all boilers are sequenced in a conventional manner described above for
"Sequenced" control, with the Part-Load boiler acting as the last unit to turn on. However, when the capacity of the part-load unit alone
is sufficient to meet the building load, all other units turn off and the part-load unit runs alone to serve the load. Therefore, the part-load
boiler runs for high and low load conditions and is off for intermediate load conditions. The following example illustrates "part-load unit:
high+low loads" control for a system comprised of two 1000 MBH boilers and one 250 MBH part-load boiler serving a building whose
peak load is 1250 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Part Load MBH
2250
1000
1000
250
2000
1000
1000
Off
1500
750
750
Off
1000
500
500
Off
500
250
250
Off
250
Off
Off
250
125
Off
Off
125
3. Equal Unloading. With this control, all boilers in the plant operate for all loads. There is no sequencing of equipment as occurs in the
other control schemes. The following example illustrates "equal unloading" control for a system comprised of three 1000 MBH boilers
serving a building whose peak load is 3000 MBH.
Building Load
Boiler 1 MBH
Boiler 2 MBH
Boiler 3 MBH
3000
1000
1000
1000
2500
833
833
833
2000
667
667
667
1500
500
500
500
1000
333
333
333
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains inputs on the Schedule of Equipment tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Schedule of Equipment Tab (Chillers) / Plant Form
The Schedule of Equipment Tab is used to specify which chillers and towers are connected together to form the plant. The contents of
the tab and procedures for using tab features are described below.
Page 46 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Tab Layout. This tab contains a table which lists the chillers and cooling towers, dry coolers or geothermal / surface water sources (if
applicable) linked together to form the plant. Totals shown in the summary section in the lower right are useful for making sure water flow
rates for chillers and towers are matched and for keeping track of the total plant cooling capacity. A button in the lower left is used for
quickly making all chillers and towers in the schedule the same. Extra drop-down lists in the lower left are used for the shared tower
configuration and for defining the plant heat source when steam absorption or steam-driven chillers are used. Key components on this
tab are described below:
1. Schedule of Chillers Table. Each row in this table contains data for one chiller. Each column contains descriptive data for the chillers
and towers linked to the plant. The sample figure above shows a plant containing two centrifugal chillers and one rotary screw chiller.
Contents of the columns in the table are as follows:
a. Sequence indicates the sequencing position of a chiller in the system using labels such as 1, 2, 3, etc… If part-load chiller control is
used, the last chiller will be labeled "Part Load". With sequencing control, chiller 1 is the first chiller turned on and the last chiller
turned off.
b. Chiller Name is the reference name for a selected chiller. Cells in this column are drop-down lists containing the names of all
chillers in the current project and a "" option. A chiller can be linked to the plant in two ways:
Selecting an Existing Chiller. If you previously created and stored chillers in your project, you can simply select the desired chiller
from the drop-down list. Note that the drop-down list will only contain chillers matching the Chiller Sizing specification for this plant.
If you specified "Auto-Sized Chiller Capacities" then only chillers with the "Autosize Capacity" option turned on will be listed. If you
specified "User Defined Chiller Capacities" then only chillers with the "Autosize Capacity" option turned off will be listed. This is
because the plant and its chillers must be synchronized with respect to this chiller sizing option.
Creating a New Chiller. If you have not yet created a chiller, choose the "" item in the drop-down list. The Chiller
Properties window will appear and will allow you define data for a new chiller. When you press the OK button to exit from the Chiller
Properties window, your chiller will be stored and linked to the plant automatically.
c. Full Load Capacity is the design cooling capacity for a selected chiller. This item is display-only. If the chiller has its "Autosize
Capacity" option turned on, then "" will appear here. If the chiller has its "Autosize Capacity" option turned off, then the
cooling capacity will be listed.
d. Cooler Flow Rate is the flow rate through the evaporator (or "cooler") of the chiller at the full load design condition. It is provided for
reference purposes. This item is display-only.
e. Condenser Flow Rate is listed for water-cooled chillers only. It is used to quickly determine whether the flow rates for a chiller and
its cooling tower match. This item is display-only.
Page 47 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Schedule of Equipment Tab (Changeover) / Plant form
12.0 Entering Plants ›› 12.10 Schedule of Equipment Data ››
f. Cooling Tower Name. When the cooling tower configuration is "One Tower per W/C Chiller", each row shows the name of the
cooling tower or dry cooler corresponding to the chiller in this row. Cells in this column are drop-down lists containing the names of
all cooling towers in the current project and a "" option. A tower can be linked to the plant in two ways described
below. This item is only enabled for water-cooled chillers.
Selecting an Existing Tower. If you previously created and stored cooling towers in your project, you can simply select the desired
tower from the drop-down list.
Creating a New Tower. If you have not yet created a tower, choose the "" item in the drop-down list. The Tower
form will appear and will allow you define data for a new tower or dry cooler. When you press the OK button to exit from the Tower
form, your tower will be stored and linked to the plant automatically.
Note that the flow rate defined for a cooling tower must match the condenser flow rate for its chiller within +/- 20 gpm (+/- 1.25 L/s).
Finally, when the cooling tower configuration is "One Tower Shared by All W/C Chillers", this column is not shown. Instead, the
shared tower is selected in a separate drop-down list in the lower left portion of the tab.
g. Tower Flow Rate lists the water flow rate for the selected cooling tower, if the "One Tower per W/C Chiller" configuration option is
used. This is useful for quickly determining whether the flow rates for a chiller and its tower match.
Note that when a row contains data for an air cooled chiller, this cell is not relevant and is displayed as blank.
When using the "One Tower Shared by All W/C Chillers" option, this column is not shown. Instead the total flow rate for the shared
tower is shown in the Summary section in the lower right portion of the tab.
2. "Make All Equipment the Same Button". This button, which appears in the lower left portion of the tab, is used to quickly make all
chillers and towers in the plant the same. Therefore, if your plant consists of a number of identical chillers (and towers or dry coolers),
you only need to select the chiller and tower for one row of the table and can then use the button to quickly copy the selections to all
other rows in the table.
To use this feature, click on one of the cells in the Chiller Name column to designate it as the current chiller. This is indicated by a blue
arrow. Then press the "Make All Equipment the Same" button. The chiller selection for the cell highlighted will be copied to all other
chiller slots in the table. If a cooling tower was selected for that chiller, the tower selection will be copied to all other rows in the table.
3. The Summary section appears in the lower right. It contains the following information:
a. Total Full Load Capacity - The sum of full load capacities for chillers in the table. This item will contain data only if the "user
defined capacities" option is selected for the plant.
b. Total Cooler Flow Rate - The sum of cooler flow rates for chillers in the table. This item will contain data only if cooler flow rate for
all chillers in the table is defined in units of gpm or L/s.
c. Total Condenser Flow Rate - The sum of condenser flow rates for chillers in the table. This item will contain data only if condenser
flow rate for all chillers in the table is defined in units of gpm or L/s.
d. Estimated Maximum Load - The peak load for the plant. This item only appears if design calculations were previously run for this
plant. When using the "user defined capacities" option, its useful to compare this maximum load with the "Total Full Load Capacity"
above to verify the plant has sufficient capacity.
4. The Shared Equipment section in the lower left contains two inputs:
a. Shared Cooling Tower - When the "one cooling tower shared by all water cooled chillers" option is selected on the Configuration
tab, a single selection of a cooling tower or dry cooler is made here rather than specifying heat rejection equipment in the schedule
of equipment table. This drop-down list contains all previously defined heat rejection equipment such as cooling towers or dry
coolers. The list also contains a  option which can be used to create a new tower or dry cooler, save it
and automatically link it to the plant.
b. Steam Source - When the plant contains a steam absorption chiller or an engine chiller which uses steam as its source, this items
appears in the Shared Equipment section. It is used to specify the source of steam for the equipment. In this drop down list is a
"remote source steam" option to model use of waste steam or steam from a district system. The drop down list also contains all
previously defined steam boilers and a  option. The latter option is used to create a new steam boiler, save it
and automatically link it to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Schedule of Equipment Tab (Changeover) / Plant form
The Schedule of Equipment Tab is used to specify which reversible chillers and water sources are connected together to form the plant.
The contents of the tab and procedures for using tab features are described below.
Page 48 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Tab Layout. This tab contains a table which lists the reversible chillers linked together to form the plant. Totals shown in the summary
section in the lower right are useful for checking plant capacity against peak load and for checking total plant water flow rates. Extra
drop-down lists in the lower left are used for the shared water source for water source reversible chillers and for defining the source of
auxiliary heat. Key components on this tab are described below:
1. Schedule of Equipment Table. Each row in this table contains data for one heat pump. Each column contains descriptive data for the
reversible chillers linked to the plant. The sample figure above shows a plant containing two reversible water source chillers. Contents
of the columns in the table are as follows:
a. Sequence indicates the sequencing position of a chiller in the system using labels such as 1, 2, 3, etc… If part-load unit control is
used, the last heat pump will be labeled "Part Load". With sequencing control, heat pump 1 is the first chiller turned on and the last
chiller turned off.
b. Equipment Name is the reference name for a selected chiller. Cells in this column are drop-down lists containing the names of all
chillers in the current project and a "" option. A chiller can be linked to the plant in two ways:
Selecting an Existing Chiller. If you previously created and stored heat pumps in your project, you can simply select the desired
chiller from the drop-down list. Note that the drop-down list will only contain chillers matching the Unit Sizing specification for this
plant. If you specified "Auto-Sized Capacities" then only chillers with the "Autosize Capacity" option turned on will be listed. If you
specified "User Defined Capacities" then only chillers with the "Autosize Capacity" option turned off will be listed. This is because
the plant and its chillers must be synchronized with respect to this sizing option.
Creating a New Chiller. If you have not yet created a chiller, choose the "" item in the drop-down list.
The Chiller Properties window will appear and will allow you define data for a new reversible chiller. When you press the OK button
to exit from the Chiller Properties window, your chiller will be stored and linked to the plant automatically.
c. Full Load Capacity displays the design cooling and heating capacities for a selected chiller. These items are display-only. If the
chiller has its "Autosize Capacity" option turned on, then "" will appear here. If the chiller has its "Autosize Capacity"
option turned off, then the cooling and heating capacities will be listed.
d. Supply Side Flow Rate displays the chilled water and hot water supply flow rates for the chillers. These items are provided for
reference purposes only..
e. Source Side Flow Rate displays the source water flow rates for cooling and heating duty. These are only listed for water source
reversible chillers as reference information.
2. "Make All Equipment the Same Button". This button, which appears in the lower left portion of the tab, is used to quickly make all
reversible chillers in the plant the same. Therefore, if your plant consists of a number of identical chillers, you only need to select the
Page 49 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Schedule of Equipment Tab (Heat Recovery) / Plant Form
12.0 Entering Plants ›› 12.10 Schedule of Equipment Data ››
chiller for one row of the table and can then use the button to quickly copy the selections to all other rows in the table. To use this
feature, click on one of the cells in the Equipment Name column to designate it as the current heat pump. This is indicated with a blue
arrow. Then press the "Make All Equipment the Same" button. The chiller selection for the cell highlighted will be copied to all other
chiller slots in the table.
3. The Summary section appears in the lower right. It contains the following information:
a. Total Full Load Capacity - The sum of full load cooling capacities and full load heating capacities for chillers in the table. This item
will contain data only if the "user defined capacities" option is selected for the plant.
b. Total Supply-Side Flow Rate - The sum of supply side flow rates for cooling and heating duty for chillers in the table. This item will
contain data only if cooler flow rate for all heat pumps in the table is defined in units of gpm or L/s.
c. Total Source-Side Flow Rate - The sum of source side flow rates for cooling and heating duty for chillers in the table. This item will
contain data only if the plant contains water source reversible chillers and the source side flow rates are defined in units of gpm or
L/s.
d. Estimated Maximum Load - The peak cooling and heating loads for the plant. This item only appears if design calculations were
previously run for this plant. When using the "user defined capacities" option, its useful to compare this maximum load with the
"Total Full Load Capacity" above to verify the plant has sufficient capacity.
4. The Shared Equipment section in the lower left contains two inputs:
a. Shared Water Source - This item defines the geo, well or surface water system for the plant. It is only applicable when the plant
contains water source reversible chillers. This drop-down list contains all previously defined geo, well or surface water systems
defined in the project. The list also contains a  option which can be used to create a water source, save
it and automatically link it to the plant.
b. Shared Auxilary Heating - When the plant contains an auxiliary heater this items appears in the Shared Equipment section. It is
used to specify the auxiliary heating equipment. In this drop down list is a "remote source" option to model use of heat from a
district hot water system.f The drop down list also contains all previously defined boilers and a  option. The
latter option is used to create a new boiler, save it and automatically link it to the plant.
Note: When modeling an electric sleeve heater, create a hot water boiler whose energy source is electricity and specify the
appropriate equipment efficiency.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Schedule of Equipment Tab (Heat Recovery) / Plant Form
The Schedule of Equipment Tab is used to specify the chillers, boilers, heat recovery and heat rejection equipment connected to form the
plant. The contents of the tab and procedures for using tab features are described below.
Page 50 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Tab Layout. This tab contains a table which lists the equipment linked together to form the plant. Totals shown in the summary section in
the lower right are useful for making sure water flow rates for chillers and towers are matched and for keeping track of the total plant
cooling capacity. A button in the lower left is used for quickly making all chillers and towers in the schedule the same, or all boilers the
same. \Key components on this tab are described below:
1. Schedule of Equipment Table. Each row in this table contains data for one chiller, one heat recovery chiller or one boiler. The intial
rows, color coded blue, contain selections for cooling-only chillers and corresponding cooling tower in the plant. If the heat recovery
plant uses a dedicated heat recovery chiller (DHRC), it is shown color coded green. Finally, rows color coded red contain hot water
boilers. Each column in the table contains descriptive data for the equipment such as capacity and flow rate. The sample figure
above shows a plant containing two centrifugal cooling-only chillers, a water-cooled screw DHRC, and two gas boilers. Contents of
the columns in the table are as follows:
a. Sequence indicates the sequencing position of a chiller or boiler in the system. Chiller position is indicated by labels like CH-1,
CH-2, etc... Boiler position is indicated by labels like B-1, B-2, etc... If part-load chiller control is used, the last chiller will be labeled
"Part Load".
b. Equipment Name is the reference name for a selected chiller or boiler. Cells in this column are drop-down lists containing the
names of all equipment in the current project and a "" option. A chiller or boiler can be linked to the plant in two ways:
Selecting an Existing Unit. If you previously created and stored chillers and boilers in your project, you can simply select the desired
item from the drop-down list. Note that the drop-down list will only contain items matching the Sizing specification for this plant. If
you specified "Auto-Sized Capacities" then only chillers and boilers with the "Autosize Capacity" option turned on will be listed. If
you specified "User Defined Capacities" then only chillers and boilers with the "Autosize Capacity" option turned off will be listed.
This is because the plant and its equipment must be synchronized with respect to this chiller sizing option.
In addition, the drop-down lists will only contain equipment valid for use in this heat recovery plant. For example, if heat recovery
method is "Chillers with Desuperheaters", then the chiller drop-down list will only include items that are either cooling only chillers or
chillers defined as containing a desuperheater. Or for example, of "Chillers with Double Bundle Condensers" heat recovery was
selected, the chiller drop down list will only contain cooling-only chillers and chillers defined as having a double-bundle condenser
Note that in heat recovery plants using a dedicated heat recovery chiller (DHRC), the DHRC must be defined as a water-to-water
heat pump. Only equipment of this type will appear in the drop-down list for the DHRC row in the equipment schedule.
Creating a New Unit. If you have not yet created a chiller or boiler, choose the "" item in the drop-down list. For chiller
items the Chiller Properties window will appear and will allow you define data for a new chiller. For boiler line items the Boiler
Page 51 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Schedule of Equipment Tab (Hot Water) / Plant Form
12.0 Entering Plants ›› 12.10 Schedule of Equipment Data ››
Properties window will appear and allow you to dfine a new boiler. When you press the OK button to exit from the Chiller or Boiler
window, the chiller or boiler you created will be saved and automatically linked to the plant..
c. Full Load Capacity is the design cooling capacity for a chiller or the design heating capacity for a boiler. For a DHRC unit the
specified heating capacity will be listed along with an estimated cooling capacity.. These items are display-only. If the plant specifies
"Autosize Capacity", then "" will appear here.
d. Supply Flow Rate is the design chilled water flow rate for a chiller or the design hot water flow rate for a boiler. For a DHRC unit
both cooling and heating flow rates will be listed. These items are display-only.
e. Source Flow Rate lists the condenser water flow rate for water-cooled chillers. For a DHRC unit both the evaporator and
condenser flow rates are listed. This data for chillers is used to quickly determine whether the flow rates for a chiller and its cooling
tower match. This item is display-only.
f. Cooling Tower Name. When the cooling tower configuration is "One Tower per W/C Chiller", each row shows the name of the
cooling tower or dry cooler corresponding to the chiller in this row. Cells in this column are drop-down lists containing the names of
all cooling towers in the current project and a "" option. A tower can be linked to the plant in two ways described
below. This item is only enabled for water-cooled chillers.
Selecting an Existing Tower. If you previously created and stored cooling towers in your project, you can simply select the desired
tower from the drop-down list.
Creating a New Tower. If you have not yet created a tower, choose the "" item in the drop-down list. The Tower
form will appear and will allow you define data for a new tower or dry cooler. When you press the OK button to exit from the Tower
form, your tower will be stored and linked to the plant automatically.
Note that the flow rate defined for a cooling tower must match the condenser flow rate for its chiller within +/- 20 gpm (+/- 1.25 L/s).
Finally, when the cooling tower configuration is "One Tower Shared by All W/C Chillers", this column is not shown. Instead, the
shared tower is selected in a separate drop-down list in the lower left portion of the tab.
g. Cooling Tower Flow Rate lists the water flow rate for the selected cooling tower, if the "One Tower per W/C Chiller" configuration
option is used. This is useful for quickly determining whether the flow rates for a chiller and its tower match.
Note that when a row contains data for an air cooled chiller, this cell is not relevant and is displayed as blank.
When using the "One Tower Shared by All W/C Chillers" option, this column is not shown. Instead the total flow rate for the shared
tower is shown in the Summary section in the lower right portion of the tab.
2. "Make All Equipment the Same Button". This button, which appears in the lower left portion of the tab, is used to quickly make
related equipment the same. For example, if the current row in the table (indicated by a triangle symbol at the far left) contains data for
one of the chillers, then pressing the "Make All the Same" button will copy the chiller and cooling tower selections from this row to all
other cooling-only chiller rows in the table. If the current row is a boiler row, pressing the button will copy the boiler selection to all
other boiler rows in the table. Pressing the "Make All the Same" button has no effect if the current row is the DHRC row of the table.
3. The Summary section appears in the lower right. It contains the following information:
a. Total Full Load Capacity - Separate sums of full load heating capacities and full load cooling capacities in the table. This item will
contain data only if the "user defined capacities" option is selected for the plant.
b. Total Supply-Side Flow Rate - Separate totals for the hot water supply flow rate and chilled water supply flow rate in the system.
This item will contain data only if cooler flow rate for all chillers in the table is defined in units of gpm or L/s.
c. Total Source-Side Flow Rate - The heating column shows the total source water flow (chilled water flow) for a DHRC unit. The
cooling column shows the total condenser water flow rate for the system. This item will contain data only if condenser flow rate for
all chillers in the table is defined in units of gpm or L/s.
d. Estimated Maximum Load - Separate totals for the peak plant heating and cooling loads. This item only appears if design
calculations were previously run for this plant. When using the "user defined capacities" option, its useful to compare this maximum
load with the "Total Full Load Capacity" above to verify the plant has sufficient capacity.
4. The Shared Equipment section in the lower left contains two inputs:
a. Shared Cooling Tower - When the "one cooling tower shared by all water cooled chillers" option is selected on the Configuration
tab, a single selection of a cooling tower or dry cooler is made here rather than specifying heat rejection equipment in the schedule
of equipment table. This drop-down list contains all previously defined heat rejection equipment such as cooling towers or dry
coolers. The list also contains a  option which can be used to create a new tower or dry cooler, save it
and automatically link it to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 52 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Schedule of Equipment Tab (Hot Water) / Plant Form
The Schedule of Equipment Tab is used to specify the boilers or heat pumps linked to the plant. Applications for this data:
1. In a space heating system, this is the equipment which generates hot water to supply to space heating coils.
2. In a standalone service hot water (SHW) system, this is the equipment which heats the water in the SHW storage tank, whether
separate from or integral to the storage tank. When the heating equipment is separate from the SHW storage tank, inputs on the
Distribution Tab define the pumping system that circulates water between the heating equipment and the SHW storage tank. Finally,
in tankless systems, data on this tab describes the equipment that generates hot water to be delivered directly to the point of use.
3. In a combined space and SHW heating system, this is the equipment which generates hot water to supply to space heating coils, and
to deliver to the SHW storage tank heat exchanger to heat the tank water.
The contents of the tab and procedures for using tab features are described below.
Tab Layout. This tab contains a table which lists the boilers or heat pumps linked together to form the plant. Totals shown in the
summary section in the lower right are useful for checking plant capacity against peak load and for checking total plant water flow rates.
Extra drop-down lists in the lower left are used for the shared water source for water to water heat pumps and for defining the source of
auxiliary heat. Key components on this tab are described below:
1. Schedule of Equipment Table. Each row in this table contains data for one boiler or heat pump. Each column contains descriptive
data for the equipment linked to the plant. The sample figure above shows a plant containing two natural gas condensing boilers.
Contents of the columns in the table are as follows:
a. Sequence indicates the sequencing position of a boiler or heat pump in the system using labels such as 1, 2, 3, etc… If part-load
unit control is used, the last boiler or heat pump will be labeled "Part Load". With sequencing control, "1" is the first boiler or heat
pump turned on and the last unit turned off.
b. Equipment Name is the reference name for a selected boiler or heat pump. Cells in this column are drop-down lists containing the
names of all boilers or heat pumps in the current project and "" and "" options.
Equipment can be linked to the plant in two ways:
Selecting Existing Equipment. If you previously created and stored boilers or heat pumps in your project, you can simply select the
desired equipment from the drop-down list. Note that the drop-down list will only contain equipment matching the Unit Sizing
specification for this plant. If you specified "Auto-Sized Capacities" then only equipment with the "Autosize Capacity" option turned
Page 53 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Schedule of Equipment Tab (Steam)
12.0 Entering Plants ›› 12.10 Schedule of Equipment Data ››
on will be listed. If you specified "User Defined Capacities" then only equipment with the "Autosize Capacity" option turned off will
be listed. This is because the plant and its boilers or heat pumps must be synchronized with respect to this sizing option.
Creating New Equipment. If you have not yet created a boiler or heat pump, choose the "" or "" item in the drop-down list. The Boiler Properties or Chiller Properties window will appear and will allow you define data for
new equipment. When you press the OK button to exit from that window, your boiler or heat pump will be stored and linked to the
plant automatically.
c. Full Load Capacity displays the design heating capacity for a selected unit. This item is display-only. If the equipment has its
"Autosize Capacity" option turned on, then "" will appear here. If the equipment has its "Autosize Capacity" option
turned off, then the heating capacity will be listed.
d. Hot Water Flow Rate displays the hot water supply flow rate for the equipment. This items are provided for reference purposes
only.
e. Evaporator Flow Rate displays the source water flow rates for water-to-water heat pump equipment. For boilers and air-to-water
heat pumps this cell will be blank since it does not apply..
2. "Make All Equipment the Same Button". This button, which appears in the lower left portion of the tab, is used to quickly make all
equipment in the plant the same. For example, if your plant consists of a number of identical boilers, you only need to select the boiler
for one row of the table and can then use the button to quickly copy the selections to all other rows in the table. To use this feature,
click on one of the cells in the Equipment Name column to designate it as the current unit. This is indicated by a blue arrow. Then
press the "Make All Equipment the Same" button. The equipment selection for the cell highlighted will be copied to all other slots in the
table.
3. The Summary section appears in the lower right. It contains the following information:
a. Total Full Load Capacity - The sum of full load heating capacities for equipment in the table. This item will contain data only if the
"user defined capacities" option is selected for the plant.
b. Total Hot Water Flow Rate - The sum of hot water flow rates for equipment in the table. This item will contain data only if the hot
water flow rates are defined in units of gpm or L/s.
c. Total Evaporator Flow Rates - The sum of evaporator flow rates for water-to-water heat pumps in the table. This item will contain
data only if the plant contains water-to-water heat pumps and the evaporator flow rates are defined in units of gpm or L/s.
d. Estimated Maximum Load - The peak heating load for the plant. This item only appears if design calculations were previously run
for this plant. When using the "user defined capacities" option, its useful to compare this maximum load with the "Total Full Load
Capacity" above to verify the plant has sufficient capacity.
4. The Shared Equipment section in the lower left contains two inputs:
a. Shared Water Source - This item defines the geo, well or surface water system for the plant. It is only applicable when the plant
contains water-to-water heat pumps. This drop-down list contains all previously defined geo, well or surface water systems defined
in the project. The list also contains a  option which can be used to create a water source, save it and
automatically link it to the plant.
b. Shared Auxilary Heating - When the plant contains an auxiliary heater this items appears in the Shared Equipment section. It is
used to specify the auxiliary heating equipment. In this drop down list is a "remote source" option to model use of heat from a
district hot water system. The drop down list also contains all previously defined boilers and a  option. The
latter option is used to create a new boiler, save it and automatically link it to the plant.
Note: When modeling an electric sleeve heater, create a hot water boiler whose energy source is electricity and specify the
appropriate equipment efficiency.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Schedule of Equipment Tab (Steam)
The Schedule of Equipment Tab is used to specify the boilers linked to the plant. The contents of the tab and procedures for using tab
features are described below.
Page 54 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Tab Layout. This tab contains a table which lists the boilers linked together to form the plant. Totals shown in the summary section in the
lower right are useful for checking plant capacity against peak load. Key components on this tab are described below:
1. Schedule of Equipment Table. Each row in this table contains data for one boiler. Each column contains descriptive data for the
equipment linked to the plant. The sample figure above shows a plant containing two natural gas steam boilers. Contents of the
columns in the table are as follows:
a. Sequence indicates the sequencing position of a boiler in the system using labels such as BLR-1, BLR-2, BLR-3, etc… If part-load
unit control is used, the last boiler or heat pump will be labeled "Part Load". With sequencing control, "BLR-1" is the first boiler
turned on and the last unit turned off.
b. Equipment Name is the reference name for a selected boiler or heat pump. Cells in this column are drop-down lists containing the
names of all boilers in the current project and "" options. Equipment can be linked to the plant in two ways:
Selecting Existing Equipment. If you previously created and stored steam boilers in your project, you can simply select the desired
equipment from the drop-down list. Note that the drop-down list will only contain equipment matching the Unit Sizing specification
for this plant. If you specified "Auto-Sized Capacities" then only equipment with the "Autosize Capacity" option turned on will be
listed. If you specified "User Defined Capacities" then only equipment with the "Autosize Capacity" option turned off will be listed.
This is because the plant and its boilers must be synchronized with respect to this sizing option.
Creating New Equipment. If you have not yet created a boiler, choose the "" item in the drop-down list. The
Boiler Properties window will appear and will allow you define data for new equipment. When you press the OK button to exit from
that window, your boiler will be stored and linked to the plant automatically.
c. Full Load Capacity displays the design heating capacity for a selected unit. This item is display-only. If the equipment has its
"Autosize Capacity" option turned on, then "" will appear here. If the equipment has its "Autosize Capacity" option
turned off, then the heating capacity will be listed.
2. "Make All Equipment the Same Button". This button, which appears in the lower left portion of the tab, is used to quickly make all
equipment in the plant the same. For example, if your plant consists of a number of identical boilers, you only need to select the boiler
for one row of the table and can then use the button to quickly copy the selections to all other rows in the table. To use this feature,
click on one of the cells in the Equipment Name column to designate it as the current unit. This is indicated by a blue arrow. Then
press the "Make All Equipment the Same" button. The equipment selection for the cell highlighted will be copied to all other slots in the
table.
3. The Summary section appears in the lower right. It contains the following information:
Page 55 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.11 Distribution System Data
12.0 Entering Plants ››
Distribution Tab / Plant Form
12.0 Entering Plants ›› 12.11 Distribution System Data ››
a. Total Full Load Capacity - The sum of full load heating capacities for equipment in the table. This item will contain data only if the
"user defined capacities" option is selected for the plant.
d. Estimated Maximum Load - The peak heating load for the plant. This item only appears if design calculations were previously run
for this plant. When using the "user defined capacities" option, its useful to compare this maximum load with the "Total Full Load
Capacity" above to verify the plant has sufficient capacity.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Distribution System tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Distribution Tab / Plant Form
The Distribution tab is used to define the distribution system and controls for chilled water and hot water plants. For steam plants it
defines the pipe heat loss factor.
The appearance of this tab changes depending on the plant type and the distribution system options that are selected. Figure 1 shows
typical tab contents for a chilled water plant. A hot water plant would have the same content except that the sub-tab title would be "Hot
Water Supply" instead of "Chilled Water Supply". Figure 2 shows the tab content for a heat recovery plant. In this case there are
separate sub-tabs for chilled water supply and hot water supply.. Figure 3 shows the tab contents for a steam plant. Contents of the tab
are discussed below these figures.
Page 56 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Figure 1. Distribution Tab Layout for Chilled Water & Hot Water Plants
Figure 2. Distribution Tab Layout for Heat Recovery Plants
Figure 3. Distribution Tab Layout for Steam Plants
This tab is divided into four sections, as shown in Figures 1 and 2. Chilled water and hot water plants use three or four of these sections.
Steam plants use only the first. These sections are:
1. Distribution System defines the type of distribution system used, the design criteria for air system coils, pipe heat gain or loss factor
and pump performance units.
2. Fluid Properties specifies the thermal properties of the fluid used in the distribution system.
3. Primary Loop provides information about the pumps and controls for the primary portion of the distribution system. The information in
this section varies depending on whether a primary only / constant speed, primary-only / variable speed or primary/secondary variable
speed distribution system is used. When working with remote source plants, this section does not appear.
4. Secondary Loop provides information about pumps and controls for the secondary portion of the distribution system, if applicable.
The content of this section varies depending on the plant type and distribution system type. For chiller and hot water plants, this
Page 57 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Distribution System
12.0 Entering Plants ›› 12.11 Distribution System Data ››
section is only used for a primary/secondary variable speed distribution system. For remote source chilled water and hot water plants,
it is used both for secondary-only / constant speed and secondary-only / variable speed distribution systems.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Distribution System
This section of the Distribution tab has different contents depending on the plant type.
Chilled Water and Hot Water Plants. For chilled water and hot water plants, this section defines the type of hydronic distribution system
used, the design criteria for air system coils, pipe heat gain or loss factor and pump performance units:
1. Type. Three different types of hydronic distribution systems are offered by the program:
a. Primary-Only, Constant Speed. This system type covers the following two operating scenarios.
(i) A plant either contains a single chiller, heat pump or boiler, or it contains multiple machines and uses the "Equal Unloading"
control scheme: The distribution system consists of one constant speed pump paired with each chiller, heat pump or boiler in the
plant. The pumps circulate a constant flow of water to air system coils. Three-way valves are used to regulate flow through the
coils. Because of the constant speed, constant flow nature of the system, the pumps operate at their design point for all operating
hours. This configuration is shown for a chilled water plant in Figure 1 below.
(ii) A plant contains multiple chillers, heat pumps or boilers and uses one of the sequencing control options: The distribution system
consists of one constant speed pump paired with each chiller, heat pump or boiler in the plant. Two-way valves are used to
regulate flow through the air system coils. This results in variable flow in the system. Because constant speed pumps are used,
each pump rides its pump curve as flow varies. Care must be used to ensure that sequencing of the chillers, heat pumps or
boilerse will prevent flow from dropping below manufacturer recommended minimum flow rates. This configuration is similar to
Figure 1 below but with 2-way valves on the air handlers.
Page 58 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Figure 1. Primary-Only, Constant Speed with 3-Way Valves
b. Primary-Only, Variable Speed. One variable speed pump or a gang of variable speed pumps in parallel circulate water through the
system. Two-way valves are used to regulate flow through air system coils. A differential pressure sensor measuring pressure
between the supply and return legs of the system controls pump speed to maintain a constant differential pressure. Due to this
control the primary pump(s) ride the system curve as flow varies. This configuration is shown in Figure 2 below.
Figure 2. Primary-Only, Variable Speed
c. Primary/Secondary, Variable Speed Secondary. One constant speed pump is paired with each chiller, heat pump or boiler in the
system. These constant speed pumps maintain a constant flow through the individual chiller, heat pump or boiler legs in the primary
portion of the system. Therefore, each primary pump operates at its design point. A separate variable speed pump, or gang of
variable speed pumps in parallel, drives flow in the secondary portion of the system. Two-way valves regulate flow through air
system coils. A differential pressure sensor measuring pressure between the supply and return legs of the secondary system
controls the secondary pump speed to maintain a constant differential pressure. As a result, the secondary pump rides the system
curve as flow varies. This configuration is shown in Figure 3 below.
Page 59 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Fluid Properties
12.0 Entering Plants ›› 12.11 Distribution System Data ››
Figure 3. Primary/Secondary, Variable Speed Secondary
2. Coil Delta-T at Design. For chilled water systems this item defines the temperature rise for water flowing through air system cooling
coils at the design condition. For hot water systems it defines the temperature drop for flow through hot water heating coils. This
delta-T is used in simulations of variable flow pumping systems to determine how flow through coils varies when 2-way valves are
used to regulate flow through the coil. For standard conditions, it is assumed the valve varies the flow as load changes to maintain this
coil delta-T.
3. Pipe Heat Gain or Heat Loss Factor. For chilled water systems pipe heat gain is computed as a percentage of the total cooling coil
load for air systems served by the plant. For hot water systems pipe heat loss is calculated as a percentage of the total hot water
heating coil load for air systems served by the plant.
4. Pump Performance defines how pump performance will be specified in the remaining sections of this input screen. Three choices are
offered:
a. ft wg or kPa. When pump head is specified, the program automatically determines the pump input power from the head, flow and
the mechanical and electrical efficiencies.
b. W/gpm or W/L/s. When pump W/gpm is specified the program automatically determines pump input power from the W/gpm or
W/L/s specification and the pump flow rate.
c. kW. When pump motor kW is specified it is directly used in simulation calculations.
Steam Plants. For steam plants it is only necessary to define the pipe heat loss factor. During plant simulations heat loss will be
calculated as a percentage of the total load for steam heating coils in air systems served by the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fluid Properties
Page 60 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
The Fluid Properties section of the Distribution tab specifies the thermal properties of the fluid used in the distribution system. These
thermal properties will affect the calculation of part-load flow rates in variable flow systems.
1. Name. You can either select one of the common fluid types listed in the drop-down list, or enter your own name for the fluid. If you
select one of the items in the drop-down list, the density and specific heat for the fluid will be defaulted automatically. If you enter your
own fluid name, you must specify the density and specific heat yourself.
Note: All brine concentrations refer to percent by weight, not percent by volume.
2. Density. Specify the density for the fluid at the average operating temperature expected for the system.
3. Specific Heat. Specify the specific heat of the fluid at the average operating temperature expected for the system.
Default properties for fluids listed in the drop-down list are shown below for reference:
Table 1. Fresh Water
Application
Temp.
(F)
Density
(lb/cuft)
Specific
Heat
(BTU/lb-F)
Temp.
(C)
Density
(kg/m3)
Specific
Heat
(kJ/kg K)
Chilled Water
44.0
62.4
1.00
6.7
999.6
4.19
Hot Water
180.0
60.6
1.00
82.2
970.7
4.19
Table 2. Ethylene Glycol Brines for Chilled Water Applications (44 F or 6.7 C)
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
62.8
1.00
1006.0
4.19
10
63.3
0.98
1014.0
4.10
15
63.8
0.96
1022.0
4.02
20
64.3
0.93
1030.0
3.89
25
64.7
0.90
1036.4
3.77
30
65.2
0.88
1044.4
3.68
35
65.6
0.85
1050.8
3.56
40
66.1
0.83
1058.8
3.48
45
66.5
0.80
1065.2
3.35
50
66.9
0.78
1071.6
3.27
Table 3. Propylene Glycol Brines for Chilled Water Applications (44 F or 6.7 C)
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
62.6
1.00
1002.8
4.19
10
62.9
0.99
1007.6
4.14
15
63.2
0.98
1012.4
4.10
20
63.6
0.96
1018.8
4.02
25
63.9
0.95
1023.6
3.98
30
64.2
0.93
1028.4
3.89
35
64.5
0.91
1033.2
3.81
40
64.8
0.89
1038.0
3.73
Page 61 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
45
65.0
0.87
1041.2
3.64
50
65.3
0.84
1046.0
3.52
Table 4. Calcium Chloride Brines for Chilled Water Applications (44 F or 6.7 C)
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
65.0
0.93
1041.2
3.89
10
67.9
0.86
1087.7
3.60
15
71.0
0.79
1137.3
3.31
20
74.2
0.74
1188.6
3.10
25
77.6
0.69
1243.0
2.89
30
81.1
0.66
1299.1
2.76
35
84.7
0.63
1356.8
2.64
40
88.4
0.62
1416.0
2.60
45
92.2
0.62
1476.9
2.60
50
95.9
0.64
1536.2
2.68
Table 5. Sodium Chloride Brines for Chilled Water Applications (44 F or 6.7 C)
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
64.7
0.94
1036.4
3.94
10
67.2
0.89
1076.4
3.73
15
69.6
0.84
1547.4
3.52
20
72.0
0.81
1153.3
3.39
25
74.7
0.79
1196.6
3.31
30
77.6
0.76
1243.0
3.18
35
80.8
0.74
1294.3
3.10
40
84.5
0.71
1353.6
2.97
45
88.7
0.67
1420.8
2.81
50
93.5
0.62
1497.7
2.60
Table 6. Ethylene Glycol Brines for Hot Water Applications (180 F or 82.2 C)
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
61.1
0.99
978.7
4.14
10
61.4
0.99
983.5
4.14
15
61.7
0.97
988.3
4.06
20
62.0
0.96
993.1
4.02
25
62.4
0.95
999.6
3.98
30
62.7
0.93
1004.4
3.89
35
63.0
0.92
1009.2
3.85
40
63.3
0.90
1014.0
3.77
45
63.7
0.88
1020.4
3.68
50
64.0
0.86
1025.2
3.60
Table 7. Propylene Glycol Brines for Hot Water Applications (180 F or 82.2 C)
Page 62 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Primary Loop for Primary-Only / Constant Speed Systems
12.0 Entering Plants ›› 12.11 Distribution System Data ››
Primary Loop for Primary-Only / Variable Speed Systems
12.0 Entering Plants ›› 12.11 Distribution System Data ››
Concentration
by Weight (%)
Density
(lb/cuft)
Specific Heat
(BTU/lb-F)
Density
(kg/m3)
Specific Heat
(kJ/kg K)
5
60.9
0.99
975.5
4.14
10
61.0
0.99
977.1
4.14
15
61.1
0.99
978.7
4.14
20
61.2
0.98
980.3
4.10
25
61.4
0.97
983.5
4.06
30
61.5
0.96
985.1
4.02
35
61.6
0.95
986.7
3.98
40
61.7
0.94
988.3
3.94
45
61.9
0.92
991.5
3.85
50
62.0
0.91
993.1
3.81
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Primary Loop for Primary-Only / Constant Speed Systems
For a Primary-Only, Constant Speed system, the Primary Loop section of the Distribution tab provides performance data for the primary
pumps. In this type of distribution system, one pump is paired with each chiller, heat pump or boiler in the system. This section consists
of a table with one row for each pump and columns containing different types of performance data:
1. Pump For Equipment No. Numbers in this column refer to the chiller, heat pump or boiler items found in the Schedule of Equipment
tab. For example, in a Chiller Plant the row labeled 2 contains data for the pump used with chiller #2 from the Schedule of Equipment
tab.
2. Flow is a display-only item which lists the design flow for the chiller, heat pump or boiler. In the case of a reversible chiller in a
changeover plant, the program uses the larger of the two chilled water supply flow and hot water supply flow for the equipment.
3. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
4. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is used to calculate pump motor kW
at design when pump head is specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
5. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in
determining pump heat gain to the water loop. It is also used to calculate pump motor kW at the design condition when pump head is
specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 63 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Primary Loop for Primary/Secondary Systems
12.0 Entering Plants ›› 12.11 Distribution System Data ››
Primary Loop for Primary-Only / Variable Speed Systems
For a Primary-Only, Variable Speed system, the Primary Loop section of the Distribution tab provides performance data for the primary
pump. This type of distribution system can consist of one large primary pump or a gang of pumps in parallel. The program analyzes a
single variable speed pump. If a gang of pumps is used, performance data must be combined into a single set of pump inputs.
This section consists of a table containing performance data for the primary pump and several additional control inputs. The values in the
pump table are as follows:
1. Flow is a display-only item which lists the total flow at design for the plant. This is the sum of supply water flow rates shown on the
Schedule of Equipment tab. If units of gpm or L/s are not used, "auto-sized" is displayed here; the flow rate will be calculated at the
start of the simulation. In the case of a reversible chiller in a changeover plant, the program uses the larger of the chilled water supply
or hot water supply flow.
2. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
3. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is involved in part-load performance
calculations for variable flow systems. It is also used to calculate pump motor kW at design when pump head is specified. It is used to
derive equivalent head when kW or W/gpm (W/L/s) is specified.
4. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in part-
load performance calculations for variable flow systems and in determining pump heat gain to the water loop. It is also used to
calculate pump motor kW at the design condition when pump head is specified. It is used to derive equivalent head when kW or
W/gpm (W/L/s) is specified.
The additional control inputs are as follows:
1. Control Head defines the differential pressure used to control the variable speed pump operation. Because control head is
independent of flow, it plays an important role in determining the shape and position of the head-vs-flow system curve. This system
curve, in turn, strongly influences part-load performance for the pump.
2. Minimum Pump Flow defines the minimum allowable flow rate for the variable speed pump as a percentage of design flow. For many
variable speed pumps, 30% is a typical minimum level. For each operating hour, the actual minimum pump flow will be determined by
this value and the Minimum Chiller Flow or Minimum Unit Flow defined in the next input, whichever results in a higher gpm or L/s flow
rate.
3. Minimum Chiller Flow, Minimum Unit Flow. In a chilled water plant, specify the minimum flow rate allowed for the chiller evaporator
as a percentage of full load flow. For hot water and changeover plants, specify the minimum flow rate allowed for the boilers or heat
pumps. Typically this information is available from equipment manufacturers in the form of a minimum flow velocity. Flow velocity
must be converted into gpm or L/s in order to determine the minimum flow percentage. When individual equipment units in the system
have different minimum flow percentages, specify the largest of these values.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Primary Loop for Primary/Secondary Systems
Page 64 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Secondary Loop for Primary/Secondary Systems
12.0 Entering Plants ›› 12.11 Distribution System Data ››
For a Primary/Secondary, Variable Speed system, the Primary Loop section of the Distribution tab provides performance data for the
primary pumps. In this type of distribution system, one constant speed pump is paired with each chiller, heat pump or boiler in the
system. This section consists of a table with one row for each pump and columns containing different types of performance data:
1. Pump For Equipment No. Numbers in this column refer to the chiller, heat pump or boiler items found in the Schedule of Equipment
tab. For example, in a Chiller Plant the row labeled 2 contains data for the pump used with chiller #2 from the Schedule of Equipment
tab.
2. Flow is a display-only item which lists the design flow for the chiller, heat pump or boiler.
3. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
4. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is used to calculate pump motor kW
at design when pump head is specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
5. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in
determining pump heat gain to the water loop. It is also used to calculate pump motor kW at the design condition when pump head is
specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Secondary Loop for Primary/Secondary Systems
For a Primary/Secondary Variable Speed system, the Secondary Loop section of the Distribution tab provides performance data for the
secondary pump. The secondary loop can use a single pump or a gang of pumps in parallel. The program analyzes a single variable
speed pump. If a gang of pumps is used, performance data must be combined into a single set of pump inputs.
This section consists of a table containing performance data for the secondary pump and several additional control inputs. The values in
the pump table are as follows:
1. Flow is a display-only item which lists the total flow at design for the plant. This is the sum of supply flow rates for the chillers, heat
pumps or boilers shown on the Schedule of Equipment tab.
Page 65 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Secondary Loop for Secondary-Only / Constant Speed Systems
12.0 Entering Plants ›› 12.11 Distribution System Data ››
Secondary Loop for Secondary-Only / Variable Speed
12.0 Entering Plants ›› 12.11 Distribution System Data ››
2. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
3. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is involved in part-load performance
calculations for variable flow systems. It is also used to calculate pump motor kW at design when pump head is specified. It is used to
derive equivalent head when kW or W/gpm (W/L/s) is specified.
4. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in part-
load performance calculations for variable flow systems and in determining pump heat gain to the water loop. It is also used to
calculate pump motor kW at the design condition when pump head is specified. It is used to derive equivalent head when kW or
W/gpm (W/L/s) is specified.
The additional control inputs are as follows:
1. Control Head defines the differential pressure used to control the variable speed pump operation. Because control head is
independent of flow, it plays an important role in determining the shape and position of the head-vs-flow system curve. This system
curve, in turn, strongly influences part-load performance for the pump.
2. Minimum Pump Flow defines the minimum allowable flow rate for the variable speed pump as a percentage of design flow. A typical
value for variable speed pumps is 30%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Secondary Loop for Secondary-Only / Constant Speed Systems
For a Secondary-Only, Constant Speed system, the Secondary Loop section of the Distribution tab provides performance data for the
secondary pump. This type of distribution system is used with remote source chilled water and hot water systems. The secondary loop
can use a single pump or a gang of pumps in parallel. The program analyzes a single variable speed pump. If a gang of pumps is used,
performance data must be combined into a single set of pump inputs.
This section consists of a table containing performance data for the secondary pump:
1. Flow defines the total flow at design for the plant. It is used to calculate pump motor kW at the design condition.
2. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
3. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is used to calculate pump motor kW
at design when pump head is specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
4. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in
determining pump heat gain to the water loop. It is also used to calculate pump motor kW at the design condition when pump head is
specified. It is used to derive equivalent head when kW or W/gpm (W/L/s) is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 66 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.12 Condenser Water Tab
12.0 Entering Plants ››
Condenser Water Tab / Plant Form
12.0 Entering Plants ›› 12.12 Condenser Water Tab ››
Secondary Loop for Secondary-Only / Variable Speed
For a Secondary-Only, Variable Speed system, the Secondary Loop section of the Distribution tab provides performance data for the
secondary pump and its associated controls. This type of distribution system is used with remote source chilled water and hot water
systems. The secondary loop can use a single pump or a gang of pumps in parallel. The program analyzes a single variable speed
pump. If a gang of pumps is used, performance data must be combined into a single set of pump inputs.
This section consists of a table containing performance data for the secondary pump and several additional control inputs. The values in
the pump table are as follows:
1. Flow defines the total flow at design for the plant. It is used to calculate pump motor kW at the design condition and is involved in part-
load performance calculations. If units of gpm or L/s are not used, "auto-sized" is displayed here. In the case of a reversible chiller in
a changeover plant, the program uses the larger of the chilled water supply flow or hot water supply flow for the equipment.
2. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Distribution System
section of this input screen. Performance can be defined as head, W/gpm (W/L/s) or kW.
3. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is involved in part-load performance
calculations for variable flow systems. It is also used to calculate pump motor kW at design when pump head is specified. It is used to
derive equivalent head when kW or W/gpm (W/L/s) is specified.
4. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in part-
load performance calculations for variable flow systems and in determining pump heat gain to the water loop. It is also used to
calculate pump motor kW at the design condition when pump head is specified. It is used to derive equivalent head when kW or
W/gpm (W/L/s) is specified.
The additional control inputs are as follows:
1. Control Head defines the differential pressure used to control the variable speed pump operation. Because control head is
independent of flow, it plays an important role in determining the shape and position of the head-vs-flow system curve. The system
curve, in turn, strongly influences part-load performance for the pump.
2. Minimum Pump Flow defines the minimum allowable flow rate for the variable speed pump as a percentage of design flow. A typical
value for variable speed pumps is 30%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Condenser Water tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Condenser Water Tab / Plant Form
The Condenser Water tab is used to define condenser water loop controls and pump performance for a chiller plant containing water-
cooled chillers. This tab is divided into two sections, as shown below:
1. Water System defines how the system and its pumps are controlled, and the units of measure for pump performance.
2. Water Loop provides performance data for condenser pumps connected to the loop.
Page 67 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Water System
12.0 Entering Plants ›› 12.12 Condenser Water Tab ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Water System
This section of inputs appears on the Condenser Water tab for chiller plants and the Source Water plant for changeover plants and hot
water plants which use water source reversible chillers or water source heat pumps. The Water System group of inputs describes how
the water system and its pumps are controlled, and the units of measure for pump performance. There are four inputs in this section:
1. Pump Control - Pumps can be controlled in one of two ways:
a. Constant Flow / Constant Speed - Water flow is held constant. Pumps run at constant speed, at their design input kW.
b. Variable Flow / Variable Speed - Water flow varies to hold the delta-T constant. When the minimum flow setting is reached, water
flow is held constant at the minimum setting and the delta-T then decreases with load. The pumps are variable speed and ride the
system curve as the flow varies.
Page 68 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Water Loop
12.0 Entering Plants ›› 12.12 Condenser Water Tab ››
12.13 Source Water Tab
12.0 Entering Plants ››
2. Minimum Pump Flow specifies the minimum flow setpoint as a percent of design water flow. This input is only enabled when
"Variable Flow / Variable Speed" pump control is specified. During system operation, the flow varies to hold the delta-T constant down
to minimum flow. As load continues to drop, flow is held constant and the delta-T decreases with load.
3. Static Head applies to condenser water systems using an open circuit cooling tower. It describes the portion of the condenser pump
head due to the vertical rise in the condenser pumping loop. This input is only enabled when "Variable Flow / Variable Speed" pump
control is specified. With open circuit cooling towers, the condenser water flows in an open loop. The presence of static head causes
the zero flow point on the pump system curve to correspond to static head, rather than passing through the zero flow, zero head point.
This has a significant effect on pump performance when operating at reduced pump flow and speed. When using closed circuit
cooling towers, dry coolers or geo well fields, condenser water is a closed loop and static head should be set to zero.
4. Pump Performance Units specifies how pump performance will be defined in the Water Loop table at the bottom of this tab. Pump
performance can be defined as pump head (ft wg or kPa), pump power per unit flow (W/gpm or W/L/s) or as pump motor input power
(kW).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Water Loop
This section of inputs appears on the Condenser Water tab for chiller plants and the Source Water tab for changeover plants and for hot
water plants which use water source equipment. The Water Loop group of inputs contains a table of performance data for the pumps in
the plant. For chiller plants where one cooling tower serves each chiller, the table will have separate rows for the condenser pump
serving each water-cooled chiller. When one cooling tower is shared by all water-cooled chillers, the table will contain one row containing
data for the pump serving the shared loop. For geo source changeover plants and hot water plants, there will typically be one shared
pumping system for the plant and therefore only one row in the table. Values in the table are as follows:
1. Flow is a display-only item which lists the water flow rate for the pump. This data is taken from the Schedule of Equipment tab.
2. Pump defines the pump performance value. Units of measure depend on the Pump Performance input in the Water System section.
Performance can be defined as head, pump power per unit flow (W/gpm or W/L/s) or pump kW.
3. Mechanical Efficiency defines inefficiencies of the pump impeller and the drive (if applicable) at the pump design condition. This
value is typically obtained from pump selection software or pump catalogs. Mechanical efficiency is involved in part-load performance
calculations for variable flow systems. It is also used to calculate pump motor kW at design when pump head is specified. It is used to
derive equivalent head when kW or W/gpm (W/L/s) is specified.
4. Electrical Efficiency defines the electrical efficiency of the pump motor at the design condition. Electrical efficiency is involved in part-
load performance calculations for variable flow systems and in determining pump heat gain to the water loop. It is also used to
calculate pump motor kW at the design condition when pump head is specified. It is used to derive equivalent head when kW or
W/gpm (W/L/s) is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 69 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
Source Water Tab / Plant Form
12.0 Entering Plants ›› 12.13 Source Water Tab ››
12.14 Common Tasks
12.0 Entering Plants ››
Creating a New Plant
This section explains input dat aon the Source Water tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Source Water Tab / Plant Form
The Source Water tab is used to define source water loop controls and pump performance for a changeover plant using water source
reversible chillers or a hot water plant using water-to-water heat pumps. This tab is divided into two sections, as shown below:
1. Water System defines how the system and its pumps are controlled, and the units of measure for pump performance.
2. Water Loop provides performance data for source water pumps connected to the loop.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with plant input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 70 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.0 Entering Plants ›› 12.14 Common Tasks ››
Editing an Existing Plant
12.0 Entering Plants ›› 12.14 Common Tasks ››
Printing Plant Inputs
12.0 Entering Plants ›› 12.14 Common Tasks ››
Deleting Plants
12.0 Entering Plants ›› 12.14 Common Tasks ››
Copying a Plant
12.0 Entering Plants ›› 12.14 Common Tasks ››
Duplicating a Plant
12.0 Entering Plants ›› 12.14 Common Tasks ››
Printing or Viewing Plant Design Reports
12.0 Entering Plants ›› 12.14 Common Tasks ››
Printing or Viewing Plant Simulation Reports
Creating a New Plant
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Plant
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Plant Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Plants
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Plant
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Plant
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing or Viewing Plant Design Reports
Please see Generating Plant Design Reports
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 71 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm
12.0 Entering Plants ›› 12.14 Common Tasks ››
Printing or Viewing Plant Simulation Reports
Please see Generating Plant Simulation Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 72 of 72
12.0 Entering Plants
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh8E5A.htm