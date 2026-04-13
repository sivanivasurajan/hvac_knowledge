25.0 Entering Boilers
Boiler Form Overview
25.0 Entering Boilers ››
This chapter explains input data for boilers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Form Overview
The Boiler Properties window is used to define the operating characteristics of one hot water or steam boiler. The boiler will later be
linked to a hot water or steam plant for use in energy simulations. Therefore, this data is only available in the full HAP edition and not
in System Design Load.
The Boiler Properties window contains three key components:
1. The Title Bar appears across the top of the window. It lists the name of the boiler whose data is being edited. At the right end of
the title bar is a button for closing the window.
2. The Working Area is in the center of the window and contains input items that describe the boiler. This area is divided into four
parts:
a. Boiler Description defines the boiler type and fuel or energy source as well as a reference name for the boiler.
b. Boiler Full Load Data describes the boiler full load capacity, design values of hot water supply temperaure (HWST), hot water
flow rate and efficiency, and accessory power for devices such as blower fans and oil pumps.
c. Part Load Model specifies which of four types of part-load performance models are used to calculate off-design and part-load
performance of the boiler..
d. Part Load Performance. If a user-defined part-load curve is used to model the boiler, the % load versus efficiency curve is
entered in this table that appears on the right side of the form (not show in screen image above).
3. Command Buttons appear along the bottom of the window. Three buttons are provided:
a. Press OK to save the boiler inputs and return to the main program window.
Page 1 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm
25.1 Inputs
25.0 Entering Boilers ››
Boiler Name
25.0 Entering Boilers ›› 25.1 Inputs ››
Fuel or Energy Type
25.0 Entering Boilers ›› 25.1 Inputs ››
b. Press Cancel to return to the main program window without saving changes. If you press Cancel while creating a new boiler, the
new boiler will not be added to your project.
c. Press Help to display this overview topic.
For more information about input items on the Boiler Properties window, click the desired item below.
Boiler Name
Fuel or Energy Type
Boiler Type
Boiler Capacity
Boiler Design HWST
Boiler Hot Water Flow Rate
Boiler Efficiency
Boiler Accessories
Boiler Part Load Model
Boiler Part Load Performance Data
Boiler Features. Finally, HAP provides useful features for:
Creating new boilers.
Editing an existing boiler.
Printing boiler data.
Deleting boilers.
Copying a boiler.
Duplicating a boiler.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Boiler Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Name
This item is a reference name for the boiler. It will appear elsewhere in the program on selection lists and reports. The reference
name appears:
a. In the list of available boilers on the HAP main window.
b. In the list of available boilers when linking a boiler to a hot water or steam plant.
c. On input data reports for boilers and plants.
Therefore, it is important to use a descriptive name. Typically the name includes information about the make and model of the boiler
and its full load capacity.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fuel or Energy Type
Select the fuel source or energy type for the boiler. Choices include natural gas, fuel oil, propane and electric resistance.
Page 2 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm
Boiler Type
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Capacity
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Design HWST
25.0 Entering Boilers ›› 25.1 Inputs ››
During energy simulations the fuel type or energy source will determine where boiler energy use is tabulated for energy cost
calculations. For example, if the fuel type is natural gas, boiler energy use will be added to the natural gas consumption profile for the
building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Type
This input specifies whether the boiler being defined is a hot water boiler or a steam boiler. When "hot water boiler" is selected, input
items that are relevant for that type of boiler, such as hot water flow and hot water supply temperature will be enabled. When "steam
boiler" is selected, input items not relevant for that type of boiler will be disabled.
The choice of boiler type also determines which part load models are available for selection. For a hot water boiler, four part load
modeling options are offered:
Constant Efficiency
User Defined Curve - Efficiency = f(PLR)
Non-Condensing Boiler - Efficiency = f(PLR, HWST)
Condensing Boiler - Efficiency - f(PLR, HWST)
For a steam boiler, two part load modeling options are offered:
Constant Efficiency
User Defined Curve - Efficiency = f(PLR)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Capacity
This input defines whether the boiler capacity will be automatically calculated by the program or will be specified directly.
For preliminary design or LEED applications where it is necessary to have the capacity automatically determined, place a check in the
"Autosize" box. When this boiler is later linked to a plant using the "Autosize Capacities" option, the program will automatically size the
boiler based on peak plant load plus an oversizing factor specified in the plant inputs.
For applications where the boiler capacity is known, leave the "Autosize" box unchecked and specify the Gross Output of the boiler at
its full load design condition.
Note that the choice of "Autosize" is important. If the "Autosize" box is checked, then this boiler can only be linked to a plant which
uses the "Autosize Capacity" option. If the "Autosize" box is not checked, then the boiler can only be linked to a plant which uses the
"User Defined Capacities" option. Once a boiler is linked to a plant this input should not be changed. Changing this value makes the
boiler incompatible with its plant and will prevent you from running an energy simulation for the plant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Design HWST
Specify the design hot water supply temperature (HWST) for the boiler. This input has two primary uses in the energy simulation:
1. If a boiler plant uses hot water supply temperature reset, this design HWST plays a role in calculation of the operating supply
temperatures for the system.
2. It has an affect on boiler energy performance when using the non-condensing and condensing boiler modeling options. Both of
these models evaluate boiler efficiency as a function of both part-load ratio and hot water supply temperature delivered by the
boiler.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 3 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm
Boiler Hot Water Flow Rate
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Efficiency
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Accessories
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Part Load Model
25.0 Entering Boilers ›› 25.1 Inputs ››
Boiler Hot Water Flow Rate
This item defines the water flow rate for a hot water boiler at its design condition. This value is typically obtained from boiler selection
results or from catalog data. The flow can be defined in one of two ways:
1. gpm or L/s - The flow is directly entered.
2. Delta-T - The program will automatically calculate the flow based on the gross output of the boiler and this delta-T.
This flow rate is used in hot water distribution system calculations during a boiler plant simulation.
1. It is used in the calculation of full load pump input power for both constant speed and variable speed pumping applications.
2. For constant speed, constant flow applications, it defines the flow rate for all boiler operating hours.
3. For variable speed applications, it helps establish the minimum flow level for the boiler. For example, if minimum flow is defined
as 70%, minimum flow is calculated as 70% of the hot water flow rate you specify here.
When defining an auxiliary boiler for a WSHP loop, this flow rate is not used. Instead the flow rate defined for the cooling tower
serving the WSHP system determines the loop flow.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Efficiency
This input defines the overall efficiency for the boiler at the full load design condition. It is calculated as Gross Output divided by
Energy Input. For combustion boilers this efficiency accounts for combustion, flue and jacket losses in the boiler. For electric boilers it
accounts only for jacket losses.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Accessories
This item is used to account for electrical equipment such as combustion blower fans and fuel oil pumps that are sometimes used with
combustion boilers. If the boiler is electric, or is combustion but does not use these devices, enter a zero value.
When the boiler is simulated, it is assumed the accessory electric equipment cycles with the boiler. For example, if accessory power
of 0.5 kW is specified and the boiler is operating at a part load ratio of 60%, the simulation will calculate 0.5 kW x 0.60 = 0.3 kW for
the accessory equipment power.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Part Load Model
This input specifies which method of modeling boiler off-design and part-load performance will be used in energy simulation
calculations. For a hot water boiler, four options are offered:
1. Constant Efficiency - This is a simplified model in which the "overall efficiency" specified for the boiler is used for all operating
hours. Therefore performance is not affected by part-load ratio or hot water supply temperature.
2. User Defined Curve - Efficiency = f(PLR) - This is a simplified model in which the user defines a table of efficiencies at 10% steps
of part-load ratio to define boiler performance. Therefore boiler performance is only considered as a function of part-load ratio.
Other factors such as hot water supply temperature are not considered.
3. Non-Condensing Boiler - Efficiency = F(PLR, HWST) - With this option HAP uses an EnergyPlus curve fit performance model
representing a non-condensing boiler. This is a 2-dimensional model in which performance is a function of both part-load ratio and
hot water supply temperature (HWST).
Page 4 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm
Boiler Part Load Performance Data
25.0 Entering Boilers ›› 25.1 Inputs ››
25.2 Common Tasks
25.0 Entering Boilers ››
Creating a New Boiler
25.0 Entering Boilers ›› 25.2 Common Tasks ››
Editing an Existing Boiler
25.0 Entering Boilers ›› 25.2 Common Tasks ››
4. Condensing Boiler - Efficiency = F(PLR, HWST) - With this option HAP uses an EnergyPlus curve fit performance model
representing a condensing boiler. This is a 2-dimensional model in which performance is a function of both part-load ratio and hot
water supply temperature (HWST).
For a steam boiler, only the first two options above are offered. The condensing and non-condensing models are specifically for hot
water boilers and therefore are not relevant for steam applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Boiler Part Load Performance Data
When the "User-Defined Curve - Efficinecy = f(PLR)" option is selected, a table of % load versus boiler efficiency data must be
supplied. As shown in the figure below, overall boiler efficiency is defined for 10% increments of load. The 100% value is copied from
your earlier input of Overall Efficiency.
1. "% Load" refers to a percentage of the gross output defined earlier in the boiler inputs.
2. "Efficiency" is Gross Output divided by Energy Input at each operating point, expressed as a percentage.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with boiler input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Boiler
Please see Creating a New Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 5 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm
Printing Boiler Inputs
25.0 Entering Boilers ›› 25.2 Common Tasks ››
Deleting Boiler Inputs
25.0 Entering Boilers ›› 25.2 Common Tasks ››
Copying a Boiler
25.0 Entering Boilers ›› 25.2 Common Tasks ››
Duplicating a Boiler
25.0 Entering Boilers ›› 25.2 Common Tasks ››
Editing an Existing Boiler
Please see Editing an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Boiler Inputs
Please see Generating Input Data Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Boiler Inputs
Please see Deleting Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Boiler
Please see Copying Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Boiler
Please see Duplicating an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 6
25.0 Entering Boilers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh2AE6.htm