28.0 Load Calculations
28.1 Overview of Load Calculations
28.0 Load Calculations ››
Load Calculation Overview
28.0 Load Calculations ›› 28.1 Overview of Load Calculations ››
This chapter explains calculation of building cooling and heating loads.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of the load calculation process.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Load Calculation Overview
About Load Estimating Procedures. Building loads are calculated for three different purposes in the Hourly
Analysis Program:
a. For design cooling conditions in order to size cooling equipment.
b. For design heating conditions in order to size heating equipment.
c. During the whole year building simulation in the energy analysis portion of HAP.
For each application, different procedures and considerations are used when computing building loads:
1. Design Cooling. Load profiles are computed for one design cooling day in each month using design
weather conditions , design day operating schedules and the ASHRAE-endorsed Transfer Function load
calculation method. Design weather data uses design temperature data, coincident humidity levels and
clear sky solar radiation conditions. Design day operating schedules represent the variation of internal heat
gains for design cooling conditions. The Transfer Function load method provides accurate estimates of
building loads considering the transient nature of heat transfer processes in the building.
2. Design Heating. Loads are computed for a single heating design condition using winter design weather
conditions, neglecting all sources of heat gain, and using instantaneous load assumptions for transmission
and infiltration load components. Design weather data represents the winter design temperature. Sources of
heat gain are neglected so that a worst-case heating load can be calculated. The instantaneous load
procedure assumes transmission and infiltration heat losses are immediately converted to heating loads.
3. Energy Simulations. Loads are computed for all 8,760 hours in the year using simulation weather data,
operating schedules for the different days of the week, and the ASHRAE Transfer Function load method.
Actual weather data is used to evaluate how the building's HVAC systems react to real sequences of
weather over the course of a year. This is necessary to generate accurate operating cost estimates.
Operating schedules define how heat gains vary on different days of the week. The Transfer Function load
method provides accurate estimates of building loads considering the transient nature of heat transfer
processes in the building.
About This Documentation. The following series of help topics provides information about the concepts and
procedures used to determine building loads. One topic introduces the fundamental concepts used in the
Transfer Function load method. Another group of topics describes how the Transfer Function principles are
applied to the load calculations for design cooling and energy analysis applications. A final help topic
discusses how loads are calculated for design heating applications. For further information on load
calculations, please click on the desired topic below:
Page 1 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
28.2 Principles of the Transfer Function Method
28.0 Load Calculations ››
Principles of the Transfer Function Load Method
28.0 Load Calculations ›› 28.2 Principles of the Transfer Function Method ››
Principles of the Transfer Function Load Method
Summary of Component Load Calculations for Design Cooling & Simulation
Summary of Component Load Calculations for Design Heating
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides a summary of principles of the Transfer Function load calculation method.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Principles of the Transfer Function Load Method
This help topic explains the key principles used to calculate building loads with the Transfer Function Method.
This method is used in the program for cooling design calculations and for energy simulation load calculations.
The explanation of Transfer Function Method principles requires covering a series of topics, including
discussion of:
1. Necessary considerations for analyzing heat transfer in buildings.
2. Principles of the Heat Balance Method, which is the most rigorous load method available.
3. Fundamental principles of the Transfer Function Method which evolved from the Heat Balance Method.
4. Fundamental procedures used to calculate Transfer Function loads.
5. Examples illustrating how loads are calculated using Transfer Function procedures.
.Each topic will be covered in a separate section below. A final section will summarize the discussions.
A. Heat Transfer Considerations for Buildings
Most who study the process of calculating loads for commercial buildings reach the conclusion that the task is
difficult and challenging because it involves:
a. The three modes of heat transfer: conduction, convection and radiation.
b. Many heat sources whose heat contributions vary with time and are usually not in phase with each other.
c. Storage and discharge of heat from massive building elements such as walls, roofs and floors. This results
in transient rather than steady-state heat transfer processes.
d. Heat transfer processes that are interrelated.
To accurately estimate building loads, all of these factors must be considered.
To analyze building heat transfer, several key terms are used:
1. Heat Gain is the total quantity of heat entering a room from a specific heat source via the different
conduction, convection and radiation modes of heat transfer.
2. Load is the heat transferred to room air which must be removed by the air-conditioning equipment if the
zone is maintained at a constant air temperature.
3. Heat Extraction is the quantity of heat actually removed by the equipment as the zone temperature varies.
To illustrate building heat transfer in a room and the use of these terms, consider the simple example of
lighting. Heat is gained from lights in the form of convected heat and radiated heat. Convected heat warms the
air in the room and thus immediately becomes a load. Radiated heat is absorbed by the surfaces of walls,
floors, ceilings and furnishings in the room. This causes the temperature of each surface to rise. Heat is then
re-radiated to other surfaces in the room, is convected to air in the room, and is conducted into the mass
adjacent to each surface. The absorption, storage, re-radiation and convection processes occur over a period
Page 2 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
of time. Consequently, lighting heat gain occurring during the current hour will be converted to a load during
the current hour and a number of following hours. This is a transient heat transfer process. Finally, cooling
equipment is sometimes not able to remove the entire load from the room as it occurs. As equipment responds
to varying loads, the temperature in the room floats within the thermostat throttling range. Over a long period of
time, the total heat extracted by equipment may equal the total load, but due to equipment and thermostat
behavior, heat extraction and loads are not equal at every point in time.
Calculations required to account for the key aspects of these thermal processes can be complex and lengthy.
The next section discusses the Heat Balance Method, which is the most rigorous approach to solving the
building heat transfer problem. This will lead to a discussion of the Transfer Function Method which evolved
from the Heat Balance Method.
B. The Heat Balance Method
The most rigorous method of calculating building loads is the Heat Balance Method. This method evaluates
each conduction, convection, radiation and heat storage process occurring in a building using the fundamental
laws of heat transfer and thermodynamics. Equations are written for each "node" in a room, where a "node"
represents a surface or mass element associated with the room. For a mass element, the heat balance
specifies in simple terms that:
(Rate of Heat In) - (Rate of Heat Out) = Energy Storage Rate
Since a surface has no mass, its heat balance equation for a surface in the room is:
(Rate of Heat In) - (Rate of Heat Out) = 0
To define the rate of heat in and out at each node, all convection, conduction and radiation processes must be
represented. Typically these take the form of differential heat transfer equations or linearized forms of these
equations. By solving all heat balances for a room simultaneously, the total rate of heat convection to room air
can be determined. This defines the room load.
To illustrate how this works, consider the calculation of loads due only to heat gain from lighting. The heat
transfer processes involved with converting lighting heat gain to load will be described first, followed by a
summary of how the Heat Balance Method would be used to solve the heat transfer problem.
One portion of lighting heat gain is convective. Thus, it warms the room air directly and is immediately
converted to a room load. The remainder of the heat gain is thermal radiation which strikes various surfaces in
the room. Each surface absorbs a portion of the radiated heat and reflects the rest to other surfaces. The
absorbed portion warms each surface which initiates further heat transfer processes. For a wall, for example,
this can create a thermal gradient between the surface and the interior mass of the wall. Therefore, some heat
might be conducted from the surface into the wall mass where it is stored. When conditions change later,
causing the wall surface to cool, the stored heat is discharged by being conducted back to the wall surface.
The warm wall surface also can create a temperature gradient between the wall surface and room air leading
to convection which converts the heat to a load. Finally, the elevated surface temperature causes a thermal
radiation exchange between the wall surface and other surfaces in the room, where similar processes are
occurring. These processes are continually occurring and changing.
Using the Heat Balance Method to solve this heat transfer problem would require writing heat balance
equations for each surface and mass element considering each process involved:
1. Convection of heat from the light to room air.
2. Radiation from the light to each surface in the room.
3. Conduction, convection and radiation exchange for each surface in the room.
4. Conduction and heat storage for each mass element in contact with a surface.
Once equations have been formulated, they must be solved simultaneously each hour to evaluate the ebb and
flow of heat in the room.
Note that the processes described above are not isolated. Each surface in the room is also receiving heat from
other sources such as people, appliances, solar heat gain and heat conducted through walls and roofs. To
determine the total heat convected to room air (i.e., the load), all processes must be simultaneously evaluated.
The results of such an analysis can be highly accurate, insofar as input data describing sources of heat gain
and the physical and geometric properties of the room allow. While computer programs have been written to
perform these calculations, they typically require powerful computer hardware, detailed input data and long
calculation times. Using desktop computers for typical design applications, the Heat Balance Method tends to
Page 3 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
be difficult to use. However, its comprehensive approach to modeling the actual heat transfer processes in a
building are desirable. The next section describes the Transfer Function Method which evolved from the Heat
Balance Method and, using key assumptions, shortens calculation times and is able to provide sophisticated,
accurate building load estimates.
C. Fundamental Transfer Function Principles
The Transfer Function Method is the culmination of work first published in 1967 by two scientists working for
the Canadian National Research Council. The method is based on an idea known as the "Response Factor
Principle". This principle states that for a specific room, the thermal response patterns (i.e., how a heat gain is
converted to load over a period of time) for each specific type of heat gain will always be the same. That is, for
a specific room, a 1000 BTU/h heat gain through an exterior wall will cause the same response over a period
of hours as a 2000 BTU/h heat gain. The sizes of the loads will differ, but the heat gain to load conversion
pattern will be the same.
The Response Factor Principle is in turn based on three additional principles:
1. The Principle of Superposition: The total room load is equal to the sum of loads calculated separately for
each heat gain component.
2. The Principle of Linearity: The magnitude of the thermal response to a heat gain varies linearly with the size
of the heat gain.
3. The Principle of Invariability: Two heat gains of equal size occurring at different times will produce the same
thermal response in a room.
Together, these principles allow the simplification of the Heat Balance Method analysis for a building:
1. The Principle of Superposition can be used to break the heat transfer problem into manageable units since
it allows loads due to each identifiable heat gain component to be computed separately. For example, loads
due to an exterior wall heat gain, and a lighting heat gain can be computed separately and then added
together to determine the total room load. By contrast, the heat balance method requires all heat gains in a
room to be considered simultaneously.
2. The Principle of Superposition also allows the effects of heat gains each hour to be considered separately.
For example, a lighting heat gain this hour will cause loads in the current hour and a number of following
hours. This is because a portion of the heat gain is thermal radiation which is absorbed by the walls, floor
and furnishings of the room, and is then convected to room air over time. When lights are on for several
hours, the load in any one hour is due to heat gain during the current hour, and heat gains in a number of
previous hours. With the Principle of Superposition, the pattern of loads due to each hourly heat gain can be
computed separately and then added together to determine the total lighting load each hour. By contrast,
the heat balance method requires the effects of heat gains for the current hour and previous hours to be
considered simultaneously.
3. The Principles of Linearity and Invariability permit a vast reduction in the number of calculations needed.
Because the pattern of loads resulting from each type of heat gain will be invariable, the pattern only needs
to be determined one time via heat balance computations. Then, because the magnitude of each load is a
linear function of the size of the heat gain, load patterns due to each hourly heat gain can be easily
computed using simple algebraic equations. By contrast, the heat balance method requires solving a series
of heat balance equations simultaneously each hour.
D. Fundamental Transfer Function Procedures
With the Transfer Function Method, a general mathematical relationship which defines load as a function of
heat gain and time is determined for each heat gain component in a room. This relationship is then used to
quickly calculate loads for each hour. The mathematical relationship is expressed in what is called a Room
Transfer Function Equation which looks like this:
Qo = voqo + v1q1 + v2q2 - w1Q1 - w2Q2
In this equation:
1. Q represents a load. The subscripts refer to specific points in time. Subscript 0 is the current hour, 1 is the
previous hour and 2 is two hours previous.
2. q represents a heat gain. The subscripts 0, 1 and 2 have the same meaning as for loads.
Page 4 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
3. vo, v1, v2, w1 and w2 are transfer function coefficients. Values of these coefficients vary for each type of heat
gain and room due to the different heat transfer processes involved in converting each kind of heat gain into
a load. ASHRAE has published tables of these coefficients for different heat gain components, room types,
and building weights.
In words, the Room Transfer Function Equation says that the load for the current hour (Qo) is a function of the
heat gain for the current and preceding two hours, plus the loads for the preceding two hours. Because loads
for the preceding two hours are themselves dependent on a series of heat gains for prior hours, this hour's
load is really dependent on the effects of heat gains from many preceding hours.
To use the Room Transfer Function Equation, transfer function coefficients must first be obtained. Then for
any type of heat gain, calculating loads is a two-step process:
1. Determine the heat gains for a series of hours.
2. Use the heat gains and transfer function coefficients together in the Room Transfer Function Equation to
calculate the loads.
The following two sections provide examples of how loads for an internal heat gain (lighting) and a
transmission heat gain (wall) are calculated.
E. Transfer Function Example for Lighting Loads
For this example, suppose lights are turned on and operated at a constant 10,000 BTU/h rate of heat gain for
six hours and are then turned off. For a specific type of room and lighting fixture, the Room Transfer Function
coefficients published by ASHRAE are:
vo= 0.55 , v1= -0.49 , v2= 0.0
w1= -0.94 , w2 = 0.0
Transfer function load calculation results for a sequence of 12 hours are shown in Table 1.
Table 1. Lighting Load Calculations for 12 Hours
Hour
Heat Gain
(BTU/h)
Qo
(BTU/h)
Q1
(BTU/h)
qo
(BTU/h)
q1
(BTU/h)
1
10,000
5,500
0
10,000
0
2
10,000
5,770
5,500
10,000
10,000
3
10,000
6,024
5,770
10,000
10,000
4
10,000
6,262
6,024
10,000
10,000
5
10,000
6,487
6,262
10,000
10,000
6
10,000
6,697
6,487
10,000
10,000
7
0
1,396
6,697
0
10,000
8
0
1,312
1,396
0
0
9
0
1,233
1,312
0
0
10
0
1,159
1,233
0
0
11
0
1,090
1,159
0
0
12
0
1,024
1,090
0
0
Page 5 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
In Figure 1 the heat gain and load profiles resulting from this calculation are shown for the 12-hour period.
Note that the loads are smaller than the heat gains while the lights are on. This is because a large portion of
the heat gain is thermal radiation. This radiant heat is absorbed by the mass of the floor, walls and furnishings
in the room, stored in the mass and then convected to room air to become a cooling load over a period of
several hours. This process causes a delay between the time a heat gain occurs and the time its full effects as
a cooling load appear. In general, the amount of delay depends on the nature of the heat gain and the building
construction. For example, heavier construction tends to absorb and hold heat longer than light construction.
Also note that cooling loads continue after lights are turned off and the heat gains cease. Again this is due to
the radiant heat and the heat storage effects. When the lights are turned off, some radiated heat from the
previous six hours is still stored in the room mass and continues to be convected to room air over time.
Thus, this example illustrates that the Transfer Function Method models the transient build-up and discharge
of heat in a building. This is an important consideration when trying to accurately estimate loads.
Most heat gain components, both internal and transmission heat gains, involve a radiant component and thus
result in transient load behavior. The Transfer Function Method accounts for the transient heat transfer
process by using the appropriate transfer function coefficients and the same 2-step calculation procedure.
More important, the Transfer Function Method can be used to easily compute loads resulting from any hourly
sequence of heat gains. This ability provides tremendous flexibility. For example, if varying heat gains rather
than constant heat gains were used in the previous example, a different load profile would result. However, the
calculation process would be the same. The new sequence of heat gains would simply be used in the Room
Transfer Function equation to determine the new profile of cooling loads.
F. Transfer Function Example for Transmission Loads
While all loads are computed with the same 2-step procedure, wall and roof transmission loads involve special
considerations for the calculation of heat gain. This is because there is a delay between the time heat gain
occurs at the outer surface of a wall or roof and the time the heat gain reaches the interior surface of the wall
or roof. Thus, the heat gain calculation must consider the transient heat transfer through the wall or roof. In
Page 6 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
contrast, for the lighting example, determining heat gains only required knowing when the lights were on and
the lighting fixture wattage. Because transfer functions are useful for representing transient heat transfer
processes, transfer function principles can be used to determine the heat gain through a wall or roof as well as
the conversion of the heat gain into a load.
Taking an exterior wall as a specific example, the first step in the process is to determine the heat gain at the
interior surface of the wall using a "Conduction Transfer Function Equation" which is written as:
qo/A = boteo + b1te1 + b2te2 + b3te3 + b4te4 + b5te5 + b6te6
- d1q1 -d2q2- d3q3- d4q4 - d5q5 - d6q6 - trc Σ cn
This transfer function equation is more complicated than the Room Transfer Function equation we examined
earlier, but its components can be easily dissected:
1. q represents a heat gain. The subscript o refers to the heat gain for the current hour. Subscript 1 refers to
the heat gain for the previous hour. Subscript 2 refers to the heat gain two hours previous, and so forth.
2. te represents the sol-air temperature for the exterior surface of the wall. The sol-air temperature is an
"effective" measure of the heat gain at the exterior surface of the wall. It isn't the actual temperature of the
surface. Instead it is a temperature that would give the actual exterior heat gain when used in place of the
ambient dry-bulb if 100% of the heat gain was convection, rather than a combination of convection and
solar radiation. Subscripts 0 through 6 refer to the same time intervals defined for q above.
3. b, d, and cn are conduction transfer function coefficients. Values of these coefficients vary depending on the
construction of the wall or roof being analyzed. Thus, they account for the different rates of heat transfer
and storage involved with different building materials.
4. trc is the indoor air temperature.
5. A is the exterior wall surface area.
Figure 2 shows the sol-air temperatures and interior wall heat gains for one 24-hour period. As mentioned
previously, the sol-air temperature is an effective measure of the exterior surface heat gain due to both
convection from outdoor air and solar radiation. Because an east-facing wall was used in the example, the sol-
air temperature curve shows the effects of large morning heat gains due to solar radiation and smaller
afternoon heat gains due to reduced sunshine but warmer outdoor air temperatures. The heat gain curve
reveals the transient heat transfer processes involved. While the sol-air temperatures peak at 8am, the interior
wall heat gains for this medium-weight wall do not peak until 2pm. This reveals the time it takes for heat to be
conducted through this specific type of wall construction.
Page 7 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Once the interior wall heat gains have been calculated, the second step in the process is to calculate the
resulting loads using the Room Transfer Function Equation. Figure 3 shows the pattern of loads resulting from
this calculation. Note that loads are smaller than the heat gains for the hours when the heat gains are largest.
This is because as the heat gains increase, some of the heat is being stored in the mass of the room so there
is a delay before its effects on the room loads occur. Eventually all this heat is converted to load and this is
why loads are larger than heat gains during the nighttime hours.
Page 8 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Considering Figures 2 and 3 together we can see that the Transfer Function Method allows us to consider the
transient heat transfer process involved in first transferring heat through the wall and then converting the heat
gain into a room load.
As already mentioned for the lighting example, the Transfer Function Method can be used to calculate loads
for any sequence of heat gains encountered. For a wall or roof this means that for any pattern of ambient
temperatures and solar flux as well as any wall or roof construction, accurate loads can be computed. Since
weather conditions vary significantly from season to season and at different latitudes, this flexibility is essential
for computing accurate loads in all situations.
G. Heat Extraction Method Principles
The Transfer Function Method also provides procedures for calculating how HVAC equipment removes heat
from rooms in the building. This is referred to as the equipment "heat extraction rate". The procedures
discussed in the preceding sections calculate loads assuming room temperature is maintained at a fixed level.
However, in actual practice room temperatures vary within the thermostat throttling range, between cooling
and heating setpoints, and when setpoints are set-up or set-back during unoccupied periods. The float of room
temperature has a significant influence on the cooling or heating provided by the equipment. These
considerations are also essential when computing pulldown and warm-up loads resulting from the change from
unoccupied to occupied period thermostat setpoints.
Heat extraction procedures are involved in the system analysis process as follows:
1. Zone loads are computed using the heat gain and room transfer function principles outlined in the preceding
sections. These loads are calculated assuming the HVAC equipment operates 24 hours a day and
maintains a fixed zone temperature. Results of this calculation are reported as zone sensible load
components on program reports. Zone sensible loads are also used to determine zone and system supply
airflow rates.
2. Operation of the air handling system is then simulated using the zone load data and heat extraction
procedures to determine how the equipment and thermostats respond to loads and extract or add heat to
Page 9 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
the zones. The zone temperature varies within the thermostat throttling range during operation, or within the
deadband between cooling and heating setpoints. These simulation procedures are ultimately used to
determine the total system heat extraction and the resulting system coil loads.
Heat extraction procedures make use of a simple model of thermostat and equipment control, and a "Space
Air Transfer Function" to determine how the thermostat and equipment respond to room loads. This section
describes the basic procedures used in this analysis.
First of all, the heat extraction method uses the following simple linear model for the thermostat control:
ERt = Wt + S Tr,t
where:
ERt
=
Heat extraction for time t, BTU/h or W.
Wt
=
Intercept for linear control profile BTU/h or W.
S
=
Slope of linear control profile, BTU/h-F or W/K.
Tt
=
Room temperature for time t, F or C.
Figure 4 illustrates thermostat control and heat extraction behavior for a situation in which the cooling setpoint
is 72 F, the heating setpoint is 70 F and a 4 F throttling range is used. Within the cooling setpoint throttling
range (72 F to 76 F), the thermostat calls for cooling and the HVAC equipment heat extraction is a linear
function of zone temperature. Above the upper end of the throttling range, the heat extraction rate is fixed at its
maximum value.
Within the heating setpoint throttling range (70 F to 66 F), the thermostat calls for heating and the HVAC
equipment heat addition rate is a linear function of zone temperature. Below the lower end of the throttling
range, heat addition is fixed at its maximum value.
Between the thermostat setpoints (70 F to 72 F), the thermostat does not call for cooling or heating. However,
if air is still being introduced into a zone, some amount of uncontrolled heat extraction or heat addition will be
occurring.
Page 10 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Using this model, the equipment heat extraction rate and the room air temperature are related by the "Space
Air Transfer Function Equation" which has the following appearance.
po(ERo - Qo) + p1(ER1 - Q1) = go(Trc - Tro)
+ g1(Trc - Tr1) + g2(Trc - Tr2)
In this equation:
1. ER represents heat extraction values.
2. Q represents a zone sensible load.
3. Trc is the assumed constant room temperature used to calculate loads from heat gains.
4. Tr is the actual room temperature considering heat extraction behavior.
5. po, p1, go, g1, g2 are space air transfer function coefficients. Reference coefficients are published by
ASHRAE. Before using the coefficients in calculations, they are modified based on the building construction
weight, the envelope U-value and area for a zone and the zone infiltration rate.
6. The subscripts for each component of the equation refer to different hours. 0 refers to the current hour. 1
refers to the previous hour. 2 refers to two hours previous.
In words, the Space Air Transfer Function Equation says that the heat extraction rate for the current hour
depends on the load for the current hour and previous hour, the heat extraction rate in the previous hour, and
the room temperatures during previous hours. The equation therefore accounts for the fact that as room
temperature and heat extraction rates vary, heat builds up and is discharged by the building mass and air
mass for the zone.
To determine the heat extraction rate for a zone, the thermostat equation and the space air transfer function
equation must be solved simultaneously using known values of the thermostat setpoint, its throttling range, the
maximum and minimum equipment heat extraction rates (ERmax, ERmin, EAmin, EAmax), zone sensible loads
and room temperatures for preceding hours.
To illustrate the results of this procedure, Figure 5 shows load, heat extraction and room temperature profiles
for a scenario in which HVAC equipment operates for the period 8am to 10pm, and is off for the remaining
hours of the day. The figure shows the cooling load profile calculated using the room transfer function
procedures and assuming a constant room temperature. The actual room temperature profile shows that
during the 8am to 10pm operating period, the equipment maintains the zone within the thermostat throttling
range of 72 F to 76 F. During the off hours, the zone temperature floats above the throttling range. During this
period, heat is accumulated in the building mass. When the equipment operating period begins at 8am, this
accumulated heat is removed in addition to the hourly cooling loads. This results in a pulldown component of
the load.
Page 11 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
28.3 Component Load Calculations for Design Cooling & Simulation
28.0 Load Calculations ››
Summary of Component Load Calculations for Design Cooling & Simulation
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
H. Summary
At first the "Transfer Function Method" may sound mysterious and complicated. But as we have seen in this
discussion it is based on several straightforward principles. And, once given transfer function coefficients,
loads are calculated using simple algebraic equations. While the equations are complex enough that
computing loads by hand is not practical, with a desktop computer, loads can be quickly determined.
The results of these calculations can yield important benefits such as the ability to analyze the realistic
transient heat transfer which occurs in all buildings. Loads can also be accurately computed for any heat gain
sequence and wall or roof construction. Consequently, resulting loads are specific and customized for each
application analyzed, accounting for local weather conditions, building construction and operating schedules.
The value of these benefits is obvious for HVAC design work.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes calculations for design cooling and energy simulation loads.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 12 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Wall and Roof Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Summary of Component Load Calculations for Design Cooling & Simulation
The following series of help topics explains how specific component loads are computed for design cooling
and energy simulation applications using transfer function procedures. As discussed in the help topic
Principles of the Transfer Function Load Method , a standard two-step procedure is used:
1. The component heat gains are computed for a series of hours.
2. Heat gains are used in the Room Transfer Function Equation to compute the resulting loads.
In the following series of help topics, considerations for computing heat gains and loads for each load
component are summarized. Figures are provided with these discussions to illustrate the differences between
heat gain and load profiles. Readers should note that these figures have been constructed using medium and
heavy weight building constructions to amplify the difference between heat gain and load profiles. Actual heat
gain to load conversion rates will vary with construction type and building weight and may show smaller or
larger conversion rates than those illustrated. For further information on component loads, please click on the
desired topic below:
Wall and Roof Transmission Loads
Window Solar Loads
Window Transmission Loads
Door Loads
Partition Transmission Loads
Floor Transmission Loads
Lighting Loads
Electric Equipment Loads
People Loads
Miscellaneous Sensible and Latent Loads
Infiltration Loads
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Wall and Roof Load Calculations (Cooling, Simulation)
This help topic discusses wall and roof transmission load calculations for design cooling and energy simulation
applications. Wall and roof transmission loads account for heat transferred through a wall or roof due to solar
radiation striking the exterior surface of the wall or roof, and due to the temperature difference between indoor
and outdoor air.
Step 1: The heat gain at the interior surface of the wall or roof is computed using the following procedure:
a. Compute the sol-air temperature using the outdoor air dry-bulb temperature and the total solar flux on the
wall or roof exposure. For cooling design calculations, design temperature profiles and clear sky solar
flux profiles are used. For energy simulations, simulation weather data is used. The sol-air temperature is
computed using the equation:
Tsa = Toa + αIt/ho - εΔR/ho
b. Obtain conduction transfer function coefficients for the wall or roof construction being analyzed. Based on
a user's specification of the wall or roof construction, the appropriate transfer function coefficients are
derived automatically by the program. As a result, the specific thermal performance of each different
construction is analyzed by the program.
Page 13 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Window Solar Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
c. Use the sol-air temperature and the conduction transfer function coefficients together in the conduction
transfer function equation to calculate the wall or roof heat gain.
Step 2: The heat gains calculated in step 1 are used together with the appropriate coefficients in the room
transfer function equation to calculate wall or roof transmission loads. Sample graphs of wall heat gain and
load profiles are provided in the help topic titled Principles of the Transfer Function Load Method.
Variable Definitions:
Tsa
=
Sol-air temperature, F or C.
Toa
=
Outdoor air dry-bulb temperature, F or C.
α
=
Wall or roof exterior surface absorptivity for solar radiation,
dimensionless.
It
=
Total solar flux on wall or roof surface, BTU/hr/sqft or
W/sqm.
ho
=
Convective heat transfer coefficient on exterior wall or roof
surface.
A value of 3.0 BTU/h-sqft-F or 17.0 W/sqm-K is used.
ε
=
Hemispherical emittance of exterior surface. A value of 1.0
is used.
ΔR
=
Difference between longwave radiation incident on exterior
surface and blackbody radiation at Toa,
BTU/h-sqft or W/sqm. For vertical surfaces,
ΔR = 0.0. For horizontal surfaces, ΔR = 20.0
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Solar Load Calculations (Cooling, Simulation)
This help topic discusses window solar load calculations for design cooling and energy simulation applications.
Window solar loads are the result of solar heat transmitted through the window into the building, and solar heat
absorbed by the window glass and the interior shading device which is transferred to the interior of the
building. In the figure below sample solar heat gain and load profiles to illustrate the transient conversion of
solar heat gain to load.
Page 14 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Step 1:Calculate Heat Gains. The procedure for calculating window solar heat gains begins with profiles of
solar heat gain for reference glass. If external shading devices are used, the fraction of the window shaded
from direct sunlight must be calculated each hour. Then, according to current ASHRAE procedures, the
absorbed and transmitted solar heat gains, and the total solar heat gain for the window are computed using
the equations:
TSHG = [TSHGFb(1 - Fs) + TSHGFd] (SC) (A)
ASHG = [ASHGFb(1 - Fs) + ASHGFd] (Ni) (SC) (A)
SHG = TSHG + ASHG
For design cooling calculations, clear sky solar heat gain data is used. For energy simulations, simulation
weather data is used.
Step 2:Derive Loads from Heat Gains. The total solar heat gain (SHG) values are used with the appropriate
coefficients in the room transfer function equation to determine solar loads. Separate sets of transfer function
coefficents are used for the case where internal shades are used and for the case where no shades are used.
These different coefficients account for the fact that internal shades such as curtains or blinds absorb a portion
of the incoming solar and convect it to room air much faster than solar absorbed by the floors and walls in the
room. As a result, solar heat gains for windows with internal shades are converted to room loads faster than
solar heat gains for windows without shades.
Variable Definitions:
A
=
Window area, sqft or sqm.
ASHG
=
Absorbed component of solar heat gain, BTU/h or W.
ASHGb
=
Beam component of absorbed solar heat gain, BTU/h-sqft
or W/sqm.
ASHGd
=
Diffuse component of absorbed solar heat gain, BTU/h-sqft
or W/sqm.
Page 15 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Window Transmission Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Fs
=
Fraction of window area shaded from direct sunlight,
decimal.
Ni
=
Fraction of solar radiation absorbed by reference glass
which conducted to the interior of the building.
A standard value of 0.267 is used.
SC
=
Window overall shade coefficient, dimensionless.
SHG
=
Total solar heat gain for window, BTU/h or W.
TSHG
=
Transmitted component of solar heat gain, BTU/h or W.
TSHGb
=
Beam component of transmitted solar heat gain, BTU/h or
W.
TSHGd
=
Diffuse component of transmitted solar heat gain,
BTU/h-sqft or W/sqm.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Transmission Load Calculations (Cooling, Simulation)
This help topic discusses window transmission load calculations for design cooling and energy simulation
applications. Window transmission loads are the result of heat flow through windows due to the difference
between indoor and outdoor temperature. Calculations consider the overall resistance to heat flow of the
window glass, the window frame and an interior shading device, if one is used.
Step 1:Calculate Heat Gains. The window transmission heat gain is computed using the following equation:
Page 16 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Door Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Partition and Ceiling Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
q = U A (Toa - Tr)
Step 2:Derive Loads from Heat Gains. The heat gain is used with the appropriate coefficients in the room
transfer function equation to calculate the window transmission load.
The figure above shows window transmission and heat gain profiles for a sample case. The difference
between heat gain and load is due to the radiant component of the heat gain which is absorbed by the building
mass, and later convected to room air to become a load.
Variable Definitions:
q
=
Window transmission heat gain, BTU/h or W.
U
=
Overall window U-value, BTU/hr-sqft-F or W/sqm-K.
A
=
Window area, sqft or sqm.
Tr
=
Room air temperature, F or C.
Toa
=
Outdoor air temperature, F or C.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Load Calculations (Cooling, Simulation)
This help topic discusses door load calculations for design cooling and energy simulation applications. When
doors are used in a space, three separate load components are calculated:
1. The load for heat conducted through the opaque portion of the door.
2. The load for heat conducted through glass panes in the door.
3. The load for solar heat gain through the glass panes in the door.
Considerations for determining heat gains and loads for all three components are summarized below.
Step 1:Calculate Heat Gains. Transmission and solar heat gains for the different door component loads are
calculated as follows:
a. Opaque Transmission Heat Gain. The door is assumed to have a low thermal capacitance. Therefore,
the conductive heat gain for the opaque portion of the door is computed using a simple U x A x ΔT
equation.
b. Glass Transmission Heat Gain. The conductive heat gain for door glass is computed using the
procedure described in the help topic titled Window Transmission Load Calculations (Cooling,
Simulation).
c. Glass Solar Heat Gain. The door solar heat gain is computed using the procedure outlined in the help
topic titled Window Solar Load Calculations (Cooling, Simulation). When the user has specified that the
door glass is unshaded, a shading fraction (Fs) of zero is used. When shaded glass has been specified,
a shading fraction of 1.0 is used.
Step 2:Derive Loads from Heat Gains. Each heat gain component is then used with the appropriate
coefficients in the room transfer function equation to calculate door loads. A separate calculation is performed
for each load component.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition and Ceiling Load Calculations (Cooling, Simulation)
Page 17 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Floor Load Calculations (Cooling, Heating, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
This help topic discusses partition and ceiling transmission load calculations for design cooling and energy
simulation applications. These loads are the result of heat flow through partitions or ceilings adjacent to
unconditioned or partially conditioned regions. Heat gain and load calculation considerations are summarized
below.
Step 1:Calculate Heat Gains. It is assumed the partition or ceiling has a low thermal capacitance. Therefore,
the heat gain is computed using the following equation:
q = U A (Tadj - Tr)
where:
q
=
Heat gain, BTU/h or W.
U
=
Partition or ceiling U-value, BTU/h-sqft-F or W/sqm-K.
A
=
Partition or ceiling area, sqft or sqm.
Tadj
=
Temperature in adjacent space, F or C.
Tr
=
Room temperature, F or C.
In this equation, the adjacent space temperature (Tadj) is determined from the user's specifications of the
maximum and minimum adjacent space temperatures and the outdoor air temperatures corresponding to
each.
Step 2:Derive Loads from Heat Gains. The heat gains from step 1 are used with the appropriate coefficients
in the room transfer function equation to determine the partition or ceiling transmission load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Floor Load Calculations (Cooling, Heating, Simulation)
This help topic discusses floor transmission load calculations for design heating and energy simulation
applications. Floor transmission loads are due to heat flow through floors which are either adjacent to
unconditioned or partially conditioned regions, or are in contact with soil. The program permits four types of
floor heat transfer situations to be evaluated:
1. Floor is Above Conditioned Region: It is assumed the adjacent region is at the same temperature as the
zone. Therefore, no heat transfer occurs.
2. Floor is Above An Unconditioned Region: The procedures outlined in the help topics titled Partition and
Ceiling Load Calculations (Cooling, Simulation) and Partition and Ceiling Load Calculations (Heating) are
used to calculate these floor transmission loads.
3. Slab On Grade Floor: Heat transmitted through the floor and the adjacent soil is computed.
4. Floor Below Grade: Heat transmitted through the floor, below-grade walls and the adjacent soil is analyzed.
The remainder of this topic discusses calculations for the slab on grade and floor below grade cases. Readers
should note that HAP does not perform load calculations for slab-on-grade and basement floors and walls for
the design cooling condition. Per ASHRAE recommendations, slab and basement heat transfer is not included
in the design cooling calculations since heat transfer is either negligible or constitutes a credit for summer
conditions.
Step 1:Calculate Heat Gains. In HAP a simplified 1-dimensional steady-state heat transfer model is used to
estimate ground heat transfer. Readers should recognize that this is a simplification since ground heat transfer
is really a 3-dimensional heat transfer problem which would require advanced numerical methods to solve
precisely. Considerations for the 1-dimensional model vary for slab-on-grade floors and below grade floors and
walls:
a. For a Slab-On-Grade Floor, it is assumed heat is transferred from the room air through the slab floor to
the soil beneath and eventually to outdoor air. Working from the slab perimeter inward, the program
calculates the total thermal resistance of the heat transfer path by considering the R-value of the slab
floor and carpet, the soil beneath the slab, slab footer insulation, the slab footer, and soil outside the slab
Page 18 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
footer. The soil thermal resistance is determined using the length of the heat transfer path through the
soil, and the user specification of the soil thermal conductivity. Figure 1 illustrates the configuration of
these components. To determine thermal resistances, it is assumed the heat transfer path is semi-
circular. Therefore, as one proceeds inward from the slab perimeter, the path of heat transfer becomes
longer and the overall resistance to heat flow becomes larger. The equation for one-dimensional heat
flow as a function of distance from the slab perimeter is integrated over the width of the floor and is then
solved to determine the total heat flow through the slab floor area. The following equation is used:
qf = P (Toa - Tr) ksoil/π x
[ ln (1/ho + πW/ksoil + Rf + Rsi + Rs)
- ln (1/ho + Rf + Rsi + Rs) ]
Figure 1. Slab-on-Grade Floor Diagram
b. For Below-Grade Floors, heat transmitted through both the floor and basement walls is considered. The
floor heat transmission gain is calculated using the procedures described above for slab-on-grade floors,
except that the slab footer and slab footer insulation are omitted from thermal resistance calculations. In
this case the heat transmission paths are also longer. For heat transmission through the basement walls,
it is assumed the heat transfer path is circular between the basement wall and the soil surface (i.e. a 90-
degree arc). The thermal resistance to heat flow depends on the R-value of the basement wall, wall
insulation and the adjacent soil. The heat transfer path becomes longer as the depth below grade
increases. The equation for one-dimensional heat transfer as a function of depth is integrated over the
interval from grade level to floor depth below grade and is then solved to determine total heat transfer
through the basement wall. When wall insulation is used, two separate calculations are performed. One
is for the portion of the wall covered by insulation, and the other is for the uninsulated portion of the wall.
Figure 2 illustrates the components involved in this analysis. The following equations are used:
qf = P (Toa - Tr) ksoil/π x
[ ln (1/ho + πDf/(2ksoil) + πW/ksoil + Rs) - ln (1/ho + πDf/(2ksoil) + Rs) ]
qw = P (Toa - Tr) 2ksoil/π x
[ ln (1/ho + πDi/(2ksoil) + Rwi + Rw) - ln (1/ho + Rwi + Rw)
+ ln (1/ho + πDf/(2ksoil) + Rw) - ln (1/ho + πDi/(2ksoil) + Rw) ]
Page 19 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Figure 2. Floor Below Grade Diagram
Step 2:Derive Loads from Heat Gains. It is assumed load equals heat gain for slab floors, basement walls
and basement floors. Therefore, room transfer function equations are not needed to convert heat gains into
loads for these load components.
Variable Definitions:
Df
=
Depth of basement floor below grade, ft or m.
Di
=
Depth that basement wall insulation extends below grade,
ft or m.
ho
=
Outdoor surface convection coefficient, 6.00 BTU/(hr-
sqft-F) or 34.1 W/(sqm-K).
ksoil
=
Thermal conductivity for soil, BTU/(hr-ft-F) or W/(m-K).
P
=
Slab floor perimeter exposed to contact with soil, ft.
qf
=
Floor heat gain, BTU/hr or W.
qw
=
Basement wall heat gain, BTU/hr or W.
Rf
=
Thermal resistance for wall foundation, 1.64 (hr-
sqft-F)/BTU or 0.289 (sqm-K)/W.
Rsi
=
Thermal resistance for slab insulation, (hr-sqft-F)/BTU or
(sqm-K)/W.
Rs
=
Thermal resistance of slab floor, including the floor
material, any covering such as tile or carpet
and the inside surface resistance, (hr-
sqft-F)/BTU or (sqm-K)/W.
Rw
=
Thermal resistance of basement wall including the wall
material, any interior wall finish material or
insulation and the inside surface resistance,
(hr-sqft-F)/BTU or (sqm-K)/W.
Rwi
=
Thermal resistance of insulation applied to the exterior of
the basement wall, (hr-sqft-F)/BTU or
(sqm-K)/W.
Toa
=
Outdoor air temperature, F or C.
Tr
=
Room air temperature, F or C.
W
=
Effective width of floor, ft. This is calculated as {space floor
area} divided by {exposed perimeter}.
Page 20 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Lighting Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Lighting Load Calculations (Cooling, Simulation)
This help topic discusses lighting load calculations for design cooling and energy simulation applications. Heat
gain and load calculations for lighting are summarized below.
Step 1:Calculating Heat Gains. Lighting heat gain is determined from user specifications of the lighting
wattage , the ballast multiplier (if used) and the hourly lighting schedule :
q = K Pl (BM) Fs / 100
where:
q
=
Lighting heat gain, BTU/h or W.
K
=
Unit conversion factor,
=
3.412 (BTU/h)/W for English units or,
=
1.0 for S.I. Metric units.
Pl
=
Lighting fixture power, watts.
BM
=
Ballast multiplier, decimal.
Fs
=
Schedule percentage value, percent of maximum lighting
watts for the hour.
Page 21 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Electrical Equipment Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Step 2:Deriving Loads from Heat Gains. Heat gains are then used with the proper coefficients in the room
transfer function equation to determine lighting loads. The room transfer function coefficients for lighting loads
vary with the type of fixture specified. In the program, three fixture options are offered:
1. Recessed, vented fixtures.
2. Recessed, unvented fixtures.
3. Free-hanging fixtures.
The figure above provides sample load profiles for each fixture type for a scenario in which a 5000 BTU/h heat
gain occurs for a duration of 9 hours starting at 0700 and continuing through 1600.
When task lighting is used, the fixture is assumed to be free-hanging. Because the nature of heat transfer from
these fixtures differs, heat gains are converted to loads at different rates. For example, a recessed vented
fixture has return air flowing through the fixture and therefore has higher rates of convective heat transfer than
an unvented fixture. Further, a free-hanging fixture is completely exposed to room air and radiates heat to all
room surfaces including the ceiling. .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Electrical Equipment Load Calculations (Cooling, Simulation)
This help topic discusses electrical equipment load calculations for design cooling and energy simulation
applications. Equipment loads are the result of heat gain from electric equipment and appliances. Examples
include copy machines, computer equipment, cash registers, kitchen appliances and industrial machinery.
Considerations for heat gain and load calculations are summarized below.
Step 1:Calculating Heat Gains. The equipment heat gain is determined directly from the user's specification
of the equipment wattage and the hourly schedule factor:
Page 22 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
People Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
q = K Pe Fs / 100
where
q
=
Heat gain, BTU/hr or W.
K
=
Unit conversion factor,
=
3.412 (BTU/h)/W for English units or
=
1.0 for S.I. Metric Units.
Pe
=
Electric equipment maximum power, watts.
Fs
=
Hourly scheduling factor, percent of maximum power use.
Step 2:Deriving Loads from Heat Gains. The load resulting from this equipment heat gain must be
calculated in separate convective and radiative components. The convective and radiative fractions of
equipment heat gain vary with the type of equipment being evaluated. HAP assumes that 75% is convective
and 25% is radiative. These assumptions are appropriate for common types of office equipment and are based
on research data published in the 2001 ASHRAE Handbook of Fundamentals.
The 75% convective fraction of the heat gain becomes a load immediately. The load due to the 25% radiative
component is calculated using the room transfer function equation and the appropriate coefficients. The figure
above shows equipment heat gain and total load profiles for a scenario in which a 5000 BTU/h equipment heat
gain occurs for a duration of 10 hours. The load profile differs from the heat gain profile because a portion of
the heat gain is radiative causing a time lag between the time the heat gain occurs and the time it is converted
to a cooling load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
People Load Calculations (Cooling, Simulation)
This help topic discusses people load calculations for design cooling and energy simulation applications.
People loads are the result of sensible and latent heat gain from people occupying a building. The latent
component of the heat gain involves the transfer of moisture to room air and is thus immediately converted to
a load. The sensible component of the heat gain involves separate convective and radiative components and
is evaluated using transfer function procedures as discussed below.
Page 23 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Misc. Sensible and Latent Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Step 1:Calculating Heat Gains. The sensible heat gain for people is calculated directly from the user's
specification of the heat gain per person , the space maximum occupancy and hourly scheduling factors:
q = (HG) (O) Fs / 100
where:
q
=
People heat gain, BTU/h or W.
HG
=
Unit heat gain, BTU/h/person or W/person.
O
=
Maximum number of occupants.
Fs
=
Hourly scheduling factor, percent of maximum occupancy.
Step 2:Deriving Loads from Heat Gains. The load resulting from the sensible people heat gain must be
calculated in separate convective and radiative components. Studies have shown that between 26% and 34%
of people sensible heat gain is convected heat and the reminder is radiated heat. Using ASHRAE
recommendations, the program assumes an average value of 30% convection.
The 30% convective fraction of the heat gain becomes a load immediately. The load due to the 70% radiative
component is calculated using the room transfer function equation and the appropriate coefficients. The figure
below shows people sensible heat gain and total sensible load profiles for a scenario in which a 7000 BTU/h
sensible heat gain occurs for a duration of 10 hours. The large separation between heat gain and load profiles
in this scenario is due to the fact that the majority of the heat gain is radiative and is therefore converted to
load more slowly than if it was convective.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 24 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Infiltration Load Calculations (Cooling, Simulation)
28.0 Load Calculations ›› 28.3 Component Load Calculations for Design Cooling & Simulation ››
Misc. Sensible and Latent Load Calculations (Cooling, Simulation)
This help topic discusses miscellaneous sensible and latent load calculations for design cooling and energy
simulation applications. Miscellaneous sensible and latent loads are used to model heat transfer from non-
electric equipment in the building. It is assumed sensible heat gain from this equipment is 100% convective
and therefore is immediately converted to a load. Consequently, transfer function procedures are not applied
to this component load. In all cases the load equals the hourly heat gain. Because latent heat gain represents
the transfer of moisture to and from room air it is also evaluated as an immediate load. Loads are computed in
each case based on the user's specification of the miscellaneous heat gain and hourly scheduling factors.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Infiltration Load Calculations (Cooling, Simulation)
This help topic discusses infiltration load calculations for design cooling and energy simulation applications.
Infiltration loads are the result of uncontrolled leakage of air into and out of the building. These loads are due
to the loss of building air and the introduction of outdoor air into rooms in the building. As a result, the air
exchange immediately affects building loads. It is not necessary to apply transfer function procedures to
determine the infiltration load.
Infiltration airflow is defined by the user on a CFM (L/s), CFM/sqft (L/s/sqm) or Air Change per Hour basis. In
the first case, infiltration airflow is directly known. In the other two cases, infiltration airflow must be calculated
Vi = (CFM/sqft or L/s/sqm) x (Gross Area of Exterior Walls in Space)
Vi = (Air Changes per Hour)(Af)(H)/(K)
In addition, the user has the opportunity to specify whether infiltration is considered for all hours of the day, or
only during the equipment "unoccupied" period hours. For those hours in which infiltration is considered, the
program computes the infiltration loads as:
Qs = ρa Cpa Vi K (Toa - Tr)
Ql = ρa hfg Vi K (ωoa - ωr)
where:
Af
=
Floor area for space, sqft or sqm.
Cpa
=
Heat capacity of air, 0.24 BTU/lbm-F or 1004.8 J/kg-K.
H
=
Average floor to ceiling height for space, ft or m.
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535
x10^6 J/kg.
K
=
Unit conversion factor,
=
60 min/hr for English units or
=
cubic meter/(1000 L) for S.I. Metric units.
ρa
=
Density of air , adjusted for altitude, lb/cuft or kg/cubic
meter.
Ql
=
Latent infiltration load, BTU/h or W.
Qs
=
Sensible infiltration load, BTU/h or W.
Toa
=
Outdoor air temperature, F or C.
Tr
=
Room temperature, F or C.
Vi
=
Infiltration airflow rate, CFM or L/s. For design cooling
calculations, the "design cooling" infiltration
specification is used. For energy simulations,
the "energy simulation" infiltration specification
is used.
ωoa
=
Outdoor air specific humidity, lb/lb or kg/kg.
Page 25 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
28.4 Component Load Calculations for Design Heating
28.0 Load Calculations ››
Summary of Component Load Calculations for Design Heating
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
Wall and Roof Load Calculations (Heating)
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
ωr
=
Room specific humidity, lb/lb or kg/kg.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculations of design heating loads.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Summary of Component Load Calculations for Design Heating
The following series of help topics explains how specific component loads are computed for design heating
applications. Unlike cooling and energy simulation load calculations, design heating calculations use traditional
procedures. With these procedures:
1. Weather data for the winter design condition is used.
2. Calculations are not linked to a specific hour or month as they are for cooling design calculations.
3. Loads are calculated assuming steady-state heat loss and instantaneous conversion of heat losses to
loads. No transient heat transfer processes are considered, and no transfer function procedures are used in
the analysis.
4. All heat gain components are excluded from the analysis to yield worst-case heating load estimates.
In the following series of help topics, procedures are described for calculating loads for each component
included in the design heating analysis. For further information on component loads, please click on the
desired topic below:
Wall and Roof Transmission Loads
Window Transmission Loads
Door Loads
Partition Transmission Loads
Floor Transmission Loads
Infiltration Loads
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Wall and Roof Load Calculations (Heating)
This help topic discusses wall and roof transmission load calculations for design heating applications. Wall and
roof transmission loads are the result of heat loss through the wall or roof due to the indoor-outdoor
temperature difference. The load is calculated as the steady state heat loss for the winter design condition:
Q = U A (Tr - Toa)
where:
Page 26 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Window Transmission Load Calculations (Heating)
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
Door Load Calculations (Heating)
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
Q
=
Transmission heating load, BTU/h or W.
U
=
Wall or roof U-value, BTU/h-sqft-F or W/sqm-K.
A
=
Net area of wall or roof, sqft or sqm.
Tr
=
Room temperature, F or C. For the design heating load
analysis, the occupied heating thermostat
setpoint is used.
Toa
=
Outdoor air winter design temperature, F or C.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Transmission Load Calculations (Heating)
This help topic discusses window transmission load calculations for design heating applications. Window
transmission loads are the result of heat loss through the window due to the indoor-outdoor temperature
difference. The load is calculated as the steady state heat loss for the winter design condition:
Q = U A (Tr - Toa)
where:
Q
=
Transmission heating load, BTU/h or W.
U
=
Window overall U-value, BTU/h-sqft-F or W/sqm-K.
A
=
Area of window, sqft or sqm.
Tr
=
Room temperature, F or C. For the design heating load
analysis, the occupied heating thermostat
setpoint is used.
Toa
=
Outdoor air winter design temperature, F or C.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Load Calculations (Heating)
This help topic discusses door load calculations for design heating applications. Two components of door heat
loss are considered for design heating applications:
• Heat loss through the opaque portion of the door.
• Heat loss through the glass portion of the door.
Both load components are calculated as the steady state heat loss for the winter design condition:
Qd = Ud Ad (Tr - Toa)
Qg = Ug Ag (Tr - Toa)
where:
Ad
=
Area of opaque portion of door, sqft or sqm.
Ag
=
Area of glass portion of door, sqft or sqm.
Qd
=
Transmission heating load for opaque portion of door,
BTU/h or W.
Qg
=
Transmission heating load for glass portion of door, BTU/h
or W.
Ud
=
Page 27 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
Partition and Ceiling Load Calculations (Heating)
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
Infiltration Load Calculations (Heating)
28.0 Load Calculations ›› 28.4 Component Load Calculations for Design Heating ››
U-value for opaque portion of door, BTU/h-sqft-F or
W/sqm-K.
Ug
=
U-value for door glass, BTU/h-sqft-F or W/sqm-K.
Tr
=
Room temperature, F or C. For the design heating load
analysis, the occupied heating thermostat
setpoint is used.
Toa
=
Outdoor air winter design temperature, F or C.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Partition and Ceiling Load Calculations (Heating)
This help topic discusses partition and ceiling transmission load calculations for design heating applications.
These loads are the result of heat flow through partitions or ceilings adjacent to unconditioned or partially
conditioned regions. The load is computed as the steady-state heat loss through the partition or ceiling:
Q = U A (Tr - Tadj)
where:
Q
=
Partition or ceiling transmission heating load, BTU/h or W.
U
=
Partition or ceiling U-value, BTU/h-sqft-F or W/sqm-K.
A
=
Partition or ceiling area, sqm or sqft.
Tr
=
Room temperature, F or C. The occupied heating
thermostat setpoint is used for these
calculations.
Tadj
=
Temperature in adjacent unconditioned or partially
conditioned region, F or C.
For this calculation the value of Tadj is determined according to user specifications concerning how the
temperature varies in the adjacent region.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Infiltration Load Calculations (Heating)
This help topic discusses infiltration load calculations for design heating applications. Infiltration loads are the
result of uncontrolled leakage of air into and out of the building. These loads are due to the loss of building air
and the introduction of outdoor air into rooms in the building. As a result, the air exchange immediately affects
building loads.
Infiltration airflow is defined by the user on a CFM (L/s), CFM/sqft (L/s/sqm) or Air Change per Hour basis. In
the first case, infiltration airflow is directly known. In the other two cases, infiltration airflow must be calculated
Vi = (CFM/sqft or L/s/sqm) x (Gross Area of Exterior Walls in Space)
Vi = (Air Changes per Hour)(Af)(H)/(K)
In addition, the user has the opportunity to specify whether infiltration is considered for all hours of the day, or
only during the equipment "unoccupied" period hours. Because the design heating calculation is performed
using the occupied heating thermostat setpoint, and assuming the system operates and provides ventilation
air, this qualifies as an hour in the "occupied" equipment operating period. Therefore, infiltration is only
Page 28 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm
considered in design heating calculations when you specify that infiltration is to be considered for all hours of
the day.
Sensible and latent infiltration loads are computed as follows. Note that the latent heat loss is needed when
sizing humidification equipment.
Qs = ρa Cpa Vi K (Toa - Tr)
Ql = ρa hfg Vi K (ωoa - ωr)
where:
Af
=
Floor area for space, sqft or sqm.
Cpa
=
Heat capacity of air, 0.24 BTU/lbm-F or 1004.8 J/kg-K.
H
=
Average floor to ceiling height for space, ft or m.
hfg
=
Heat of vaporization of water, 1054.8 BTU/lbm or 2.4535
x10^6 J/kg.
K
=
Unit conversion factor,
=
60 min/hr for English units or
=
cubic meter/(1000 L) for S.I. Metric units.
ρa
=
Density of air , adjusted for altitude, lb/cuft or kg/cubic
meter.
Ql
=
Latent infiltration heat loss, BTU/h or W.
Qs
=
Sensible infiltration heat loss, BTU/h or W.
Toa
=
Outdoor air temperature at winter design condition, F or C.
Tr
=
Room temperature, F or C.
Vi
=
Infiltration airflow rate, CFM or L/s. Derived from "design
heating" specification.
ωoa
=
Outdoor air specific humidity calculated using the winter
design dry-bulb and coincident wet-bulb
temperatures, lb/lb or kg/kg.
ωr
=
Room specific humidity, lb/lb or kg/kg.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 29 of 29
28.0 Load Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6C1A.htm