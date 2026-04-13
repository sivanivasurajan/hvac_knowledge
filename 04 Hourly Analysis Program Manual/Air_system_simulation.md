30.0 Air System Simulations
Air System Simulation Overview
30.0 Air System Simulations ››
This chapter explains sequence of operation simulated for the air systems modeled in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Air System Simulation Overview
About Air System Simulations. "Air System Simulation" is a mathematical procedure used to calculate how an air system performs
in response to different load and weather conditions. Equations in this procedure are organized into an "algorithm" which imitates how
the system controls operate. For example, a VAV simulation algorithm varies the zone terminal airflow rate as room cooling loads vary
to imitate the operation of the zone thermostat and terminal VAV box. Within the constraints of input data and computer capabilities,
system simulations can provide accurate and sophisticated estimates of how systems perform.
Air system simulations are performed by HAP for three different applications:
1. To determine design cooling coil loads during design calculations.
2. To determine design heating coil loads during design calculations.
3. To estimate hourly cooling and heating coil loads, and energy consumption by fans and ventilation reclaim devices in the HAP
energy analysis.
How Simulations Are Performed. To start a simulation, system sizing data such as design airflow rates for zones, fans and outdoor
ventilation air must already be known. Hourly weather data and load information must also be available. Then, for each hour of the
day, the simulation algorithm analyzes how the system controls respond to load and weather conditions. Operating airflow rates,
temperatures and humidities are computed for each key point in the system. These points include the zone terminals, points in the
system where flow diverges and converges, and the inlet and outlet of all coils and fans in the system. From these results, the
program calculates fan energy consumption and coil loads. For example, coil loads are calculated using the coil airflow rate and the
inlet and outlet temperatures and humidities.
For the various system simulation applications, input data and simulation procedures vary:
1. In simulations for design cooling load calculations, weather data for one design cooling day each month is used with loads
calculated from the same design weather and using design day operating schedules.
2. In simulations for design heating calculations, the winter design temperature and humidity are used as the weather conditions with
loads computed for the design heating condition. A simulation is performed for the single design heating hour.
3. In energy simulations, one year of simulation weather data is used with loads calculated from this weather data and operating
schedules for each day of the week. Simulations are performed hour by hour for all 365 days in the year.
System Operation Documentation. The following series of help topics explains assumptions about system operation which are used
during air system simulations. Separate topics deal with each air system type analyzed by the program. Because of the flexibility
offered by HAP, it is not feasible to discuss every possible operating scenario and component configuration. Instead, to provide
effective explanations, basic system operation will be described for the most common configurations of each system. Further,
explanations of simulation procedures for system components and controls such as fans, outdoor air economizers and zone heating
units are provided separately. Finally, explanations in this chapter assume cooling and/or heating is available. For situations in which
cooling or heating has been disabled or scheduled off for certain months, readers must note that the portions of the discussions
dealing with cooling or heating operation do not apply.
For further information a specific system type, please click on the desired item below:
CAV Single Zone
CAV Terminal Reheat
CAV 2-Deck Multizone
CAV 3-Deck Multizone
CAV Dual Duct
CAV 4-Pipe Induction
CAV Make Up Air / DOAS
VAV
VAV 1-Fan Dual Duct VAV
VAV 2-Fan Dual Duct VAV
VVT
Terminal Units
Page 1 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV Single Zone System
30.0 Air System Simulations ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV Single Zone System
This help topic describes the operating assumptions for a CAV single zone air system. This single-zone system uses a central air
handler to provide a constant volume of conditioned air to the zone terminal. Depending on the user's description of the system,
operation for cooling and heating in the occupied and unoccupied periods varies, as described in the following sections.
CAV Single Zone System (Basic Configuration)
CAV Single Zone System (with Optional Features)
A. Occupied Period Operation
1. Zone Thermostat Calls for Cooling
a. If fan cycling has been specified, the supply fan and cooling coil cycle on only when a cooling demand exists. Air is supplied to
the zone at the design cooling supply temperature.
b. Otherwise, the supply fan runs continuously. The cooling coil and the supply temperature are controlled according to user
specifications.
2. Zone Thermostat Calls for Heating
a. If cycled fan operation has been specified, the supply fan and heating coil cycle on only when a heating demand exists. Air is
supplied to the zone at the design heating supply temperature.
b. Otherwise, the supply fan runs continuously. The heating coil and the supply temperature are controlled according to user
specifications.
Page 2 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV Terminal Reheat System
30.0 Air System Simulations ››
c. If a zone heating unit using room thermostat control exists, it acts as a second stage of heat for the zone and is only used if
central heat is insufficient to meet the heating demand.
3. Zone Thermostat Does Not Call for Cooling or Heating
a. If fan operation is cycled, the supply fan is off when no calls for cooling or heating exist.
b. Otherwise, the supply fan runs continuously and provides unconditioned air to the zone. The cooling and heating coils are off.
B. Unoccupied Period Operation
1. Zone Thermostat Calls for Cooling
a. The supply fan and cooling coil cycle on to meet the cooling demand. Air at the design cooling supply temperature is provided.
2. Zone Thermostat Calls for Heating
a. If a zone heating unit using room thermostat control exists, the supply fan is off. The zone heating unit provides the heat needed
to maintain zone comfort conditions.
b. Otherwise, the supply fan and heating coil cycle on to meet the heating demand. Air at the design heating supply temperature is
provided.
3. Zone Thermostat Does Not Call for Cooling or Heating
a. The supply fan is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV Terminal Reheat System
This help topic describes operating assumptions for a CAV Terminal Reheat air system. This multiple-zone system uses a central fan
to provide a constant volume of conditioned air to zone terminals. Zone thermostats control the output of terminal heating coils in
order to regulate the air temperature delivered to the zone and maintain comfort conditions. Depending on the user's description of
the system, cooling and heating operation varies in the occupied and unoccupied periods as described in the following sections.
CAV Terminal Reheat System (Basic Confiruation)
Page 3 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV 2-Deck Multizone System
30.0 Air System Simulations ››
CAV Terminal Reheat System (with Optional Features)
A. Occupied Period Operation
1. The supply fan runs continuously for all hours to supply a constant volume of air to zone terminals.
2. Supply air temperature is controlled according to user specifications.
3. Zone Thermostat Calls For Cooling:
a. The zone receives a constant volume of air at the supply temperature. The terminal heating coil is off.
4. Zone Thermostat Calls For Heating:
a. The zone terminal receives a constant volume of air at the supply temperature. The terminal heating coil is energized to reheat
the air in order to maintain zone comfort conditions.
b. If zone heating units using room thermostat control are used, they act as a second stage of heat only when heat output from the
terminal reheat coil is not sufficient to maintain conditions in the zone.
5. Zone Thermostat Does Not Call For Cooling or Heating:
a. The zone receives a constant volume of air at the supply temperature. The terminal heating coil is off.
B. Unoccupied Period Operation
1. Supply Fan:
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating, unless all
zones calling for heating have zone heating units with room thermostat control available.
b. If zone heating units are used and zones call only for heating, the supply fan is off. The zone heating units operate to meet zone
heating loads.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. If one or more zones call for cooling, supply air temperature is controlled according to user specifications.
b. When zones only call for heating and the supply fan is operating, unconditioned air is provided to zone terminals.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. If zone heating units with room thermostat control are not used, operation is the same as described for the occupied period.
b. If zone heating units with room thermostat control are used, these units provide heat sufficient to maintain zone conditions.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 4 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV 2-Deck Multizone System
This help topic describes operating assumptions for a 2-Deck Multizone air system. This multiple-zone system uses a central two-
deck blow-thru air handler to provide a constant volume of conditioned air to zone terminals. Each zone has its own supply air duct to
carry conditioned air from the central air handling unit. The zone thermostat controls the blending of air from the hot and cold decks
into its supply air duct to provide air at a temperature sufficient to maintain the zone temperature within comfort conditions. Depending
on the user's description of the system, cooling and heating operation varies in the occupied and unoccupied periods as described in
the following sections.
CAV 2-Deck Multizone CAV System
A. Occupied Period Operation
1. Supply Fan runs continuously for all hours to supply a constant volume of air to zone terminals.
2. Hot deck and cold deck supply air temperatures are controlled according to user specifications.
3. Each zone controls the amount of air it receives from the hot and cold decks, to provide air at a temperature sufficient to maintain
the zone temperature within comfort conditions.
B. Unoccupied Period Operation
1. Supply Fan
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating, unless all
zones calling for heating have zone heating units with room thermostat control available.
b. If zone heating units with room thermostat control are used and zones call only for heating, the supply fan is off. The zone
heating units operate to meet zone heating loads.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. If the supply fan is on, supply temperature is controlled in the same way as in the occupied period.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. If zone heating units with room thermostat control are not used, operation is the same as described for the occupied period.
b. If zone heating units with room thermostat control are used, these units operate to meet the heating demand.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Page 5 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV 3-Deck Multizone System
30.0 Air System Simulations ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV 3-Deck Multizone System
This help topic describes the operating assumptions for a CAV 3-Deck Multizone air system. This multiple-zone system uses a central
three-deck blow-thru air handler to provide a constant volume of conditioned air to zone terminals. Each zone has its own supply air
duct to carry conditioned air from the central air handling unit. The zone thermostat controls the blending of air from the neutral deck
with air from the hot or cold deck, to provide air at a temperature sufficient to maintain zone comfort conditions. Depending on the
user's description of the system, cooling and heating operation varies in the occupied and unoccupied periods as described in the
following sections.
CAV 3-Deck Multizone System
A. Occupied Period Operation
1. Supply Fan runs continuously for all hours to supply a constant volume of air to zone terminals.
2. Hot deck and cold deck supply air temperatures are controlled according to user specifications.
3. Zone Thermostat Operation
a. When a zone thermostat calls for cooling, air from the cold and neutral decks are mixed to supply sufficient cooling to maintain
zone comfort conditions.
b. When a zone thermostat calls for heating, air from the hot and neutral decks are mixed to supply sufficient heating to maintain
zone comfort conditions.
c. When a zone thermostat does not call for cooling or heating, air from the neutral deck is supplied to the zone. The zone
temperature floats.
B. Unoccupied Period Operation
1. Supply Fan
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating, unless all
zones calling for heating have zone heating units with room thermostat control available.
b. If zone heating units with room thermostat control are used and zones call only for heating, the supply fan is off. Zone heating
units operate to meet zone heating loads.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
Page 6 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV Dual Duct System
30.0 Air System Simulations ››
a. If the supply fan is on, supply temperature is controlled in the same way as in the occupied period.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. If zone heating units with room thermostat control are not used, operation is the same as described for the occupied period.
b. If zone heating units with room thermostat control are used, these units provide heat sufficient to maintain the zone temperature
in the heating setpoint throttling range.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV Dual Duct System
This help topic describes the operating assumptions for a CAV Dual Duct air system. This multiple-zone system uses a central two-
deck blow-thru air handler to provide a constant volume of conditioned air to zone terminals. Air is distributed to the terminals through
two parallel main ducts. The hot deck supply duct carries warm air to the zones; the cold deck supply duct carries cold air to the
zones. The zone thermostat controls the mixing of air from the hot and cold supply ducts to provide air at a temperature sufficient to
maintain zone comfort conditions. Depending on the user's description of the system, cooling and heating operation varies in the
occupied and unoccupied periods as described in the following sections.
CAV Dual Duct System
A. Occupied Period Operation
1. The supply fan runs continuously for all hours to supply a constant volume of air to zone terminals.
2. Hot deck and cold deck supply air temperatures are controlled according to user specifications.
3. Each zone controls the amount of air it receives from the hot and cold supply air ducts to provide air at a temperature sufficient to
maintain the zone temperature within the thermostat throttling range.
B. Unoccupied Period Operation
1. Supply Fan
Page 7 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV 4-Pipe Induction System
30.0 Air System Simulations ››
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating, unless all
zones calling for heating have zone heating units with room thermostat control available.
b. If zone heating units with room thermostat control are used and zones call only for heating, the supply fan is off. Zone heating
units operate to meet the zone heating loads.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. If the supply fan is on, supply temperature is controlled in the same way as in the occupied period.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. If zone heating units with room thermostat control are not used, operation is the same as described for the occupied period.
b. If zone heating units with room thermostat control are used, these units provide sufficient heat to maintain the zone temperature
in the heating throttling range.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV 4-Pipe Induction System
This help topic describes operating assumptions for a CAV 4-Pipe Induction air system. This multiple-zone system uses a primary air
handler to provide ventilation air to zone induction terminals. A central cooling coil provides cooling and dehumidification of the
primary air. Primary air flowing through the induction nozzles in the zone terminals induces secondary air from the zone to flow over
cooling and heating coils located in the induction unit. The zone thermostat controls the terminal coils to heat or cool the secondary air
as needed to maintain comfort conditions. Depending on the user's description of the system, cooling and heating operation varies in
the occupied and unoccupied periods as described in the following sections.
CAV 4-Pipe Induction System
A. Occupied Period Operation
1. The supply fan runs continuously for all hours to supply a constant volume of 100% ventilation air to zone induction units.
Page 8 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
CAV Make Up Air Unit / DOAS
30.0 Air System Simulations ››
2. Supply air is maintained at the primary supply air setpoint. If the air temperature entering the primary cooling coil is below the
supply air setpoint, the cooling coil does not operate, and the unconditioned air is delivered to the induction units.
3. Zone Induction Units
a. The zone induction unit receives a constant volume of primary air at the supply temperature. Induction nozzles mix room air with
the primary air.
b. If the zone calls for cooling, the terminal unit cooling coil operates to provide additional cooling to maintain zone comfort
conditions.
c. If the zone calls for heating, the terminal unit heating coil operates to provide heating to maintain zone comfort conditions.
B. Unoccupied Period Operation
1. Supply Fan
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating.
b. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. When the supply fan is operating, supply air temperature is maintained at the supply air setpoint.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. Operation is the same as in the occupied period.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
CAV Make Up Air Unit / DOAS
This help topic describes the operating assumptions for a CAV Make Up Air Unit / DOAS system. This system type is used to
represent a standalone make up air system or a standalone dedicated outdoor air system (DOAS) unit. This system provides 100%
treated or untreated outdoor air to a region of the building, but does not provide conditioning to control the space air temperature. That
is, any space conditioning is done with separate HVAC equipment. This system model should be used for applications such as
kitchens, factories, warehouses or gymnasiums which are supplied with treated or untreated outdoor air. Depending on the user’s
description of the system, system operation in the occupied and unoccupied periods varies as described below.
Page 9 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
VAV System
30.0 Air System Simulations ››
CAV Make Up Air Unit / DOAS System
A. Occupied Period Operation
1. The supply fan runs continuously to supply 100% outside air.
2. If a cooling coil is available, the coil will operate whenever the duct temperature downstream of the unit is above the duct cooling
setpoint. The air will be cooled so the duct temperature is held at the setpoint.
3. If a cooling coil is available and dehumidification control is used, the unit will control both dry-bulb temperature and relative humidity
(RH) downstream of the unit. If the temperature of duct air downstream of the unit is above the duct cooling setpoint, the cooling
coil will be energized to hold the duct air at the setpoint. If the duct humidity is above the RH setpoint, the cooling coil will provide
additional cooling to lower the coil dewpoint, thus condensing more moisture, and holding the duct air at the dehumidification
setpoint. A heating coil will provide reheat so the duct air temperature continues to be held at duct cooling setpoint.
4. If a heating coil is available, the coil will operate whenever the duct temperature downstream of the unit is below the duct heating
setpoint. The air will be heated so the duct temperature is held at the setpoint.
5. If a heating coil is available and humidification control is used, the unit will control both dry-bulb temperature and relative humidity
(RH) downstream of the unit. If the temperature of duct air downstream of the unit is below the duct heating setpoint, the heating
coil will be energized to hold the duct air at the setpoint. If the duct humidity is below the RH setpoint, the humidifier will add
moisture to the air stream to hold the duct humidity at the setpoint.
B. Unoccupied Period Operation
1. The system is off during the unoccupied period.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
VAV System
This help topic describes the operating assumptions for single-duct VAV systems. This multiple-zone system uses a central supply
fan to provide a variable volume of conditioned air to zone terminals. Zone thermostats control the supply terminal equipment to
regulate the flow of air into each zone and maintain zone comfort conditions. In a VAV system, any of the following supply terminal
devices can be used, either one type exclusively for all zones, or a mixture of types among the various zones served by the system.
1. VAV boxes.
2. VAV boxes with terminal reheat.
Page 10 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
3. Series fan powered mixing boxes with terminal reheat.
4. Parallel fan powered mixing boxes with terminal reheat.
Cooling and heating operation of the system varies in the occupied and unoccupied periods as described in the following sections.
VAV System with VAV Reheat Terminals (Basic Configuration)
VAV System with VAV Reheat Terminals (with Optional Features)
VAV System with Series Fan Powered Mixing Box Terminals
Page 11 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
VAV System with Parallel Fan Powered Mixing Box Terminals
A. Occupied Period Operation
1. The supply fan runs continuously to supply a variable volume of supply air to each zone.
2. Supply air temperature is controlled according to user specifications.
3. Zone Thermostat Calls for Cooling
a. For zones using VAV and VAV/RH terminals, the terminal damper regulates the flow of air into the zone to maintain comfort
conditions.
b. For zones using Series Fan Powered Mixing Box terminals, the terminal fan operates so that a constant volume of air equal to
the design zone airflow rate is provided at all times. This airflow is a mixture of cold primary air and plenum return air. The
primary air damper is positioned so the mixture of primary air and plenum return air will provide air at a temperature sufficient to
maintain comfort conditions in the zone.
c. For zones using Parallel Fan Powered Mixing Box terminals, the primary damper is positioned to provide sufficient cold primary
air to the zone to maintain comfort conditions. The terminal fan is off
4. Zone Thermostat Calls for Heating
a. For zones using VAV terminals, the terminal damper closes to the minimum airflow position. If zone heating units with room
thermostat control are used, the zone heating units operate to maintain comfort conditions in the zone. Otherwise, there is no
heating capability and the zone temperature floats.
b. For zones using VAV/RH terminals, the terminal damper closes to the minimum airflow position. The terminal reheat coil
operates to maintain comfort conditions in the zone. If a zone heating unit with room thermostat control is used, it serves as a
second stage of heat and is only used if the terminal reheat coil cannot maintain zone conditions.
c. For zones using Series Fan Powered Mixing Box terminals, the primary air damper closes to its minimum position. The terminal
fan continues to provide a constant volume of air to the zone which is a mixture of cold primary air and plenum return air.
Plenum return air serves as the first stage of heat. If this is not sufficient to maintain zone conditions, the terminal reheat coil
turns on and serves as a second stage of heat. If a zone heating unit with room thermostat control is used, it serves as a third
stage of heat and is only used if the terminal reheat coil cannot maintain zone conditions.
d. For zones using Parallel Fan Powered Mixing Box terminals, the primary air damper closes to its minimum position. The
terminal fan turns on and mixes warm plenum return air with cold primary air. This serves as the first stage of heat. If first stage
heat is not sufficient to maintain zone conditions, the terminal reheat coil turns on and serves as the second stage of heat. If a
zone heating unit with room thermostat control is used it serves as the third stage of heat and is only used if the terminal reheat
coil cannot maintain zone conditions.
5. Zone Thermostat Does Not Call for Cooling or Heating
a. For zones using VAV and VAV/RH terminals, the terminal damper closes to its minimum flow position. The zone temperature
floats.
b. For zones using Series Fan Powered Mixing Box terminals, the primary air damper closes to its minimum flow position. The
terminal fan runs to provide a constant volume of air to the zone. This air is the mixture of cold primary air and warm plenum air.
The zone temperature floats.
c. For zones using Parallel Fan Powered Mixing Box terminals, the primary air damper closes to its minimum flow position. The
zone temperature floats. The terminal fan is off.
B. Unoccupied Period Operation.
1. Supply Fan
a. Cycles on when one or more zones call for cooling.
Page 12 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
VAV 1-Fan Dual Duct System
30.0 Air System Simulations ››
b. Cycles on when one or more zones call for heating and these zones cannot meet the heating demand independently. See
discussion in items 4 below.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. When the supply fan is operating, supply air temperature is controlled according to user specifications.
3. Zone Thermostat Calls for Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls for Heating
a. For zones using VAV or VAV/RH terminals which contain a zone heating unit with room thermostat control, the zone heating unit
operates to maintain zone conditions.
b. If zones using VAV terminals exist which do not contain a zone heating unit with room thermostat control, the central supply fan
remains off. The zone temperature floats and the heating demand cannot be met.
c. If zones using VAV/RH terminals exist which do not contain a zone heating unit with room thermostat control, the central supply
fan must run to allow the terminal reheat coil to operate. Operation in this mode is the same as in the occupied period.
d. For zones using Series or Parallel Fan Powered Mixing Box terminals, the terminal fan turns on and supplies plenum return air to
the zone. This serves as the first stage of heating. If first stage heat is not sufficient to maintain zone conditions, the terminal
reheat coil turns on and serves as the second stage of heat. If a zone heating unit with room thermostat control exists, it serves
as the third stage of heat and only operates if 1st and 2nd stage heating are not sufficient to maintain zone conditions.
5. Zone Thermostats Do Not Call for Cooling or Heating
a. The system and all terminal equipment are off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
VAV 1-Fan Dual Duct System
This help topic describes the operating assumptions for a VAV 1-Fan Dual Duct air system. This multiple-zone system uses a central
two-deck blow-thru air handler to provide a variable volume of conditioned air to zone terminals. Air is distributed to the terminals
through two parallel main ducts. The hot deck supply duct carries warm air to the zones; the cold deck supply duct carries cold air to
the zones. The zone terminals mix air from the hot and cold supply ducts providing air to the zones at a temperature sufficient to
maintain comfort conditions. Depending on the user's description of the system, cooling and heating operation varies in the occupied
and unoccupied periods as described in the following sections.
Page 13 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
VAV 2-Fan Dual Duct System
30.0 Air System Simulations ››
1-Fan Dual Duct VAV System
A. Occupied Period Operation
1. The supply fan runs continuously to supply a variable volume of air to zone terminals.
2. The hot deck and cold deck supply air temperatures are controlled according to user specifications.
3. Zone Damper Control
a. When a zone thermostat calls for cooling, the heating damper is fully closed and the cooling damper controls the amount of air
received from the cold supply duct to maintain zone comfort conditions.
b. When a zone thermostat calls for heating, the cooling damper closes to its minimum airflow position and the heating damper
controls the amount of air received from the hot supply duct to maintain zone comfort conditions. If a zone heating unit with room
thermostat control exists, it serves as a second stage of heat and is only used if central heating is not sufficient to maintain zone
conditions.
c. When a zone thermostat does not call for cooling or heating, the heating damper is fully closed and the cooling damper is at its
minimum flow position. The zone temperature floats.
B. Unoccupied Period Operation
1. Supply Fan
a. Cycles on when one or more zones call for cooling. The fan also cycles on when one or more zones call for heating, unless all
zones calling for heating have zone heating units with room thermostat control units available.
b. If zone heating units with room thermostat control are used and zones call only for heating, the supply fan is off.
c. If no zones call for cooling or heating, the supply fan is off.
2. Supply Air Temperature
a. If the supply fan is on, supply temperature is controlled in the same way as in the occupied period.
3. Zone Thermostat Calls For Cooling
a. Operation is the same as in the occupied period.
4. Zone Thermostat Calls For Heating
a. If zone heating units with room thermostat control are not used, operation is the same as described for the occupied period.
b. If zone heating units with room thermostat control are used, these units provide sufficient heat to maintain zone comfort
conditions.
5. Zone Thermostats Do Not Call For Cooling or Heating
a. The system is off.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
VAV 2-Fan Dual Duct System
This help topic describes the operating assumptions for a VAV 2-Fan Dual Duct air system. This multiple-zone system uses a central
two-deck, two-fan air handler which provides a variable volume of conditioned air to zone terminals. Air is distributed to the terminals
through two parallel main ducts. The hot deck has its own VAV fan which supplies warm return air to the zones. A heating coil in the
hot deck operates whenever the warm return air is insufficient to meet zone demand. The cold deck has its own VAV fan and cooling
coil, and supplies cold air to the zones. The zone terminals mix air from the hot and cold supply ducts, providing air to the zones at a
temperature sufficient to maintain comfort conditions. Depending on the user's description of the system, cooling and heating
operation varies in the occupied and unoccupied periods as described in the following sections.
Page 14 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
2-Fan Dual Duct VAV System
A. Occupied Period Operation
1. The cold deck supply fan runs continuously to supply a variable volume of cold air to zone terminals.
2. The hot deck supply fan runs continuously during the hour whenever one or more zones call for heating; otherwise, the hot deck
fan is off.
3. Hot deck and cold deck supply air temperatures are controlled according to user specifications.
4. Zone Thermostat Control
a. When a zone thermostat calls for cooling, the heating damper is fully closed while the cooling damper controls the amount of air
received from the cold supply duct to maintain zone comfort conditions.
b. When a zone thermostat calls for heating, the cooling damper is closed to its minimum flow position and the heating damper
controls the amount of air received from the hot supply duct to maintain zone comfort conditions. If a zone heating unit with room
thermostat control is used, it serves as a second stage of heat and only operates if central heating is not sufficient to maintain
zone conditions.
c. When a zone thermostat calls for neither cooling nor heating, the heating damper is fully closed and the cooling damper is closed
to its minimum flow position. The zone temperature floats.
B. Unoccupied Period Operation
1. Cold Deck Supply Fan
a. Cycles on when one or more zones call for cooling. Also cycles on whenever the hot deck supply fan is operating.
2. Hot Deck Supply Fan
a. Cycles on when one or more zones call for heating, unless all zones calling for heating have zone heating units with room
thermostat control available.
b. If zone heating units with room thermostat control are available, the hot deck fan is off.
3. Supply Air Temperature
a. If the supply fan is on, supply temperature is controlled in the same way as in the occupied period.
4. Zone Thermostat Control
a. When a zone thermostat calls for cooling, operation is the same as in the occupied period.
b. When a zone thermostat calls for heating and zone heating units with room thermostat control are not used, operation is the
same as in the occupied period.
c. When a zone thermostat calls for heating and zone heating units with room thermostat control are used, the zone heating units
provide the heat needed to maintain zone conditions.
Page 15 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Variable Volume / Temperature (VVT) System
30.0 Air System Simulations ››
d. When a zone thermostat does not call for cooling or heating, the system is off. The zone temperature floats.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Variable Volume / Temperature (VVT) System
This help topic describes the operating assumptions for a VVT air system. VVT stands for "Variable Volume/Variable Temperature".
VVT is essentially a time-sharing system in which the same set of equipment and controls alternately provides cooling and heating as
required by the zones it serves. During operation, for example, the system may provide cooling to one group of zones for part of an
hour, heating to another group of zones for another part of the hour, and ventilation air to all zones for the remainder of the hour. VVT
system operation is similar in both the occupied and unoccupied periods. Operation in both periods is described below.
VVT System
A. Occupied Period Operation
1. Summary Of Operation. During the occupied period, the supply fan runs continuously for all hours. Depending on the zone load
conditions, the system may operate in cooling, changeover, heating, and/or ventilation modes during the hour. The length of time
spent in any mode depends on the magnitude of the zone cooling and heating loads. If the zone cooling and heating loads are
small, the system will spend only short periods of time in the cooling or heating modes, and much longer periods of time will be
spent in ventilation mode. Descriptions of each operating mode follow.
2. Cooling Mode Operation. If one or more zone thermostats call for cooling, the system will enter the cooling mode. The central
cooling coil is energized, and supplies a variable volume of air at the cooling supply temperature. Terminal dampers control the
amount of cold air entering the zone to maintain comfort conditions. As each zone thermostat falls below the cooling setpoint, its
terminal damper is closed. When all terminal dampers are closed, the system leaves the cooling mode.
3. Changeover Mode Operation. When the system switches operation from cooling mode to heating mode (or from heating mode to
cooling mode), the system first goes into changeover mode to purge conditioned air from the supply ducts before entering the next
mode. For example, when switching from cooling mode to heating mode, the system purges the supply ducts of cold air so that
zones requiring heating do not receive cold air.
During changeover mode, all terminal dampers are closed. The supply fan blows air directly through the bypass duct into the return
duct. The supply airflow rate is equal to the bypass flow rate. The length of time spent in changeover mode is specified by the user.
4. Heating Mode Operation. If one or more zone thermostats call for heating, the system will enter the heating mode. The central
heating coil is energized, and supplies a variable volume of air at the heating supply temperature. Terminal dampers control the
amount of warm air entering the zone to maintain comfort conditions. As each zone thermostat rises above the heating setpoint, its
terminal damper is closed. When all terminal dampers are closed, the system leaves the heating mode.
5. Ventilation Mode Operation. When all zone cooling and heating demands have been satisfied, the system operates in ventilation
mode. During the ventilation period, all zone terminal dampers are open to the minimum ventilation position. The supply fan
provides neutral air. Zone temperatures float.
B. Unoccupied Period Operation
1. Summary Of Operation. During the unoccupied period, the system operates only when one or more zones call for cooling or
heating. When all cooling and heating requests have been satisfied, the system is shut off. The system will not operate in
ventilation mode. Descriptions of each operating mode follow.
2. Cooling Mode Operation. Operation is the same as in the occupied period.
Page 16 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Terminal Unit Systems
30.0 Air System Simulations ››
3. Changeover Mode Operation. Operation is the same as in the occupied period.
4. Heating Mode Operation. Operation is the same as in the occupied period.
5. System Off Mode Operation. When all zone cooling and heating demands have been satisfied, the supply fan is turned off. No
conditioning is provided to the zones. Zone temperatures float.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Terminal Unit Systems
This topic describes the operating assumptions for the following terminal HVAC systems:
Packaged DX Fan Coils
Split DX Fan Coils
Variable Refrigerant Flow
2-Pipe Fan Coils
4-Pipe Fan Coils
Water Source Heat Pumps
Groundwater Source Heat Pumps
Ground Source Heat Pumps
Air side operation of all eight types of equipment is the same. The terminal unit is a single-zone constant air volume unit providing
conditioned air to the zone. Ventilation air may be provided to the terminal unit directly from outdoors as shown in Figure 1. As an
alternative, unconditioned or pre-conditioned outdoor ventilation air can be provided by a centrally located dedicated outdoor air
system (DOAS). When used, it is assumed air from the DOAS unit is ducted to the inlet of each terminal unit in the system. This
arrangement is shown in Figure 2.
Operating assumptions for the terminal units and the DOAS unit are described separately below.
Figure 1. Terminal Units with Direct Ventilation Air
Page 17 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Figure 2. Terminal Units with Dedicated Outdoor Air System (DOAS)
A. Operation of Terminal Units
A-1. Occupied Period Operation
1. Continuous Fan Operation
a. The terminal supply fan runs continuously.
b. If the zone thermostat calls for cooling, the cooling coil operates to maintain zone conditions.
c. If the zone thermostat calls for heating, the heating coil operates to maintain zone conditions.
d. If the zone thermostat does not call for cooling or heating, neither coil operates but the supply fan continues to run in order to
ventilate the zone. The zone temperature floats in the deadband between cooling and heating setpoints.
2. Cycled Fan Operation
a. If the zone thermostat calls for cooling, the terminal supply fan cycles to meet the cooling demand. Air is provided at the design
cooling supply temperature. The supply fan is on only as long as necessary to meed the demand and then turns off.
b. If the zone thermostat calls for heating, the supply fan cycles to meet the heating demand. Air is provided at the design heating
supply temperature. The supply fan is on only as long as necessary to meed the demand and then turns off.
c. If the zone does not call for cooling or heating, the fan is off.
A-2. Unoccupied Period Operation
1. Continuous or Cycled Fan Operation
a. If the zone thermostat calls for cooling, the terminal supply fan cycles to meet the cooling demand. Air is provided at the design
cooling supply temperature. The supply fan is on only as long as necessary to meed the demand and then turns off.
b. If the zone thermostat calls for heating, the terminal supply fan cycles to meet the heating demand. Air is provided at the design
heating supply temperature. The supply fan is on only as long as necessary to meed the demand and then turns off.
c. If the zone does not call for cooling or heating, the terminal supply fan is off.
B. Operation of Dedicated Outdoor Air System (DOAS)
When the terminal unit system is configured with a DOAS unit, the DOAS unit operates as follows:
B-1. Occupied Period Operation
1. The ventilation supply fan runs continuously to supply 100% outside air.
2. If a ventilation cooling coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the
unit rises above the duct cooling setpoint. The air will be cooled so the duct temperature is held at the setpoint.
3. If a cooling coil is present and scheduled on, and dehumidification control is used, the unit will control both dry-bulb temperature
and relative humidity (RH) downstream of the unit. If the temperature of duct air downstream of the unit is rises above the duct
cooling setpoint, the cooling coil will be energized to hold the duct air at the setpoint. If the duct humidity is above the maximum RH
setpoint, the cooling coil will provide additional cooling to lower the coil dew point, thus condensing more moisture, and holding the
duct air at the maximum RH setpoint. A heating coil will provide dehumidification reheat so the duct air temperature continues to be
held at duct cooling setpoint.
4. If a heating coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit falls
below the duct heating setpoint. The air will be heated so the duct temperature is held at the setpoint.
Page 18 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Induction Beam System
30.0 Air System Simulations ››
5. If a heating coil is present and scheduled on, and humidification control is used, the unit will control both dry-bulb temperature and
relative humidity (RH) downstream of the unit. If the temperature of duct air downstream of the unit falls below the duct heating
setpoint, the heating coil will be energized to hold the duct air at the setpoint. If the duct humidity is below the minimum RH
setpoint, the humidifier will add moisture to the air stream to hold the duct humidity at the minimum RH setpoint.
B-2. Unoccupied Period Operation
1. The DOAS system is off during all unoccupied period hours.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Induction Beam System
This topic describes the air-side operating assumptions for Induction Beam systems
In this system a Dedicated Outside Air System (DOAS) provides pre-conditioned air to ceiling-mounted induction beam terminals
serving each zone (Figure 1). This primary air flows through specially designed nozzles to produce high velocity jets of air. The air
jets create a region of negative pressure relative to zone air pressure in a mixing chamber which induces air from the room into the
terminal where it flows over a cooling or heating coil. This induced, conditioned air then mixes with primary air in the mixing chamber,
and the mixed air is supplied through a supply louver to the zone to provide conditioning (Figure 2).
An induction beam terminal is a total cooling device, able to provide both sensible and latent cooling. Typically the DOAS unit is
designed to meet the ventilation sensible and latent loads, and may meet a portion of the zone sensible and latent loads. The
induction beam terminal is sized to meet the remainder of the zone sensible and latent loads.
Operating assumptions for the system are described below.
Figure 1. Induction Beam System
Page 19 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Figure 2. Induction Beam Terminal Diagram
A. Operation During Occupied Period Hours
A-1. Ventilation Unit Operation
1. The ventilation supply fan runs continuously at its design airflow to supply 100% outside air.
2. If a ventilation cooling coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the
unit rises above the occupied period discharge cooling setpoint. The air will be cooled so the duct temperature is held at this
setpoint.
3. If a cooling coil is present and scheduled on, and dehumidification control is used, the unit will control both dry-bulb temperature
and relative humidity (RH) downstream of the unit. If the temperature of duct air downstream of the unit rises above the occupied
discharge cooling setpoint, the cooling coil will be energized to hold the duct air at the setpoint. If the duct humidity is above the
maximum RH setpoint, the cooling coil will provide additional cooling to lower the coil dew point, thus condensing more moisture,
and holding the duct air at the maximum RH setpoint. A heating coil will provide dehumidification reheat so the duct air temperature
is held at occupied discharge heating setpoint (if a heating coil exists) or the occupied discharge cooling setpoint (if no heating coil
exists).
4. If a heating coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit falls
below the occupied discharge heating setpoint. The air will be heated so the duct temperature is held at this setpoint.
A-2. Induction Beam Terminal Operation
1. The zone thermostat operates with occupied period settings.
2. If the zone thermostat calls for cooling, the water valve for the cooling coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required sensible cooling to satisfy the thermostat. If the coil apparatus dew point is below
the dew point of room air entering the coil, latent cooling will also occur. Condensed moisture is collected in a drain pan in the
terminal which drains into the condensate removal system.
3. If the zone thermostat calls for heating, the water valve for the heating coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required heating to satisfy the thermostat.
4. If the zone thermostat does not call for cooling or heating, the water valves for the terminal cooling and heating coils remain closed.
The terminal continues to induce room air into the terminal and supply air to the zone but no cooling or heating by the induction
beam terminal occurs.
B. Operation During Unoccupied Period Hours
B-1. Ventilation Unit Operation
1. If "Continuous Operation" was chosen for unoccupied hours, the ventilation supply fan runs continuously.
a. If the reduced airflow option is not used, the fan runs at its design airflow rate.
b. If reduced airflow is specified, the fan runs to deliver the specified reduced airflow rate (50% to 95% of design flow).
Page 20 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
Active Chilled Beam System
30.0 Air System Simulations ››
c. If ventilation dampers are open during the unoccupied period, the ventilation unit provides 100% outdoor air.
d. If ventilation dampers are closed during the unoccupied period, the ventilation unit provides air that is the mixture of recirculated
air and outdoor air leaked through the outdoor air dampers, if leakage was specified. If leakage was not specified, then the unit
provides 100% recirculated air.
2. If "Cycled on Demand" was chosen for unoccupied hours, the ventilation supply fan operates as follows:
a. If the air temperature in all zones is floating in the zone thermostat deadbands, there are no calls for cooling or heating and the
ventilation unit remains off.
b. If the air temperature in one or more zones rises above the cooling setpoint or falls below the heating setpoint, the thermostat
issues a call for cooling and the ventilation unit turns on.
c. If the reduced airflow option is not used, the fan runs at its design airflow rate.
d. If reduced airflow is specified, the fan runs to deliver the specified reduced airflow rate (50% to 95% of design flow).
e. If ventilation dampers are open during the unoccupied period, the ventilation unit provides 100% outdoor air.
f. If ventilation dampers are closed during the unoccupied period, the ventilation unit provides air that is the mixture of recirculated
air and outdoor air leaked through the outdoor air dampers, if leakage was specified. If leakage was not specified, then the unit
provides 100% recirculated air. If leakage is not specified, the ventilation unit provides 100% recirculated air.
g. The ventilation unit runs until all thermostats are satisified and then turns off. Therefore it cycles on when a cooling or heating
demand exists in one or more zones, and cycles off as soon as all demands have been satisfied. If the demands can be
satisified with run time less than 60 minutes, the ventilation unit will only run for the portion of the hour necessary.
2. Cooling coil operation is the same as for the occupied period except that the unoccupied period setpoint is used: If a ventilation
cooling coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit rises above
the unoccupied period discharge cooling setpoint. The air will be cooled so the duct temperature is held at this setpoint.
3. Dehumidification control is the same as for the occupied period: If a cooling coil is present and scheduled on, and dehumidification
control is used, the unit will control both dry-bulb temperature and relative humidity (RH) downstream of the unit. If the temperature
of duct air downstream of the unit rises above the unoccupied discharge cooling setpoint, the cooling coil will be energized to hold
the duct air at the setpoint. If the duct humidity is above the maximum RH setpoint, the cooling coil will provide additional cooling to
lower the coil dew point, thus condensing more moisture, and holding the duct air at the maximum RH setpoint. A heating coil will
provide dehumidification reheat so the duct air temperature continues to be held at the unoccupied discharge heating setpoint (if a
heating coil exists) or the unoccupied discharge cooling setpoint (if no heating coil exists).
4. Heating coil operation is the same as for the occupied period except that the unoccupied period setpoint is used: If a heating coil is
present and scheduled on, the coil will be energized when the duct temperature downstream of the unit falls below the unoccupied
discharge heating setpoint. The air will be heated so the duct temperature is held at this setpoint.
B-2. Induction Beam Terminal Operation
1. The zone thermostat operates with unoccupied period settings.
2. If the zone thermostat calls for cooling, the water valve for the cooling coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required sensible cooling to satisfy the thermostat. If the coil apparatus dew point is below
the dew point of room air entering the coil, latent cooling will also occur. Condensed moisture is collected in a drain pan in the
terminal which drains into the condensate removal system.
3. If the zone thermostat calls for heating, the water valve for the heating coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required heating to satisfy the thermostat.
4. If the zone thermostat does not call for cooling or heating, the water valves for the terminal cooling and heating coils remain closed.
The terminal continues to induce room air into the terminal and supply air to the zone but no cooling or heating is done by the
induction beam terminal.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Active Chilled Beam System
This topic describes the air-side operating assumptions for Active Chilled Beam systems
In this system a Dedicated Outside Air System (DOAS) provides pre-conditioned air to ceiling-mounted chilled beam terminals serving
each zone (Figure 1). This primary air flows through nozzles to produce high velocity jets of air. The air jets create a region of
negative pressure relative to zone air pressure in a mixing chamber which induces air from the room into the terminal where it flows
over a cooling or heating coil. This induced, conditioned air then mixes with primary air in the mixing chamber, and the mixed air is
supplied through a supply louver to the zone to provide conditioning (Figure 2).
An active chilled beam is a sensible-only cooling device. The DOAS unit is designed to meet the ventilation sensible and latent loads,
and must also provide dry enough air to absorb the latent load in the zone. Special care in design is required to ensure moisture will
Page 21 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
not condense on active chilled beam terminals in the zone. The active chilled beam is designed to meet the portion of the zone
sensible cooling load not met by the DOAS unit..
Operating assumptions for the system are described below.
Figure 1. Chilled Beam System
Figure 2. Chilled Beam Terminal Diagram
A. Operation During Occupied Period Hours
A-1. Ventilation Unit Operation
1. The ventilation supply fan runs continuously at its design airflow to supply 100% outside air.
2. If a cooling coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit rises
above the occupied period discharge cooling setpoint. The air will be cooled so the duct temperature is held at the setpoint.
3. If a cooling coil is present and scheduled on, and dehumidification control is used, the unit will control both dry-bulb temperature
and relative humidity (RH) downstream of the unit. If the temperature of discharge air downstream of the unit rises above the
occupied discharge cooling setpoint, the cooling coil will be energized to hold the duct air at the setpoint. If the duct humidity is
above the maximum RH setpoint, the cooling coil will provide additional cooling to lower the coil dew point, thus condensing more
moisture, and holding the duct air at the maximum RH setpoint. A heating coil will provide dehumidification reheat so the duct air
temperature is held at the occupied period discharge heating setpoint (if a heating coil exists) or the discharge cooling setpoint (if
no heating coil exists).
4. If a heating coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit falls
below the occupied period discharge heating setpoint. The air will be heated so the duct temperature is held at the setpoint.
A-2. Active Chilled Beam Terminal Operation
1. The zone thermostat operates with occupied period settings.
2. If the zone thermostat calls for cooling, the water valve for the cooling coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required sensible cooling to satisfy the thermostat.
3. If the zone thermostat calls for heating, the water valve for the heating coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required heating to satisfy the thermostat.
4. If the zone thermostat does not call for cooling or heating, the water valves for the terminal cooling and heating coils remain closed.
The terminal continues to induce room air into the terminal, and supply air to the zone but no cooling or heating is done by the
chilled beam terminal.
B. Operation During Unoccupied Period Hours
Page 22 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm
B-1. Ventilation Unit Operation
1. The ventilation supply fan runs continuously at the design airflow rate.
a. If ventilation dampers are open during the unoccupied period, the ventilation unit provides 100% outdoor air.
b. If ventilation dampers are closed during the unoccupied period, the ventilation unit provides air that is the mixture of recirculated
air and outdoor air leaked through the outdoor air dampers, if leakage was specified. If no leakage was specified, then the
ventilation unit provides 100% recirculated air.
2. Cooling coil operation is the same as for the occupied period except that the unoccupied setpoint is used: If a ventilation cooling
coil is present and scheduled on, the coil will be energized when the duct temperature downstream of the unit rises above the
unoccupied period discharge cooling setpoint. The air will be cooled so the duct temperature is held at this setpoint.
3. Dehumidification control is the same as for the occupied period: If a cooling coil is present and scheduled on, and dehumidification
control is used, the unit will control both dry-bulb temperature and relative humidity (RH) downstream of the unit. If the temperature
of duct air downstream of the unit rises above the unoccupied discharge cooling setpoint, the cooling coil will be energized to hold
the duct air at the setpoint. If the duct humidity is above the maximum RH setpoint, the cooling coil will provide additional cooling to
lower the coil dew point, thus condensing more moisture, and holding the duct air at the maximum RH setpoint. A heating coil will
provide dehumidification reheat so the duct air temperature continues to be held at the unoccupied discharge heating setpoint (if a
heating coil exists) or the unoccupied discharge cooling setpoint (if no heating coil exists).
4. Heating coil operation is the same as for the occupied period except that the unoccupied setpoint is used: If a heating coil is
present and scheduled on, the coil will be energized when the duct temperature downstream of the unit falls below the unoccupied
period discharge heating setpoint. The air will be heated so the duct temperature is held at this setpoint.
B-2. Active Chilled Beam Terminal Operation
1. The zone thermostat operates with unoccupied period settings.
2. If the zone thermostat calls for cooling, the water valve for the cooling coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required sensible cooling to satisfy the thermostat.
3. If the zone thermostat calls for heating, the water valve for the heating coil in the induction beam is opened. The valve regulates
water flow through the coil to deliver the required heating to satisfy the thermostat.
4. If the zone thermostat does not call for cooling or heating, the water valves for the terminal cooling and heating coils remain closed.
The terminal continues to induce room air into the terminal, and supply air to the zone but no cooling or heating is done by the
chilled beam terminal.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 23 of 23
30.0 Air System Simulations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh3283.htm