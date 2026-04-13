24.0 Entering Cooling Towers
Cooling Tower Form Overview
24.0 Entering Cooling Towers ››
This chapter explains input data for heat rejection equipment such as cooling towers, dry coolers, and surface, well, or
river water.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Tower Form Overview
The Cooling Tower Properties window is used to define the operating characteristics for one set of heat rejection
equipment such as a cooling tower or dry cooler, or a heat rejection / heat source system such as geo, well or surface
water. This data is used in energy simulation calculations. Therefore this data is only available in the full HAP edition
and not in System Design Load.
The Cooling Tower Properties window contains three key components:
1. The Title Bar appears across the top of the window. It lists the name of the equipment whose data is being edited.
At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the window and contains multiple input items that describe the heat rejection
equipment. This area is divided into four parts:
a. Name. The first item on the left-side of the window defines a reference name for the heat rejection equipment
being entered.
b. Modeling Method. The next item on the left-side of the form allows the user to choose whether to model a
cooling tower, a dry cooler or use of geothermal, well or surface water as the heat sink or source.
c. Water Flow Rate. An additional item on the left-hand side of the window defines the water flow rate for the heat
rejection device or system.
Page 1 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
24.1 Inputs
24.0 Entering Cooling Towers ››
Cooling Tower Name
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
d. Performance Data: Inputs on the right-hand side of the form define the performance of the equipment. These
inputs change depending what kind of equipment is being modeled. The figure above shows data for a cooling
tower.
3. Command Buttons appear along the bottom of the window. Three buttons are provided:
a. Press OK to save the inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes. If you press Cancel while creating a
new tower, the data will not be added to your project.
c. Press Help to display this overview topic.
For more information about input items on the Cooling Tower Properties window, click the desired item below.
Name
Modeling Method
Water Flow Rate
Cooling Tower Data
Dry Cooler Data
Geo/Well/Surface Water Data
Cooling Tower Features. Finally, HAP provides useful features for:
Creating new cooling towers.
Editing an existing cooling tower.
Printing cooling tower data.
Deleting cooling towers.
Copying a cooling tower.
Duplicating a cooling tower.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data for heat rejection equipment;
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Tower Name
This item is a reference name for the heat rejection equipment. It will appear elsewhere in the program on selection
lists and reports. The reference name appears:
a. In the list of available heat rejection equipment on the HAP main window.
b. In the list of available heat rejection equipment when linking heat rejection equipment to a plant or air system.
c. On input data reports for heat rejection equipment, plants and systems.
Therefore, it is important to use a descriptive name. Typically the name includes information about the make and model
of the equipment, its heat rejection capacity or its water flow rate.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 2 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
Modeling Method
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
Water Flow Rate
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
Cooling Tower Model Data
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
Modeling Method
This item is used to specify whether data is being entered for a cooling tower, a dry cooler or for geo/well/surface.
1. Cooling Tower Model. Choose this option to enter data for a cooling tower. The program will use a detailed
thermodynamic model to calculate tower performance for off design and part-load operation. Inputs to the model
include design wet-bulb, range, approach and fan power.
In a cooling tower condenser water is sprayed on splash bars or film-type fill. A fan draws ambient air through the
tower in a cross-flow or counter-flow manner. Contact between the air and water results in evaporation and sensible
heat transfer which cools the water before it returns to the HVAC unit.
2. Dry Cooler. Choose this option to enter data for a dry cooler. The program will use a thermodynamic model to
calculate performance of the dry cooler at off design and part-load operation. Inputs to the model include design
dry-bulb, range, approach, airflow and fan power.
In a dry cooler condenser water flows through a water-to-air heat exchanger. Fans draw air across the heat
exchanger so the water is cooled by sensible heat transfer..
3. Geo/Well/Surface. Choose this option to model use of geothermal, well or surface water as the heat source or sink
for the HVAC equipment. With this method the user specifies the average source temperature for water for each
month of the year. The program uses that monthly average value as the entering water temperature for the HVAC
equipment.
Once a modeling method is chosen, the appropriate inputs appear on the right side of the form.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Water Flow Rate
This item defines the fluid flow rate for the heat rejection device. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the cooling equipment capacity. This
option should only be used for heat rejection equipment linked to a chiller plant or a WSHP, GWSHP, or GSHP
system. When linking a geo / well / surface system to a changeover plant or a central heat pump plant, the gpm or
Delta-T options should be used instead.
3. Delta-T - The program will calculate gpm automatically based on the design heat rejection or heat extrction rate and
the specified delta-T.
Water flow rate is used in simulation calculations. Flow and heat rejection together determine the range for the heat
rejection equipment which is a key value that drives the performance of a cooling tower or dry cooler at design
conditions. The design condition is the anchor point for calculation heat rejection equipment performance at off design
and part load conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Tower Model Data
Page 3 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
When modeling a cooling tower, the program uses a detailed thermodynamic algorithm to calculate tower performance
for off-design and part-load conditions. This performance algorithm requires 5 to 7 inputs. Typically these values are
obtained from equipment selection software supplied by a cooling tower manufacturer or from catalog data.
1. Design Wet-Bulb defines the outdoor wet-bulb temperature for the full load design point for the cooling tower.
2. Range at Design defines the difference between the inlet and outlet water temperatures at the tower’s full load
design point.
3. Design Approach defines the approach between the temperature of water leaving the tower and the outdoor wet-
bulb temperature for the tower’s full load design point.
Together these first three inputs are used to define full load heat transfer effectiveness of the cooling tower. Once full
load performance is known, performance at off-design and part-load conditions can be calculated using the
thermodynamic algorithm.
4. Full Load Fan kW defines the fan motor input power at the tower’s full load design point. This item can be entered
in two ways: (1) as a motor input kW or (2) as a power ratio expressed as kW per ton of heat rejection (kW per kW
of heat rejection in Metric units). To choose the units of measure for this input, use the drop down list to the right of
the input item.
When selection data for a specific cooling tower is being used, the fan motor input power will typically be known and
can be entered directly.
When specifics for the cooling tower are not known, it is usually more convenient to enter a fan power ratio. Based
on a survey of manufacturer’s catalogs, the ratio of fan power to heat rejection generally ranges from 0.016 to 0.112
kW per ton of heat rejection (or 0.006 to 0.043 kW per kW of heat rejection in Metric units).
5. Fan Control. Four control options are provided for maintaining water leaving the tower at the minimum setpoint for
times of low wet-bulb or low load. The four options listed in the drop-down list are:
a. Water Bypass - Warm inlet water will be bypassed around the tower to blend with tower outlet water to produce
the required temperature. When using water bypass, the tower fan continues to run at full speed.
b. Fan Cycling - The tower fan will cycle ON and OFF, thereby reducing the tower airflow and the heat transfer
effectiveness to produce the required return water temperature.
c. 2-Speed Fan – The tower fan uses a two speed fan motor. For conditions where high airflows are sufficient to
maintain minimum setpoint, the fan will cycle between high and low speed. For conditions where low airflows are
sufficient to maintain minimum setpoint, the fan will cycle between low speed and OFF.
d. Variable Speed Fan – The tower fan uses a variable speed drive. Motor speed is adjusted to produce the airflow
rate necessary to maintain the minimum setpoint temperature.
6. Fan Electrical Efficiency – This item is only required when the 2-Speed Fan or Variable Speed Fan control options
are chosen. For 2-Speed Fan control, specify the motor electrical efficiency. For Variable Speed Fan, specify the
Page 4 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
Dry Cooler Data
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
overall electrical efficiency which is a combined value accounting for both the motor electrical efficiency and the VFD
drive efficiency.
For applications in the United States where electrical efficiency is not known from tower selection data, it can be
estimated from the minimum efficiency requirements dictated by the Energy Policy Act of 1992. Click here for
details.
7. % Airflow at Low Fan Speed – This item is only required when 2-Speed Fan control is selected. Specify the airflow
at low fan speed as a percentage of the high speed airflow. Typically low fan speed is either 67% or 50% of high
speed airflow.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Dry Cooler Data
When modeling a dry cooler, the program uses a thermodynamic algorithm to calculate tower performance of the dry-
cooler's water-to-air heat exchanger for off-design and part-load conditions. This algorithm requires five inputs.
Typically these values are obtained from equipment selection software supplied by a dry cooler manufacturer or from
catalog data.
1. Design Dry-Bulb defines the outdoor air dry-bulb temperature for the full load design point for the dry cooler.
2. Range at Design defines the difference between the inlet and outlet water temperatures at the dry cooler's full load
design point.
3. Design Approach defines the approach between the temperature of water leaving the dry cooler and the outdoor air
dry-bulb temperature for the dry cooler's full load design point.
4. Full Load Airflow defines the airflow through the water-to-air heat exchanger in the dry cooler at the full load design
condition. Airflow can be defined in two ways: (1) in terms of air flow per unit heat rejection capacity (CFM/ton of
heat rejection or L/s/kW of heat rejection), or (2) as an airflow quantity (CFM or L/s). Units of measure are selected
using the drop down list to the right of the input item.
When selection data for a specific dry-cooler is being used, the airflow will typically be known and can be entered
directly. When specifics for the dry-cooler are not known, it is usually more convenient to enter an airflow ratio.
Together these first four inputs are used to define full load heat transfer effectiveness of the dry cooler. Once full load
performance is known, performance at off-design and part-load conditions can be calculated using the thermodynamic
algorithm.
Page 5 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
Geo / Well / Surface Water Data
24.0 Entering Cooling Towers ›› 24.1 Inputs ››
24.2 Common Tasks
24.0 Entering Cooling Towers ››
Creating a New Cooling Tower
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
5. Full Load Fan kW defines the fan motor input power at the dry cooler's full load design point. This item can be
entered in two ways: (1) as a motor input kW or (2) as a power ratio expressed as kW per ton of heat rejection (kW
per kW of heat rejection in Metric units). To choose the units of measure for this input, use the drop down list to the
right of the input item.
When selection data for a specific dry-cooler is being used, the fan motor input power will typically be known and
can be entered directly. When specifics for the dry-cooler are not known, it is usually more convenient to enter a fan
power ratio.
When the leaving water temperature for the dry cooler reaches the minimum setpoint temperature, HAP assumes
the dry cooler fans are cycled to hold leaving water at the setpoint temperature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Geo / Well / Surface Water Data
When geothermal, well or surface water is used as the heat source or sink for HVAC equipment, average source water
temperatures are defined for each month of the year. During energy simulations, the program assumes source water at
this temperature is available for all equipment operating hours.
Data is entered in a table in which each row contains data for a different month. The left-hand column lists the month
name. The right-hand column lists the average source water temperature for the month.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with heat rejection equipment input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm
Editing an Existing Cooling Tower
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
Printing Cooling Tower Inputs
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
Deleting Cooling Tower Inputs
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
Copying a Cooling Tower
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
Duplicating a Cooling Tower
24.0 Entering Cooling Towers ›› 24.2 Common Tasks ››
Creating a New Cooling Tower
Please see Creating a New Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Cooling Tower
Please see Editing an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Cooling Tower Inputs
Please see Generating Input Data Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Cooling Tower Inputs
Please see Deleting Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Cooling Tower
Please see Copying Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Cooling Tower
Please see Duplicating an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 7
24.0 Entering Cooling Towers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhA1D0.htm