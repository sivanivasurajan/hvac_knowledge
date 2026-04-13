6.0 Energy Analysis Applications
Overview for Energy Analysis Applications
6.0 Energy Analysis Applications ››
Energy Analysis Strategies
6.0 Energy Analysis Applications ››
This chapter provides guidance for using HAP for common HVAC energy modeling applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Energy Analysis Applications
The following series of help topics explain how to use the program for common energy analysis applications.
Topics in the "Getting Started" section of the help system contained general discussions of how to use the
program for energy analysis studies. However, the program can be used in studies involving a many different
types of HVAC equipment. Procedures for using the program for these applications are not always obvious,
especially for new program users. Therefore, this chapter covers the following twelve application topics:
1. General energy analysis strategies.
2. Troubleshooting strategies.
3. Simulating packaged rooftop units
4. Simulating vertical packaged units.
5. Simulating split DX air handlers.
6. Simulating chilled water air handlers.
7. Simulating packaged or split DX fan coil units.
8. Simulating hydronic fan coil units.
9. Simulating induction beam or active chilled beam systems.
10. Simulating water source heat pump systems.
11. Simulating ground water and ground source heat pump systems.
12. Simulating chilled water plants.
13. Simulating hot water and steam plants
14. Simulating heat recovery plants.
In all of these discussions it is assumed the reader is familiar with the basic program operating procedures.
Further, it is assumed input data has been gathered and entered for weather, schedules, walls, roofs,
windows, doors and shading geometries. Therefore, entry of this data will not be covered in the application
discussions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Strategies
The purpose of an energy analysis is to compare the annual energy use and energy costs of alternate system
designs. To generate energy use data, the operation of all energy-consuming equipment in a building must be
simulated. This includes energy use by air handling systems, plant equipment, and non-HVAC systems such
as lighting and office equipment. In small buildings, the analysis is easy to organize due the relatively small
number of components involved. For larger buildings, however, the analysis can be much harder to organize.
In these cases it is important to consider ways to minimize input effort and calculation time. This section
discusses strategies for maximizing the accuracy of energy analysis results while minimizing effort.
The most accurate energy analysis results can be obtained by analyzing equipment exactly as it is installed.
For example, if a building contains 400 water source heat pump (WSHP) units, the most accurate approach
would be to model 400 heat pump units and the spaces they serve separately. In this way loads experienced
by each WSHP unit and the performance of each unit could be accurately evaluated.
Page 1 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
While this is conceptually the simplest approach to energy analysis, it can often require the largest amount of
time for gathering and inputting data and then running simulations. In certain situations the number of spaces,
zones, air systems and plants can be systematically reduced without significantly affecting the accuracy of
results.
Simplification of the energy analysis is achieved using two techniques. One involves combining or "lumping"
together similar components in the analysis. Two identical zones in an air system, for example, can be
combined without affecting system simulation results. The other is simulating identical equipment only once,
and then using multipliers to account for the total number of units in the building. In a hotel, for example,
packaged terminal air conditioner (PTAC) units might be used in 75 identical south-facing guest rooms. Rather
than simulate all 75 PTAC units separately, one representative unit can be simulated and then multiplied by 75
to account for the total energy consumption of the equipment in energy cost calculations.
Both these approaches require careful evaluation of which components in the analysis can and cannot be
combined. If the analysis is oversimplified, energy use and costs can be significantly over or under-estimated.
Separate paragraphs below summarize considerations involved with reducing the number of spaces, zones,
air systems and plants involved in the analysis.
1. Space Data. In many situations, rooms in a zone can be combined and defined as one space. Because a
zone has only one thermostat, it is the total zone load that drives air terminal operation and therefore
system operation, not the individual space loads. Therefore, the same total zone loads will be calculated
whether the zone is defined using one large combined space or multiple spaces representing separate
rooms.
In a zone containing several identical rooms, another approach is to define only one of the rooms as a
space. When linking spaces to zones, a multiplier can be used to account for the total number of this type of
room in the zone.
These techniques reduce the number of spaces entered and the time required for the program to compute
loads during the energy simulations.
Note: For several reasons design considerations may prevent using this reduction technique. If a project
involves both system design and energy analysis, it may be necessary to define each room as a space in
order to size air diffusers for each room. Further, if design zone airflow rates are based on the sum of peak
space airflow rates, then spaces in the zone cannot be combined. To properly size zone airflow rates, the
individual spaces in the zone must be defined.
2. Zone Data. A zone is defined as the region of a building served by one thermostat. Large air-handling
systems which contain many zones and systems involving multiple single-zone units, such as fan coils,
offer the greatest potential for simplification.
In a central air-handling system serving an office building, for example, each perimeter office may contain a
thermostat. However, many offices on the same perimeter exposure may experience identical or very
similar patterns of loads. Rather than analyzing each room as a separate zone, many zones can be lumped
together without sacrificing accuracy. For example, 20 offices on the south exposure of a building might be
combined into one large south-facing zone. The same principles apply when terminal units such as fan coils
serve the offices. When combining zones:
a. Do combine zones with identical or similar patterns of loads. Typically these zones will have the same
exterior exposure and the same patterns of occupancy and internal heat gains.
b. Don't combine zones with different exterior exposures. For example, combining north-facing and south-
facing offices is a poor choice since each experiences significantly different patterns of solar loads.
c. Don't combine zones which do have a roof exposure with those that don't. The presence of the roof
causes load patterns to differ from those in zones without a roof exposure.
d. Don't combine interior regions with perimeter zones. For much of the year, interior heat gains will offset
perimeter heat losses causing heating loads to be understated.
e. Don't combine zones with different use patterns. For example, in a school building, a classroom zone
should not be combined with a cafeteria zone since the occupancy and heat gain patterns in each differ.
The advantages of reducing the number of zones are that fewer spaces need to be input, and times for load
calculations and air system simulations are reduced.
Page 2 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Energy Analysis Troubleshooting Strategies
6.0 Energy Analysis Applications ››
3. Air System Data. Opportunities for reducing the number of air systems in an analysis vary between central
air handling systems and terminal systems such as fan coils.
Opportunities for combining central air handling systems are usually limited, except in special cases where
several similar or identical systems serve different parts of a building. For central air systems to be "similar",
the systems must contain the same components, be sized in the same way, serve the same number of
zones, and experience the same pattern of loads. This situation might occur in a multi-story building where
separate air systems serve each floor, and patterns of loads on each floor are very similar. In such a case,
an air system for a typical intermediate floor could be defined and simulated once. When the air system is
linked a plant or a building, a multiplier can be used to account for the total number of air systems of this
type in the building.
Opportunities for reducing the number of terminal type air systems in an analysis are much more common.
As discussed earlier, the number terminal air-conditioner units in guest rooms in a hotel can be vastly
reduced analyzing typical units and using multipliers. When identifying typical units, or when lumping units
together, the criteria previously described for combining zones should be used. In addition, units which use
different components or controls should not be lumped together since these differences will affect
performance and energy consumption.
4. Plant Data. Opportunities for combining central plants such as chiller and boiler plants rarely exist, since
buildings typically contain one of each, if plants are used at all.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Analysis Troubleshooting Strategies
This topic describes general strategies used to investigate energy analysis results. These investigations may
be necessary when diagnosing problems or simply learning more about results generated by the program.
General strategies useful in a variety of situations will be described below.
1. Investigate Input and Output Data. When a question about results arises, generate and inspect printouts
of pertinent input and simulation data. Checking input printouts often reveals input errors which cause
incorrect results. In addition, checking and comparing printouts of simulation data often reveals the reason
for results, or provides clues to simulation problems, as discussed below.
Questions frequently arise about unusual building energy cost results. Energy costs are the final, bottom-
line results of the energy analysis. Because costs are dependent on many factors, it is necessary to
generate details showing how the costs were calculated and intermediate results showing the performance
of air systems and plants contributing to building energy consumption. The strategy should be to work
backward from the final results to determine how they were derived. This work can be performed in two
stages. First, generate detailed building outputs. The following building simulation reports are often useful:
a. Energy Budget by System Component: When complex rate structures are used, operating costs are not
proportional to energy use due to the demand, fixed and tax charge components of the energy bill.
Therefore, operating costs often do not present a clear picture of energy use by the building. Comparing
only the bottom line cost figures may obscure the energy performance of the building. The Energy
Budget by System Component report lists annual energy use totals in common units (kBTU in English,
kWh in Metric) and can be a better basis for comparison.
c. Monthly Energy Use By System Component: This report lists month by month energy use by both system
component and energy type. It provides more detailed information than the Energy Budget report, listing
energy use in billing units (e.g., kWh for electric, Therms for gas, etc..) for each system component
category. This makes it much easier to make direct comparisons between buildings and identify key
differences in energy performance.
b. Billing Details: These reports document the individual charges contributing to the total electric and fuel
bills. The reports also list the monthly average price of energy, energy consumption totals, monthly
demands and the time when each demand occurs. This data can be used to determine how the utility bill
Page 3 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Packaged Rooftop Units
6.0 Energy Analysis Applications ››
was calculated, and to identify factors contributing to unusual results. For example, an unusual increase
in costs may be due to a large peak demand in one month. This might focus the investigation on
equipment performance during the particular month with the large demand.
If building reports do not reveal the cause of a problem, the second stage in the analysis is to investigate
simulation results for the plants and air systems in the building. Two ways of doing this are discussed
below.
a. Monthly-Daily-Hourly Simulation Results. One approach is to first inspect the monthly report to identify
months with unusual results, then inspect the daily report for that month to focus on the individual days
with odd results, and finally inspect hourly reports for those days.
b. Hourly Graphics. An alternate approach is to generate hourly graphs for long sequences of time in order
to pinpoint portions of the year showing unusual behavior, and then generate graphs for shorter periods
of time to investigate behavior in greater detail. For example, cooling coil loads for all 8,760 hours in the
year can be included in one plot. This plot might show times of year when unusually large or small
cooling loads exist. The next step would be to generate graphs for these shorter periods of time to
understand this behavior.
Using these strategies, problems can be efficiently investigated and diagnosed.
2. Research Input Definitions and Calculation Procedures. In many cases, thorough knowledge of how the
program uses inputs and performs its energy simulations is necessary to understand program results.
Material in the program's on-line help system provides this information. The operation sections of the on-line
help system discuss program inputs and explain how inputs are used by the program. The documentation
sections of the on-line help system explain calculation assumptions and procedures.
3. Perform Comparative Analyses. In some cases, investigating input and output data, and researching
calculation procedures are not sufficient to diagnose problems with results. In these situations, various
types of comparative analyses performed with the program can be helpful. The success of this technique
depends on the user's ingenuity, knowledge of load, system and equipment behavior, and knowledge of the
program. A common example of how comparative analysis can be used is provided below.
Example: Suppose unusual energy costs results are obtained and an investigation of program outputs
shows that results are due to peculiar air system behavior. The air system in question uses dehumidification
control, a preheat coil and an enthalpy economizer. Careful inspection of monthly, daily and hourly
simulation results does not reveal a logical reason for the results.
Because it is possible behavior of one of the system components or unanticipated interaction between
components is causing the results, a useful strategy is to run simulations for variations of the air system to
try to identify how each component influences system performance. First make four copies of the air
system. One should represent a base case without dehumidification control, a preheat coil or an
economizer. The other three copies should include one of the extra components each. For example, one
system would include only the dehumidification control, one would include the preheat coil, and one would
include the economizer. Generate air system simulation reports for all four systems and compare results.
The comparison will clearly show the effect of each component on system behavior, and may allow you to
determine the reason for the original results. If not, it may be necessary to run simulations for simple
combinations of components such as the economizer and dehumidification control, dehumidification control
and the preheat coil, etc... Inspection of results for these simulations may reveal unanticipated interaction or
conflicts between the components.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Packaged Rooftop Units
This topic explains how to model packaged rooftop equipment in energy simulations. This equipment contains
a supply fan, condenser fans, DX cooling apparatus and heating apparatus all in one packaged unit. Heating
Page 4 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Vertical Packaged Units
6.0 Energy Analysis Applications ››
options are electric resistance, combustion, heat pump and, in unusual cases, hot water or steam. Modeling
procedures are described below.
1. Air Systems. Define one air system per rooftop unit. If the building contains multiple rooftops which are
identical, serving identical or similar areas of the building, a single rooftop unit can be modeled and a
multiplier can be applied to account for the total number of these units. Modeling tips:
a. Specify the Equipment Class as "Packaged Rooftop Unit"
b. Specify the appropriate system type and enter system data.
c. Define the performance characteristics of the DX cooling equipment using the Equipment Tab in the Air
System window.
d. If heat pump or combustion heating is used, define performance characteristics of the heating equipment
using the Equipment Tab in the Air System window.
e. If electric heat is used, no additional heating equipment inputs are required.
2. Plants. It is not necessary to define a plant except in the unusual cases where a hot water or steam heating
coil has been added to the rooftop unit. In these cases a hot water or steam plant must be defined to serve
these coils. The rooftop air system will be linked to this plant. If a heating plant serves multiple systems, a
single heating plant can be defined and all systems can be linked to it.
3. Building. If electric, combustion or heat pump heating is used, the air system is linked directly to the
building. A multiplier can be used if the rooftop represents one of a group of identical units. If hot water or
steam heating is used, then both the heating plant and the rooftop air system must be linked to the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Vertical Packaged Units
This topic explains how to model vertical packaged (VPAC) equipment in energy simulations. The air-cooled
version of this equipment contains a supply fan, condenser fans, DX cooling apparatus and heating apparatus
all in one packaged indoor unit; in some cases a remote condenser is used. The water-cooled version of this
equipment contains a supply fan, DX cooling apparatus and heating apparatus in one packaged indoor unit.
The water cooled condenser is connected to a cooling tower. Heating options include electric resistance,
combustion, hot water and steam. Modeling procedures are described below.
1. Air Systems. Define one air system per vertical packaged unit. If the building contains multiple VPACs
which are identical, serving identical or similar areas of the building, a single VPAC unit can be modeled
and a multiplier can be applied to account for the total number of these units. Modeling tips:
a. Specify the Equipment Class as "Packaged Vertical Unit"
b. Specify the appropriate system type and enter system data.
c. Define the performance characteristics of the DX cooling equipment using the Equipment Tab in the Air
System window.
d. For water-cooled units, a cooling tower must be defined and linked to the air system. This is done using
the "Miscellaneous Equipment" button on the Equipment Tab.
e. If combustion heating is used, define performance characteristics of the heating equipment using the
Equipment Tab in the Air System window.
f. If electric heat is used, no additional heating equipment inputs are required.
2. Plants. Plant equipment is not needed unless hot water or steam heating is used. In these cases a hot
water or steam plant must be defined and the VPAC air system is linked to this plant. If the heating plant
serves multiple air systems, a single heating plant can be defined and all air systems linked to it.
Page 5 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Split DX Air Handling Units
6.0 Energy Analysis Applications ››
Simulating Chilled Water Air Handling Units
6.0 Energy Analysis Applications ››
3. Building. If electric or combustion heating is used, the VPAC air system is linked directly to the building. A
multiplier can be used if the VPAC represents one of a group of identical units. If hot water or steam heating
is used, then both the heating plant and the VPAC air system must be linked to the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Split DX Air Handling Units
This topic explains how to model split DX air handling units in energy simulations. This equipment includes an
indoor unit containing fans, a DX cooling coil and heating apparatus, plus an outdoor condensing unit. Heating
options include electric resistance, combustion, heat pump, hot water and steam. Modeling procedures are
described below.
1. Air Systems. Define one air system per split DX air handler. If the building contains multiple split units
which are identical, serving identical or similar areas of the building, a single air handler can be modeled
and a multiplier can be applied to account for the total number of these units. Modeling tips:
a. Specify the Equipment Class as "Split DX AHU"
b. Specify the appropriate system type and enter system data.
c. Define the performance characteristics of the DX cooling equipment using the Equipment Tab in the Air
System window.
d. If heat pump or combustion heating is used, define performance characteristics of the equipment using
the Equipment Tab in the Air System window.
e. If electric heat is used, no additional heating equipment inputs are required.
2. Plants. Plant equipment is not needed unless hot water or steam heating is used. In these cases a hot
water or steam plant must be defined and the split DX air system is linked to this plant. If the heating plant
serves multiple air systems, a single heating plant can be defined and all the air systems linked to it.
3. Building. If heat pump, combustion or electric heat is used, the split DX air handler is linked directly to the
building. A multiplier can be used if the split DX unit represents one of a group of identical units. If hot water
or steam heating is used, then both the heating plant and the split DX air system must be linked to the
building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Chilled Water Air Handling Units
This topic explains how to model chilled water air handling units in energy simulations. This equipment
includes fans, a chilled water cooling coil and heating apparatus in a packaged or built-up unit. Heating options
include electric resistance, combustion, hot water and steam.
Modeling procedures are described below.
1. Air Systems. Define one air system per chilled water air handler. Typically these are larger systems which
are unique. But in those situations where a building contains multiple chilled water AHUs which are
identical, serving identical or similar areas of the building, a single air handler can be defined and a
multiplier can be applied to account for the total number of these units. Modeling tips:
a. Specify the Equipment Class as "Chilled Water AHU".
b. Specify the appropriate system type and enter system data.
Page 6 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Packaged or Split DX Fan Coil Units
6.0 Energy Analysis Applications ››
c. If combustion heating is used, define performance characteristics of the equipment using the Equipment
tab in the Air System window.
d. If electric heat is used, no heating equipment inputs are required on the Equipment tab.
e. If you are defining a 2-pipe changeover system, specify the type of changeover control using the
Changeover Controller option on the Equipment Tab. Changeover can be based on a monthly schedule
or outdoor air temperature threshold. These settings affect all cooling components using chilled water,
and all heating components using hot water.
When the monthly schedule option is selected, make sure to specify the appropriate on/off schedules in
the Central Cooling, Central Heating, Precool Coil and/or Preheat Coil sections of the System
Components tab, and the Supply Terminals and Zone Heating Units sections of the Zone Components
tab. If the outdoor air temperature threshold option is selected, you can set all the coil schedules to ON
for 12 months, unless there are also specific times of year when cooling or heating is off, in which case
the on/off schedules can also be set.
2. Plants.
a. If the AHUs are served by a chilled water plant, define a chiller plant or a remote chilled water (district
cooling) plant.
b. If the AHUs are linked to a changeover plant with reversible chillers, define a changeover plant.
c. If hot water or steam heating is used, define a hot water or steam plant to provide heat to air system
heating coils. Plant options include hot water plants (boilers or dedicated heat pumps), steam boiler
plants and remote (district) heating.
Typically these plants will serve two or more air handlers. When defining the plant, link to all the air systems
served by the plant. When a system represents one of a group of identical systems, a multiplier can be
used when linking it to the plant.
3. Building. Link the chilled water AHU air system as well as the cooling plant, changeover plant and/or
heating plant to the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Packaged or Split DX Fan Coil Units
This topic explains how to model packaged or split DX fan coil units in energy simulations. This equipment
includes Packaged Terminal Air Conditioners (PTACs), Packaged Terminal Heat Pumps (PTHPs), Variable
Refrigerant Flow (VRF), DX unit ventilators, room air conditioners, split DX fan coils, ductless split units and
other similar products. The packaged version of the equipment contains a supply fan, air-cooled DX cooling
apparatus and heating apparatus in one packaged unit. The split version of the equipment contains a supply
fan, DX cooling coil and heating apparatus in an indoor unit plus an outdoor condensing unit. Heating options
include electric resistance, combustion, heat pump, hot water and steam. Modeling procedures are described
below.
1. Air Systems. Define one air system for the entire collection of DX fan coil units. HAP will model each zone
in the system as containing one fan coil unit. Loads for each zone and the performance of each zone's fan
coil unit will be performed separately. Loads and energy use are then summed to obtain system totals
which are displayed on the simulation reports. Modeling tips:
a. Specify the Equipment Class as "Terminal Units"
b. Specify the System Type as "Packaged DX Fan Coil", "Split DX Fan Coil", or "Variable Refrigerant Flow"
and enter system data.
c. Define performance characteristics of the DX cooling equipment using the Equipment Tab on the Air
System window. Be sure to define performance data for all zone fan coils.
Page 7 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Hydronic Fan Coil Units
6.0 Energy Analysis Applications ››
d. If heat pump or combustion heating is used, define performance characteristics of the equipment using
the Equipment Tab in the Air System window. Again, be sure to define performance for all zones.
e. If electric heat is used, no additional heating equipment inputs are required.
f. If the number of fan coil units exceeds the number of zones permitted in a system, then an additional
system will be required to accommodate the extra fan coils.
2. Plants. If heat pump, combustion or electric heat is used then no plant equipment is required. If hot water or
steam heating is used, a hot water or steam plant must be defined and must link to the fan coil air system. If
the heating plant serves multiple air systems, a single plant can be defined and linked to all air systems
containing hot water or steam coils.
3. Building. If electric resistance, heat pump or combustion heating is used, link the air system directly to the
building. If hot water or steam heating is used, link both the system and the plant to the building.
Note: Fan coil systems are good candidates for the data reduction techniques discussed in the Energy
Analysis Strategies topic. However, if you use these techniques to reduce input and calculation time,
planning is required to account for the correct number of fan coil units in the building.
Example: A hotel is being studied which has 75 identical fan coil zones on the south face of the building, 62
identical fan coil zones on the north face of the building and 48 fan coil zones which are unique. In this
situation it may be best to define three air systems. System #1 would contain 48 zones holding the 48 fan
coil units that are unique. System #2 would contain only one zone representing the typical south-facing
zone. System #3 would contain only one zone representing the typical north-facing zone. When linking
systems to the building a system multiplier of 1 would be used for system #1, a multiplier of 75 would be
used for system #2 and a multiplier of 62 would be used for system #3. This is necessary because
multipliers are applied at the system level when linking systems to plants and buildings.
An alternate approach is to lump identical fan coils together rather than defining a single typical unit for
each. This means that the 75 south facing fan coil zones would be combined, using a space multiplier of 75.
The cooling and heating equipment inputs would define full load capacity and input power values that are
the sum of the 75 fan coil capacities and input powers rather than the actual capacity and power for one
representative unit. This approach would allow the typical north and typical south zones to be included in
System #1 with the 48 unique zones while still correctly accounting for the total loads and energy use of
these fan coil units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Hydronic Fan Coil Units
This topic explains how to model hydronic fan coil units in energy simulations. This equipment contains a
supply fan, a chilled water coil and a heating coil in one packaged indoor unit. Heating options include hot
water, steam and electric resistance. Modeling procedures are described below.
1. Air Systems. Define one air system for the entire collection of hydronic fan coils. HAP will model each zone
in the system as containing one fan coil unit. Loads for each zone and the performance of each zone's fan
coil unit will be performed separately. Loads and energy use are then summed to obtain system totals
which are displayed on the simulation reports. Modeling tips:
a. Specify the Equipment Class as "Terminal Units"
b. Specify the System Type as "2-Pipe Fan Coil" or "4-Pipe Fan Coil" and enter system data.
c. Choose whether a Dedicated Outdoor Air System (DOAS) unit or direct ventilation is used.
d. If electric heat is used, no heating equipment inputs are required on the Equipment tab.
e. For 2-Pipe Fan Coil systems, specify the type of changeover control using the Changeover Controller
option on the Equipment tab. Changeover can be based on a monthly schedule or outdoor air
temperature threshold.
Page 8 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Induction Beam and Active Chilled Beam Systems
6.0 Energy Analysis Applications ››
When the monthly schedule option is selected, make sure to specify the appropriate on/off schedules in
the Common Data section of the Zone Components tab, and in the Cooling Coil and Heating Coil
sections of the DOAS Components tab if a Dedicated Outdoor Air System (DOAS) is used. If the
outdoor air temperature threshold option is selected, you can set all the coil schedules to ON for 12
months, unless there are also specific times of year when cooling or heating is off, in which case the
on/off schedules can also be set.
f. If the number of fan coil units exceeds the number of zones permitted in a system, then an additional
system will be required to accommodate the extra fan coils.
2. Plants.
a. If the fan coils are served by a chilled water plant, define a chiller plant or a remote chilled water (district
cooling) plant.
b. If the fan coils are linked to a changeover plant with reversible chillers, define a changeover plant.
c. If hot water or steam heating is used, define a hot water or steam plant to provide heat to fan coil system
heating coils. Plant options include hot water plants (boilers or dedicated heat pumps), steam boiler
plants and remote (district) heating.
Typically these plants will serve two or more fan coil systems. When defining the plant, link to all the air
systems served by the plant. When a system represents one of a group of identical systems, a multiplier
can be used when linking it to the plant.
3. Building. Link the hydronic fan coil system as well as the cooling plant, changeover plant and/or the heating
plant to the building.
Note: Fan coil systems are good candidates for the data reduction techniques discussed in the Energy
Analysis Strategies topic. Also, please refer to the note at the end of the Packaged and Split DX Fan Coil
topic for a discussion of special considerations when reducing the number of fan coil units modeled.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Induction Beam and Active Chilled Beam Systems
This topic explains how to model induction beam and active chilled beam systems in energy simulations.
These systems consist of a dedicated outdoor air system (DOAS) which provides cooled and dehumidified air
to ceiling-mounted induction terminals in each conditioned zone. Induction beams are total cooling devices
which include a drain pan and therefore can serve both sensible and latent loads in the zone. Active chilled
beams are sensible-only cooling devices which can only serve the zone sensible load. Both types of terminals
can also provide heating. Modeling procedures are described below.
1. Air Systems. Define one air system representing the DOAS system and all the induction beam (IB) or
active chilled beam (ACB) terminals it serves. Each zone in the system has a single thermostatic control
which controls one or more IB or ACB terminals in the zone. Loads are calculated separately for each
zone. The performance of the each zone's IB or ACB terminals is calculated separately (when the actual
system has multiple terminals per zone, HAP lumps the terminals into one large terminal for purposes of
analysis). Loads for the terminals are then summed to obtain system totals for terminal cooling and
terminal heating which are displayed on the simulation reports. Modeling tips:
a. Specify the Equipment Class as "Terminal Units"
b. Specify the System Type as "Induction Beam" or "Active Chilled Beam" and enter system data.
c. If the system is a 2-pipe cooling and heating system, specify the type of changeover control using the
Changeover Controller option on the Equipment tab. Changeover can be based on a monthly schedule
or outdoor air temperature threshold.
When the monthly schedule option is selected, make sure to specify the appropriate on/off schedules in
the Common Data section of the Zone Components tab, and in the Cooling Coil and Heating Coil
Page 9 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Water Source Heat Pump Systems
6.0 Energy Analysis Applications ››
sections of the DOAS Components tab. If the outdoor air temperature threshold option is selected, you
can set all the coil schedules to ON for 12 months, unless there are also specific times of year when
cooling or heating is off, in which case the on/off schedules can also be set.
d. If the number of IB or ACB zones exceeds the number of zones permitted in a system, then an additional
system will be required to accommodate the extra zones.
2. Plants.
a. For applications using separate cooling and heating plants, first define a chiller plant or a remote chilled
water (district cooling) plant to provide chilled water to system cooling coils. Then define a hot water
plant or remote hot water plant to provide hot water to system heating coils.
b. For 2-pipe changeover applications using reversible chillers, define a changeover plant to provide both
chilled water and hot water to coils in the system.
Typically these plants will serve two or more air systems. When defining the plant, link to all the air systems
served by the plant. When a system represents one of a group of identical systems, a multiplier can be
used when linking it to the plant.
3. Building. Link the chilled water and hot water plants, or the changeover plant to the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Water Source Heat Pump Systems
This topic explains how to model water source heat pump systems in energy simulations. HAP deals with
three types of water source heat pump equipment:
1. Water source heat pump (WSHP) systems consist of a number of heat pump units connected to a closed
water loop. In this system, heat is rejected from the loop through a cooling tower and heat is added by a hot
water boiler.
2. Ground water source heat pump (GWSHP) systems consist of a number of heat pump units generally
connected to a closed loop. In these systems the water loop uses an open source such as well, river or lake
water as the heat source/sink. Auxiliary heating is provided by electric resistance heaters.
3. Ground source heat pump (GSHP) systems consist of a number of heat pump units connected to a closed
loop. In these systems one of a number of different heat source/heat sink schemes are used such as
vertical borehole wells, buried horizontal ground heat exchangers, and heat exchangers submerged in lake
or river water. Auxiliary heat is provided by electric resistance heaters.
Modeling procedures are described below.
1. Air Systems. Define one air system for the entire collection of WSHP, GWSHP or GSHP units. HAP will
model each zone in the system as containing one heat pump unit. Loads for each zone and the
performance of each zone's heat pump will be performed separately. In a closed loop WSHP system
interaction of the heat pump units via the water loop will also be analyzed. Loads and energy use for the
individual heat pump units are then summed to obtain system totals which are displayed on the simulation
reports. Modeling tips:
Specify the Equipment Class as "Terminal Units"
a. Specify the System Type as WSHP, GWSHP or GSHP and enter system data.
b. Select whether ventilation air is introduced directly at the terminal unit, or whether a Dedicated Outdoor
Air System (DOAS) unit is used.
c. Define performance characteristics of the heat pump units for both cooling duty and heating duty using
the Equipment Tab in the Air System window.
Page 10 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Ground Water and Ground Source Heat Pump Systems
6.0 Energy Analysis Applications ››
Simulating Chilled Water Plants
6.0 Energy Analysis Applications ››
d. Also enter system information using the "Miscellaneous Equipment" button on the Equipment tab. For a
WSHP system, these inputs define the cooling tower and auxiliary boiler and the loop control setpoints.
For GWSHP and GSHP systems, these inputs define the source of modeling data for the ground water
or ground heat source/sink.
e. When a DOAS unit is used, it can be designated as a heat pump unit, or as an Air-Cooled DX unit. When
used, performance of the cooling and heating apparatus in the DOAS unit must be defined using the
Vent Cooling and Vent Heating buttons on the Equipment tab.
f. If the number of heat pump units exceeds the number of zones permitted in a system, then an additional
system will be required to accommodate the extra heat pump units.
2. Plants. No plant needs to be defined for this type of equipment. All equipment energy use is accounted for
in air system calculations.
3. Building. Link the WSHP, GWSHP or GSHP air system to the building.
Note: WSHP, GWSHP and GSHP systems are good candidates for the reduction techniques discussed in
the Energy Analysis Strategies topic. If these techniques are used it important to use a "lumping" technique
to reduce the number of heat pump units modeled rather than modeling single "typical" units.
Example: A hotel is being studied which has 30 identical WSHP zones on the south face of the building, 25
identical WSHP zones on the north face of the building and 28 WSHP zones which are unique. In this
situation it may be best to still define one air system so all 83 heat pump units can be connected to a
common water loop. The first 28 zones in the system could represent the WSHP zones which are unique.
Zone 29 would represent a combination of the 30 identical WSHP units in south facing rooms. This means
the full load capacity and input power for this WSHP unit would be the sum for the 30 identical units. Also,
the space multiplier for this zone would be 30. Finally, zone 30 would represent a combination of the 25
identical WSHP units in north facing rooms. Its space multiplier would be 25. The lumped capacity and the
space multipliers must be used to account for the total cooling and heating loads imposed by the spaces.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Ground Water and Ground Source Heat Pump Systems
This topic explains how to model ground water source heat pump (GWSHP) and Ground Source Heat Pump
(GSHP) systems in energy simulations. These systems consist of a number of heat pump units connected to a
water loop. In a GWSHP system source water is drawn from a well, river or lake. In a GSHP system the heat
source/sink is a vertical borehole well or a horizontal buried heat exchanger.
The modeling procedures for these types of equipment are nearly identical to those described in section 6.10.
The exception is that instead of modeling a cooling tower and auxiliary boiler, the heat source/sink is modeled
using the "river / sea / well water" option in which average source water temperatures are defined for each
month of the year. Auxiliary heat is assumed to be electric.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Chilled Water Plants
This topic explains how to model chilled water plants in energy simulations. The program simulates three types
of chilled water plants:
a. In a chiller plant, a group of one or more chillers operate to provide chilled water to cooling coils in one or
more air handling unit or fan coil systems.
Page 11 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Hot Water and Steam Plants
6.0 Energy Analysis Applications ››
b. In a changeover plant, reversible air-to-water (A2W) or water-to-water (W2W) chillers provide chilled
water and hot water to 2-pipe coils in air handlers or fan coils.
c. In a remote chilled water system, chilled water is supplied to air systems from an external source, such
as a district cooling system.
Modeling procedures are described below.
1. Air Systems. Define one or more air systems containing chilled water cooling coils using the procedures
described in the previous application topics.
2. Plants. Define a chilled water plant or a changeover plant serving these air systems. Modeling tips:
a. Specify the Plant Type as "Chiller Plant", "Changeover Plant" or "Remote Chilled Water".
b. Chillers and cooling towers (if used) can be created while you are entering the plant via the "create
new..." options or can be defined prior to entering data for a chiller plant.
c. If steam absorption chillers are used, users have a choice of modeling a boiler to generate steam for the
chillers, or using steam from a remote source such as waste steam. When using a boiler, it can be
created while you are entering the plant via the "create new boiler" option or it can be defined prior to
entering data for the chiller plant.
d. Use the Systems tab in the Plant window to link the plant to the set of air systems in the building which
use chilled water cooling coils. The plant will serve the combined load of all these cooling coils. A
changeover plant will also serve the hot water coil loads for these systems.
e. For chiller plants and changeover plants, use the Configuration tab in the Plant window to define the
configuration and control of the plant. Use the Schedule of Equipment tab to link the necessary chillers,
cooling towers and boilers to the plant.
f. For any of the plant types use the Distribution Tab to define characteristics of the water distribution
system and its pumps.
g. If you define a chiller or a remote chilled water plant, you will need to define a separate hot water or
steam plant if heating is provided from those sources. If you define a changeover plant, then that single
plant will provide for both the cooling and heating needs of the air systems.
h. If reversible chillers are used, it may be necessary to provide a source of auxiliary heat. Options for
describing and controlling auxiliary heat are provided on the Configuration tab. The source of auxiliary
heat is specified on the Schedule of Equipment tab and can be a hot water boiler or remote source hot
water.
3. Building. Link the plant to the building. This will include its energy use in energy cost calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Hot Water and Steam Plants
This topic explains how to model hot water and steam plants in energy simulations. The program simulates
four types of heating plants:
a. In a Hot Water plant, boilers, air-to-water (A2W) or water-to-water (W2W) heat pumps or a combination of
these equipment types provide hot water to one or more air handling unit or fan coil systems.
b. In a Remote Hot Water plant, hot water is supplied to air system coils from an external source, such a
district heating system.
c. In a Steam Boiler plant, steam boilers supply steam to coils in one or more air systems.
d. In a Remote Steam plant, steam is supplied to air system coils from an external source, such as a district
steam system.
Modeling procedures are described below.
Page 12 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
Simulating Heat Recovery Plants
6.0 Energy Analysis Applications ››
1. Air Systems. Define one or more air systems containing hot water or steam heating coils using the
procedures described in the previous sections.
2. Plants. Define a heating plant serving these air systems. Modeling tips:
a. For hot water, specify the Plant Type as "Hot Water Plant" or "Remote Hot Water".
b. For steam, specify the Plant Type as "Steam Boiler Plant" or "Remote Steam".
c. Boilers and A2W or W2W heat pumps can be defined at the same time you create the plant using the
"create new ..." option in the equipment drop-down list, or can be defined prior to entering the plant.
d. Use the Systems tab in the Plant window to link the plant to the set of air systems in the building which
use hot water heating coils or steam coils. The plant will serve the combined load of all these heating
coils. A changeover plant will also supply the combined chilled water coil loads for these systems.
e. Use the Configuration tab in the Plant window to define the number of boilers or heat pumps in the plant,
the method of control and, for hot water plants, the method of hot water supply temperature control.
f. For hot water plants use the Distribution tab to define characteristics of the hot water distribution system
and its pumps.
g. For steam plants use the Distribution tab to define the pipe heat loss factor.
h. If heat pumps are used, it may be necessary to provide a source of auxiliary heat. Options for defining
and controlling auxiliary heat are provided on the Configuration tab. The source of auxiliary heat is
specified on the Schedule of Equipment tab and can be a hot water boiler or remote source hot water.
3. Building. Link the heating plant to the building. This will include its energy use in energy cost calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulating Heat Recovery Plants
This topic explains how to model heat recovery plants in energy simulations. The program offers heat
recovery plants using six types of heat recovery schemes:
a. Dedicated heat recovery chiller (DHRC) in parallel with cooling only chillers.
b. Air-cooled chillers with water-cooled heat recovery condensers.
c. Heat exchanger in condenser water loop.
d. Dedicated heat recovery chiller (DHRC) in condenser loop.
e. Air-cooled or water-cooled chillers with desuperheaters
f. Double-bundle chillers.
Modeling procedures are described below.
1. Air Systems. Define one or more air systems containing chilled water cooling coils and/or hot water heating
coils using the procedures described in the previous application topics.
2. Plants. Define a "heat recovery" type of plant serving these air systems. A "heat recovery" plant is a
special type of plant in HAP which combines all of the equipment for the chilled water plant, hot water plant
and heat recovery equipment into one. Modeling tips:
a. Specify the Plant Type as "Heat Recovery Plant" on the General Tab in the Plant Properties window.
b. Use the Systems tab in the Plant window to link the plant to a set of air systems which use chilled water
cooling and/or hot water heating coils.
c. Use the Service Hot Water tab to define service water heating loads and equipment, if applicable.
d. Use the Configuration tab to define the number of chillers and boilers in the plant, the methods of control
for the cooling and heating equipment, and the type of heat recovery used.
Page 13 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm
e. On the Schedule of Equipment tab choose or create the chillers, boilers and heat recovery units included
in the plant. When linking heat recovery equipment, it must match the type of heat recovery specified.
For example, if you specified "Double-Bundle Chiller" heat recovery, then at least one of the chillers
selected must specify that double-bundle heat recovery is present in the chiller.
f. On the Distribution tab, specify the configurations for the chilled water and hot water distribution loops and
the performance of the pumps.
g. On the Source Water tab specify the configuration, controls and performance of pumps in the condenser
water loop.
3. Building. Link the heat recovery plant to the building. When building energy use and energy cost are
calculated, the calculations will include energy use by this plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 14 of 14
6.0 Energy Analysis Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh29A3.htm