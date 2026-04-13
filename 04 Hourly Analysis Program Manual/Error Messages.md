32.0 Error Messages
32.1 Calculation Error Messages
32.0 Error Messages ››
Calculation Error Report
32.0 Error Messages ›› 32.1 Calculation Error Messages ››
This chapter explains causes and corrective action for program error messages.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains error messages generated during calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Calculation Error Report
The Calculation Error Report lists problems found with input data for buildings, plants, systems or spaces. These problems prevent calculations from being
performed and therefore prevent the reports you selected from being generated.
When you choose to print or view reports, HAP first determines whether data required for the reports already exists. If it does, the reports are generated
immediately. If the required data does not exist, HAP will automatically run calculations to supply the needed data. Once calculations have been completed, the
reports will be generated. Before running calculations, HAP checks all the data required for the calculations. If errors are found in this data, the calculation
procedure halts. Errors must be corrected before calculations can proceed and the requested reports can be generated.
When errors are found, a message appears asking if you wish to generate a report listing the errors. Press the Yes button to generate the report. A sample of this
report is shown below.
The Calculation Error Report consists of one table. Each row in the table describes one error condition found in your data. Separate columns in the table
provide details about the error. Columns are as follows:
1. Type indicates whether the error involves a building, a plant, an air system or a space.
2. Name lists the name of the building, plant, air system or space which contains the error. In the sample above, the first error item is for an air system whose
name is "Central Station AHU".
3. # lists the error number. A list of all calculation errors is provided later in this help topic. This list is arranged by error number. Therefore, the error number can
be used to quickly locate information about the error and how to correct it.
4. Description provides a brief description of the error.
Example: The sample error report shown above indicates that the space whose name is "Northeast Office" contains two errors. Both the schedules for occupant
heat gains and for overhead lighting are missing. To correct these errors, edit the "Northeast Office" space and make sure valid schedules are specified for both
people and overhead lighting.
List of Errors. A complete list of building, plant, system and space error numbers and descriptions is provided below. The list is arranged according to error
number. To obtain further information about an error message, click on the desired item below.
Building Errors
4: Plant included in this building is missing.
5: System included in this building is missing.
6: Misc. energy schedule is missing.
7: Misc. energy schedule is not a fractional schedule.
8-15: Utility rate is missing.
16-23: TOD schedule for utility rate is missing.
Page 1 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
24-31: TOD schedule for utility rate is not valid.
32: Chilled water coils in an air system have no source of chilled water.
33: Multipliers for chilled water coils are inconsistent.
34: Hot water coils in an air system have no source of hot water.
35: Multipliers for hot water coils are inconsistent.
36: Steam coils for an air system have no source of steam.
37: Multipliers for steam coils are inconsistent.
38: Building does not contain any air systems.
Plant Errors
104: System included in this plant is missing.
105: Chiller or heat pump included in this plant is missing.
106: Cooling tower included in this plant is missing.
107: Boiler included in this plant is missing.
108: Chiller or heat pump mismatched with plant. Plant uses "autosize capacity" option
109: Chiller or heat pump mismatched with plant. Plant uses "user defined capacity" option
110: Boiler mismatched with plant. Plant uses "autosize capacity" option
111: Boiler mismatched with plant. Plant uses "user defined capacity" option
112: Generic type of plant cannot be used in energy simulations.
113: Chiller with mismatched equipment function included in plant.
120: Service hot water usage schedule included in this plant is missing
121: Service hot water usage schedule is not a fractional schedule
122: Service hot water resupply schedule included in this plant is missing
123: Service hot water resupply schedule is not a fan/thermostat schedule
130: Shared steam source included in this plant is missing
131: Auxiliary boiler included in this plant is missing.
132: Shared water source for this plant is not geo., surface, or well water
133: Dedicated heat recovery chiller is not a water source heat pump
134: Heat recovery plant requires at least one chiller with heat recovery features.
135: Heat recovery plant includes a chiller with incorrect heat recovery features.
136: Heat recovery plant includes heat rejection which is a geo/well/surface water type.
140: An air-cooled chiller plant with free cooling requires a shared cooling tower.
System Errors
204: Zone contains no spaces.
205: Space included in zone is missing.
206: Ventilation schedule is missing.
207: Ventilation schedule is not a fractional schedule.
208: Thermostat schedule is missing.
209: Thermostat schedule is not a Fan/Thermostat type of schedule.
210: Cooling tower included in this system is missing.
211: Boiler included in this system is missing.
212: System with `Undefined' equipment type cannot be used in energy simulations.
213: Wrong heat rejection equipment used with WSHP system.
214: Simulation weather data is missing.
215: OA Requirement Not Compatible with 62.1 Ventilation Rate Procedure
Space Errors
304: People schedule is missing.
305: People schedule is not a fractional schedule.
306: Overhead lighting schedule is missing.
307: Overhead lighting schedule is not a fractional schedule.
308: Task lighting schedule is missing.
309: Task lighting schedule is not a fractional schedule.
310: Electric equipment schedule is missing.
311: Electric equipment schedule is not a fractional schedule.
312: Miscellaneous sensible heat gain schedule is missing.
313: Miscellaneous sensible heat gain schedule is not a fractional schedule.
314: Miscellaneous latent heat gain schedule is missing.
315: Miscellaneous latent heat gain schedule is not a fractional schedule.
Page 2 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
32.1.1 Building Errors
32.0 Error Messages ›› 32.1 Calculation Error Messages ››
Error 4: Plant Included in this Building is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 5: System Included in this Building is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 6: Misc. Energy Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 7: Misc. Energy Schedule is not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Errors 8-15: Utility Rate is Missing
316: Wall type is missing for wall exposure.
317: Window type is missing for wall exposure.
318: Shade type is missing for window in wall exposure.
319: Door type is missing for wall exposure.
320: Roof type is missing for roof exposure.
321: Skylight type is missing for roof exposure.
322: Window and door area exceed gross area for wall exposure
323: Skylight area exceeds gross area for roof exposure
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors for building simulations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 4: Plant Included in this Building is Missing
Description: One of the plants linked to this building no longer exists. This error typically this occurs when a plant is deleted after it has been linked to a building.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the building and make sure the correct plants are linked to the building. Then save the building and run calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 5: System Included in this Building is Missing
Description: One of the systems linked to this building no longer exists. This error typically this occurs when a system is deleted after it has been linked to a
building.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the building and make sure the correct systems are linked to the building. Then save the building and run calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 6: Misc. Energy Schedule is Missing
Description: The fractional schedule used for one of the Miscellaneous Energy items in the building no longer exists. This error typically occurs when a schedule
is deleted after it has been linked to the building.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the building and make sure a schedule is specified for each Miscellaneous Energy item. Then save the building and run calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 7: Misc. Energy Schedule is not a Fractional Schedule
Description: The schedule used for one of the Miscellaneous Energy items in the building is not a "fractional" type of schedule. In this application, a "fractional"
schedule defines the percentage of energy in use each hour. This error typically occurs when the schedule is edited and changed to a different type of schedule
after it has been linked to the building.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Check the schedules used for Miscellaneous Energy items in the building and verify that each is a "fractional" type of schedule. The schedule
type is listed on the "Schedule Type" tab in the schedule form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 3 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Errors 16-23: TOD Schedule for Utility Rate is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Errors 24-31: TOD Schedule for Utility Rate is Not Valid
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 32: Chilled Water Coils have no Source of Chilled Water
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 33: Multipliers for Chilled Water Coils are Inconsistent
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Errors 8-15: Utility Rate is Missing
Description: The utility rate used for electric service or one of the fuel sources in the building no longer exists. The error message will indicate which of the rates
is missing:
Error 8: Utility rate for electric meter is missing.
This error typically occurs when a utility rate is deleted after it has been linked to the building.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the building and make sure a valid utility rates are specified for the electric meter and all fuel sources used in the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Errors 16-23: TOD Schedule for Utility Rate is Missing
Description: The time-of-day schedule used by one of the utility rates linked to the building no longer exists. The error message will indicate which of the utility
rates is missing a time-of-day schedule:
Error 16: TOD schedule for electric meter is missing.
This error typically occurs when a time-of-day schedule for a utility rate is deleted after the utility rate was defined.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the utility rate indicated in the error message and make sure a valid time-of-day schedule is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Errors 24-31: TOD Schedule for Utility Rate is Not Valid
Description: The schedule used to define time-of-day periods for one of the utility rates linked to the building is no longer a "time-of-day" type of schedule and
therefore cannot be used. The error message will indicate which of the utility rates is faulty:
Error 24: TOD schedule for electric meter is not valid.
This error typically occurs when a time-of-day schedule for a utility rate is modified after the utility rate was defined so that it is a "fractional" or "fan/thermostat"
type of schedule instead of a time-of-day schedule.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the utility rate indicated in the error message and make sure a valid time-of-day schedule is specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 32: Chilled Water Coils have no Source of Chilled Water
Description: An air system linked to the building contains chilled water cooling coils, but a chilled water plant has not been defined to serve these coils. When an
air system with chilled water cooling coils is defined, it must be linked to a chilled water plant so chilled water can be supplied to the coils. Both the chilled water
plant and the air system must be linked to the building. This error can occur for several reasons including:
1. The air system with chilled water cooling coils was linked to the building, but the chilled water plant was not linked to the building. The solution is to include both
the plant and the system in the building.
2. No chilled water plant has been defined. The solution is to define a chilled water plant serving all air systems in the building having chilled water coils.
3. A chilled water plant was defined, but it was not linked to one of the air systems containing chilled water coils. The solution is to edit the plant and link it to the
missing air systems.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Verify that all air systems with chilled water cooling coils are linked to a chilled water plant and that chilled water plant is included in the
building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 33: Multipliers for Chilled Water Coils are Inconsistent
Description: This error occurs when connections between plants and an air system using chilled water cooling are inconsistent. This problem is best illustrated
with an example:
Example: Air system AHU-1 is linked to a chiller plant using a system multiplier of 2. This means there are are two AHU-1 air systems which have identical
characteristics and both are served by the chiller plant. Air system AHU-1 is also linked to a hot water boiler plant using a system multiplier of 3. Both the chiller
Page 4 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 34: Hot Water Coils have no Source of Hot Water
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 35: Multipliers for Hot Water Coils are Inconsistent
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 36: Steam Coils have no Source of Steam
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
plant and hot water boiler plant are linked to a building. The connections between the plants and the AHU-1 system are inconsistent. The chiller plant indicates
that loads and energy use of AHU-1 should be counted 2 times in building energy calculations. The boiler plant indicates loads and energy use for AHU-1 should
be counted 3 times.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Print input data for the building and the plants it contains. Inspect these reports to determine how plants and systems are linked together.
Tabulate the linkage data to quickly identify problems. For the scenario described above, this tabulation would appear as follows:
System Name
Multiplier Used With
Chilled Water Plant
Multiplier Used With
Hot Water Plant
Multiplier Used With
Steam Plant
AHU-1
2
3
not applicable
Once you’ve tabulated the air system multipliers, inspect each row in the table. Any air system whose multipliers differ will cause this error. Linkages between the
system and its plants should then be revised to make the multipliers consistent.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 34: Hot Water Coils have no Source of Hot Water
Description: An air system linked to the building contains hot water heating coils, but a hot water plant has not been defined to serve these coils. When an air
system with hot water heating coils is defined, it must be linked to a hot water plant so hot water can be supplied to the coils. Both the hot water plant and the air
system must be linked to the building. This error can occur for several reasons including:
1. The air system with hot water coils was linked to the building, but the hot water plant was not linked to the building. The solution is to include both the plant and
the system in the building.
2. No hot water plant has been defined. The solution is to define a hot water plant serving all air systems in the building having hot water heating coils.
3. A hot water plant was defined, but it was not linked to one of the air systems containing hot water heating coils. The solution is to edit the plant and link it to the
missing air systems.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Verify that all air systems with hot water heating coils are linked to a hot water plant and that hot water plant is included in the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 35: Multipliers for Hot Water Coils are Inconsistent
Description: This error occurs when connections between plants and an air system using hot water heating are inconsistent. This problem is best illustrated with
an example:
Example: Air system AHU-1 is linked to a chiller plant using a system multiplier of 2. This means there are are two AHU-1 air systems which have identical
characteristics and both are served by the chiller plant. Air system AHU-1 is also linked to a hot water boiler plant using a system multiplier of 3. Both the chiller
plant and hot water boiler plant are linked to a building. The connections between the plants and the AHU-1 system are inconsistent. The chiller plant indicates
that loads and energy use of AHU-1 should be counted 2 times in building energy calculations. The boiler plant indicates loads and energy use for AHU-1 should
be counted 3 times.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Print input data for the building and the plants it contains. Inspect these reports to determine how plants and systems are linked together.
Tabulate the linkage data to quickly identify problems. For the scenario described above, this tabulation would appear as follows:
System Name
Multiplier Used With
Chilled Water Plant
Multiplier Used With
Hot Water Plant
Multiplier Used With
Steam Plant
AHU-1
2
3
not applicable
Once you’ve tabulated the air system multipliers, inspect each row in the table. Any air system whose multipliers differ will cause this error. Linkages between the
system and its plants should then be revised to make the multipliers consistent.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 36: Steam Coils have no Source of Steam
Description: An air system linked to the building contains steam heating coils, but a steam plant has not been defined to serve these coils. When an air system
with steam heating coils is defined, it must be linked to a steam plant so steam can be supplied to the coils. Both the steam plant and the air system must be
linked to the building. This error can occur for several reasons including:
1. The air system with steam coils was linked to the building, but the steam plant was not linked to the building. The solution is to include both the plant and the
system in the building.
2. No steam plant has been defined. The solution is to define a steam plant serving all air systems in the building having steam heating coils.
3. A steam plant was defined, but it was not linked to one of the air systems containing steam heating coils. The solution is to edit the plant and link it to the
missing air systems.
Severity: Building calculations cannot be performed until the error is corrected.
Page 5 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 37: Multipliers for Steam Coils are Inconsistent
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
Error 38: Building Does Not Contain Any Air Systems
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.1 Building Errors ››
32.1.2 Plant Errors
32.0 Error Messages ›› 32.1 Calculation Error Messages ››
Error 104: System Included in This Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 105: Chiller or Heat Pump Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Suggested Action: Verify that all air systems with steam heating coils are linked to a steam plant and that steam plant is included in the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 37: Multipliers for Steam Coils are Inconsistent
Description: This error occurs when connections between plants and an air system using steam heating are inconsistent. This problem is best illustrated with an
example:
Example: Air system AHU-1 is linked to a chiller plant using a system multiplier of 2. This means there are are two AHU-1 air systems which have identical
characteristics and both are served by the chiller plant. Air system AHU-1 is also linked to a steam boiler plant using a system multiplier of 4. Both the chiller plant
and steam boiler plant are linked to a building. The connections between the plants and the AHU-1 system are inconsistent. The chiller plant indicates that loads
and energy use of AHU-1 should be counted 2 times in building energy calculations. The boiler plant indicates loads and energy use for AHU-1 should be counted
4 times.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Print input data for the building and the plants it contains. Inspect these reports to determine how plants and systems are linked together.
Tabulate the linkage data to quickly identify problems. For the scenario described above, this tabulation would appear as follows:
System Name
Multiplier Used With
Chilled Water Plant
Multiplier Used With
Hot Water Plant
Multiplier Used With
Steam Plant
AHU-1
2
not applicable
4
Once you’ve tabulated the air system multipliers, inspect each row in the table. Any air system whose multipliers differ will cause this error. Linkages between the
system and its plants should then be revised to make the multipliers consistent.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 38: Building Does Not Contain Any Air Systems
Description: This error typically occurs when a building is entered and saved, and then all air systems linked to the building are deleted. The program requires
that the building contain at least one air system.
Severity: Building calculations cannot be performed until the error is corrected.
Suggested Action: Edit the building and link one or more air systems to the building. Then save the building and rerun the energy simulation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors for plant simulations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 104: System Included in This Plant is Missing
Description: One of the air systems linked to this plant no longer exists. This error typically this occurs when an air system is deleted after it has been linked to a
plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit and save the plant. When data for the plant is read so it can be edited, links to air systems that no longer exist are deleted. When you
save the plant all invalid links to air systems will be eliminated. You can then run plant calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 105: Chiller or Heat Pump Included in this Plant is Missing
Description: One of the chillers or heat pumps linked to this plant no longer exists. This error typically occurs when a chiller or heat pump is deleted after it has
been linked to a plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and make sure a complete set of chillers or heat pumps has been specified on the "Schedule of Equipment" tab.
Page 6 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 106: Cooling Tower Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 107: Boiler Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 108: Chiller or Heat Pump Mismatched with Plant. Plant uses Autosize Capacity Option...
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 109: Chiller or Heat Pump Mismatched with Plant. Plant uses User-Defined Capacity Option...
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 110: Boiler Mismatched with Plant. Plant Uses Autosize Capacity Option
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 111: Boiler Mismatched with Plant. Plant Uses User Defined Capacity Option...
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 106: Cooling Tower Included in this Plant is Missing
Description: One of the cooling towers linked to this plant no longer exists. This error typically occurs when a cooling tower is deleted after it has been linked to a
plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and make sure cooling towers have been specified for all water-cooled chillers on the "Schedule of Equipment" tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 107: Boiler Included in this Plant is Missing
Description: A boiler linked to this plant no longer exists. This error typically occurs when a boiler is deleted after it has been linked to a plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and make sure a valid boiler has been linked to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 108: Chiller or Heat Pump Mismatched with Plant. Plant uses Autosize Capacity Option...
Description: A plant uses the "Autosize Capacity" option but one or more chillers or heat pumps linked to the plant are specified with "User-Defined Capacity"
rather than "Autosize Capacity". When the plant was first input the plant and its equipment were synchronized - both the plant and the chiller or heat pump
specified "Autosize Capacity". Later, the chiller or heat pump was edited and changed to specify "User-Defined Capacity". This makes the equipment
incompatible with the plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit each chiller or heat pump linked to this plant and place a check in the "Autosize" box on the Design Inputs tab. Then save the
equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 109: Chiller or Heat Pump Mismatched with Plant. Plant uses User-Defined Capacity Option...
Description: A plant uses the "User-Defined Capacities" option but one or more chillers or heat pumps linked to the plant are specified with "Autosize
Capacity"rather than "User Defined Capacity". When the plant was first input the plant and its equipment were synchronized - both the plant and the chillers or
heat pumps specified "User Defined Capacities". Later, the chiller or heat pump was edited and changed to specify "Autosize Capacity". This makes the
equipment incompatible with the plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit each chiller or heat pump linked to this plant and remove the check mark in the "Autosize" box on the Design Inputs tab. Then save the
equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 110: Boiler Mismatched with Plant. Plant Uses Autosize Capacity Option
Description: A plant uses the "Autosize Capacity" option but a boiler linked to the plant is specified with "User-Defined Capacity" rather than "Autosize Capacity".
When the plant was first input the plant and boiler were synchronized - both the plant and the boiler specified "Autosize Capacity". Later, the boiler was edited and
changed to specify "User-Defined Capacity". This makes the boiler incompatible with the plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the boiler linked to this plant and place a check in the "Autosize" box. Then save the boiler.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 112: Generic Type of Plant cannot be used in Energy Simulations
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 113
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 120: Service Hot Water Usage Schedule Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 121: Service Hot Water Usage Schedule Included in this Plant is not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 111: Boiler Mismatched with Plant. Plant Uses User Defined Capacity Option...
Description: A plant uses the "User-Defined Capacities" option but the boiler linked to the plant is specified with "Autosize Capacity"rather than "User Defined
Capacity". When the plant was first input the plant and the boiler were synchronized - both the plant and boiler specified "User Defined Capacities". Later, the
boiler was edited and changed to specify "Autosize Capacity". This makes the boiler incompatible with the plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the boiler linked to this plant and remove the check mark in the "Autosize" box on the Design Inputs tab. Then save the boiler.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 112: Generic Type of Plant cannot be used in Energy Simulations
Description: One of the plants you selected is a "Generic" type of plant. This plant can be used to generate design reports, but not for energy simulation reports.
Generic plants only contain sufficient information for a plant design calculation. They do not contain the equipment configuration, performance and control
information necessary to run energy simulation calculations.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: You can either remove the Generic plants from the set of plants you selected for energy simulation reports, or you can modify the plant to
change it from "Generic" to one of the specific plant types. Once the plant type has been changed and the extra configuration, performance and control data has
been entered, the plant can be used in energy simulations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 113
Chiller with mismatched equipment function included in plant
Description: A chiller or heat recovery plant is created, chillers are attached to the plant and the plant is saved. Later the chiller data is edited separately and the
chiller equipment function is changed from “chiller (chilled water only)” to a different value such as “heat pump (hot water only)” or “reversible (chilled and hot
water)”. Neither heat pumps nor reversible equipment are valid for use in a chiller or heat recovery plant.
This error can also occur for a hot water plant including air-to-water or water-to-water heat pumps which are later edited and changed to be a chiller or a
reversible chiller.
This error can also occur for a changeover plant including air-to-water or water-to-water reversible chillers which are later edited and changed to be a chiller or a
dedicated heat pump.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and re-select valid equipment to link to the plant. A chiller or heat recovery plant requires chillers. A hot water plant requires
boilers or heat pumps. A changeover plant requires reversible chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 120: Service Hot Water Usage Schedule Included in this Plant is Missing
Description: In a Service Hot Water (SHW) plant the hot water usage schedule defines how hot water flow rate requirements vary hour by hour. A fractional
schedule is linked to the plant to define the hot water usage pattern. This error occurs when the schedule linked to the plant is later deleted.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a hot water usage schedule.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 121: Service Hot Water Usage Schedule Included in this Plant is not a Fractional Schedule
Description: In a Service Hot Water (SHW) plant the hot water usage schedule defines how hot water flow rate requirements vary hour by hour. A fractional
schedule is linked to the plant to define the hot water usage pattern. This error occurs when the schedule linked to the plant is later changed so it is no longer a
fractional schedule. As a different schedule type (such as fan/thermostat or utility rate time of day) the schedule no longer provides usable data or calculating hot
water requirements.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a valid fractional schedule to define hot water usage.
Page 8 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 122: Service Hot Water Resupply Schedule Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 123: Service Hot Water Resupply Schedule is not a Fan/Thermostat Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 130: Shared Steam Source Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 131: Auxiliary Boiler Included in this Plant is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 132: Shared Water Source for this Plant is not Geo., Surface, or Well Water
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 122: Service Hot Water Resupply Schedule Included in this Plant is Missing
Description: In a hot water plant that serves both space heating loads and service hot water (SHW) loads, controls can be specified to prioritize when the plant
serves space heating or SHW needs, if insufficient capacity exists to serve all loads. One priorization option uses a fan/thermostat schedule to identify
"unoccupied" HVAC operating periods as the time to give resuppy of the hot water storage tank priority over space heating loads. This error occurs when the
fan/thermostat schedule linked to the plant for prioritization control has been deleted.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a valid fan/thermostat schedule for the prioritization control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 123: Service Hot Water Resupply Schedule is not a Fan/Thermostat Schedule
Description: In a hot water plant that serves both space heating loads and service hot water (SHW) loads, controls can be specified to prioritize when the plant
serves space heating or SHW needs, if insufficient capacity exists to serve all loads. One priorization option uses a fan/thermostat schedule to identify
"unoccupied" HVAC operating periods as the time to give resuppy of the hot water storage tank priority over space heating loads. This error occurs when the
fan/thermostat schedule linked to the plant for prioritization control is later changed to a different type of schedule. When the schedule is a fractional or utility rate
time of day schedule, it cannot supply the information needed to simulate prioritization control.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a valid fan/thermostat schedule for the prioritization control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 130: Shared Steam Source Included in this Plant is Missing
Description: Chiller plants which use steam-driven absorption chillers or steam-driven vapor-compression chillers require specification of a shared steam source.
This can be remote source steam or a steam boiler. This error occurs when the steam boiler linked to the plant as the shared steam source has been deleted
and is therefore not available for calculations.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a different steam source for the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 131: Auxiliary Boiler Included in this Plant is Missing
Description: Changeover plants and hot water plants using air-to-water or water-to-water heat pumps can include auxiliary heating equipment for times when the
heat pump does not have enough capacity to meet the heating demand. One option for the source of auxiliary heating is a hot water boiler. This error occurs
when the hot water boiler linked to the plant as the auxiliary heater has been deleted. It is therefore not available for use in calculations.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a different source of auxiliary heat.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 133
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 134
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 135
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 132: Shared Water Source for this Plant is not Geo., Surface, or Well Water
Description: A changeover plant or a hot water plant using water-to-water heat pumps requires that a heat source/sink be specified. This is referred to as the
"shared water source". It is specified by choosing from items in the cooling tower library which have type "geo, surface, or well water". These items represent a
geothermal well field, a surface water source such as a lake, or a water well field. This error occurs when the shared water source is changed to a different type
of heat sink, such as a cooling tower or dry cooler. In that form, the heat rejection system cannot be used for calculation of water-to-water heat pump
performance.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and select a valid "geo., surface, or well water" item as the shared water source for the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 133
Dedicated heat recovery chiller is not a water-source heat pump
Description: A heat recovery plant has been defined with heat recovery method specified as “Dedicated heat recovery chiller in parallel with cooling only chillers”
or “Dedicated heat recovery chiller in condenser loop”. A water-to-water (W2W) heat pump is created and linked to the plant to serve as the dedicated heat
recovery chiller (DHRC). Sometime after the plant is saved the W2W heat pump is separately edited and its equipment function is changed to “chiller (chilled
water only)” or “reversible (chilled and hot water)”, or, its type is changed to an air-to-water heat pump. Once this change is made, the equipment is no longer
suitable to function as the DHRC unit in the heat recovery plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and re-select a valid W2W heat pump as the DHRC unit in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 134
Heat recovery plant requires at least one chiller with heat recovery features
Description: A heat recovery plant has been defined with heat recovery method specified as “Chillers with double-bundle condenser”, “Chillers with
desuperheater” or “Chillers with heat recovery condensers”. At least one chiller with the required heat recovery equipment was linked to the plant before it was
saved. Later, this chiller was edited and the heat recovery equipment was removed. Therefore, the plant now contains cooling-only chillers without any heat
recovery capability. The plant cannot perform any heat recovery.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and re-select a valid chiller with heat recovery equipment that matches the heat recovery method specified. Specifically:
1. For “Chillers with double bundle condensers” at least one chiller with a double-bundle condenser must be linked to the plant.
2. For “Chillers with desuperheaters” at least one chiller with desuperheater equipment must be linked to the plant.
3. For “Chillers with heat recovery condensers” at least one air-cooled chiller with a heat recovery condenser specified must be linked to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 135
Heat recovery plant includes a chiller with incorrect heat recovery features
Description: A heat recovery plant has been defined with heat recovery method specified as “Chillers with double-bundle chillers”, “Chillers with desuperheaters”
or “Chillers with heat recovery condensers”. At least one chiller with the required heat recovery equipment was linked to the plant before it was saved. Later, this
chiller was edited and the heat recovery equipment was changed to a different type. For example, the plant uses “Chillers with desuperheaters” and the chiller
containing the desuperheater was edited and changed to have a heat recovery condenser instead of a desuperheater. The chiller’s heat recovery equipment is
now mismatched with the plant. The plant, as specified, cannot operate correctly with this type of heat recovery.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and re-select a valid chiller with heat recovery equipment that matches the heat recovery method specified. Specifically:
1. For “Chillers with double bundle condensers” at least one chiller with a double-bundle condenser must be linked to the plant.
2. For “Chillers with desuperheaters” at least one chiller with a desuperheater equipment must be linked to the plant.
3. For “Chillers with heat recovery condensers” at least one air-cooled chiller with a heat recovery condenser specified must be linked to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 10 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 136
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
Error 140
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.2 Plant Errors ››
32.1.3 System Errors
32.0 Error Messages ›› 32.1 Calculation Error Messages ››
Error 204: Zone Contains No Spaces
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 205: Space Included in Zone is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 206: Ventilation Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 136
Heat recovery plant includes heat rejection which is a geo./well/surface water type. Only cooling towers or dry coolers are
allowed.
Description: A heat recovery plant has been defined including water-cooled cooling-only chillers. Cooling towers or dry coolers were linked to the plant and the
plant was saved. Later the cooling tower or dry cooler data was edited separately and was changed to a “geo/well/surface water” heat rejection system. Once
this change is made, the equipment is no longer suitable to function as a part of a heat recovery plant.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant and re-select cooling towers or dry coolers for the water-cooled chillers in the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 140
An air-cooled chiller plant with free cooling requires a “shared” cooling tower
Description: A chiller plant was defined to model air-cooled chillers with a cooling tower or dry cooler providing waterside economizer free cooling. To model this
type of plant the cooling tower configuration must be specified as “one cooling tower shared by all water-cooled chillers”. Instead, cooling tower configuration was
specified as “one cooling tower for each water-cooled chiller”.
Severity: Plant calculations cannot be performed until the error is corrected.
Suggested Action: Edit the plant. On the Configuration tab specify the cooling tower configuration as “one cooling tower shared by all water-cooled chillers”. On
the Schedule of Equipment tab specify a “shared cooling tower”. Save the plant and run the simulation again.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors for air system simulations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 204: Zone Contains No Spaces
Description: One or more of the zones in this air system contain no spaces. When defining an air system, each zone must contain at least one space.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit this air system and inspect space assignments for all zones in the system. Space assignments are found in the "Space Assignments"
data view on the "Zone Components" tab. Make sure that each zone contains at least one space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 205: Space Included in Zone is Missing
Description: A space assigned to one of the zones in this air system no longer exists. This typically happens when you delete spaces after defining an air
system, and one of the spaces you deleted was assigned to a zone in your system.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit and save the air system. When data for the system is read so it can be edited, links to spaces that no longer exist are deleted. When you
save the system all invalid links to spaces will be eliminated. You can then run system calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 206: Ventilation Schedule is Missing
Page 11 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 207: Ventilation Schedule is not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 208: Thermostat Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 209: Thermostat Schedule is not a Fan/Thermostat Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 210: Cooling Tower Included in this System is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 211: Boiler Included in this System is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Description: The fractional schedule specified for outdoor ventilation airflow control in this air system no longer exists. When you choose the "scheduled" option
for controlling outdoor ventilation air, a schedule must be selected from your project database to define the hourly variation of ventilation airflow. This error
typically occurs when the schedule you chose is deleted after the air system is defined.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the air system and specify a valid schedule for ventilation airflow control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 207: Ventilation Schedule is not a Fractional Schedule
Description: The schedule specified for outdoor ventilation airflow control in this air system is not a fractional schedule. When you choose the "scheduled" option
for controlling outdoor ventilation air, a schedule must be selected from your project database to define the hourly variation of ventilation airflow. The schedule
you select must be a "fractional" schedule meaning define the percentage of maximum ventilation airflow that occurs each hour.
If the schedule you select is a "Fan/Thermostat" schedule or a "Utility Rate Time-of-Day" type of schedule, it will not contain percentage data and therefore cannot
be used for scheduling ventilation airflow. Fan/Thermostat schedules designate each hour as belonging to the "occupied" or "unoccupied" thermostat period.
Utility Rate Time-of-Day schedules designate each hour as belonging to the various peak, mid-peak and off-peak pricing periods for electricity.
This error typically occurs when you first assign a fractional schedule for ventilation airflow control and later edit the schedule data, changing the schedule type
from Fractional to Fan/Thermostat or Utility Rate Time-Of-Day.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the air system and specify a fractional schedule for ventilation airflow control.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 208: Thermostat Schedule is Missing
Description: The thermostat schedule you specified for this air system no longer exists. This error typically occurs when the thermostat schedule you assigned to
the air system is deleted after the air system is defined.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the air system data and specify a valid thermostat schedule.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 209: Thermostat Schedule is not a Fan/Thermostat Schedule
Description: The thermostat schedule specified for this air system is not the correct type. It must be a "Fan/Thermostat" type of schedule which designates each
hour as belonging to the occupied or unoccupied thermostat periods. Instead, a Fractional schedule has been used (which specifies hourly percentage values) or
a Utility Rate Time-Of-Day schedule has been used (which designates hours as belonging to the peak and off-peak pricing periods for electricity).
This error typically occurs when you first choose a Fan/Thermostat schedule for your air system, but later edit the schedule data, changing the schedule type from
Fan/Thermostat to either Fractional or Utility Rate Time-Of-Day.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the air system and specify a valid Fan/Thermostat schedule.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 210: Cooling Tower Included in this System is Missing
Description: The cooling tower linked to this system no longer exists. This error typically occurs when a cooling tower is deleted after it has been linked to a
system.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the system and make sure a valid cooling tower has been specified. When editing system data, the cooling tower specification is found
by going to the Equipment tab and pressing the "Miscellaneous Equipment" button.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 211: Boiler Included in this System is Missing
Description: The boiler linked to this system no longer exists. This error typically occurs when a boiler is deleted after it has been linked to a system.
Page 12 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 212: System with Undefined Equipment Type cannot be used in Energy Simulations
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 213: Wrong Heat Rejection Equipment used with WSHP System
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 214: Simulation Weather Data is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Error 215: OA Requirement Not Compatible with 62.1 Ventilation Rate Procedure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.3 System Errors ››
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the system and make sure a valid boiler has been specified. When editing system data, the boiler specification is found by going to the
Equipment tab and pressing the "Miscellaneous Equipment" button.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 212: System with Undefined Equipment Type cannot be used in Energy Simulations
Description: One of the systems you selected uses the "Undefined" equipment type. This system can be used to generate design reports, but not for energy
simulation reports. Systems in the "Undefined" equipment class only contain sufficient information for a system design calculation. They do not contain the cooling
and heating source information or equipment performance information necessary to run energy simulation calculations.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: You can either remove the systems having "Undefined" equipment type from the set of systems you selected for energy simulation reports,
or you can modify the system to change it from "Undefined" to a specific equipment type. Once the system uses a specific equipment type, and cooling source,
heating source and equipment performance data has been entered, the system can be used in energy simulations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 213: Wrong Heat Rejection Equipment used with WSHP System
Description: This error occurs in two situations:
1. A WSHP system is defined and the heat rejection equipment specified is "Geo / Well / Surface Water". A closed loop WSHP system must use a mechanical
cooling tower. The "Geo / Well / Surface Water" option cannot be used for this type of system.
2. The GSHP or GWSHP system is defined and the heat rejection equipment specified is a cooling tower. GSHP and GWSHP systems must use the "Geo / Well /
Surface Water"" option for heat rejection. A cooling tower cannot be used with this type of system.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Edit the WSHP air system. Go to the Equipment Tab and press the "Edit Equipment Data" button opposite "Miscellaneous Components".
Then select the proper type of heat rejection equipment. As noted above, a closed loop system must use a cooling tower. An open loop system must use the
"river, sea or well water".
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 214: Simulation Weather Data is Missing
Description: This error occurs when you attempt to generate simulation reports but have not yet added simulation weather data to your project. Simulation
weather data is required for all system and plant simulations and is therefore an essential component of the project data.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Use the following steps to correct this problem:
1. Edit your weather data.
2. Click on the Simulation tab.
3. On the Simulation tab press the "Change City" button to add simulation weather data to your project.
4. Choose the simulation weather data you wish to use for your project. Each file names indicates the content of the file. For example
USA\_ILLINOIS\_CHICAGO.HW1 contains simulation weather data for Chicago.
5. After adding simulation weather to your project, save the weather data and then request your energy simulation reports again.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 215: OA Requirement Not Compatible with 62.1 Ventilation Rate Procedure
Description: This error occurs when an air system specifies the ventilation sizing method as one of the ASHRAE Standard 62.1 methods (2004, 2007, 2010,
2013) and one or more of the spaces served by the system define outdoor air ventilation requirements in terms of CFM, L/s or % of supply air.
The ASHRAE Standard 62.1 sizing methods use the Ventilation Rate Procedure from the Standard to determine outdoor ventilation airflow. The Ventilation Rate
Procedure requires that space ventilation requirements be defined in terms of CFM/person and/or CFM/sqft (L/s/person and/or L/s/sqm). When a space
ventilation requirement is defined in terms of CFM, L/s or % of supply airflow, it cannot be used in the Ventilation Rate Procedure and is therefore incompatible
with the ventilation sizing method you selected.
Severity: System calculations cannot be performed until the error is corrected.
Suggested Action: Use the following steps to correct this problem:
Page 13 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
32.1.4 Space Errors
32.0 Error Messages ›› 32.1 Calculation Error Messages ››
Error 304: People Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 305: People Schedule is Not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 306: Overhead Lighting Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 307: Overhead Lighting Schedule is Not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
1. Edit the space whose name is listed in the error message and change its OA ventilation requirements to use units of CFM/person and/or CFM/sqft (L/s/person
and/or L/s/sqm).
OR
2. Edit your air system and change the ventilation sizing method to "Sum of OA Airflows".
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains error messages for spaces that occur during calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 304: People Schedule is Missing
Description: The people schedule you specified for this space no longer exists. This error typically occurs when the people schedule is deleted after the space is
defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for people.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 305: People Schedule is Not a Fractional Schedule
Description: The people schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of people in the space.
This error typically occurs when you originally choose a fractional schedule to define the varying occupancy levels for the space, but later edit data for this
schedule and change its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for people.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 306: Overhead Lighting Schedule is Missing
Description: The overhead lighting schedule you specified for this space no longer exists. This error typically occurs when the schedule used for overhead
lighting is deleted after the space is defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for overhead lighting.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 307: Overhead Lighting Schedule is Not a Fractional Schedule
Description: The overhead lighting schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of overhead lighting in the space.
This error typically occurs when you originally choose a fractional schedule to define lighting levels in the space, but later edit data for this schedule and change
its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for overhead lighting.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 14 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 308: Task Lighting Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 309: Task Lighting Schedule is Not a Fractioinal Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 310: Electric Equipment Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 311: Electric Equipment Schedule is Not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 312: Miscellaneous Sensible Heat Gain Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 313: Miscellaneous Sensible Heat Gain Schedule is Not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 308: Task Lighting Schedule is Missing
Description: The task lighting schedule you specified for this space no longer exists. This error typically occurs when the schedule used for task lighting is
deleted after the space is defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for task lighting.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 309: Task Lighting Schedule is Not a Fractional Schedule
Description: The task lighting schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of task lighting in the space.
This error typically occurs when you originally choose a fractional schedule to define lighting levels in the space, but later edit data for this schedule and change
its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for task lighting.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 310: Electric Equipment Schedule is Missing
Description: The electric equipment schedule you specified for this space no longer exists. This error typically occurs when the schedule used for electric
equipment is deleted after the space is defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for electric equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 311: Electric Equipment Schedule is Not a Fractional Schedule
Description: The electric equipment schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of electric equipment heat gains in the space.
This error typically occurs when you originally choose a fractional schedule to define electric equipment heat gains in the space, but later edit data for this
schedule and change its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for electric equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 312: Miscellaneous Sensible Heat Gain Schedule is Missing
Description: The miscellaneous sensible heat gain schedule you specified for this space no longer exists. This error typically occurs when the schedule used for
miscellaneous sensible heat gains is deleted after the space is defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for miscellaneous sensible heat gains.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 15 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 314: Miscellaneous Latent Heat Gain Schedule is Missing
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 315: Miscellaneous Latent Heat Gain Schedule is Not a Fractional Schedule
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 316: Wall Type is Missing for Wall Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 317: Window Type is Missing for Wall Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 318: Shade Type is Missing for Window in Wall Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 313: Miscellaneous Sensible Heat Gain Schedule is Not a Fractional Schedule
Description: The miscellaneous sensible heat gain schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of miscellaneous sensible heat gains in the space.
This error typically occurs when you originally choose a fractional schedule to define miscellaneous sensible heat gains in the space, but later edit data for this
schedule and change its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for miscellaneous sensible heat gains.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 314: Miscellaneous Latent Heat Gain Schedule is Missing
Description: The miscellaneous latent heat gain schedule you specified for this space no longer exists. This error typically occurs when the schedule used for
miscellaneous latent heat gains is deleted after the space is defined.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and specify a valid schedule for miscellaneous latent heat gains.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 315: Miscellaneous Latent Heat Gain Schedule is Not a Fractional Schedule
Description: The miscellaneous latent heat gain schedule specified for this space is not a fractional schedule.
In HAP there are three types of schedules. Fractional schedules contain hourly percentage data. Fan/Thermostat schedules designate hours as belonging to the
occupied or unoccupied thermostat periods. Utility Rate Time-of-Day schedules designate hours as belonging to the various peak, mid-peak and off-peak pricing
periods for electricity. Fractional schedules must be used to define the hourly variation of miscellaneous latent heat gains in the space.
This error typically occurs when you originally choose a fractional schedule to define miscellaneous latent heat gains in the space, but later edit data for this
schedule and change its type from Fractional to Fan/Thermostat or Utility Rate Time-of-Day.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid fractional schedule for miscellaneous latent heat gains.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 316: Wall Type is Missing for Wall Exposure
Description: The wall assembly specified for one of the wall exposures in this space no longer exists. This error typically occurs when a wall assembly is deleted
after it has been linked to a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid wall assembly type for this wall exposure. The wall exposure number is listed in the error message. For
example, if the error message is "Wall type is missing for wall exposure 3", a valid wall assembly must be defined for the third wall exposure in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 317: Window Type is Missing for Wall Exposure
Description: A window assembly specified for one of the wall exposures in this space no longer exists. This error typically occurs when a window assembly is
deleted after it has been linked to a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid window assembly for this wall exposure. The wall exposure number is listed in the error message. For
example, if the error message is "Window type is missing for wall exposure 4", a valid window assembly must be defined for the fourth wall exposure in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 16 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 319: Door Type is Missing for Wall Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 320: Roof Type is Missing for Roof Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 321: Skylight Type is Missing for Roof Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 322: Window and Door Area Exceeds Gross Area for Wall Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 323: Skylight Area Exceeds Gross Area for Roof Exposure
32.0 Error Messages ›› 32.1 Calculation Error Messages ›› 32.1.4 Space Errors ››
Error 318: Shade Type is Missing for Window in Wall Exposure
Description: An external shade type that was assigned to one of the windows in this space no longer exists. This error typically occurs when an external shading
geometry is deleted after it has already been linked to windows in a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid external shade type for windows on this wall exposure. The wall exposure number and window number are
listed in the error message. For example, if the error message is "Shade type is missing for window 2 in wall exposure 3", a valid shade type must be defined for
the window #2 in the third wall exposure in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 319: Door Type is Missing for Wall Exposure
Description: A door assembly specified for one of the wall exposures in this space no longer exists. This error typically occurs when a door assembly is deleted
after it has been linked to a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid door assembly for this wall exposure. The wall exposure number is listed in the error message. For
example, if the error message is "Door type is missing for wall exposure 5", a valid door assembly must be defined for the fifth wall exposure in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 320: Roof Type is Missing for Roof Exposure
Description: The roof assembly specified for one of the roof exposures in this space no longer exists. This error typically occurs when a roof assembly is deleted
after it has been linked to a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid roof assembly type for this roof exposure. The roof exposure number is listed in the error message. For
example, if the error message is "Roof type is missing for roof exposure 2", a valid roof assembly must be defined for the second roof exposure in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 321: Skylight Type is Missing for Roof Exposure
Description: A skylight assembly specified for one of the roof exposures in this space no longer exists. This error typically occurs when a skylight assembly is
deleted after it has been linked to a space.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: Edit the space and choose a valid skylight assembly for this roof exposure. The roof exposure number is listed in the error message. For
example, if the error message is "Skylight type is missing for roof exposure 2", a valid skylight assembly must be defined for the second roof exposure in the
space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 322: Window and Door Area Exceeds Gross Area for Wall Exposure
Description: This error occurs when the sum of window and door area for a wall exposure is larger than the gross area specified for the wall. The error message
will indicate which of the wall exposures in this space is in error.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: The error can be corrected in several ways:
1. By increasing the gross area for the wall exposure so it equals or exceeds the total window plus door area.
2. By reducing the quantity of windows and doors specified for this exposure.
3. By adjusting the window dimensions or door area so the sum of window and door areas is equal to or less than the gross wall area.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 323: Skylight Area Exceeds Gross Area for Roof Exposure
Page 17 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
32.2 Plant Input Error Messages
32.0 Error Messages ››
Plant Input Errors
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 400
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 401
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Description: This error occurs when the total skylight area for a roof exposure exceeds the gross area for the roof. The error message will indicate which of the
roof exposures in this space is in error.
Severity: Calculations cannot be performed until the error is corrected.
Suggested Action: The error can be corrected in several ways:
1. By increasing the gross area for the roof exposure so it equals or exceeds the total skylight area.
2. By reducing the quantity of skylights specified for this exposure.
3. By adjusting the skylight dimensions so the total skylight area is equal to or less than the gross roof area.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors occurring when saving plant input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Plant Input Errors
When the OK button on the Plant form is pressed to save input data, the program checks the inputs prior to saving them. If any problems with the data are found,
the program will display a message explaining the error. Input errors must be corrected before saving the data. For further information on a plant input error, click
on one of the items below.
Plant Error 400 - No Systems Linked to Plant
Plant Error 401 - Cooling Tower not Assigned to a Water-Cooled Chiller
Plant Error 402 - Shared Cooling Tower not Assigned for Water-Cooled Chillers
Plant Error 403 - Absorption Steam Source not Assigned for Absorption Chillers
Plant Error 405 - Schedule of Equipment Incomplete
Plant Error 406 - Evaporator Flow Rate and Water Source Flow Rate Do Not Match
Plant Error 407 - Water Source Not Assigned for Water Source Heat Pump
Plant Error 408 - Heat Source / Heat Rejector Not Assigned for Water Source Reversible Chiller
Plant Error 409 - Missing Shared Auxiliary Heat Source
Plant Error 410 - Missing Shared Water Source
Plant Error 411 - Water Source Flow Rate Must Equal Maximum Source-Side Flow Rate
Plant Error 412 - Changeover Plant Requires at least one Chilled Water Coil and at least one Hot Water Coil
Plant Error 421 - Schedule Which Indicates Service Hot Water Consumption Has Not Been Specified
Plant Error 422 - The Schedule for Unoccupied Service Hot Water Resupply Has Not Been Specified
Plant Error 424 - The Water-Source Flow Rate Units Do Not Match the Heating and Cooling Source-Side Flow Rate Units
Plant Error 454 - Condenser Flow Rate and Tower Flow Rate Do Not Match
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 400
No Systems Linked to Plant
Description: This error occurs when no air systems were linked to the plant. All plants other than a standalone service hot water plant must serve at least one air
system. For example a chiller plant must serve chilled water cooling coils in one or more air systems.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct the error, go to the Systems tab and specify air systems served by this plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 401
Cooling Tower not Assigned to a Water-Cooled Chiller
Page 18 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 402
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 403
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 405
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 406
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Description: This error occurs when a water-cooled chiller was specified on the Schedule of Equipment tab, but no cooling tower was specified for that chiller.
This applies to chiller plants using the "One Tower for Each Water-Cooled Chiller" configuration option. In these plants, a cooling tower must be specified for each
water-cooled chiller in the plant.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct the error, go to the Schedule of Equipment tab and make sure a cooling tower has been selected for each water-cooled chiller in
the schedule table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 402
Shared Cooling Tower not Assigned for Water-Cooled Chillers
Description: This error occurs when no shared cooling tower was specified on the Schedule of Equipment tab. This applies to chiller plants using the "One Tower
Shared by all Water-Cooled Chillers" configuration option. In these plants a cooling tower must be selected in the "Shared Tower" item in the lower right portion of
the tab.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct the error, go to the Schedule of Equipment tab and make sure a shared cooling tower has been selected in the lower right portion
of the tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 403
Absorption Steam Source Not Assigned for Absorption Chillers
Description: This error occurs when a chiller plant includes steam absorption chillers, but a shared steam source has not been specified. To be complete the
plant must have a shared steam source specified.
Severity: The plant cannot be saved until the problem is corrected.
Suggested Action:
1. Go to the Schedule of Equipment tab and specify a shared steam source in the lower left quadrant of the tab. This can be remote source steam or a steam
boiler..
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 405
Schedule of Equipment Incomplete
Description: This error occurs when one or more rows in the schedule of equipment table is empty meaning an equipment unit has not been specified. This
could involve a missing chiller, reversible chiller, boiler or heat pump. Or it could involve a missing assignment for heat rejection equipment.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error, go to the Schedule of Equipment tab and make sure each row in the schedule has equipment assigned.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 406
Evaporator Flow Rate and Water Source Flow Rate Do Not Match
Description: This error occurs in hot water or service hot water plants using a water-to-water heat pumps when the total source side water flow rate for the heat
pumps does not match the flow rate specified for the shared water source.
Example: The heat pumps use a flow specification of 10 F delta-T. The shared water source uses a flow specification of 15 F delta-T. The error occurs because
the flow specifications must match.
When flow units are delta-T, the flow specifications must match exactly. When flow specifications are gpm or L/s, the flows must match within 20 gpm or 1.25 L/s.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error, either choose different equipment which does have matching flow specifications, or modify the heat pump and water
source inputs to adjust flows to match.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 19 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 407
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 408
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 409
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 410
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 411
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 407
Water Source Not Assigned for Water Source Heat Pump
Description: This error applies to hot water plants using water-to-water heat pumps. In this type of plant a shared water source (geo well field, surface water or
well water) must be specified on the Schedule of Equipment tab. This error occurs when no water source is specified..
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error, go to the Schedule of Equipment Tab and specify a shared water source. This input is found in the lower left quadrant
of the tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 408
Heat source / Heat Rejector Not Assigned for a Water Source Reversible Chiller
Description: This error applies to changeover plants using water source reversible chillers. In this type of plant a shared water source (geo well field, surface
water or well water) must be specified on the Schedule of Equipment tab. This error occurs when no water source is specified..
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error, go to the Schedule of Equipment Tab and specify a shared water source. This input is found in the lower left quadrant
of the tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 409
Missing Shared Auxiliary Heat Source
Description: This error applies to changeover plants and to hot water plants using air-to-water or water-to-water heat pumps. If auxiliary heating is specified on
the Configuration tab for these plants, a shared auxiliary heater must also be specified on the Schedule of Equipment tab. This error occurs when a shared
auxiliary heater is not specified.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error, specify a shared auxiliary heater on the Schedule of Equipment tab. This input is found in the lower left quadrant of the
tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 410
Missing Shared Water Source
Description: This error can occur in a changeover plant that uses water-to-water reversible chillers, or in a hot water plant that uses water-to-water heat pumps.
In either situation a shared water source such as a geo well field, surface water or well water must be specified as the heat source and sink for the water source
equipment. This error occurs when no water source is specified.
Severity: Plant input data cannot be saved until the problem is corrected.
Suggested Action:
1. Go to the Schedule of Equipment tab and specify a shared water source in the lower left quadrant of the tab. You can select an existing geo well field, surface
water or well water source from the drop-down list, or you can use the  option to create a water source and link it to the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 411
Page 20 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 412
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 421
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 422
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Water Source Flow Rate Must Equal Maximum Source Side Flow Rate
Description: This error applies to changeover plants using water source reversible chillers. The error occurs when the total source side flow rate for the
reversible chillers does not match the flow rate for the shared water source.
Example: The sum of source side cooling flow rates for the chillers is 600 gpm. The sum of source side heating flow rates is 400 gpm. The shared water source
has a flow rate of 750 gpm. Because the water source flow rate (750 gpm) does not match the larger of reversible chiller supply side cooling or heating flow rates
(600 gpm), this error occurs.
When flow rates are specified as gpm or L/s the program requires flows to match within 20 gpm or 1.25 L/s. When flow rates is specified as delta-T, the flow
specifications must match exactly (for example 10 F matches with 10 F).
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error either select different equipment that has matching flows, or adjust the inputs for the selected reversible chillers or
shared water source so the flow specifications match.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 412
Changeover Plant Requires at least one Chilled Water Coil and at least one Hot Water Coil
Description: This error when the loads linked to a changeover plant only include cooling loads or only include heating loads. This can happen in two situations:
1. All air systems linked to the plant are cooling only and no service hot water loads are specified, or
2. All air systems linked to the plant are heating only.
Neither situation is allowed since by definition a changeover plant is designed to serve a cooling and heating loads.
Severity: Plant input data cannot be saved until the problem is corrected.
Suggested Action: There are several possible solutions to this problem:
1. If you intended this to be a cooling and heating changeover plant, link different air systems to the plant which have cooling and heating loads, or revise the
linked air systems to add cooling or heating capability. Service water heating can also be added to the plant.
2. If the building only has cooling loads, define the plant as a "Chiller Plant" instead of a "Changeover Plant".
3. If the building only has heating loads, define the plant as a "Hot Water Plant" or "Service Hot Water Plant", as applicable.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 421
Schedule Which Indicates Service Hot Water Consumption Has Not Been Specified
Description: If a plant serves service hot water (SHW) loads and the SHW inputs define consumption in terms of gpm (L/s) or load (KBTU/day or kWh/day), a
fractional schedule must be specified to define how SHW requirements change hour by hour. This error occurs when such a schedule has not been specified.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error go to the Service Hot Water tab and select a schedule in the Consumption section in the upper left quadrant of the tab..
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 422
Schedule for Unoccupied Service Hot Water Resupply Has Not Been Specified
Description: In a plant which serves both space heating loads and service hot water (SHW) loads, there is an option to specify priority for recharging the SHW
storage tank based on a schedule. With this option, space heating loads have first priority during "occupied" fan/thermostat operating hours and SHW loads have
first priority during "unoccupied" fan/thermostat operating hours. This error occurs when no fan/thermostat schedule has been specified for the resupply priority
control.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error go to the Service Hot Water tab and select a schedule in the Stored Hot Water section of the tab, in the lower right.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 21 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 424
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
Error 454
32.0 Error Messages ›› 32.2 Plant Input Error Messages ››
32.3 Utility Rate Input Error Messages
32.0 Error Messages ››
Utility Rate Input Errors
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 424
Water Source Flow Units Do Not Match the Heating and Cooling Source-Side Flow Units
Description: This error applies to changeover plants using water source reversible chillers. The error occurs when the units of measure for the shared water
source flow rate are different from the units of measure for source side flow for the reversible chillers..
Example: The units of measure for shared water source flow are delta-T (F or K). The units of measure for the source-side cooling and heating flow rates for the
reversible chillers in the plant are gpm (or L/s). The error occurs because different units are used..
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: To correct this error either select different equipment that has matching flow units, or adjust the inputs for the selected reversible chillers or
shared water source so the flow units match.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 454
Condenser Flow Rate and Tower Flow Rate Do Not Match
Description: This applies to chiller plants including water-cooled chillers. The flow rates for a chiller and its corresponding heat rejection equipment must match.
This error occurs when flow rates do not match.
Example: A water cooled chiller has a condenser flow rate of 750 gpm. The cooling tower linked to the chiller has a water flow rate of 900 gpm. The error occurs
because the flows do not match.
When flow is specified as gpm (or L/s) the program only requires that flows match to within 20 gpm or 1.25 L/s. When flow is specified in terms of delta-T (F or K)
or in terms of flow per unit capacity (gpm/ton or L/s/kW), then flow specifications must match exactly.
Severity: This is a warning error. Data containing this error can be saved, but we recommend correcting the flow mismatch before running simulation
calculations..
Suggested Action: To correct this error, either choose different chiller or heat rejection equipment that does have matching flows, or edit the selected equipment
and adjust flow rates so they do match.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors occurring when saving utility rate input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Utility Rate Input Errors
When the OK button on the Electric Rate or Fuel Rate forms is pressed to save input data, the program checks the inputs prior to saving them. If any problems
with the data are found, the program will display a message explaining the error. Input errors must be corrected before saving the data.
There are several rules that need to be observed when entering utility rate data so the program can properly interpret and use the data in calculations. Errors
occur when these rules are not observed. Links to explanations of the various utility rate error messages are provided below.
Note: If you are encountering a large number of errors when trying to save utility rate data, it may be helpful to review the basic rules for entering data and the
utility rate application topic.
Error 500: Name for utility rate is missing.
Error 501: No energy charge was specified.
Error 502: No fuel charge was specified.
Error 503: No time-of-day schedule was specified.
Error 504: Demand prices not specified for the following.
Error 505: Energy prices need to be specified for the following.
Error 506: Overlap found in energy charge items.
Error 507: Overlap found in fuel charge items.
Error 508: Overlap found in demand charge items.
Error 509: Unbilled energy use.
Error 510: Unbilled fuel use.
Error 511: Unbilled demand levels.
Page 22 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 500: Name for Utility Rate is Missing
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 501: No Energy Charge was Specified
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 502: No Fuel Charge was Specified
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 503: No Time-of-Day Schedule was Specified
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 512: Energy charge item is out of sequence.
Error 513: Fuel charge item is out of sequence.
Error 514: Demand charge item is out of sequence.
Error 515: Steps within a demand series must have the same demand clause ID.
Error 516: Compound block charge has energy steps not assigned to a demand block.
Error 517: Compound block charge has demand blocks out of sequence.
Error 518: Compound block charge must have at least one energy step per demand block.
Error 519: Last energy step in a demand block must be 9999999
Error 520: Season/Period for all steps in a demand block must be the same.
Error 521: Compound block charge has fewer than 2 demand blocks.
Error 522: Demand blocks do not cover all levels of demand.
Error 523: Season+Period combination in energy charge is not valid
Error 524: Season+Period combination in demand charge is not valid.
Error 525: Season+Period combination in demand multiplier clause is not valid.
Error 526: Season+Period combination in fuel charge is not valid.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 500: Name for Utility Rate is Missing
Description: A name for the electric rate or fuel rate you are entering was not specified. A name must be defined for each rate you create.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the General tab and enter a name for the rate.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 501: No Energy Charge was Specified
Description: This error occurs when you are defining a complex rate and no energy charge was defined. At least one step must be defined for the energy charge
in all electric rates.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and make sure at least one step is selected for the charge. Steps are selected by marking the check box on
the left end of each row in the table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 502: No Fuel Charge was Specified
Description: This error occurs when you are defining a complex rate and no fuel charge was defined. At least one step must be defined for the fuel charge in all
fuel rates.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Fuel Charge tab and make sure at least one step is selected for the charge. Steps are selected by marking the check box on
the left end of each row in the table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 503: No Time-of-Day Schedule was Specified
Description: This error occurs when you elected to use time-of-day scheduling but did not choose a time-of-day schedule. When you check the box for time-of-
day scheduling you must also choose a schedule in the schedule drop-down list. This schedule defines the hours in each of the time of day pricing periods (e.g.,
on-peak, off-peak times).
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the General tab and select a time-of-day schedule from the drop-down list. If no time-of-day schedules exist, one can be created by
pressing the Schedule button or by choosing  in the drop-down list. This will launch the Schedule form and allow you to enter data. On the
schedule form, be sure to specify the schedule type as "time of day utility rate".
Page 23 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 504: Demand Prices Not Specified For ...
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 505: Prices Need to Be Specified for ...
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 506: Overlap Found in Energy Charge Items
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 507: Overlap Found in Fuel Charge Items
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 504: Demand Prices Not Specified For ...
Description: This warning error occurs when demand prices have not been specified for all time periods during the year. For example, if Peak and Off-Peak time-
of-day periods were specified, but demand prices were only specified for Peak times, this error message will appear. The error message will indicate times when
prices are missing:
Error 504: Demand prices not specified for Winter/Off-Peak
It is acceptable for demand prices to be defined for certain times of day or times of year and not others. It is very common for demand prices to apply only to
certain time-of-day periods or seasons. Therefore, this is simply a warning message. Users should make sure the condition is intended. If it was intended, you
can continue and save the data without making changes.
Severity: This is a warning error. Data may be saved without making changes, if desired.
Suggested Action: If changes must be made, return to the Demand Charge tab and enter data for the missing time-of-day and/or season times.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 505: Prices Need to Be Specified for ...
Description: This error occurs when energy prices in an electric rate do not cover all time periods. It also occurs when fuel prices in a fuel rate do not cover all
time periods. One of the rules for entering utility rate data is that energy or fuel charges must cover all time periods during the year.
Example: A utility rate uses Peak and Off-Peak time-of-day periods. Energy prices were specified for the Peak times but not the Off-Peak times. Therefore energy
use during Off-Peak times is unbilled and this is not allowed.
The error message will indicate the season and time-of-day period for which energy or fuel prices are missing:
Error 505: Prices need to be specified for Summer/Off-Peak
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: For an electric rate, return to the Energy Charge tab and make sure energy prices have been specified covering all times of year. For a fuel
rate, return to the Fuel Charge tab and check for the same condition. In both cases you will need to focus on the season and period specifications for each step in
the charge.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 506: Overlap Found in Energy Charge Items
Description: This error occurs when electric energy prices are assigned to the same quantity of energy use for the same time period two or more times. This
normally happens when:
1. One step defines a price for energy use during a specific season and/or time-of-day period.
2. Another step defines a price for energy use for the "All" season or "All" period. The "All" step overlaps with the step defining energy prices for the specific
season or time-of-day period.
For example, the following two steps in an energy charge will cause this error.
Season
Period
Block Size
Block Units
Price
Summer
Peak
9999999
kWh
0.0408
All
All
9999999
kWh
0.0655
One of the rules for entering utility rates is that energy use can only be billed once, so overlapping conditions are not allowed. There are situations where a utility
defines the energy charge in separate components, such as separate generation, transmission and distribution charges. For these situations, the separate
charges must be combined before entering them into the program.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and check for overlapping conditions such as the one shown above. Revise energy charge data to eliminate
these conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 507: Overlap Found in Fuel Charge Items
Description: This error occurs when fuel prices are assigned to the same quantity of fuel use for the same period of time two or more times. This normally
happens when:
1. One step defines a price for fuel use during a specific season and/or time-of-day period.
Page 24 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 508: Overlap Found in Demand Charge Items
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 509: Unbilled Energy Use
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
2. Another step defines a price for fuel use for the "All" season or "All" period. The "All" step overlaps with the step defining fuel prices for the specific season or
time-of-day period.
For example, the following two steps in an fuel charge will cause this error.
Season
Period
Block Size
Block Units
Price
Winter
Peak
9999999
Therms
0.3254
All
All
9999999
Therms
0.1687
One of the rules for entering utility rates is that fuel use can only be billed once, so overlapping conditions are not allowed. There are situations where a utility
defines the fuel charge in separate components, such as separate commodity and distribution charges. For these situations, the separate charges must be
combined before entering them into the program.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Fuel Charge tab and check for overlapping conditions such as the one shown above. Revise fuel charge data to eliminate these
conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 508: Overlap Found in Demand Charge Items
Description: This warning error occurs when demand prices are assigned to the same quantity of demand for the same time period two or more times. This error
can occur for both electric and fuel demand charges. This normally happens when:
1. One step defines a price for demand during a specific season and/or time-of-day period.
2. Another step defines a price for demand for the "All" season or "All" period. The "All" step overlaps with the step defining demand prices for the specific season
or time-of-day period.
For example, the following two steps in an electric demand charge will cause this error.
Season
Period
Block Size
Price
Summer
Peak
9999999 kW
8.4600
All
All
9999999 kW
3.2500
Some rate schedules contain a "non-time-related" or "NTR" demand charge. For example one demand charge applies to demands measured only during the
summer peak period. A second demand charge is not related to time-of-day or seasons and applies to the maximum demand measured during any hour of the
day.
If your rate schedule contains such overlapping demand charges, then this error message can be ignored. If your rate schedule does not include an NTR demand
charge, you should stop at this point and check your demand charge inputs before saving the data.
Severity: This is a warning error. Data may be saved without making changes, if desired.
Suggested Action: If changes must be made, return to the Demand Charges tab and remove the overlapping demand charge.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 509: Unbilled Energy Use
Description: This error occurs when a stepped energy charge structure does not specify prices for all quantities of energy use. This is typically due to one of the
following:
1. The last in a series of related steps does not specify the block size as 9999999. The quantity "9999999" is used by the program to designate "all remaining
energy use". The following example illustrates this problem. In order for the last step in the series to cover all remaining energy use, its block size must be
"9999999" instead of "100000".
Season
Period
Block Size
Price
All
All
20000 kWh
0.12530
All
All
70000 kWh
0.09436
All
All
100000 kWh
0.07456
2. Steps in a related series of steps are not placed in consecutive rows of the energy charge table. One of the rules for entering utility rate data is that related
steps must be consecutive. The following example illustrates this problem. Because the three Summer/All steps in the charge are not consecutive, the input
data is ambiguous and could be interpreted as missing energy use above 90000 kWh for the Summer season.
Season
Period
Block Size
Price
Summer
All
20000 kWh
0.12530
Summer
All
70000 kWh
0.09436
Winter
All
9999999 kWh
0.08823
Summer
All
9999999 kWh
0.07456
Severity: Input data cannot be saved until this error is corrected.
Page 25 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 510: Unbilled Fuel Use
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 511: Unbilled Demand Levels
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 512: Energy Charge Item is Out of Sequence
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Suggested Action: Return to the Energy Charge tab and inspect data for the two problems described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 510: Unbilled Fuel Use
Description: This error occurs when a stepped fuel charge structure does not specify prices for all quantities of fuel use. This is typically due to one of the
following:
1. The last in a series of related steps does not specify the block size as 9999999. The quantity "9999999" is used by the program to designate "all remaining fuel
use". The following example illustrates this problem. In order for the last step in the series to cover all remaining fuel use, its block size must be "9999999"
instead of "1000".
Season
Period
Block Size
Price
All
All
200 THM
0.7524
All
All
700 THM
0.4487
All
All
1000 THM
0.3814
2. Steps in a related series of steps are not placed in consecutive rows of the fuel charge table. One of the rules for entering utility rate data is that related steps
must be consecutive. The following example illustrates this problem. Because the three Winter/All steps in the charge are not consecutive, the input data is
ambiguous and could be interpreted as missing fuel use above 900 Therms for the Winter season.
Season
Period
Block Size
Price
Winter
All
200 THM
0.7524
Winter
All
700 THM
0.4487
Summer
All
9999999 THM
0.5106
Winter
All
9999999 THM
0.3814
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Fuel Charge tab and inspect data for the two problems described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 511: Unbilled Demand Levels
Description: This error occurs when a stepped demand charge structure does not specify prices for all quantities of demand. This is typically due to one of the
following:
1. The last in a series of related steps does not specify the block size as 9999999. The quantity "9999999" is used by the program to designate "all remaining
demand". The following example illustrates this problem for an electric demand charge. In order for the last step in the series to cover all remaining demand, its
block size must be "9999999" instead of "1000".
Season
Period
Block Size
Price
All
All
100 kW
14.85
All
All
500 kW
10.05
All
All
1000 kW
8.35
2. Steps in a related series of steps are not placed in consecutive rows of the demand charge table. One of the rules for entering utility rate data is that related
steps must be consecutive. The following example illustrates this problem for an electric demand charge. Because the three Summer/All steps in the charge
are not consecutive, the input data is ambiguous and could be interpreted as missing energy use above 600 kW for the Summer season.
Season
Period
Block Size
Price
Summer
All
100 kW
14.85
Summer
All
500 kW
10.05
Winter
All
9999999 kW
7.75
Summer
All
9999999 kW
8.35
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Demand Charge tab and inspect data for the two problems described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 26 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 513: Fuel Charge Item is Out of Sequence
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 514: Demand Charge Item is Out of Sequence
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 515: Steps Within a Demand Series Must Have the Same Demand Clause ID
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 516: Compound Block Charge Has Energy Steps Not Assigned to a Demand Block
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 512: Energy Charge Item is Out of Sequence
Description: This error occurs when related items in a stepped energy charge structure are not placed in consecutive rows of the energy charge table. One of
the rules for entering utility rate data is that related items in a stepped charge must be in consecutive rows of the table to avoid ambiguity. The following example
illustrates the problem. Because the three Summer/All steps in the charge are not consecutive, the input data is ambiguous and could be interpreted as missing
energy use above 90000 kWh for the Summer season.
Season
Period
Block Size
Price
Summer
All
20000 kWh
0.12530
Summer
All
70000 kWh
0.09436
Winter
All
9999999 kWh
0.08823
Summer
All
9999999 kWh
0.07456
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect data for the problem described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 513: Fuel Charge Item is Out of Sequence
Description: This error occurs when related items in a stepped fuel charge structure are not placed in consecutive rows of the fuel charge table. One of the rules
for entering utility rate data is that related items in a stepped charge must be in consecutive rows of the table to avoid ambiguity. The following example illustrates
the problem. Because the three Summer/All steps in the charge are not consecutive, the input data is ambiguous and could be interpreted as missing fuel use
above 900 Therms for the Winter season.
Season
Period
Block Size
Price
Winter
All
200 THM
0.7524
Winter
All
700 THM
0.4487
Summer
All
9999999 THM
0.5106
Winter
All
9999999 THM
0.3814
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Fuel Charge tab and inspect data for the problem described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 514: Demand Charge Item is Out of Sequence
Description: This error occurs when related items in a stepped demand charge structure are not placed in consecutive rows of the demand charge table. One of
the rules for entering utility rate data is that related items in a stepped charge must be in consecutive rows of the table to avoid ambiguity. The following example
illustrates the problem. Because the three Summer/All steps in the charge are not consecutive, the input data is ambiguous and could be interpreted as missing
demand above 600 kW for the Summer season.
Season
Period
Block Size
Price
Summer
All
100 kW
14.85
Summer
All
500 kW
10.05
Winter
All
9999999 kW
7.75
Summer
All
9999999 kW
8.35
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Demand Charge tab and inspect data for the problem described above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 515: Steps Within a Demand Series Must Have the Same Demand Clause ID
This error condition does not apply in the current version of HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 27 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 517: Compound Block Charge has Demand Blocks Out of Sequence
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 518: Compound Block Charge Must Have at Least One Energy Step Per Demand Block
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 516: Compound Block Charge Has Energy Steps Not Assigned to a Demand Block
Description: This error occurs when the first row in the energy charge table for a Compound Block energy charge is an "energy" step rather than a "demand"
step. This indicates that energy and demand steps are not arranged in the correct order. The step type for the first row in the charge must always be "demand".
The Compound Block charge is a two-tier structure. The first tier consists of a series of demand blocks having block units of kWh/kW. Each demand block is
subdivided into individual energy blocks. The following table shows the correct way to arrange blocks at the beginning of the charge table.
Step Type
Season
Period
Block Size
Price
Demand
All
All
150 kWh/kW
Energy
All
All
10000 kWh
0.08632
Energy
All
All
40000 kWh
0.07092
Energy
All
All
9999999 kWh
0.05338
The following example shows data that will generate this error. The first step in the table is an "energy" step rather than a "demand" step.
Step Type
Season
Period
Block Size
Price
Energy
All
All
10000 kWh
0.08632
Energy
All
All
40000 kWh
0.07092
Energy
All
All
9999999 kWh
0.05338
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and check the step type for the first row in the table. In some cases the "Step Type" input is overlooked so
the solution may only require changing the Step Type for the first row from "Energy" to "Demand". In other cases the first Demand step has been omitted and
must be added to the table.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 517: Compound Block Charge has Demand Blocks Out of Sequence
Description: This error occurs when demand blocks for a particular season and period in a Compound Block energy charge are not consecutive in the charge
table. One of the rules for entering Compound Block energy charges is that related demand blocks must be consecutive in the table. The following example
illustrates the problem. The demand block, and its associated energy steps for the Winter season must not appear in the middle of a series of demand and energy
steps for the Summer season.
Step Type
Season
Period
Block Size
Price
Demand
Summer
All
200 kWh/kW
Energy
Summer
All
30000 kWh
0.07092
Energy
Summer
All
9999999 kWh
0.05338
Demand
Winter
All
250 kWh/kW
Energy
Winter
All
40000 kWh
0.05889
Energy
Winter
All
9999999 kWh
0.04557
Demand
Summer
All
9999999 kWh/kW
Energy
Summer
All
9999999 kWh
0.03215
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data for Demand and Energy steps that are out of order, such as those shown in the
example above. Correct any problems that are found.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 518: Compound Block Charge Must Have at Least One Energy Step Per Demand Block
Description: This error occurs when a Demand block in a Compound Block energy charge contains no energy steps. A Compound Block energy charge is a two-
tier structure containing a series of demand blocks each subdivided into separate energy steps. One of the rules for defining a Compound Block charge is that
every demand block must have at least one energy step. The following example illustrates the problem. The second demand block contains no energy steps.
Step Type
Season
Period
Block Size
Price
Demand
Summer
All
200 kWh/kW
Energy
Summer
All
30000 kWh
0.07092
Energy
Summer
All
9999999 kWh
0.05338
Demand
Summer
All
250 kWh/kW
Demand
Summer
All
9999999 kWh/kW
Page 28 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 519: Last Energy Step in Demand Block must be 9999999
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 520: Season/Period for all Steps in Demand Block Must be the Same
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 521: Compound Block Charge has Fewer than 2 Demand Blocks
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Energy
Summer
All
9999999 kWh
0.03215
This error also occurs when the last row in the energy charge table has Step Type = "Demand".
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data for cases where two or more consecutive rows are designated as "Demand" blocks, or
the case where the final row in the table is a "Demand" block.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 519: Last Energy Step in Demand Block must be 9999999
Description: This error occurs when the final energy step in a demand block in a Compound Block energy charge does not have a block size of 9999999 kWh.
The program interprets the quantity "9999999" as meaning "all additional kWh". Therefore, if the last energy step in one of the demand blocks is not "9999999",
there may be quantities of energy not covered by the charge. One of the rules for defining energy charges is that prices must cover all quantities of energy use.
The following example illustrates the problem. If the 200 kWh/kW demand block covers more than 115,000 kWh during a particular month, then energy use above
115,000 kWh will not be billed. (The quantity 115,000 is sum of the 10,000, 30,000 and 75,000 kWh energy steps). Either the final energy step for a demand block
must be changed to 9999999 or additional energy steps must be inserted.
Step Type
Season
Period
Block Size
Price
Demand
All
All
200 kWh/kW
Energy
All
All
10000 kWh
0.07092
Energy
All
All
30000 kWh
0.05338
Energy
All
All
75000 kWh
0.03991
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data for the problem described above. Make sure the last energy step in each demand
block has a block size of 9999999 kWh.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 520: Season/Period for all Steps in Demand Block Must be the Same
Description: This error occurs when the energy steps within a demand block in a Compound Block energy charge use different season and/or time-of-day period
specifications than are used for the demand block.
A Compound Block energy charge is a two tier structure. It consists of a series of demand blocks each of which is subdivided into individual energy steps.
Because the demand block and its energy steps are related, the must all apply to the same season and time-of-day period.
The following example illustrates this problem. The second energy step in this demand block specifies the Winter season instead of the Summer season.
Therefore, it is not matched to its demand block and will cause Error 520 to occur.
Step Type
Season
Period
Block Size
Price
Demand
Summer
All
150 kWh/kW
Energy
Summer
All
10000 kWh
0.08632
Energy
Winter
All
40000 kWh
0.07092
Energy
Summer
All
9999999 kWh
0.05338
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data for the type of problem described above. Correct data so season and period
specifications for energy steps match the season and period for the related demand block.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 521: Compound Block Charge has Fewer than 2 Demand Blocks
Description: This error occurs when a Compound Block energy charge contains no demand blocks or only one demand block. Often this error occurs when a
user forgets to define the "step type" for each row in the table.
A Compound Block energy charge is a two tier structure. It consists of a series of demand blocks each of which is subdivided into individual energy steps. All
Compound Block energy charges contain at least two demand blocks, each containing one or more energy steps.
The following example illustrates the problem. All steps were inadvertently defined as "energy steps". Instead, the first, fourth and seventh rows in the table (those
having block units of kWh/kW) must be designated as "demand" steps rather than "energy" steps.
Step Type
Season
Period
Block Size
Price
Page 29 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 522: Demand Blocks do Not Cover All Levels of Demand
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 523: Season+Period Combination in Energy Charge is Not Valid
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 524: Season+Period Combination in Demand Charge is Not Valid
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Energy
All
All
200 kWh/kW
Energy
All
All
30000 kWh
0.07092
Energy
All
All
9999999 kWh
0.05338
Energy
All
All
250 kWh/kW
Energy
All
All
40000 kWh
0.05889
Energy
All
All
9999999 kWh
0.04557
Energy
All
All
500 kWh/kW
Energy
All
All
9999999 kWh
0.03215
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data. If the "step type" input was overlooked, it may be possible to resolve the error simply
by designating the proper row items as "demand" steps. In other cases it may be necessary to insert additional rows to define the demand blocks.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 522: Demand Blocks do Not Cover All Levels of Demand
Description: This error occurs when the final demand block in a series of related blocks in a Compound Block energy charge does not have a block size of
9999999. The program interprets the quantity "9999999" as meaning "all additional kWh/kW". Therefore, if the last demand block in a series of related blocks is
not "9999999", there may be quantities of energy not covered by the charge. One of the rules for defining energy charges is that prices must cover all quantities
of energy use.
The following example illustrates the problem. If energy use greater than 1250 kWh/kW exists for a month, this energy use will not be covered by the charge
structure. (The quantity 1250 kWh/kW is the sum of the 200, 250 and 500 kWh/kW demand blocks.) Either the final demand block size must be changed to
9999999 or additional demand blocks must be added.
Step Type
Season
Period
Block Size
Price
Demand
All
All
200 kWh/kW
Energy
All
All
30000 kWh
0.07092
Energy
All
All
9999999 kWh
0.05338
Demand
All
All
250 kWh/kW
Energy
All
All
40000 kWh
0.05889
Energy
All
All
9999999 kWh
0.04557
Demand
All
All
500 kWh/kW
Energy
All
All
9999999 kWh
0.03215
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Return to the Energy Charge tab and inspect the data for the problem described above. Make sure the last demand block in each related
group of blocks has a block size of 9999999 kWh/kW.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 523: Season+Period Combination in Energy Charge is Not Valid
Description: This error occurs when the combination of season and time-of-day period you selected for one of the rows in the energy charge table does not exist.
Your specification of seasons and your selection of a time-of-day schedule result in only certain combinations of season and period being valid. For example,
suppose you define Summer and Winter seasons. You also link a schedule which defines Peak, Mid-Peak and Off-Peak periods for the Summer months, but only
Peak and Off-Peak periods for Winter months. Therefore Mid-Peak is not used in the Winter. If you specify the combination of Winter + Mid-Peak for one of the
energy charge items, this error will occur.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Inspect your inputs for seasonal scheduling and for your time-of-day schedule to determine which combinations of season and time-of-day
period are valid. Then inspect data on the Energy Charge tab to identify and correct any season+period combinations that are not valid.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 524: Season+Period Combination in Demand Charge is Not Valid
Description: This error occurs when the combination of season and time-of-day period you selected for one of the rows in the demand charge table does not
exist.
Page 30 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 525: Season+Period Combination in Demand Multiplier Clause is Not Valid
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
Error 526: Season+Period Combination in Fuel Charge is Not Valid
32.0 Error Messages ›› 32.3 Utility Rate Input Error Messages ››
32.4 Chiller Input Error Messages
32.0 Error Messages ››
Chiller Input Errors
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Your specification of seasons and your selection of a time-of-day schedule result in only certain combinations of season and period being valid. For example,
suppose you define Summer and Winter seasons. You also link a schedule which defines Peak, Mid-Peak and Off-Peak periods for the Summer months, but only
Peak and Off-Peak periods for Winter months. Therefore Mid-Peak is not used in the Winter. If you specify the combination of Winter + Mid-Peak for one of the
demand charge items, this error will occur.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Inspect your inputs for seasonal scheduling and for your time-of-day schedule to determine which combinations of season and time-of-day
period are valid. Then inspect data on the Demand Charge tab to identify and correct any season+period combinations that are not valid.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 525: Season+Period Combination in Demand Multiplier Clause is Not Valid
Description: This error occurs when the combination of season and time-of-day period you selected for the demand multiplier clause does not exist.
Your specification of seasons and your selection of a time-of-day schedule result in only certain combinations of season and period being valid. For example,
suppose you define Summer and Winter seasons. You also link a schedule which defines Peak, Mid-Peak and Off-Peak periods for the Summer months, but only
Peak and Off-Peak periods for Winter months. Therefore Mid-Peak is not used in the Winter. If you specify the combination of Winter + Mid-Peak for the demand
multiplier clause, this error will occur.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Inspect your inputs for seasonal scheduling and for your time-of-day schedule to determine which combinations of season and time-of-day
period are valid. Then inspect data on the Demand Clause tab and change it to one of the valid season+period combinations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 526: Season+Period Combination in Fuel Charge is Not Valid
Description: This error occurs when the combination of season and time-of-day period you selected for one of the rows in the fuel charge table does not exist.
Your specification of seasons and your selection of a time-of-day schedule result in only certain combinations of season and period being valid. For example,
suppose you define Summer and Winter seasons. You also link a schedule which defines Peak, Mid-Peak and Off-Peak periods for the Summer months, but only
Peak and Off-Peak periods for Winter months. Therefore Mid-Peak is not used in the Winter. If you specify the combination of Winter + Mid-Peak for one of the
fuel charge items, this error will occur.
Severity: Input data cannot be saved until this error is corrected.
Suggested Action: Inspect your inputs for seasonal scheduling and for your time-of-day schedule to determine which combinations of season and time-of-day
period are valid. Then inspect data on the Fuel Charge tab to identify and correct any season+period combinations that are not valid.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors occurring when saving chiller input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Chiller Input Errors
When the OK button on the Chiller form is pressed to save input data, the program checks the inputs prior to saving them. If any problems with the data are
found, the program will display a message explaining the error. Input errors must be corrected before saving the data. For further information on a specific error,
click on one of the items below.
Error 600 - The File You Selected Appears to Contain Invalid Data
Error 601 - Full Load Cooling Entering Condenser Water Temperature is Outside Range Specified on Performance Map
Error 602 - Minimum Entering Condenser Temperature Outside Range Specified on Performance Map
Error 603 - Full Load Heating Entering Water Temperature Outside Range Specified on Performance Map
Error 604 - Full Load Heating Outdoor Air Temperature Outside Range Specified on Performance Map
Error 605 - Full Load Cooling Outdoor Air Temperature Outside Range Specified on Performance Map
Error 606 - Import is only Available when creating a Chiller or Heat Pump from the Main Window
Error 607 - Chiller Template cannot be used to Create Auto-Sized Chillers
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 31 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 600
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 601
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 602
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 603
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 600
The File You Selected Appears to Contain Invalid Data
Description: This error occurs while importing chiller data if you select an import file which is damaged, uses the wrong data format, or contains values which are
too large or too small. Chiller data files generated by Carrier Electronic Catalog have a file extension of .CD2, .CD4 or .CD5 and are formatted in a specific way. If
the file has the wrong file extension, has incorrectly formatted data, or is corrupt this error will occur. In unusual cases the file may be properly formatted but
contains values which are too large or too small for HAP to accept.
Severity: Data cannot be imported until the error is corrected.
Suggested Action: If you obtained the import file from a sales engineer, contact the sales engineer to ask for a replacement file. The original file may be
damaged.
If you generated the import file yourself, try using Electronic Catalog to generate a new file. The original file may be damaged.
After trying these workarounds, if the file is still not accepted, please contact Carrier technical support for assistance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 601
Full Load Cooling Entering Condenser Water Temperature is Outside Range Specified on Performance Map
Description: This error occurs when the full load cooling entering water temperature on the Design Inputs tab is mismatched with data in the cooling performance
map. If the full load entering water temperature value is outside the range covered by the performance map, this error will occur.
Example: For a water-cooled chiller, the full load cooling entering condenser water temperature (ECWT) is 85 F, but the cooling performance map only defines
operation between 80 F and 60 F ECWT. Therefore, the program has no source of data for performance between 80 F and 85 F ECWT.
Severity: Chiller data cannot be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Go to the Design Inputs tab and change the full load entering water temperature input so it is within the range of entering water temperatures specified in the
cooling performance map. For water-cooled chillers it is "Full Load ECWT" or "Full Load EACWT".
2. Go to the Cooling Performance Map tab and modify the map data so it covers a range of temperatures that includes the full load entering condenser
temperature input shown on the Design Inputs tab. Note that if you change an entering water temperature in the map, all performance data in that row of the
map and all capacity data in the corresponding row in the capacity table must be modified also.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 602
Minimum Entering Condenser Water Temperature Outside Range Specified on Performance Map
Description: This error occurs when the minimum condenser water temperature value is mismatched with data in the chiller’s performance map. During chiller
inputs you define the minimum entering condenser water temperature on the Design Inputs tab. You also define a chiller performance map for a range of entering
condenser water temperature conditions. If the minimum condenser water temperature value is outside the range covered by the performance map, this error will
occur.
Example: For a water-cooled chiller, the Minimum ECWT is 55 F, but the performance map only defines operation between 85 F and 70 F ECWT. Therefore, the
program has no source of performance data between 70 F and 55 F ECWT.
Severity: Chiller data cannot be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Go to the Design Inputs tab and change the "Minimum ECWT" or "Minimum EACWT" input so it is within the range of condenser temperatures specified in the
performance map.
2. Go to the Performance Map tab and modify the map data so it covers a range of temperatures that includes the minimum entering condenser temperature input
shown on the Design Inputs tab. Note that if you change a condenser temperature in the map, all performance data in that row of the map and all capacity data
in the corresponding row in the capacity table must be modified also.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 603
Full Load Heating Entering Water Temperature Outside Range Specified on Performance Map
Description: This error occurs when the full load heating entering water temperature value is mismatched with data in the heat pump or reversible chiller
performance map. During chiller inputs you define the full load heating entering water temperature on the Design Inputs tab. You also define a heating
performance map for a range of entering water temperature conditions. If the full load water temperature value is outside the range covered by the performance
map, this error will occur.
Page 32 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 604
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 605
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Error 606
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
Example: For a water-to-water heat pump, the full load entering water temperature (EWT) for heating is 28 F, but the heating performance map only defines
operation between 70 F and 40 F EWT. Therefore, the program has no source of data for performance between 40 F and 28 F ECWT.
Severity: Equipment data cannot be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Go to the Design Inputs tab and change the full load entering water temperature for heating so it is within the range of entering water temperatures specified in
the performance map.
2. Go to the Heating Performance Map tab and modify the map data so it covers a range of temperatures that includes the full load entering water temperature
input shown on the Design Inputs tab. Note that if you change a water temperature in the map, all performance data in that row of the map and all capacity
data in the corresponding row in the capacity table must be modified also.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 604
Full Load Heating Outdoor Air Temperature is Outside Range Specified on Performance Map
Description: This error occurs when the full load heating outdoor air temperature on the Design Inputs tab is mismatched with data in the heating performance
map. If the full load outdoor air temperature is outside the range covered by the performance map, this error will occur.
Example: For an air-to-water heat pump the full load outdoor air temperature (OAT) for heating is 30 F, but the heating performance map only defines operation
between 70 F and 40 F OAT. Therefore, the program has no source of data for performance between 40 F and 30 F OAT.
Severity: Equipment data cannot be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Go to the Design Inputs tab and change the full load outdoor air temperature for heating so it is within the range of entering temperatures specified in the
performance map.
2. Go to the Heating Performance tab and modify the map data so it covers a range of temperatures that includes the full load outdoor air temperature input
shown on the Design Inputs tab. Note that if you change a entering air temperature in the map, all performance data in that row of the map and all capacity
data in the corresponding row in the capacity table must be modified also.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 605
Full Load Cooling Outside Air Temperature is Outside Range Specified on Performance Map
Description: This error occurs when the full load cooling outdoor air temperature on the Design Inputs tab is mismatched with data in the cooling performance
map. If the full load outdoor air temperature is outside the range covered by the performance map, this error will occur.
Example: For an air-cooled chiller the full load outdoor air temperature (OAT) for heating is 95 F, but the cooling performance map only defines operation
between 90 F and 55 F OAT. Therefore, the program has no source of data for performance between 90 F and 95 F OAT.
Severity: Equipment data cannot be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Go to the Design Inputs tab and change the full load outdoor air temperature for cooling so it is within the range of entering temperatures specified in the
performance map.
2. Go to the Cooling Performance tab and modify the map data so it covers a range of temperatures that includes the full load outdoor air temperature input
shown on the Design Inputs tab. Note that if you change a entering air temperature in the map, all performance data in that row of the map and all capacity
data in the corresponding row in the capacity table must be modified also.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 606
Import is only Available when Creating Chiller or Heat Pump from the Main Window
Description: This error occurs for the following situation:
1. You are entering a plant.
2. On the Schedule of Equipment tab you used the  option in the equipment drop-down list to create a new chiller or heat pump.
3. In the Chiller Properties window that appears, you tried to create a chiller or heat pump by pressing the Import button to import equipment performance data
from Carrier Electronic Catalog.
The "Import" feature is currently only available when you create a chiller or heat pump using the "" option from the HAP main window.
Severity: Chiller or heat pump data be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
Page 33 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 607
32.0 Error Messages ›› 32.4 Chiller Input Error Messages ››
32.5 gbXML Translation Errors
32.0 Error Messages ››
gbXML Translation Report
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
1. Use another means of creating the chiller or heat pump such as directly entering data on the General, Design Inputs and Performance tabs.
2. Press Cancel to exit the Chiller Properties window without saving data. You can later create chiller or heat pump data from the main HAP window and in that
case can use the Import option.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 607
Chiller Template cannot be used to Create Auto-Sized Chillers
Description: This error occurs for the following situation:
1. You are entering a plant.
2. On the Configuration tab you specified chillers in the plant are to be "auto-sized".
3. On the Schedule of Equipment tab you used the  option in the equipment drop-down list to create a new chiller.
4. In the Chiller Properties window that appears, you tried to create a chiller using by pressing the Template button.
The "Template" feature only creates chillers with user-defined full load capacity. Therefore the Template option is incompatible with plants using the "auto-sized"
option.
Severity: Chiller data be saved until the problem is corrected.
Suggested Action: There are two possible solutions to this problem:
1. Use another means of creating the chiller such as directly entering data on the General, Design Inputs and Performance tabs.
2. Press Cancel to exit the Chiller Properties window without saving data. Change the selection on the plant Configuration tab to specify chillers have user
defined capacities. Then use the  option on the Schedule of Equipment tab. In this case you will be allowed to use the Template option to
create chiller data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains errors generated when importing data from a Green Building XML (gbXML) file.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
gbXML Translation Report
After translating the gbXML file, HAP provides an option for displaying a summary of data that was imported and a list of any problems encountered while
importing the data. This report is useful for understanding what was imported, for cross checking imported data and for understanding problems that may require
you to revise the data in HAP. This topic explains the content of the gbXML Translation Report and provides links to explanations of the error messages that
appear in the report.
Note: In unusual cases where the gbXML file contains a very large number of spaces and a very large number of translation problems were encountered, it may
take a long time to generate the gbXML Translation Report. In most cases the report generates quickly.
Overview for Report. The gbXML Translation Report provides a summary of the gbXML data that was imported and lists any problems which occurred during
translation. Section A in the report provides the summary of data. Section B describes problems, if any occurred. Contents of each section are described below.
Page 34 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Figure 1
Section A – Summary of Translation Results. This section (shown in Figure 1) consists of a brief summary listing the source gbXML file, the destination
project, the total number of spaces imported and total surface areas for floors, walls, windows and roofs. This is followed by a table which lists key statistics for
each space that was imported. In this table each row contains data for a different space. Each column contains descriptive data including the space name, floor
area, gross area of exterior walls, area of exterior windows and gross area of roofs.
Figure 2
Section B – Translation Issues and Problems. This section (shown in Figure 2) consists of a series of tables, with one table for each item in which problems
were encountered. These items could be spaces, schedules or wall, roof, window, skylight or door assemblies. If no problems occurred during the translation,
then this section will be omitted from the report. Typically there are no problems or only a few problems.
Each problem report table consists of separate rows for each problem condition, and columns containing descriptive data for the problem. Column data includes:
1. Ref. No. lists the error reference number. Links below can be used to obtain more information about each error number appearing on the report.
2. Item describes the data involved with the problem. For example, "occupant sensible heat gain" indicates there was a problem with this data item in a particular
space.
3. Problem describes the nature of the problem. For example "value is too large" indicates the value supplied in gbXML exceeds the maximum limit permitted by
HAP.
4. Action Taken describes the action taken to correct the problem. For example "value set to HAP maximum limit" indicates a value from gbXML that was too
large has been adjusted to equal the largest value permitted by HAP.
5. Value has two different meanings. For a problem / action condition that is "Value is missing. / Default value set", the "Value" column lists the default value that
has been inserted in the HAP data. For all other problem conditions, the "Value" column lists the original data from gbXML that must be adjusted in HAP. For
example, with item / problem / action as "occupant sensible heat gain / value is too large / value set to HAP maximum limit", a "Value" of 1505 BTU/hr/person is
the original value in gbXML that exceeds the maximum limit permitted in HAP.
Error Messages. For further information on a particular problem click on one of the following:
Error 701 - Building Weight Could not be Calculated
Error 702 - Infiltration not Specified with Units of ACH
Error 703 - Insufficient Information Exists to Import Floor Construction
Error 704 - Insufficient Information Exists to Import Roof Construction
Error 705 - Insufficient Information Exists to Import Wall Construction
Error 706 - More than 4 Roof Surfaces Exist for this Space
Error 707 - More than 8 Exterior Wall Surfaces Exist for this Space
Error 708 - Name is Too Long
Error 709 - Roof Contains More Than 8 Material Layers
Error 710 - Roof Contsins More Than One Skylight Type
Error 711 - Schedule Contains More Than 8 Profiles
Error 712 - Schedule Not Specified
Error 713 - Space Contains More Than One Floor Type
Error 714 - Value is Missing
Error 715 - Value is Too Large
Error 716 - Value is Too Small
Error 717 - Wall Contains More Than 8 Material Layers
Page 35 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 701 - Building Weight Could not be Calculated
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 702 - Infiltration not Specified with Units of ACH
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 703 - Insufficient Information Exists to Import Floor Construction
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 704 - Insufficient Information Exists to Import Roof Construction
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 705 - Insufficient Information Exists to Import Wall Construction
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 706 - More than 4 Roof Surfaces Exist for this Space
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 718 - Wall Contains More Than One Type of Door
Error 719 - Wall Contains More Than Two Different Window Types
Error 720 - Exterior Wall is Tilted
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 701 - Building Weight Could not be Calculated
Description: This problem occurs when construction data for at least one surface in a space is not defined. The translation software will automatically calculate
the building weight for a space based on the net surface area and construction weights for all floor, exterior wall, interior wall, ceiling and roof surfaces in a space.
However, if construction information is missing for any surface, the calculation cannot be performed and a standard default building weight is used for the space.
Suggested Action: After gbXML data has been imported, review the building weight for the space and adjust it as necessary.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 702 - Infiltration not Specified with Units of ACH
Description: Infiltration data can only be imported from gbXML if the units are specified as ACH (air changes per hour). Other units of measure such as sqft or
sqm of crack area cannot be interpreted by HAP. When these other units are used, the HAP defaults the infiltration airflow to zero.
Suggested Action: After gbXML data has been imported, edit the space and add the desired infiltration airflow values.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 703 - Insufficient Information Exists to Import Floor Construction
Description: This problem occurs when construction information for a floor is provided in gbXML, but the data is incomplete and therefore cannot be imported.
This typically occurs when a floor construction is created (element type = Construction) but no material layer information is provided making it impossible to
calculate the overall U-value for the floor. In this situation, HAP assigns a default U-value for the floor.
Suggested Action: After gbXML data has been imported, edit the space and revise the floor U-value if necessary.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 704 - Insufficient Information Exists to Import Roof Construction
Description: This problem occurs when construction information for a roof is provided in gbXML, but the data is incomplete and therefore cannot be imported.
This typically occurs when a roof construction is created (element type = Construction) but no material layer information is provided. In this situation, HAP inserts
a "standard default roof assembly" in place of the roof construction defined in gbXML.
Suggested Action: After gbXML data has been imported, create a roof assembly in HAP having the desired characteristics and then link it to the roof surfaces in
the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 705 - Insufficient Information Exists to Import Wall Construction
Description: This problem occurs when construction information for a wall is provided in gbXML, but the data is incomplete and therefore cannot be imported.
This typically occurs when a wall construction is created (element type = Construction) but no material layer information is provided. In this situation, HAP inserts
a "standard default wall assembly" in place of the wall construction defined in gbXML.
Suggested Action: After gbXML data has been imported, create a wall assembly in HAP having the desired characteristics and then link it to the wall surfaces in
the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 706 - More than 4 Roof Surfaces Exist for this Space
Page 36 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 707 - More than 8 Exterior Wall Surfaces Exist for this Space
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 708 - Name is Too Long
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 709 - Roof Contains More Than 8 Material Layers
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 710 - Roof Contains More Than One Skylight Type
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 711 - Schedule Contains More Than 8 Profiles
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Description: This problem occurs when a space in gbXML has more than four roof surfaces. HAP limits a space to a maximum of four roof surfaces. Therefore,
data for the first four roof surfaces can be imported, but data for additional roof surfaces must be discarded. For this error item, the "Value" column lists the ID for
the roof surface in gbXML that was discarded. An error item will be generated for each surface that is discarded so that each surface ID can be reported.
Suggested Action: After gbXML data has been imported, revise space data to account for the discarded data. One strategy is to combine the areas of discarded
surfaces with the four surfaces already included in the HAP data. Another strategy is to divide the space into multiple parts, each with 4 roof surfaces, until all
surfaces have been included. Note: If you anticipate importing gbXML again for this project as floor plan drawings change, you should not split the space into
multiple parts. The "Replace Existing" feature used when updating HAP data with gbXML from revised drawings depends on being able to match gbXML and
HAP spaces. Splitting a space into multiple parts will prevent this matching.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 707 - More than 8 Exterior Wall Surfaces Exist for this Space
Description: This problem occurs when a space in gbXML has more than eight exterior wall surfaces. HAP limits a space to a maximum of eight exterior wall
surfaces. Therefore, data for the first eight wall surfaces can be imported, but data for additional wall surfaces must be discarded. For this error item, the "Value"
column lists the ID for the wall surface in gbXML that was discarded. An error item will be generated for each surface that is discarded so that each surface ID
can be reported.
Note: The limit of eight exterior wall surfaces only applies to above grade walls. Below grade basement walls are not affected by this limit.
Suggested Action: After gbXML data has been imported, revise space data to account for the discarded data. One strategy is to combine the areas of discarded
surfaces with the eight surfaces already included in the HAP data. Another strategy is to divide the space into multiple parts, each with eight wall surfaces, until all
surfaces have been included. Note: If you anticipate importing gbXML again for this project as floor plan drawings change, you should not split the space into
multiple parts. The "Replace Existing" feature used when updating HAP data with gbXML from revised drawings depends on being able to match gbXML and
HAP spaces. Splitting a space into multiple parts will prevent this matching.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 708 - Name is Too Long
Description: This problem occurs when the name of an item in gbXML exceeds the name length permitted by HAP. For example if the name of a space is too
long, the translation software will truncate the name when importing it into HAP. This problem could occur for any item: spaces, schedules, or wall, roof, window,
skylight, or door assemblies.
Suggested Action: After gbXML data has been imported, revise the item name, if desired.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 709 - Roof Contains More Than 8 Material Layers
Description: This problem occurs when roof construction information is supplied in gbXML, and the roof assembly contains more than eight material layers. In
HAP a roof assembly can contain up to eight material layers. When this problem occurs, HAP will import the first eight material layers working from the inner
surface outward, but then must discard all additional layers.
Suggested Action: After gbXML data has been imported, edit the roof assembly and adjust material layer properties as necessary. Strategies include combining
existing layers which have similar properties in order to create space to add additional layers, or revising the layer data to represent overall thermal performance
of the actual roof.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 710 - Roof Contains More Than One Skylight Type
Description: This problem occurs when a roof surface in gbXML contains more than one "type" of skylight. A "skylight type" in HAP is defined as a unique set of
height, width, U-value and shade coefficient (or SHGC) properties. HAP only permits one skylight type per roof surface, so this problem typically arises when a
roof has two or more differently-sized skylight openings. Data for the first skylight opening encountered will be imported, but all additional skylight openings must
be discarded.
Suggested Action: After gbXML data has been imported, edit the space and revise the roof and skylight data as necessary. If the space has only one roof
surface, it may be possible to divide the surface into two or more roof items in HAP and associate different skylights with each portion of the roof.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 711 - Schedule Contains More Than 8 Profiles
Page 37 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
Error 712 - Schedule Not Specified
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 713 - Space Contains More Than One Floor Type
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 714 - Value is Missing
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 715 - Value is Too Large
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 716 - Value is Too Small
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 717 - Wall Contains More Than 8 Material Layers
Description: This problem occurs when a gbXML Schedule contains more than eight 24-hour profiles of data. A schedule can consist of one or more 24-hour
profiles associated with specific days of the week and times of year. HAP permits up eight profiles in a schedule. HAP will import the first eight profiles
encountered, but must discard all additional profiles. The eighth profile imported will be assigned to the days and times of year associated with the discarded
profiles.
Suggested Action: After gbXML data has been imported, edit the schedule and revise as necessary. One strategy is to combine original profiles which are
similar in order to accommodate all original profiles which differ significantly.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 712 - Schedule Not Specified
Description: This problem occurs when gbXML indicates schedule data is to be provided, but a schedule ID is not supplied. For example, if a Space element in
gbXML contains a lightScheduleIdRef attribute, but no ID value is supplied, this error will occur. This tends to indicate an error in the gbXML.
Suggested Action: If this error occurs, the software tool used to generate the gbXML must be rerun to either add the schedule ID or delete the reference to the
schedule altogether. For example, if the Space element does not contain a lightScheduleIdRef attribute at all, this error will not occur.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 713 - Space Contains More Than One Floor Type
Description: This problem occurs when a space contains more than one floor surface. HAP only permits one floor construction type per space. When this
problem arises, HAP will import data for the first floor surface encountered but must discard additional floor surfaces. The "Value" column will list the ID for each
surface discarded. Note that the area for the space shown on the General tab of HAP space inputs will account for the total space floor area, but the area shown
on the Floors tab will only account for the portion of the floor whose construction information was imported.
Suggested Action: After gbXML data has been imported, edit the space data and adjust data on the Floors tab as necessary to account for the portion of the
floor that was discarded.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 714 - Value is Missing
Description: This error message appears when an item is referenced in gbXML but a value is not supplied. For example, a Space element might contain a
LightPowerPerArea element, but supply no W/sqft value. This tends to indicate an error in the creation of the gbXML. When this error occurs, HAP will insert a
default value for the missing item. The default is listed in the "Value" column for the error.
Suggested Action: If this error occurs, the software tool used to generate the gbXML should be rerun to either add the missing data or delete the reference to
the item altogether.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 715 - Value is Too Large
Description: This problem occurs when a value in gbXML exceeds the maximum limit permitted in HAP. For example, if an occupant sensible heat gain value of
1505 BTU/hr/person is found in gbXML, this exceeds the maximum of 1500 BTU/hr/person permitted in HAP. Consequently HAP will adjust the value so it equals
the maximum limit allowed.
Suggested Action: After gbXML data has been imported, edit the data and adjust as necessary. For example, if an occupant heat gain was reduced, you might
increase the number of occupants so the total heat gain desired is still produced using the adjusted BTU/hr/person value.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 716 - Value is Too Small
Description: This problem occurs when a value in gbXML is less than the minimum limit permitted in HAP. For example, if the occupancy for a space is 0.10
sqft/person, this is less than the minimum of 0.15 sqft/person permitted in HAP. Consequently HAP will adjust the value so it equals the minimum limit allowed.
Suggested Action: After gbXML data has been imported, edit the data and adjust as necessary. For example, if a sqft/person value was increased, you might
switch to "number of people" in order to specify the desired number of occupants in the space.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 38 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 718 - Wall Contains More Than One Door Type
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 719 - Wall Contains More Than Two Different Window Types
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 720 - Exterior Wall is Tilted
32.0 Error Messages ›› 32.5 gbXML Translation Errors ››
Error 717 - Wall Contains More Than 8 Material Layers
Description: This problem occurs when wall construction information is supplied in gbXML, and the wall assembly contains more than eight material layers. In
HAP a wall assembly can contain up to eight material layers. When this problem occurs, HAP will import the first eight material layers working from the inner
surface outward, but then must discard all additional layers.
Suggested Action: After gbXML data has been imported, edit the wall assembly and adjust material layer properties as necessary. Strategies include combining
existing layers which have similar properties in order to create space to add additional layers, or revising the layer data to represent overall thermal performance
of the actual wall.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 718 - Wall Contains More Than One Door Type
Description: This problem occurs when a wall surface in gbXML contains more than one "type" of door. A "door type" in HAP is defined as a unique set of height,
width and U-value properties. HAP only permits one door type per wall surface, so this problem typically arises when a wall has two or more differently-sized door
openings or opening using different door constructions. Data for the first door opening encountered will be imported, but all additional door openings must be
discarded.
Suggested Action: After gbXML data has been imported, edit the space and revise the wall and door data as necessary. If the space has only a few wall
surfaces, it may be possible to divide a wall surface into two or more wall items in HAP and associate different door types with each portion of the wall.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 719 - Wall Contains More Than Two Different Window Types
Description: This problem occurs when a wall surface in gbXML contains more than two "types" of window. A "window type" in HAP is defined as a unique set of
height, width, U-value and shade coefficient (or SHGC) properties. HAP only permits two window types per wall surface, so this problem typically arises when a
wall has three or more differently-sized window openings or openings using different window constructions. Data for the first two unique types of window openings
encountered will be imported, but all additional unique window openings must be discarded.
Suggested Action: After gbXML data has been imported, edit the space and revise the wall and window data as necessary. If the space has only a few wall
surfaces, it may be possible to divide the wall surface into two or more wall items in HAP and associate different sets of window types with each portion of the
wall.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Error 720 - Exterior Wall is Tilted
Description: This problem occurs when an exterior wall surface in gbXML is not vertical (vertical is tilt = 90 deg). HAP can only accept vertical walls. Any tilted
wall surface must be discarded. When this problem arises, the "Value" column lists the surface ID for the surface that was discarded.
Suggested Action: After gbXML data has been imported, edit the space and adjust the data as necessary. For example, the tilted wall could be added as a
vertical wall with gross area equal to the projection of the actual wall on a vertical surface.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 39 of 39
32.0 Error Messages
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh597E.htm