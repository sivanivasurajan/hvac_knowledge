5.0 System Design Applications
Overview for System Design Applications
5.0 System Design Applications ››
Applications Involving Single-Zone HVAC Units
5.0 System Design Applications ››
This chapter provides guidance for using HAP for common HVAC system design applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for System Design Applications
The following series of help topics explains how to use the program for common system design applications.
Topics in the "Getting Started" section of the help system contained general discussions of how to use the
program to design systems . However, the program can be used in design work involving a wide variety of
different types of HVAC systems and equipment. Procedures for using the program for these applications are
not always obvious, especially for new program users. Therefore, the following topics summarize how the
program can be used for four common categories of design applications:
• Sizing single-zone HVAC units .
• Sizing terminal HVAC units such as fan coils.
• Sizing multiple-zone HVAC systems .
• Sizing cooling and heating plants.
Discussions will dwell on modeling strategies and procedures for generating sizing information. In each case it
is assumed the reader is familiar with the basic program operating procedures . Further, it is assumed input
data has been gathered and weather, schedule, wall, roof, window, door and shading data has already been
entered. Therefore, entry of this data will not be covered in the application discussions.
Finally, this section of the help system also contains a topic which discusses troubleshooting strategies
required when investigating program results.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Applications Involving Single-Zone HVAC Units
Introduction. Many design applications involve single-zone HVAC equipment. These include small buildings
with open areas that can be properly air-conditioned with one single-zone unit, or regions of a larger building
served by separate single-zone units. These applications generally fall into two categories:
• Applications involving rooftop or vertical packaged equipment. However, it could also involve
applications with split DX units and central station air handlers.
• Applications involving terminal units such as hydronic fan coils, DX fan coils, packaged terminal air
conditioners (PTACs) and water source heat pumps (WSHPs).
Applications in the first category will be discussed in this help topic. A separate help topic describes how to
analyze terminal unit systems .
Analysis Strategy. To size single-zone HVAC units with the program, each HVAC unit must be defined as a
separate air system. When calculations are performed, reports will be generated with sufficient information to
size the cooling and heating coils, the unit fan and any system ductwork. Considerations for this analysis are
discussed below.
1. Defining Spaces. Spaces can represent each room in the area served by the HVAC unit. This will allow
load and airflow sizing data to be calculated on a room-by-room basis as well as on a zone basis. If your
Page 1 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Applications Involving Terminal Units
5.0 System Design Applications ››
objectives for the design calculation do not require a room-by-room sizing analysis, then one space
representing the entire region served by the unit can be defined instead.
2. Defining The Air System. One air system must be defined for each single-zone HVAC unit to be sized.
Typically units will be constant volume, so the "Single Zone CAV" system option should be used and the
appropriate system attributes should be defined. During air system inputs, the spaces contained in the zone
served by the unit are specified. When a space is used to represent the entire building or the entire region
served by the unit, the zone will include only one space. When spaces represent separate rooms in the
region served by the unit, the zone will contain a group of spaces.
3. Generating System Design Reports. First choose the air systems to be sized. In cases where multiple
single-zone units are involved, it may be more efficient to enter the air system data for all the HVAC units,
and then generate reports all in one batch. The program provides capabilities for doing this.
When choosing outputs, select the Air System Sizing Summary and the Zone Sizing Summary. The Air
System Sizing Summary provides data for sizing and selecting the supply fan and central cooling and
heating coils. This data includes the design supply airflow rate, the design cooling and heating coil loads,
coil selection parameters and useful check figures. The Zone Sizing Summary provides information for
sizing space supply diffusers, zone and space ductwork and any zone heating units or reheat coils.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Applications Involving Terminal Units
Introduction. This help topic discusses applications involving a second category of single-zone HVAC units.
This category of equipment includes packaged and split terminal air conditioners, hydronic fan coil units,
induction beams, active chilled beams, variable refrigerant flow (VRF) indoor units and water source heat
pumps (WSHPs) which are used to condition separate rooms or groups of rooms. Examples include units
serving separate offices in an office building, separate guest rooms in a hotel, or classrooms in a school
building. Applications involving these types of equipment typically require that a large number of units be
sized. To assist in this task, the program provides special features for efficiently entering system information
and producing sizing data.
Analysis Strategy. Rather than defining one air system per single-zone HVAC unit as is done for rooftop units
and central AHUs, the program allows one "air system input" to represent multiple HVAC units. This feature is
available when using the Packaged DX Fan Coil, Split DX Fan Coil, 2-Pipe Fan Coil, 4-Pipe Fan Coil, WSHP,
GWSHP, GSHP, VRF, Induction Beam, or Active Chilled Beam air system types. The program also produces
streamlined output for sizing this equipment. These features help minimize input effort and the quantity of
output produced. Considerations for the analysis are summarized in the following paragraphs.
1. Defining Spaces. A space should represent a single room when your design analysis requires room-by-
room sizing data. When this is not necessary, each space can represent the entire area served by one
HVAC unit. In many applications, each HVAC terminal unit will serve a single room, such as a fan coil in a
hotel room, so the space must represent a single room in these cases.
A more important consideration in this analysis is minimizing the number of spaces and units that are
defined in order to save time and effort. In most applications it is not necessary to define one space and one
HVAC unit for every terminal unit in the building. For rooms with the same sizes and patterns of loads, it
may be possible to size an HVAC unit once, and then use the same unit in multiple rooms. For example,
guest rooms on the same exposure of a hotel might all be the same size, use the same wall and window
construction and experience the same internal loads. One space input and system sizing calculation for a
typical guest room might suffice for selecting units for 10 or even 100 guest rooms in this situation. When
considering how to reduce the number of units analyzed, remember to evaluate all factors that affect loads.
For example, separate calculations must be performed for two rooms of the same size on the same
exposure if one is on the top floor and the other is on an intermediate floor, since only one has a roof
exposure.
Page 2 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Applications Involving Multiple-Zone HVAC Systems
5.0 System Design Applications ››
2. Defining the Air System. When entering air system data,specify Equipment Type as Terminal Units and
then choose the Packaged DX Fan Coil, Split DX Fan Coil, 2-Pipe Fan Coil, 4-Pipe Fan Coil, WSHP,
GWSHP, GSHP, VRF, Induction Beam, or Active Chilled Beam system type.
When one of these system options is chosen, the program allows multiple terminal HVAC units to be
defined in one air system input. In addition, outdoor ventilation can be supplied either directly to the terminal
unit from outdoors, or by a Dedicated Outdoor Air System (DOAS). When a DOAS unit is used, the
temperature and humidity of air delivered to the terminal units will affect coil loads for the terminal HVAC
units. This interaction between DOAS and terminal units is considered in program calculations.
3. Generating System Design Reports. First choose the air system containing the terminal unit data. When
choosing sizing reports, select the Zone Sizing Summary report. If ventilation air is provided via a Dedicated
Outdoor Air System (DOAS), also select the Air System Sizing Summary report.
The Zone Sizing Summary provides data for sizing cooling coils, heating coils, fans and airflow for each
terminal unit and also airflow to individual spaces served by the terminal units. If an HVAC terminal unit
serves two or more spaces, this space airflow data will be essential for sizing space diffusers and ductwork.
The Air System Sizing Summary will provide sizing data for the DOAS unit, if one is used. This includes
information for sizing the airflow, fan motor, cooling coil and heating coil in the DOAS unit.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Applications Involving Multiple-Zone HVAC Systems
Introduction. Many design projects involve a central packaged unit or a built-up air handling unit which
provides conditioned air to many different regions in a building. Each of these regions has its own thermostat
making this a multiple-zone HVAC system.
Analysis Strategy. To design multiple-zone HVAC systems with the program, each packaged unit or AHU
must be defined as a separate air system. When design calculations are performed, output data will provide
sizing information for all cooling and heating coils, fans and terminals in the system. Considerations for this
analysis are described below.
1. Organizing Zones & Defining Spaces. How to zone the system is one of the first decisions required when
organizing the analysis. Zoning usually depends on the building use and layout, and the HVAC system
controls. The goal is to provide a thermostat for each region of the building requiring specific temperature
control. Since the program defines a zone as the region served by one thermostat, the location of
thermostats in the system dictates how rooms will be grouped into zones.
Examples: Offices on a south exposure of a building might be included in one zone since they are of similar
size and experience the same patterns of loads. A conference room on the same exposure might have a
separate thermostat since its pattern of loads will differ from those of the offices on the same exposure.
Further, north and south offices in a building would typically be assigned to separate zones since offices on
each exposure experience significantly different patterns and magnitudes of loads.
Once zoning decisions have been made, all spaces included in each zone must be defined. As discussed in
previous sections, each space should represent a separate room when room-by-room load and airflow
sizing data is required. When a room-by-room sizing analysis is not required, each space can represent the
entire area in one zone.
Another important consideration when entering spaces is how to minimize input effort. When each space
represents a single room, the brute force approach is to define a separate space for every room in the
building. However, in many cases series of identical rooms (same size, same pattern and magnitude of
loads) will exist in a zone. In these situations, one of the identical rooms can be defined as a space once.
Later during air system input, a multiplier can be applied to this space to account for the total number of
rooms present in the zone. This reduces input effort.
Page 3 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Applications Involving Cooling and Heating Plants
5.0 System Design Applications ››
2. Defining The Air System. One air system must be entered to represent the multiple-zone HVAC system.
The program provides options for defining and sizing many different types of constant volume and variable
volume multiple-zone HVAC systems. Define the appropriate attributes for the system being designed.
Entering air system data also requires defining the zones served by the system. The number of zones is
specified first. Next, spaces included in each zone are identified by specifying the quantity of each space
included in a zone. In a simple case in which a zone contains one space, a quantity of 1 would be defined.
In another case, a zone might contain six identical offices. If one space has been defined to represent one
of these offices, the zone would contain one space but the space would be assigned a quantity of 6. Finally,
a zone might contain a group of different rooms each defined as a separate space. In this case, the zone
would contain multiple spaces.
3. Generating System Design Reports. First choose the air system to be sized. When designing multiple air
systems in a large building, it may be more efficient to define all the systems and then generate reports for
all in one batch. The program provides features for doing this.
On the report selection screen, choose the Air System Sizing Summary and Zone Sizing Summary options.
The Air System Sizing Summary lists maximum coil loads for all central cooling and heating coils in the
system, required airflow rates for central supply and return fans, coil selection parameters, and useful check
figures. This data can be used to select coils and fans for the system. The Zone Sizing Summary provides
data for sizing zone terminals such as VAV boxes, zone reheat coils, zone baseboard or fan coil heating
units and fan powered mixing boxes, as well as space diffusers and ductwork.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Applications Involving Cooling and Heating Plants
Introduction. System design work can also require sizing central chilled water, hot water and/or steam plants.
In these situations a plant might serve several central air handling units in a large building and/or a large
number of hydronic fan coil units located in different rooms of a building. In either case, the program provides
capabilities for sizing both the air handling and terminal units as well as the plant equipment. This topic
describes the analysis procedure required.
Analysis Strategy. Performing this analysis requires developing inputs for all the air systems served by the
plant first and then generating system sizing reports. Next, a chilled water plant is created and systems having
chilled water cooling coils are linked to it. A hot water or steam plant is also created and systems having hot
water or steam heating coils are linked to it. For cases where reversible heat pumps in a changeover plant are
used, a changeover plant is created and linked to the systems having both chilled water and hot water coils.
In cases where a heat recovery plant is used, a single heat recovery plant is created and linked to the
systems having chilled water and hot water coils. Finally, plant design reports for the plants are generated.
Considerations required in the analysis are discussed below.
1. Defining Air Systems. The same principles discussed earlier in this chapter for single-zone and multiple-
zone systems are required when defining air systems for this application. In previous discussions the choice
of an equipment type and the specification of the cooling and heating sources for coils were not critical.
However, when sizing plant equipment, these details are important.
Cooling coils served by the plant must have chilled water designated as the cooling source. Chilled water is
the default cooling source when the systems equipment classification is Chilled Water AHU, and when
using the 2-Pipe Fan Coil, 4-Pipe Fan Coil, Induction Beam or Active Chilled Beam system types. When
using systems in the Undefined equipment class, the cooling source is "Any" and can be used for chilled
water plant design calculations.
Heating coils served by the plant must have hot water or steam designated as the heating source. When
using systems in the Undefined equipment class, the heating source is "Any" and can be used for both hot
water and steam design calculations.
Page 4 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Air systems utilizing both hot water and chilled water coils can be configured with specific changeover
settings. These settings determine what criteria the air system will use to switch between heating and
cooling modes of operation, and as a result may affect the peak loads used for equipment sizing.
Special Consideration. Finally, a key requirement of the plant analysis is that the total load imposed on
equipment must be considered. Because techniques for minimizing work when analyzing terminal
equipment such as fan coils involves analyzing duplicate units only once, this can cause problems in
generating correct plant load totals.
Example: A hotel contains 220 guest rooms served by 4-pipe fan coils. 100 of these rooms are on one face
of the building and have identical size and load patterns. Another group of 100 are on the opposite face of
the building and also have identical size and load patterns. The remaining 20 rooms must be modeled
separately because each has unique characteristics. To save time, we could model this situation with one
4-pipe fan coil system having 22 zones - 1 zone representing one unit out of the first group of 100 identical
zones, 1 zone representing one unit out of the second group of 100 zones and one zone each for the
remaining 20 unique zones. This would vastly reduce effort required to size and select the fan coils.
However, if we linked this fan coil air system to a chilled water or hot water plant, we would have a problem
since loads would be under counted. We have only accounted for the loads of 22 out of the 220 fan coil
units in the building.
To correct this problem, an alternate approach would be used. Define three 4-pipe fan coil air systems. The
first contains 20 zones, one for each of the 20 unique hotel zones. The second contains 1 zone
representing a single zone in the first group of 100 identical zones. The third system contains 1 zone
representing a single zone in the second group of 100 identical zones. System sizing reports can be run as
before to generate data needed to select the fan coil units.
To size the chilled water plant, the three fan coil air systems would be linked to the plant. The system
containing the 20 unique zones would be assigned a system multiplier of 1. The single-zone systems
representing each group of 100 identical zones would each be assigned a system multiplier of 100. In this
way the total load for all 220 fan coil units would be accounted for and the chiller would be properly sized.
The same sort of approach would be used when linking the fan coil air systems to the hot water plant.
2. Generating System Design Reports. Once air systems have been defined, generate system design
reports for each. As discussed in earlier sections, the system design reports provide information for sizing
cooling coils, heating coils, fans, diffusers and ductwork.
If system sizing data is not a concern (e.g., if you are performing a preliminary block load calculation), this
step can be skipped. The plant sizing calculations performed as part of step 4 will automatically run system
sizing calculations first if system sizing results do not already exist.
3. Defining Plants.
a. For a chilled water plant, create one plant and choose "Generic Chilled Water Plant" as the plant type.
Then specify the air systems served by this plant. For each system linked to the plant, HAP will assume
that all chilled water coils, and coils whose cooling source is "Any" are served by the plant.
b. For a changeover plant using reversible chillers, create one plant and choose "Generic Changeover
Plant" as the plant type. Then specify the air systems served by this plant. For each air system linked to
the plant, HAP will assume that all cooling coils with chilled water or "any" as the source, and all heating
coils with hot water or "any" as the source are served by the plant.
c. For a heat recovery plant, create one plant and choose "Generic Heat Recovery Plant" as the plant type.
Then specify the air systems served by this plant. For each air system linked to the plant HAP will
assume that all cooling coil loads with chilled water or "any" as the source, and all heating coils with hot
water or "any" as the source are served by the plant. There is also the option to specify service water
heating load profiles for the plant.
c. For hot water or steam plant create one plant. For a hot water plant, choose "Generic Hot Water Plant" as
the plant type. For a steam plant, choose "Generic Steam Plant" as the plant type. Then specify the air
systems served by this plant. In a hot water plant HAP will assume all hot water coils and coils with a
heating source of "any" are served by the plant. In a steam plant HAP will assume that all steam coils
and coils with a heating source of "any" are served by the plant. For hot water plants there is also the
option to specify service water heating load profiles for the plant.
Page 5 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Troubleshooting Strategies
5.0 System Design Applications ››
As mentioned in item 1 above, system multipliers can be used when an air system represents one of a
number of identical systems or units served by any of these plant types.
For HAP users who will later run energy analyses, "Generic" plants can later be converted into specific plant
types. When converting plants, system selection data is preserved.
4. Generating Plant Design Reports. Finally, generate design reports for the plants.
a. For the chilled water plants, choose the Cooling Plant Sizing Summary report. This report lists the peak
cooling plant load as well as the coincident loads for all systems served by the chiller.
b. For a hot water plant, choose the Heating Plant Sizing Summary report. This report lists the peak heating
plant load as well as coincident loads for systems served by the plant.
c. For changeover plants using reversible chillers select both the Cooling Plant Sizing Summary and the
Heating Plant Sizing Summary to obtain both cooling and heating sizing data.
d,.For heat recovery plants select both the Cooling Plant Sizing Summary and the Heating Plant Sizing
Summary to obtain both cooling and heating sizing data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Troubleshooting Strategies
This help topic describes general strategies used to investigate load calculation and system sizing results.
These investigations may be necessary when diagnosing problems with results or simply learning more about
results generated by the program. Due to the wide range of situations requiring diagnosis, it is not possible to
discuss troubleshooting procedures for specific applications. Rather, general strategies useful in a variety of
situations will be described below.
1. Investigate Input and Output Data. When a question about results arises, first generate reports of all input
data and pertinent load calculation results. Inspect and compare data on the different printouts. Sometimes
unusual sizing results are caused by inadvertent input errors.
2. Research Input Definitions and Calculation Procedures. In many cases, a thorough knowledge of how
the program uses certain inputs and performs its load and sizing calculations is necessary to understand
program results. Topics in the on-line help system provide definitions of all program inputs and explain how
inputs are used by the program. Documentation topics in the help system explain calculation procedures.
3. Perform Comparative Analysis. When a more detailed investigation is needed various types of
comparative analyses can be helpful. The success of this technique depends on the user's ingenuity,
knowledge of system and load behavior, and knowledge of the program. Two common applications for
comparative analysis are provided below to serve as examples.
a. Single-Hour vs Multiple Hour Data. Frequently, unusual results found on the Air System Sizing
Summary or Zone Sizing Summary reports can be successfully diagnosed by comparing data with full
24-hour load profiles.
Example: Suppose the Air System Sizing Summary report shows that the peak coil load occurs at 7am.
Since peak coil loads usually occur in the mid to late afternoon, this is an unexpected result. One way to
diagnose this result is to generate the Hourly Air System Design Day Loads report which lists cooling coil
loads for all hours in a specific month. By comparing coil loads at different times of day, a user can gain
insight into why the maximum load occurs in the early morning. Sometimes this type of result will be due
to an unusually large pulldown load which causes loads during the first few hours of operation in the
occupied period to exceed coil loads during the mid-afternoon hours. Such results could be due to
legitimate system behavior or could be due to errors in modeling building heat gains or system controls.
b. Air System Variations. When an air system containing several components and accessory controls
yields unusual sizing results, a useful diagnostic strategy is to run calculations for variations of the
system to determine the effect of each component or control.
Page 6 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm
Example: An air system including dehumidification control, a preheat coil and a ventilation reclaim device
yields unusual sizing results. To diagnose this problem, make four copies of the air system. From one
copy remove all three supplemental components and controls. This system will represent a base case.
For the other three copies include each of the components separately. For example, one system would
only include the dehumidification control. Another would include the preheat coil only, and so forth.
Finally, run sizing calculations for each for the four system variations. A comparison of results from these
systems should demonstrate the individual effect of each component control. Often this points out the
reason for the original results that were questioned. When it does not, it may be necessary to use 24-
hour load profile reports to evaluate differences in system performance, or to run further test cases using
combinations of two components at a time (e.g., dehumidification and the preheat coil together, the
preheat coil and ventilation reclaim, etc...).
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 7
5.0 System Design Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh64FC.htm