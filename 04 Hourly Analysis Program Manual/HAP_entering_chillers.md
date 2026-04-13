23.0 Entering Chillers
Chiller Form Overview
23.0 Entering Chillers ››
This chapter explains input data for chiller equipment.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Chiller Form Overview
The Chiller Properties window is used to define full load and part load performance data for the following types of equipment:
1. Chillers (producing chilled water only)
2. Reversible chillers (producing chilled water and hot water).
3. Heat Pumps (producing hot water only).
This data is used in the plant simulation portion of energy analysis calculations. Therefore this window is only available in the full HAP
edition and not in HAP System Design. The window is comprised of three key components discussed below.
1. The Title Bar appears across the top of the window. It lists the name of the equipment whose data is being entered or edited. At the
right end of the title bar is a button for closing the window.
2. The Working Area is in the center of the window and contains three categories of information for the equipment represented as three
separate tabs in a notebook. To move from one tab to another simply click on the desired tab name. The three tabs are as follows:
a. General contains the name, function, type and reference notes for the equipment. It also contains buttons for generating input data
from a Chiller Template and for importing chiller data from an external file. Please refer to the discussions of chiller creation
methods below for details on templating and importing data.
b. Design Inputs contains information about the full load performance of the equipment.
c. Performance contains the part load performance maps for the equipment. This tab has one or two sub-tabs depending on the
equipment function and characteristics:
Page 1 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
23.1 General Chiller Inputs
23.0 Entering Chillers ››
General Tab / Chiller Form
23.0 Entering Chillers ›› 23.1 General Chiller Inputs ››
Cooling Mode contains the cooling part-load performance map for a chiller or a reversible chiller. This data is used to simulate
equipment operation in the cooling mode at off-design and part-load conditions. For an air-cooled chiller with heat recovery
condenser there will be two cooling mode sub-tabs: one for air-cooled condenser operation and one for water-cooled condenser
operation.
DX Free Cooling Mode contains cooling performance for an air-cooled chiller running equipped with DX free cooling capability.
Heating Performance contains the heating part-load performance map for a reversible chiller or for a heat pump. This data is used
to simulate equipment operation in the heating mode at off-design and part-load conditions.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the equipment inputs and return to the HAP main program window.
b. Press Cancel to return to the main program window without saving changes. If you press Cancel while creating new equipment, the
new item will not be added to your project and any data entered will be discarded.
c. Press Help to display this overview topic.
Methods of Inputting Equipment Data. HAP provides three different ways of entering equipment performance data. Which is best to
use depends on the availability of data.
1. Importing a Chiller. If your sales engineer has provided you with a electronic file from one of Carrier's Electronic Catalog Chiller
Selection programs, a full set of performance data for a specific chiller, reversible chiller or heat pump selection can be imported into
HAP. To use the Import feature, press the Import Chiller button on the General tab.
2. Chiller Template (chillers only). If you have full load performance data for a chiller plus limited part-load data such as IPLV or NPLV
points, you can use the "Chiller Template" feature. Full load and part-load data is entered and the program uses it to automatically
generate a complete performance map for the chiller. Currently templates are offered for W/C Centrifugal, W/C Rotary Screw, W/C
Packaged Screw and W/C Packaged Reciprocating types of chillers. When working with other chiller types, the default data provided
by the "User Input" approach below can be used to construct performance maps. To use the Template feature, press the Chiller
Template button on the General tab.
3. User Input. The "User Input" approach is currently used for two situations.
In the first situation you have full load performance data and a complete part-load performance map for the equipment obtained from
catalogs or from the manufacturer. Use your data to manually enter all required values on the General, Design Inputs and Cooling
Performance and/or Heating Performance tabs.
In the second situation, you have full load performance data and limited part-load data, but cannot use the Template option above
because templating features are not currently offered for the type of equipment you are working with. In this situation, select your
equipment function and type on the General tab and then enter your full load performance values on the Design Inputs tab. Each
equipment type is provided with a default performance map containing representative performance data. When you specify full load
capacity and full load input power, the map will automatically adjust to your specifications.
Chiller Features. Finally, HAP provides useful features for:
Creating a new chiller or heat pump .
Editing an existing chiller or heat pump .
Printing chiller or heat pump input data .
Deleting chillers or heat pumps .
Copying a chiller or heat pump .
Duplicating a chiller or heat pump .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the General tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
General Tab / Chiller Form
The General tab in the Chiller window contains inputs which describe the general nature of the chiller or heat pump being defined. Inputs
on this tab are described below.
Page 2 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Equipment Name
23.0 Entering Chillers ›› 23.1 General Chiller Inputs ››
1. Name is a reference name used to identify the equipment.
2. Equipment Function defines whether the equipment is a chiller (cooling-only), a reversible chiller (cooling and heating) or a heat pump
(heating only).
2. Equipment Type defines the type of equipment being specified. This item will determine the inputs required on the Design Inputs and
Performance tabs.
3. Notes provide space to enter information about what the equipment represents or the origin of the data. These notes are sometimes
useful when referring to the data at some point in the future.
4. The Chiller Template button is used to auto-generate a complete part-load performance map for a chiller. It is typically used when you
have a set of full load performance data and only a limited set of part-load data such as IPLV or NPLV points. The Template feature
allows you to enter this limited set of data. It then uses it to generate a complete part-load performance map for the chiller. To use this
feature, first enter the desired chiller name and then press the Chiller Template button. Not that templating features are currently
offered for W/C Centrifugal, W/C Rotary Screw, W/C Packaged Screw and W/C Packaged Reciprocating types of chillers. Note that
this option is not offered for reversible chillers or heat pumps.
5. The Import button is used to import data from an external file. Carrier Electronic Catalog Chiller Selection programs are able to export
data for specific chiller, reversible chiller or heat pump selections to a file. HAP is then able to import this data from the file. This allows
you to use performance data for specific equipment selections in your energy analysis calculations. It also saves you the time of
entering equipment data. To use this feature, simply press the Import button.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Name
This item is a reference name for the equipment. It will appear elsewhere in the program on selection lists and reports. The name
appears:
1. In the list of available chillers and heat pumps that appears on the HAP main window.
Page 3 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Equipment Function
23.0 Entering Chillers ›› 23.1 General Chiller Inputs ››
Equipment Type
23.0 Entering Chillers ›› 23.1 General Chiller Inputs ››
2. In the list of available chillers or heat pumps when assembling a chilled water or hot water plant.
3. On input data reports for chillers, heat pumps and plants.
Therefore, it is important to use a descriptive name. Typically the name includes information about the make and model of the equipment
or its size.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Function
This item describes the function of the equipment being defined:
1. A chiller, which produces chilled water only. In certain cases heat recovery equipment such as a double bundle condenser, a
desuperheater or a heat recovery condenser (for air cooled chillers) can be added so the chiller simultaneously produces chilled
and hot water to serve building loads.
2. A reversible chiller which produces chilled water in cooling mode and produces hot water in heating mode.
3. A heat pump which produces hot water only.
The choice of equipment function will affects the equipment types that are offered in the next input, and the input items which appear on
the Design Inputs and Performance tabs.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Equipment Type (Chiller Properties)
This item describes the type of chiller or heat pump equipment being entered. It will determine the input items required on subsequent
tabs of the Chiller Properties window. For example condenser water flow data will be required for water-cooled chillers, but not for air-
cooled chillers. Users can choose from a list of 18 common equipment types. Which of the following options is offered, depends on the
Equipment Function selected.
Chillers (producing chilled water only)
Water-Cooled Centrifugal
Water-Cooled Rotary Screw
Water-Cooled Packaged Screw
Water-Cooled Packaged Reciprocating
Water-Cooled Packaged Scroll
Water-Cooled Single-Effect Steam Absorption
Water-Cooled Double-Effect Steam Absorption
Water-Cooled Direct-Fired Absorption
Water-Cooled Engine Chiller
Air-Cooled Packaged Screw
Air-Cooled Packaged Reciprocating
Air-Cooled Packaged Scroll
Reversible Chillers (producing chilled water and hot water, but not simultaneously)
Water-Source Packaged Screw
Water-Source Packaged Scroll
Air-Source Packaged Scroll
Heat Pumps (producing hot water)
Water-Source Packaged Screw
Water-Source Packaged Scroll
Air-Source Packaged Scroll
When an equipment type is selected, all items on the Design Inputs and Performance tabs will be updated with default data for the
equipment type you chose. Defaults represent a "typical" unit of the selected type. Default data can then be revised so the r data
represents the specific equipment you are modeling.
About Default Performance Maps. The data found on the Cooling Performance and/or Heating Performance tabs is a matrix of
performance data defining input power and capacity at various combinations operating conditions:
1. For chillers, the matrix defines performance at combinations of entering condenser water or air temperature and part-load ratio.
Data is for the design leaving chilled water temperature (LCHWT).
2. For reversible chillers the cooling performance matrix defines performance at entering condenser water or air temperatures and
part-load ratio, for the design LCHWT. The heating performance matrix defines performance at entering source water or air
temperatures and part-load ratio for the design hot water supply temperature (HWST).
Page 4 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Notes
23.0 Entering Chillers ›› 23.1 General Chiller Inputs ››
23.2 Design Inputs
23.0 Entering Chillers ››
Design Inputs Tab / Chiller Form
23.0 Entering Chillers ›› 23.2 Design Inputs ››
3. For heat pumps the heating performance matrix defines performance at entering source water or air temperatures and part-load
ratio for the design HWST.
Correction factors are used to adjust performance when the equipment uses chilled water reset or hot water reset and operates at
varying leaving supply water temperatures.
Cooling Performance Maps. The default cooling performance maps for water-cooled chillers and water-to-water reversible chillers
assume a design condition of 85 F entering condenser water temperature (ECWT) and 44 F LCHWT. In Metric this is 29.4 C ECWT and
6.7 C LCHWT. The default map can be adjusted for different design LCHWT conditions by specifying the new LCHWT and the full load
capacity and input power values on the Design Inputs tab. The program will automatically update the default map when these inputs are
changed.
While the assumed design for water-cooled chillers is 85 F (29.4 C), most default map data extends to 90 F ECWT (32.2 C) to cover
extreme operating conditions. Maps generally extend to 60 F ECWT (15.6 C) as a minimum. Each map is intended to represent a
"typical" chiller.
For air-cooled chillers and air-to-water reversible chillers the cooling performance maps assume a design condition of 95 F outdoor air
temperature (OAT) and 44 F LCHWT. In Metric this is 35 C OAT and 6.7 C LCHWT. As with the water-cooled maps, the default map can
be adjusted for different LCHWT conditions by specifying the new LCHWT and the full load capacity and input power values. The
program will automatically update the default map when these inputs are changed.
While the assumed design for air-cooled chillers is 95 F (35 C) OAT, map data for warmer temperatures is provided to cover extreme
operating conditions. On the low ambient side of the map, it is assumed head pressure control begins at 75 F OAT (23.9 C). Maps then
extend to a minimum temperature of 0 F (-17.8 C). Because the 0 to 75 F range involves head pressure control, changes in performance
are relatively linear in this range, so the map only provides data at the upper and lower limits of this range (75 F and 0 F respectively).
Heating Performance Maps. The default heating performance maps for water-to-water heat pumps assume a design condition of 43 F
entering source water temperature (ECWT) and 95 F HWST. In Metric this is 6.1 C EWT and 35 C HWST. The default map can be
adjusted for different design HWST conditions by specifying the new HWST and the full load capacity and input power values on the
Design Inputs tab. The program will automatically update the default map when these inputs are changed. Each map is intended to
represent a "typical" chiller or heat pump.
For air-to-water heat pumps the heating performance maps assume a design condition of 23 F outdoor air temperature (OAT) and 95 F
HWST. In Metric this is -5 C OAT and 35 C HWST. As with the water-cooled maps, the default map can be adjusted for different HWST
conditions by specifying the new HWST and the full load capacity and input power values on the Design Inputs tab. The program will
automatically update the default map when these inputs are changed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Notes
This item is optional. Sometimes it is useful to enter notes about what the equipment data represents such as the part number or special
options used when selecting the chiller or heat pump. In other cases notes about the origin of the performance data you are entering are
useful. Both may be helpful when referring to the data in the future.
These notes only appear on this input screen and the input data report. The notes do not appear elsewhere in the program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data in the Design Inputs tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs Tab / Chiller Form
The Design Inputs tab in the Chiller Properties window contains items which describe the full load performance of the equipment. The
content of this tab varies depending on the equipment type selected on the General tab. The links below connect to topics describing the
layout and content of the Design Inputs tab for the different equipment types:
Water-Cooled Applied Chillers (Centrifugal and Rotary Screw)
Page 5 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W/C Applied Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Water-Cooled Packaged Chillers (Screw, Scroll and Reciprocating)
Water-Cooled Absorption Chillers (Single and Double-Effect Steam, and Direct-Fired)
Water-Cooled Engine Chillers
Air-Cooled Chillers
Water-to-Water Reversible Chillers
Air-to-Water Reversible Chillers
Water-to-Water Heat Pumps
Air-to-Water Heat Pumps
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for W/C Applied Chillers
Data required on the Design Inputs tab for water-cooled centrifugal and rotary screw chillers is shown in Figure 1. For further explanation
of these inputs, click on the items below.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load ECWT
Condenser Flow Rate
Full Load Capacity
Minimum ECWT
Full Load Power
Minimum Load
Average Operating Loss
Heat Recovery
Figure 1. Design Inputs for W/C Applied Chillers
Page 6 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
When Double-Bundle Condenser heat recovery is specified, the additional inputs shown in Figure 2 appear. For further explanation of
this input, click on the item below.
Condenser
Flow
Rate
(Recovery)
Figure 2. Double-Bundle Heat Recovery Inputs for W/C Applied Chillers
When Desuperheater heat recovery is specified, the additional inputs shown in Figure 3 appear. For further explanation of this inputs,
click on the items below.
Desuperheater Flow Rate
Desuperheater Max Heat
Recovery
Figure 3. Desuperheater Heat Recovery Inputs for W/C Applied Chillers
Page 7 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W/C Packaged Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for W/C Packaged Chillers
Data required on the Design Inputs tab for water-cooled packaged chillers is shown in Figure 1. This applies to water-cooled screw,
scroll and reciprocating chillers. For further explanation of these inputs, click on the items below.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load ECWT
Condenser Flow Rate
Full Load Capacity
Minimum ECWT
Full Load Power
Minimum Load
Average Operating Loss
Heat Recovery
Hot Gas Bypass
Figure 1. Design Inputs for W/C Packaged Chillers
When Desuperheater heat recovery is specified, the additional inputs shown in Figure 2 appear. For further explanation of this inputs,
click on the items below.
Desuperheater Flow Rate
Desuperheater Max Heat
Recovery
Page 8 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W/C Absorption Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Figure 2. Desuperheater Heat Recovery Inputs for W/C Packaged Chillers
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for W/C Absorption Chillers
HAP offers modeling features for single and double-effect steam absorption chillers as well as direct-fired absorption chillers.
Data required on the Design Inputs tab for steam absorption chillers is shown in Figure 1 below. For further information on these inputs
click on the following items.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load EACWT
Absorber/Condenser Flow Rate
Full Load Capacity
Minimum EACWT
Full Load Steam Input
Minimum Load
Average Operating Loss
Electric Input
Steam Heat Content
Data required on the Design Inputs tab for direct-fired absorption chillers is shown in Figure 2 below. For further information on these
inputs click on the following items.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load EACWT
Absorber/Condenser Flow Rate
Full Load Capacity
Minimum EACWT
Full Load Burner Input
Minimum Load
Average Operating Loss
Electric Input
Figure 1. Design Inputs for W/C Single Effect and Double Effect Steam Absorption Chillers
Page 9 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W/C Engine Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Figure 2. Design Inputs for W/C Direct-Fired Absorption Chillers
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 10 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W/C Engine Chillers
Data required on the Design Inputs tab for water-cooled engine or turbine driven chillers is shown below. For further information on these
inputs click on the following items.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load ECWT
Condenser Flow Rate
Full Load Capacity
Minimum ECWT
Full Load Engine Input
Minimum Load
Fuel Type
Heat Recovery
Average Engine Efficiency
Electric Input
Figure 1. Design Inputs for W/C Engine Chillers
When Desuperheater heat recovery is specified, the additional inputs shown in Figure 2 appear. For further explanation of this inputs,
click on the items below.
Desuperheater Flow Rate
Desuperheater Max Heat
Recovery
Page 11 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for A/C Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Figure 2. Desuperheater Heat Recovery Inputs for W/C Engine Chillers
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for A/C Chillers
Data required on the Design Inputs tab for air-cooled chillers is shown in Figure 1. This data applies to air-cooled reciprocating, screw
and scroll chiller equipment. For further explanation of these inputs, click on the items below.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load OAT
Minimum Load
Full Load Capacity
DX Free Cooling
Full Load Power
Heat Recovery
Average Operating Loss
Hot Gas Bypass
Page 12 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Figure 1. Design Inputs for A/C Packaged Chillers
When Desuperheater heat recovery is specified, the additional inputs shown in Figure 2 appear. For further explanation of this inputs,
click on the items below.
Desuperheater Flow Rate
Desuperheater Max Heat
Recovery
Figure 2. Desuperheater Heat Recovery Inputs for A/C Packaged Chillers
When Chiller with Heat Recovery Condenser heat recovery is specified, the additional inputs shown in Figure 3 appear. For further
explanation of this input, click on the item below.
Full Load ECWT
Full Load Capacity (W/C)
Page 13 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W2W Reversible Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load Power (W/C)
Condenser Flow Rate
Minimum ECWT Setpoint
Figure 3. Water-Cooled Heat Recovery Condenser Inputs for A/C Packaged Chillers
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for W2W Reversible Chillers
Data required on the Design Inputs tab for water-to-water reversible heat pumps is shown in the figure below. For further explanation of
these inputs, click on the items below.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load ECWT
Condenser Flow Rate
Full Load HWST
Hot Water Supply Flow Rate
Full Load EWT
Source Water Flow Rate
Full Load Capacity (Cooling)
Minimum ECWT
Full Load Capacity (Heating)
Minimum Load
Full Load Power (Cooling)
Hot Gas Bypass
Full Load Power (Heating)
Average Operating Loss
Page 14 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for A2W Reversible Chillers
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for A2W Reversible Chillers
Data required on the Design Inputs tab for air-to-water reversible heat pumps is shown in the figure below. For further explanation of
these inputs, click on the items below.
Full Load LCHWT
Chilled Water Supply Flow Rate
Full Load OAT (Cooling)
Hot Water Supply Flow Rate
Full Load HWST
Minimum Load
Full Load OAT (Heating)
DX Free Cooling
Full Load Capacity (Cooling)
Hot Gas Bypass
Full Load Capacity (Heating)
Full Load Power (Cooling)
Full Load Power (Heating)
Average Operating Loss
Page 15 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for W2W Heat Pumps
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for W2W Heat Pumps
Data required on the Design Inputs tab for water-to-water heat pumps is shown in the figure below. For further explanation of these
inputs, click on the items below.
Full Load HWST
Hot Water Supply Flow Rate
Full Load EWT
Source Water Flow Rate
Full Load Capacity
Minimum Load
Full Load Power
Hot Gas Bypass
Average Operating Loss
Page 16 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Design Inputs for A2W Heat Pumps
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Inputs for A2W Heat Pumps
Data required on the Design Inputs tab for air-to-water heat pumps is shown in the figure below. For further explanation of these inputs,
click on the items below.
Full Load HWST
Hot Water Supply Flow Rate
Full Load OAT
Source Water Flow Rate
Full Load Capacity
Minimum Load
Full Load Power
Hot Gas Bypass
Average Operating Loss
Page 17 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Full Load LCHWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load HWST
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load ECWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load LCHWT
This item defines the leaving chilled water temperature (LCHWT) for the chiller at its full load cooling design point. The full load capacity
and input power specified on this tab are rated at this LCHWT. In addition, the performance map data shown on the next tab lists
performance data rated at this LCHWT.
If a chiller is included in a plant which uses a different design LCHWT or uses chilled water reset, then equipment performance will be
adjusted to the new LCHWT using the correction factors found on the Cooling Performance tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load HWST
This item defines the hot water supply temperature (HWST) for the heat pump at its full load heating design point. The full load capacity
and input power specified on this tab are rated at this HWST. In addition, the performance map data shown on the next tab lists
performance data rated at this HWST.
If a chiller or heat pump is included in a plant which uses a different design HWST or uses hot water reset, then heat pump performance
will be adjusted to the new HWST using the correction factors found on the Heating Performance tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load ECWT
This item defines the entering condenser water temperature (ECWT) for the chiller at its full load cooling design point. The full load
capacity and input power specified on this tab are rated at this ECWT.
For an air-cooled chiller with heat recovery condenser, this input refers to the entering condenser water temperature (ECWT) for the
chiller at full load design point when using the water-cooled heat recovery condenser for heat rejection.
Page 18 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Full Load EWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load EACWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load OAT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load Capacity
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load EWT
This item defines the entering source water temperature (EWT) for the heat pump at its full load heating design point. The full load
capacity and input power specified on this tab are rated at this EWT.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load EACWT
This item defines the entering absorber/condenser water temperature (EACWT) for the chiller at its full load cooling design point. The full
load capacity and generator heat input items specified on this tab are rated at this EACWT.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load OAT
For chillers:
This item defines the entering condenser air temperature for the chiller at its full load cooling design point. This entering condenser
temperature is assumed to be equal to the outdoor air temperature (OAT). The full load capacity and input power specified on this tab
are rated at this OAT.
For air-to-water reversible chillers:
Full Load OAT (Cooling) defines the entering condenser air temperature for a reversible chiller at its full load cooling design point. This
entering condenser temperature is assumed to be equal to the outdoor air temperature (OAT). The full load cooling capacity and
cooling input power specified on this tab are rated at this OAT.
Full Load OAT (Heating) defines the entering evaporator air temperature for a reversible chiller at its full load heating design point.
This entering temperature is assumed to be equal to the outdoor air temperature (OAT). The full load heating capacity and heating
input power specified on this tab are rated at this OAT.
For heat pumps:
Full Load OAT defines the entering evaporator air temperature for a heat pump at its full load heating design point. This entering
temperature is assumed to be equal to the outdoor air temperature (OAT). The full load heating capacity and heating input power
specified on this tab are rated at this OAT.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load Capacity
Equipment capacity can be defined in one of two ways:
1. Auto-Size Capacity - For preliminary design or LEED applications where it is necessary to have the capacity automatically
determined, place a check in the "Auto-Size Capacity" box. During plant simulation calculations, the program will automatically size
the equipment based on peak plant load plus an oversizing factor specified in the plant inputs. In a multiple-chiller plant or multiple
heat pump plant, the plant inputs will also specify how plant capacity should be divided among individual equipment units (e.g.
60%/40%, equally sized, etc...).
2. User-Defined Capacity - For applications where the equipment capacity is known, leave the "Auto-Size Capacity" box unchecked and
specify the Full Load Capacity of the equipment.
For chillers:
Page 19 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Full Load Power
23.0 Entering Chillers ›› 23.2 Design Inputs ››
The cooling capacity is rated at the full load LCHWT and entering condenser temperature (ECWT, EACWT or OAT) specified earlier
on this tab.
For air-cooled chillers with heat recovery condenser:
Two cooling capacity ratings are required. The first is the cooling capacity at the full load LCHWT and entering condenser OAT
temperature for the chiller operating with air-cooled condenser. The second is the cooling capacity at the full load LCHWT and the
entering condenser water temperature for the chiller operating in water-cooled condenser heat recovery mode..
For reversible chillers:
The cooling capacity is rated at the full load LCHWT and entering condenser temperature (ECWT or OAT) specified earlier on this
tab. The heating capacity is rated at the full load HWST and entering source temperature (EWT or OAT) specified earlier on this
tab.
For heat pumps:
The heating capacity is rated at the full load HWST and entering source temperature (EWT or OAT) specified earlier on this tab.
When you specify a full load capacity, all values in the capacity portion of the Cooling Performance and Heating Performance tabs will
be updated automatically. For example, if you change the full cooling load capacity from 100 tons to 150 tons, all values in the capacity
portion of the coling performance map will be multiplied by the ratio 150/100. In this way, HAP automatically scales your performance
map data to your full load inputs.
Note that the choice of "Auto-Size Capacity" is important. If the "Auto-Size Capacity" box is checked, then this equipment can only be
linked to a plant which itself uses the "Autosize Capacity" option. If the "Auto-Size Capacity" box is not checked, then the equipment can
only be linked to a plant which uses the "User Defined Capacities" option. Once equipment is linked to a plant its "Auto-Size Capacity"
input should not be changed. Changing this value makes the equipment incompatible with its plant and will cause an error message to
appear when you try to launch the plant simulation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load Power
For chillers:
Full Load Power defines the chiller input power rated at the full load LCHWT, entering condenser temperature (ECWT or OAT) and the
full load capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, input power can be defined as kW/Ton (ikW/kW) or as total kW. To change the
units of measure, select the desired units label in the drop-down list to the right of this input item. If "Auto-Size Capacity" is selected,
then input power can only be defined as kW/Ton (ikW/kW)
For air-to-water reversible chillers:
Full Load Power (Cooling) defines the cooling mode input power rated at the full load LCHWT, entering condenser temperature
(ECWT or OAT) and the full load cooling capacity conditions specified earlier on this tab.
Full Load Power (Heating) defines the heating mode input power rated at the full load HWST, entering source temperature (EWT or
OAT) and the full load heating capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, input power can be defined in relative terms as input power per unit capacity
(kW/Ton, kW/MBH, ikW/kW) or as total input kW. To change the units of measure, select the desired units label in the drop-down list to
the right of this input item. If "Auto-Size Capacity" is selected, then input power can only be defined in relative terms (kW/Ton,
kW/MBH, ikW/kW).
For air-cooled chillers with heat recovery condenser:
Full Load Power (A/C) defines the input power rated at design LCHWT and OAT conditions when using the air-cooled condenser.
Full Load Power (W/C) defines the input power rated at design LCHWT and ECWT conditions when using the water-cooled heat
recovery condenser.
When the "Auto-Size Capacity" option is not selected, input power can be defined in relative terms as input power per unit capacity
(kW/Ton or ikW/kW) or as total input kW. To change the units of measure, select the desired units label in the drop down list to the
right of this item. On the other hand, if "Auto-Size Capacity" is selected, then input power can only be defined in relative terms.
For heat pumps:
Full Load Power defines the heating mode input power rated at the full load HWST, entering source temperature (EWT or OAT) and
the full load heating capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, input power can be defined as in relative terms as input power per unit capacity
(kW/MBH, ikW/kW) or as total input kW. To change the units of measure, select the desired units label in the drop-down list to the right
of this input item. If "Auto-Size Capacity" is selected, then input power can only be defined in relative terms (kW/MBH, ikW/kW).
For all equipment types:
Page 20 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Full Load Steam Input
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load Burner Input
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Full Load Engine Input
23.0 Entering Chillers ›› 23.2 Design Inputs ››
When you change either the input power or the units of measure, all data in the power data section of the Cooling Performance and
Heating Performance tabs will be updated automatically. For example, if you change the full load power value for a chiller from 0.6
kW/Ton to 0.65 kW/Ton, all values in the power section of the cooling performance map will be multiplied by the ratio 0.65/0.60. Or, if
you change the units from kW/Ton to kW, the units of measure shown in the Performance Map will be changed to kW and all the data
cells will be automatically converted. In this way HAP automatically scales performance map data to your full load performance inputs.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load Steam Input
This item defines the chiller steam input rated at full load LCHWT, entering absorber/condenser temperature (EACWT) and the full load
capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, steam input can be defined as lb/ton-hr (kg/kWh) or as total lb/hr (kg/hr). To
change the units of measure, select the desired units label in the drop-down list to the right of this input item. If "Auto-Size Capacity" is
selected, then steam input can only be defined as lb/ton-hr (kg/kWh).
When you change either the steam input or the units of measure, all data in the steam input section of the Performance Map will be
updated automatically. For example, if you change the value from 10 to 12 lb/ton-hr, all values in the steam section of the map will be
multiplied by the ratio 12/10. Or, if you change the units from lb/ton-hr to lb/hr, the units of measure shown in the Performance Map will
be changed to lb/hr.
This item only applies to steam absorption chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load Burner Input
This item defines the burner energy input rated at the full load LCHWT, entering absorber/condenser temperature (EACWT) and the full
load capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, burner input can be defined as MBH/ton (ikW/kW) or as total MBH (ikW) energy
input. To change the units of measure, select the desired units label in the drop-down list to the right of this input item. If "Auto-Size
Capacity" is selected, then burner input can only be entered as MBH/Ton (ikW/kW).
When you change either the burner input or the units of measure, all data in the energy input section of the Performance Map will be
updated automatically. For example, if you change the value from 11 to 13 MBH/Ton, all values in the energy input section of the map will
be multiplied by the ratio 13/11. Or, if you change the units from MBH/ton to MBH, the units of measure shown in the Performance Map
will be changed to MBH.
This item only applies to direct-fired absorption chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Full Load Engine Input
This item defines the chiller energy input rated at the full load LCHWT, entering condenser temperature (ECWT) and the full load
capacity conditions specified earlier on this tab.
When the "Auto-Size Capacity" option is not selected, engine energy input can be defined as MBH/ton (ikW/kW) or as total MBH (ikW)
energy input. To change the units of measure, select the desired units label in the drop-down list to the right of this input item. If "Auto-
Size Capacity" is selected, then burner input can only be entered as MBH/Ton (ikW/kW).
When you change either the engine input or the units of measure, all data in the energy input section of the Performance Map will be
updated automatically. For example, if you change the value from 9 to 10 MBH/Ton, all values in the energy input section of the map will
be multiplied by the ratio 10/9. Or, if you change the units from MBH/Ton to MBH, the units of measure shown in the Performance Map
will be changed to MBH.
This item only applies to engine chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 21 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Steam Heat Content
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Fuel Type
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Average Engine Efficiency
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Average Operating Loss
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Steam Heat Content
This item defines the heat content of steam (BTU/lb or kJ/kg) used to run a steam absorption chiller. During chiller performance
calculations it is used to convert chiller performance data in lb/hr (kg/hr) into standard energy units of MBH (kW). Once in standard
energy units, the steam value can be used to determine a boiler load or remote steam load.
Steam heat content depends on the supply steam pressure, superheat and condensate temperature. Generally small to moderate
changes in steam supply conditions result in changes in steam heat content of only a few percent. Default values for this input are based
on the following assumptions:
a. Single-Effect Absorption Chillers. Assumes 15 psig dry steam at 946.2 BTU/lb. In SI Metric units this is 103.4 kPa dry steam at
2200.9 kJ/kg.
b. Double-Effect Absorption Chillers. Assumes 125 psig dry steam at 869.2 BTU/lb. In SI Metric units this is 861.8 kPa dry steam at
2021.8 kJ/kg.
If data concerning the supply steam conditions is not known, we recommend accepting these defaults. If steam conditions are known,
then the default should be replaced with the actual steam heat content.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fuel Type
This item defines the type of fuel used for a direct-fired absorption chiller or an engine chiller. This must be defined so the program can
assign chiller energy use to the proper fuel category for fuel cost calculations.
For direct-fired absorption chillers, natural gas, fuel oil and propane can be used.
For engine chillers, natural gas or steam can be used. Use of steam means you are modeling a turbine driven chiller.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Average Engine Efficiency
This item defines the average efficiency of the engine which drives the compressors. This value is required to analyze heat rejection for
the chiller. A large portion of the energy consumed by the engine is used to compress refrigerant thereby increasing its energy content.
This energy is ultimately rejected through the chiller condenser. The remaining energy input is lost through mechanical and combustion
inefficiencies in the engine. Because chiller performance is defined in terms of engine fuel input for various operating conditions, the
average engine efficiency must be known to allow heat rejection to be accurately analyzed.
If the engine chiller uses a jacket cooler for the engine and rejects this heat through the cooling tower, then the average engine efficiency
should be inflated to account for this heat rejection. If all engine heat is rejected to the cooling tower, an efficiency value of 100% should
be used.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Average Operating Loss
This is an optional item used for some types of equipment to increase the accuracy of heat rejection calculations for chillers and heat
output calculations for heat pumps. Specify 0% if you don't wish to use this feature. Specify a value greater than 0% if you have
equipment performance data that allows determination of this factor.
Discussion:
Under ideal conditions from a first law of thermodynamics analysis:
For an ideal chiller: Heat Rejection = Evaporator Load + Compressor Input Energy.
For an ideal heat pump: Heat Output = Evaporator Load + Compressor Input Energy.
For chillers or heat pumps with hermetic compressors, these are reasonable assumptions since the compressor motor is cooled by
refrigerant. However, there are certain equipment units that deviate from ideal conditions by several percent due to heat loss through the
Page 22 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Electric Input
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Minimum ECWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
compressor casing or heat exchanger shell. Other energy consumers such as fans for air-cooled or air-source units, may contribute to
this discrepancy. These losses reduce the amount of heat rejection or heat output and can have an effect on the accuracy of energy
simulation results. For example, a water-to-water heat pump assumed to be ideal can underestimate the energy input needed to meet a
given heating load if the operating loss is significant and is not considered.
The Average Operating Loss input allows you to account for heat losses of this kind. If you do not know the loss value for the equipment
or don't wish to consider these losses, specify 0%. In that case the program will calculate heat rejection or heat output using the ideal
assumptions. If you do know the loss value, specify it as a % of input power. The Application section below explains how to compute
this value using manufacturer's performance data.
For certain chiller types, HAP provides "typical" default values of average operating loss: W/C rotary screw, W/C packaged screw, W/C
packaged scroll, A/C packaged screw, and A/C packaged scroll. For other types, a default value of 0% is used, which indicates that
"typical" data was not available.
Application Data.
If you have a full load performance sheet for the equipment provided by the manufacturer, you can calculate the operating loss as
follows. If you have data at full and part-load conditions such as IPLV or NPLV points, a more accurate value can be derived by
calculating loss for each condition and averaging the results. This yields an average loss that is reasonable to apply across the range of
equipment operating conditions.
For chillers or reversible chillers in cooling mode:
English Units:
Operating Loss (MBH) = Evaporator Load (Tons) x 12 + Compressor Input kW x 3.412 - Heat Rejection (MBH)
Operating Loss % = 100 x (Operating Loss (MBH)) / (Compressor Input kW x 3.412)
SI Metric Units:
Operating Loss (kW) = Evaporator Load (kW) + Compressor Input kW - Heat Rejection (kW)
Operating Loss % = 100 x (Operating Loss (kW)) / (Compressor Input kW)
For heat pumps or reversible chillers in heating mode:
English Units:
Operating Loss (MBH) = Evaporator Load (MBH) + Compressor Input kW x 3.412 - Heat Output (MBH)
Operating Loss % = 100 x (Operating Loss (MBH)) / (Compressor Input kW x 3.412)
SI Metric Units:
Operating Loss (kW) = Evaporator Load (kW) + Compressor Input kW - Heat Output (kW)
Operating Loss % = 100 x (Operating Loss (kW)) / (Compressor Input kW)
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Electric Input
This item defines the electrical input for an absorption chiller or for an engine chiller.
a. For absorption chillers it typically accounts for the input power to solution pumps, refrigerant pumps and controls.
b. For engine chillers it accounts for controls and miscellaneous electrical components such as the spark ignition system.
During chiller performance calculations the program assumes this electric input remains constant for all operating conditions whenever
the chiller is on. The only exception is when the chiller is cycling at low load conditions. For this case, the electric input power use will be
cycled along with the rest of the chiller.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum ECWT
This item defines the minimum entering condenser water temperature (ECWT) for a water-cooled chiller, a water-to-water reversible
chiller in cooling mode, or an air-cooled chiller with heat recovery condenser. This temperature is used as the minimum setpoint for water
Page 23 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Minimum EACWT
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Minimum Load
23.0 Entering Chillers ›› 23.2 Design Inputs ››
DX Free Cooling
23.0 Entering Chillers ›› 23.2 Design Inputs ››
returning from the cooling tower, dry cooler or geo field to the chiller. When return water colder than this setpoint is detected, the system
modulates to to keep return water at the minimum setpoint. For example, with a cooling tower, water bypass, fan cycling, 2-speed fan or
variable speed fan control could be used to reduce tower heat rejection effectiveness to hold return water at the setpoint.
Use of Minimum ECWT controls restricts chiller or reversible chiller operation to certain parts of its cooling performance map and can be
a key factor in differentiating the performance of different makes and models of equipment. For example, certain equipment are able to
operate at cold ECWT temperatures thereby achieving high levels of efficiency. Other equipment are restricted to operating at warmer
ECWT temperatures and cannot attain the same levels of efficiency at part load operation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum EACWT
This item defines the minimum entering absorber/condenser water temperature (EACWT) setpoint for a water-cooled absorption chiller.
For further information on how minimum water temperature control is modeled please refer to the Minimum ECWT topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum Load
This item defines the part-load ratio below which cycled operation occurs. This cycling point is defined as a percentage of full load
capacity.
If the equipment uses hot gas bypass, then this input defines the part-load ratio below which hot gas bypass is used to falsely load the
compressors to maintain the equipment at this minimum load level.
Example #1 - A chiller without hot gas bypass has a minimum load specified as 10%. When the chiller load is less than 10%, the chiller
is assumed to cycle between a 10% loaded condition and OFF to meet the load.
Example #2 - A chiller with hot gas bypass has a minimum load specified as 30%. When the chiller load is less than 30%, hot gas
bypass is used to falsely load the compressor so the chiller operates at 30% load and the corresponding efficiency.
Note: If the performance map is organized according to compressor stages instead of % load columns, then this input does not appear.
In this case the minimum load is determined directly from the performance map - whenever the chiller load is below the capacity for
compressor stage 1 at the given ECWT or OADB, the chiller will cycle. Currently the performance map will only be organized according
to compressor stages when chiller or heat pump data is imported from the ECAT Packaged Chiller Builder program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
DX Free Cooling
This item specifies whether the chiller has DX free cooling capability. Two types of DX free cooling operation are offered:
1. Integrated DX Free Cooling - The chiller operates in three modes:
a. In conventional mode, compressors are used to meet the chiller load.
b. In partial free cooling mode, one circuit continues to run the compressor and the other circuit operates in DX free cooling mode.
With DX free cooling mode the compressor is turned off and a refrigerant pump circulates refrigerant between evaporator and
condenser to provide cooling effect. Sufficient difference between leaving chilled water temperature and entering condenser air
temperature is required before DX free cooling can operate.
c. In full free cooling mode, both refrigerant circuits operate in DX free cooling mode. Again sufficient difference between leaving
chilled water temperature and entering condenser air temperature is needed before DX free cooling can serve the full chiller load.
2. Non-Integrated DX Free Cooling - The chiller operates in the conventional and full free cooling modes described above. This type of
chiller cannot operate in partial free cooling mode.
When the Integrated or Non-Integrated DX Free Cooling options are selected, an sub-tab for DX free cooling performance data will
appear on the Performance tab
Notes:
Page 24 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Hot Gas Bypass
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Heat Recovery
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Desuperheater Max Heat Recovery
23.0 Entering Chillers ›› 23.2 Design Inputs ››
a. Performance data for partial DX free cooling mode is not directly specified on the Performance Map tab. Instead, the program
estimates performance in partial free cooling mode using data from all three tables shown on the Performance Map tab.
b. When DX free cooling is selected, the option for heat recovery is disabled. When a heat recovery option is selected, the DX free
cooling option is disabled. Its not possible to have both heat recovery features and DX free cooling in the same chiller.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Hot Gas Bypass
This item specifies whether hot gas bypass control is used for the chiller or heat pump. Hot gas bypass is used to keep the refrigerant
suction pressure at an acceptable level. Below the Minimum Load level specified, compressor discharge gas is diverted to the evaporator
inlet or compressor inlet to maintain the minimum suction pressure. This falsely loads the compressors.
To select Hot Gas Bypass, place a check mark in the box. When Hot Gas Bypass is not used, leave the check box blank.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heat Recovery
This item defines whether the chiller contains special heat recovery components. Depending on the chiller type, one or more of the
following options will be offered:
1. Desuperheater. Select this option to add a desuperheater to the chiller. This is a refrigerant gas to water heat exchanger that is
upstream of the condenser. Hot discharge gas from the compressor flows through the desuperheater and transfers its sensible heat to
incoming water, heating the water. The desuperheater is designed and operated so it will not cool the refrigerant gas to the saturation
point. While the desuperheater can generate high temperature hot water, it can only capture sensible heat from the refrigerant so the
amount of heat recovery is limited to the amount by which refrigerant gas has been superheated above saturation. Once the
refrigerant gas leaves the desuperheater, it passes through an air-cooled or water-cooled condenser and rejects the remainder of its
heat as it would in a conventional chiller. In order to use the "Chillers with Desuperheaters" heat recovery method in a heat recovery
plant, one or more chillers must be defined with this Desuperheater component.
When a Desuperheater is specified, separate inputs for the desuperheater flow rate and the maximum heat recovery fraction must also
be provided.
2. Double-Bundle Condenser. Select this option to specify this chiller contains a condenser with two separate water circuits. One
circuit is connected to the cooling tower heat rejection loop. One circuit is a heat recovery circuit connected to the hot water system.
When a heating plant load exists valves are set so water flows through the heat recovery circuit and heat is rejected to the hot water
system. When no heating plant load exists, valves are set so water flows through the heat rejection circuit and heat is rejected to the
cooling tower loop. In order to use the "Chillers with Double Bundle Condensers" heat recovery method in a heat recovery plant, one
or more chillers must be defined with this Double Bundle Condenser component.
When a Double-Bundle Condenser is specified, the heat recovery condenser flow rate must also be specified. In addition, it is
necessary to specify data in the performance map at elevated entering condenser water temperatures so HAP can calculate chiller
input power accurately when the heat recovery condenser circuit is in operation.
This heat recovery device is sometimes referred to as a "split condenser". The separate circuits are sometimes referred to as the
"summer bundle" and "winter bundle" instead of "heat rejection" and "heat recovery" circuits, respectively.
Some water-cooled chillers use dual condensers for heat recovery, switching both refrigerant flow and water flow between the
condensers to reject heat to the cooling tower loop, or to reject heat to the heat recovery loop.
3. Heat Recovery Condensers. When this option is selected, the air-cooled chiller contains two condensers - a refrigerant-to-air
condenser for normal heat rejection to the atmosphere, and a refrigerant-to-water heat exchanger for heat recovery. When a heating
plant load exists, the valves are set so the refrigerant-to-water condenser is used to reject heat to the hot water loop. When no heating
plant load exists, valves are set so the refrigerant-to-air condenser to reject heat to the atmosphere.
When a Heat Recovery Condenser is selected, separate inputs for full load ECWT, minimum ECWT, full load capacity in water cooled
condenser mode, full load input power in water cooled condenser mode, and water-cooled performance map must be defined.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 25 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Chilled Water Supply Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Condenser Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Condenser Flow Rate (Recovery)
Desuperheater Max Heat Recovery
This input specifies desuperheater heat recovery as a percentage of total heat rejection. For example, the default value of 20% means
that desuperheater heat recovery is calculated as 20% of the chiller's total heat rejection for the each operating hour.
Discussion. In an actual application of a chiller with desuperheater, heat recovery is largest at full load and high entering condenser
water temperatures (ECWT) for water-cooled chillers or high outdoor air temperatures (OAT) for air-cooled chillers. This is because the
amount of discharge gas superheat tends to be largest at this condition. As the chiller moves into part-load operation and/or faces cooler
ECWTs or OATs, the amount of available superheat in the refrigerant gas discharged from the compressor typically decreases and that
means the desuperheater component recovers steadily smaller quantities of heat. Therefore desuperheater heat recovery varies with
operating conditions. Heat recovery as a percentage of total heat rejection is largest at full load design conditions, and the percentage
tends to decrease as the chiller moves into part-load and off-design conditions.
HAP uses a simplified model of desuperheater performance which calculates heat recovery as a constant percentage of total heat
rejection. This will yield the largest BTU/hr (or W) of heat recovery at full load design conditions, because the total heat rejection is
largest there. It will yield less BTU/hr (or W) of heat rejection at part-load and off-design conditions because there is less total heat
rejection there. However, this simplified method does not account for the fact that there is less superheat available at off-design and
part-load conditions. Therefore, if you set the desuperheater heat recovery factor based on heat recovery potential at full load, this will
usually produce a generous estimate of annual heat recovery because it overestimates heat recovery at part-load and off-design
conditions. Specifying a desuperheater heat recovery factor that is an average of full load and part-load conditions is likely to yield a
more accurate estimate over the course of a year since it underestimates heat recovery at some times and overestimates it at other times
and these errors tend to offset each other over the course of the year.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Chilled Water Supply Flow Rate
This item defines the chilled water flow rate at the design condition. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the full load cooling capacity.
3. Delta-T - The program will calculate gpm automatically based on the full load cooling capacity and the specified delta-T.
Chilled water supply flow rate is used in chilled water distribution system calculations during a plant simulation:
a. It is used in the calculation of full load pump input power for both constant speed and variable speed pumping applications.
b. For constant speed, constant flow applications, it defines the flow rate for all chiller operating hours.
c. For variable speed applications, it helps establish the minimum flow level for the chiller. For example, if minimum flow is defined as
70%, minimum flow is calculated as 70% of the cooler flow rate you specify here.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Condenser Flow Rate
This item defines the condenser water flow rate for a water-cooled chiller, a water-to-water reversible chiller in cooling mode, or an air-
cooled chiller with heat recovery condenser. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the full load cooling capacity. (Note: This option is not
available for reversible chillers.)
3. Delta-T - The program will calculate gpm automatically based on the design heat rejection and the specified delta-T.
Condenser flow rate is used in water-cooled chiller or water to water reversible chiller and heat rejection calculations during a plant
simulation. Flow and heat rejection together determine the range for the heat rejection device (cooling tower or dry cooler) which is a key
value that drives cooling tower performance at off design and part load conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 26 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Desuperheater Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Heat Recovery Condenser Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Absorber/Condenser Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Hot Water Supply Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
Condenser Flow Rate (Recovery)
Specify the condenser water flow rate for heat recovery circuit of the double-bundle condenser. This input only appears when a double
bundle condenser has been specified. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the full load cooling capacity. (Note: This option is not
available for reversible chillers.)
3. Delta-T - The program will calculate gpm automatically based on the design heat rejection and the specified delta-T.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Desuperheater Flow Rate
Specify the water flow rate for the desuperheater component. This input only appears when a desuperheater has been specified for the
chiller. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the full load cooling capacity. (Note: This option is not
available for reversible chillers.)
3. Delta-T - The program will calculate gpm automatically based on the design heat rejection and the specified delta-T.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heat Recovery Condenser Flow Rate
Specify the water flow rate for the water-cooled heat recovery condenser. This input only appears when a heat recovery condenser is
specified for an air-cooled chiller. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the full load cooling capacity. (Note: This option is not
available for reversible chillers.)
3. Delta-T - The program will calculate gpm automatically based on the design heat rejection and the specified delta-T.
For hours when the air-cooled chiller is operating in water-cooled heat recovery mode, this flow rate will be used for chiller performance
and heat recovery calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Absorber/Condenser Flow Rate
This item defines the fluid flow rate for the absorber and condenser for an absorption chiller. Flow can be specified in one of three ways:
1. gpm or L/s - The flow is defined directly.
2. gpm/Ton or L/s/kW - The program will calculate gpm automatically based on the chiller capacity.
3. Delta-T - The program will calculate gpm automatically based on the chiller design heat rejection and the specified delta-T.
The flow rate data is used in chiller and heat rejection calculations during a plant simulation. Flow and heat rejection together determine
the range for the heat rejection device (cooling tower or dry cooler) which is a key value that drives performance at off design and part
load conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 27 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Source Water Flow Rate
23.0 Entering Chillers ›› 23.2 Design Inputs ››
23.3 Performance Map Inputs
23.0 Entering Chillers ››
Cooling Performance Map Tab
23.0 Entering Chillers ›› 23.3 Performance Map Inputs ››
Hot Water Supply Flow Rate
This item defines the hot water supply flow rate at the design condition. Flow can be specified in one of two ways:
1. gpm or L/s - The flow is defined directly.
2. Delta-T - The program will calculate gpm automatically based on the full load heating capacity and the specified delta-T.
Hot water supply flow rate is used in hot water distribution system calculations during a plant simulation:
a. It is used in the calculation of full load pump input power for both constant speed and variable speed pumping applications.
b. For constant speed, constant flow applications, it defines the flow rate for all heat pump operating hours.
c. For variable speed applications, it helps establish the minimum flow level for the heat pump. For example, if minimum flow is defined
as 70%, minimum flow is calculated as 70% of the cooler flow rate you specify here.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Source Water Flow Rate
This item defines the source water flow rate for a water-to-water heat pump or reversible chiller in heating mode. Flow can be specified in
one of two ways:
1. gpm or L/s - The flow is defined directly.
2. Delta-T - The program will calculate gpm automatically based on the design heat extraction required and the specified delta-T.
Source water flow rate is used to determine the source water pump input power.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Performance Map tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Cooling Performance Map Tab
The Cooling Mode sub-tab on the Performance tab defines the off-design and part-load performance of a chiller or reversible chiller in
cooling mode. This tab contains five key components described below.
Page 28 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Figure 1. Cooling Performance Tab
1. The Cooling Performance table is the upper of the two grids on this tab. It contains input power data for off-design and part-load
cooling conditions.
In this table each row contains performance data for a different entering condenser temperature. Each column contains data for a
different part-load ratio. For example, in this sample screen image the input power for 75 F entering condenser air temperature and
50% load is 1.056 kW/ton.
Together the rows and columns in this table define a "map" of performance data across the range of expected condenser
temperatures and part-load conditions. During energy simulations, HAP will use this data to perform 2-way interpolations to determine
equipment input power at specific combinations of condenser temperature and part-load ratio. When chilled water reset is used, the
LCHWT Factors shown to the right of the Cooling Performance table will be used to adjust performance for leaving chilled water
temperatures.
Entering condenser temperature rows in this table should be chosen to span the expected range of operating conditions. For example,
if a water-cooled chiller operates between 85 F and 60 F ECWT, these should be the maximum and minimum temperatures for row
headings. Intermediate rows should have temperature headings evenly spaced between these maximum and minimum headings.
Also, because temperatures warmer than the design condition can sometimes occur for limited periods of time, it is useful to supply
data for warmer condenser temperatures if possible. For example, you will note that default performance maps and maps generated
by the Template feature provide data for 5 F above the design entering condenser temperature to provide for these conditions.
Column headings are automatically defined based on the number of columns specified for the table. An extra column is automatically
provided for the Maximum Capacity condition. This refers the maximum cooling that can be provided at each condenser temperature.
Currently plant simulation algorithms do not consider the use of capacities greater than the full load design capacity (special piping and
controls are required to utilize excess capacity). Therefore all the default maps and maps generated by the template feature will show
maximum capacity values equal to the values in the 100% load column.
Other important details:
a. If you are manually entering equipment performance data, all cells in this table must be filled in. Due to minimum load or surge
conditions in certain types of chillers, it may not be possible for the chiller to operate at certain conditions defined in the map. In
these special cases, simply enter a zero for a cell where operation is not possible. However, the number of zero cells in the table
must not exceed 25% of the total cells in the table.
b. If you are using the Chiller Template feature, then this table will contain the performance map the program generated using your
Template inputs. In this case, you will be able to view the performance data but cannot change the data.
c. The units of measure for the Cooling Performance table are determined by the units of measure used to define full load input power
on the Design Inputs tab. For example, for an electric drive chiller the choices would be input kW or kW/Ton (kW or ikW/kW in
Metric). The example above shows a case where the units of input are kW/Ton.
2. The Cooling Capacity table is the second grid on this tab. It lists cooling capacity as a function of entering condenser temperature
and part-load percent.
Page 29 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
DX Free Cooling Performance Map Tab
23.0 Entering Chillers ›› 23.3 Performance Map Inputs ››
Like the Cooling Performance table above, each row in this table contains data for a different entering condenser temperature. Each
column contains data for a different part-load ratio.
The only column in the table that can receive input is the Maximum Capacity column. This defines the maximum cooling that can be
provided for the corresponding condenser temperature. Currently "maximum capacity" features are not simulated by the program, so
the values in this column will always equal those in the 100% column.
If you are using the Chiller Template feature, then this table will contain the performance map the program generated using your
Template inputs. In this case, you will be able to view the performance data but cannot change the data.
Note: If the "Auto-Size Capacity" option is selected on the Design Inputs tab, this table will not appear since cooling capacity is not
known until capacity is calculated at the start of the simulation.
3. Table Dimensions are defined in the upper right-hand portion of the tab. The user is able to define the number of columns in the
Cooling Performance and Capacity tables, each containing data for a different part-load condition. The user is also able to define the
number of rows in the table, each containing data for a different entering condenser temperature.
4. LCHWT Factors for Performance are defined in the two input items immediately below the table dimensions on the right-hand side of
the tab. The map data in the Performance and Capacity tables represent performance at the design leaving chilled water temperature
for the chiller or heat pump. These LCHWT correction factors are only relevant if the equipment will be used in a plant which uses
chilled water reset, or a plant that uses a design LCHWT different from that defined for the chiller.
This first set of LCHWT factors is used to correct data in the Performance table. The correction factor is calculated using the equation:
(Input kW at new LCHWT) = Correction x (Input kW at Design LCHWT)
Correction = 1 + a x (LCHWT - Design LCHWT) + b x (LCHWT - Design LCHWT)2
The coefficients "a" and "b" in this equation can be defined by the user. Values are defaulted based on the chiller type that was
chosen. In most cases users accept the defaults. However, in special cases where correlations have been constructed for specific
equipment, users supply their own alternate values for the "a" and "b" coefficients.
5. LCHWT Factors for Capacity are defined in the lower two input items on the right-hand side of the tab. Similar to the LCHWT Factors
for Performance described above, these factors are used to correct for capacity at leaving chilled water temperatures other than the
design LCHWT.
Notes:
1. About Default Performance Maps. When using the "User-Defined" approach to entering chiller or heat pump data, a default
performance map is provided when you choose a equipment type on the General tab. The following paragraph provides additional
information about the data in these default maps.
Default performance maps are intended to represent "typical" performance for each class of chiller or reversible chiller. The water-
cooled equipment maps assume a design condition of 85 F entering condenser water temperature (ECWT) and 44 F LCHWT. In
Metric this is 29.4 C ECWT and 6.7 C LCHWT. The air-cooled equipment maps assume a design condition of 95 F outdoor air
temperature (OAT) and 44 F LCHWT. In Metric this is 35 C OAT and 6.7 C LCHWT. HAP will automatically adjust input power and
capacity data in the map when a new full load capacity and/or full load power value is entered on the Design Inputs tab. However, if
you switch to a different design condenser temperature, its important that you input map data appropriate for that new design point.
The program cannot do this automatically.
2. Air Cooled Chiller with Heat Recovery Condenser. When inputting an air cooled chiller that includes a heat recovery condenser,
there are two cooling sub-tabs on the Performance Map tab. One contains performance data for air-cooled chiller operation, and one
contains performance data for operating when the water-cooled heat recovery condenser is operating. Its important to make sure the
water-cooled performance map includes performance data at high entering condenser water temperatures so the program can
calculate accurate performance. Because the entering condenser water in this case is return water in the heating system, the entering
condenser water temperatures typically run at much higher levels than in a typical water-cooled chiller.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
DX Free Cooling Performance Map Tab
The DX Free Cooling Mode sub-tab on the Performance tab defines the performance of the chiller when operating in DX free cooling
mode. This tab contains two key components described below.
Page 30 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Heating Performance Map Tab
23.0 Entering Chillers ›› 23.3 Performance Map Inputs ››
1. The Performance Units inputs appear at the top of the tab. Performance data for DX fee cooling can be entered in one of two ways.
a. Relative Units - Capacity is specified as percent of full load chiller capacity and input power is input as kW/Ton (or ikW/kW). This
choice is required when a chiller is autosized since these units allow performance to be scaled to the full load capacity and input kW
of the chiller once those sizes are calculated.
b. Absolute Units - Capacity is specified as tons (or kW) and input power is specified as kW. This choice is only available when the
autosizing feature is turned off for the chiller and full load capacity is directly specified.
2. The DX Free Cooling Performance table appears next. This table defines the performance of the DX Free Cooling feature. The table
contains one row for each of three performance parameters. Columns in the table contain data for different operating conditions. The
performance parameters are:
a. "LCHWT - OAT" is the difference between the leaving chilled water temperature and the outdoor air dry-bulb temperature. As this
delta-T becomes larger, the ability of the DX free cooling system to provide cooling increases.
b. Capacity defines the cooling capacity of the DX free cooling system at the corresponding LCHWT-OAT delta-T.
c. Power defines the input power for the equipment running in DX free cooling mode at the corresponding LCHWT-OAT delta-T. It
includes power for the DX free cooling refrigerant pump and the condenser fans.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Heating Performance Map Tab
The Heating Performance sub-tab on the Performance tab defines the off-design and part-load performance of an air-to-water or water-
to-water heat pump in heating mode. This tab contains five key components described below.
Page 31 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
1. The Heating Performance table is the upper of the two grids on this tab. It contains input power data for off-design and part-load
heating conditions.
In this table each row contains performance data for a different entering evaporator temperature. Each column contains data for a
different part-load ratio. For example, in this sample screen image the heat pump input power for 32 F entering outdoor air
temperature and 50% load is 0.104 kW/MBH.
Together the rows and columns in this table define a "map" of performance data across the range of expected entering evaporator
temperatures and part-load conditions. During energy simulations, HAP will use this data to perform 2-way interpolations to determine
equipment input power at specific combinations of source temperature and part-load ratio. When hot water reset is used, the HWST
Factors shown to the right of the Heating Performance table will be used to adjust performance for leaving hot water supply
temperatures.
Entering source temperature rows in this table should be chosen to span the expected range of operating conditions. For example, if a
water-to-water heat pump operates between 60 F and 40 F EWT, these should be the maximum and minimum temperatures for row
headings. Intermediate rows should have temperature headings evenly spaced between these maximum and minimum headings.
Column headings are automatically defined based on the number of columns specified for the table. An extra column is automatically
provided for the Maximum Capacity condition. This refers to the maximum heating that can be provided at each entering evaporator
temperature. Currently plant simulation algorithms do not consider the use of capacities greater than the full load design capacity
(special piping and controls are required to utilize excess capacity). Therefore all the default maps and maps generated by the
template feature will show maximum capacity values equal to the values in the 100% load column.
Other important details:
a. If you are manually entering heat pump performance data, all cells in this table must be filled in. It may not be possible for the heat
pump to operate at certain conditions defined in the map. In these special cases, simply enter a zero for a cell where operation is
not possible. However, the number of zero cells in the table must not exceed 25% of the total cells in the table.
b. The units of measure for the Heating Performance table are determined by the units of measure used to define full load input power
on the Design Inputs tab such as kW or kW/MBH (ikW/kW).
2. The Heating Capacity table is the second grid on this tab. It lists heating capacity as a function of entering evaporator water
temperature and part-load percent.
Like the Heating Performance table above, each row in this table contains data for a different entering evaporator temperature. Each
column contains data for a different part-load ratio.
Page 32 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
23.4 Creating Chillers from Templates
23.0 Entering Chillers ››
Overview for Chiller Template Form
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
The only column in the table that can receive input is the Maximum Capacity column. This defines the maximum heating that can be
provided for the corresponding entering evaporator temperature. Currently "maximum capacity" features are not simulated by the
program, so the values in this column will always equal those in the 100% column.
Note: If the "Auto-Size Capacity" option is selected on the Design Inputs tab, this table will not appear since heating capacity is not
known until capacity is calculated at the start of the simulation.
3. Table Dimensions are defined in the upper right-hand portion of the tab. The user is able to define the number of columns in the
Heating Performance table, each containing data for a different part-load condition. The user is also able to define the number of rows
in the table, each containing data for a different entering condenser temperature.
4. HWST Factors for Performance are defined in the two input items immediately below the table dimensions on the right-hand side of
the tab. The map data in the Performance and Capacity tables represent performance at the design hot water supply temperature.
These HWST correction factors are only relevant if the heat pump will be used in a plant which uses hot water temperature reset, or a
plant that uses a design HWST different from that defined for the heat pump.
This first set of HWST factors is used to correct data in the Performance table. The correction factor is calculated using the equation:
(Input kW at new HWST) = Correction x (Input kW at Design HWST)
Correction = 1 + a x (HWST - Design HWST) + b x (HWST - Design HWST)2
The coefficients "a" and "b" in this equation can be defined by the user. Values are defaulted based on the heat pump type that was
chosen. In most cases users accept the defaults. However, in special cases where correlations have been constructed for specific
heat pumps, users supply their own alternate values for the "a" and "b" coefficients.
5. HWST Factors for Capacity are defined in the lower two input items on the right-hand side of the tab. Similar to the HWST Factors for
Performance described above, these factors are used to correct for capacity at leaving chilled water temperatures other than the
design HWST.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains how to create a chiller using the Chiller Template feature.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Chiller Template Form
The Chiller Template dialog appears when you press the Chiller Template button on the Chiller form. This dialog is used to generate a
complete chiller performance map based on a limited set of full load and part-load performance data. It serves as a useful alternative to
manually entering chiller performance data.
Example: For a chiller the design LCHWT, design condensing temperature, full load capacity, full load input power and a set of IPLV or
NPLV part-load performance points are all known. This set of data is not sufficient to create a complete set of chiller inputs for HAP
energy simulations. However, this limited set of data can be entered using the Template option. HAP will then use your input data in
performance correlations to generate the complete set of chiller performance data required for energy simulations.
Note that template features are currently offered for water-cooled centrifugal, rotary screw, packaged screw and packaged reciprocating
types of chillers.
Page 33 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
The Chiller Template form consists of three components.
1. The Title Bar appears across the top of the form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains inputs required by the Template feature.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to generate a full set of chiller inputs based on the Template data you specified. After chiller data is generated, you'll be
returned to the Chiller form. Results of the Template calculation will be displayed on the Performance Map tab of the Chiller form.
b. Press Cancel to return to the Chiller form without performing Template calculations.
c. Press Help to display this overview topic.
How To. To use the Chiller Template dialog to generate chiller performance data:
1. Select the chiller type in the "Chiller Template" drop-down list.
2. Enter the full load performance data and minimum control points on the left-hand side of the dialog.
3. Specify the number of part-load data points you have. When using IPLV or NPLV points the number will typically be 4. If you have a
more detailed part-load curve, a larger number of points could be entered.
4. Enter the % load, entering condenser temperature and input power data in the performance table on the right-hand side of the dialog.
5. Press the OK button to use the Template inputs to generate a complete performance map for the chiller. After pressing OK, you will
return to the Chiller form.
6. Review data on the Design Inputs tab of the Chiller form. Many of these items are copied directly from your Template inputs. Others,
such as cooler and condenser flow rates, are defaulted and may need to be revised.
7. Review data on the Performance Map tab. This tab contains the results of the template calculation – a complete performance map
based on the limited set of performance points you entered. You will only be able to view this performance data. Template-generated
performance maps may not be changed.
8. Once all the data has been reviewed, press the OK button to save the chiller and return to the HAP main window.
For more information about input items on the Template dialog, click the desired item below.
Chiller Type
Full Load Burner Input
Full Load LCHWT
Full Load Engine Input
Full Load Condensing Temperature
Minimum Condenser Temperature
Full Load Capacity
Minimum Load
Full Load Power
Number of Part Load Points
Full Load Steam Input
Part Load Performance Data
Page 34 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Template Chiller Type
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load LCHWT
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load ECWT, EACWT or OAT
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load Capacity
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load Power
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Chiller Type
This item is used to choose the chiller type for the template data you are entering. Chiller type is used for two purposes:
• It will determine the input items that appear on the template dialog.
• It will determine the correlations used to produce the complete performance map for your chiller. The Template feature uses your
input data together with performance correlations to estimate a complete performance map for the chiller. Which correlations are
used depend on the type of chiller involved.
Currently template features are offered for water-cooled centrifugal, rotary screw, packaged screw and packaged reciprocating chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load LCHWT
This item defines the leaving chilled water temperature (LCHWT) for the chiller at its full load design point. The full load capacity and
input power specified on this dialog are rated at this LCHWT. In addition, the performance data entered on the right-hand side of the
dialog is also rated at this LCHWT.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load ECWT, EACWT or OAT
This item defines the entering condenser temperature for the chiller at its full load design point. The full load capacity and input power
specified on this tab are rated at this temperature.
• For a water-cooled electric-drive chiller, the entering condenser water temperature (ECWT) is defined.
• For a water-cooled absorption chiller, the entering absorber/condenser water temperature (EACWT) is entered.
• For an air-cooled chiller, the entering outdoor air temperature (OAT) for the condenser is defined.
This value establishes the upper boundary for the performance map generated for your template inputs. This performance map extends
from 5 F (2.8 K) above the full load condenser temperature to the minimum condenser temperature specified.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load Capacity
This item defines the chiller capacity at the its full load design point. This capacity corresponds to the full load LCHWT and entering
condenser temperature (ECWT, EACWT or OAT) conditions specified earlier on this dialog. Typically full load capacity is obtained from
chiller selection results or catalog data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load Power
This item defines the chiller input power at its full load design point. It corresponds to the full load LCHWT, entering condenser
temperature (ECWT or OAT) and the full load capacity conditions specified earlier on this dialog. Typically full load power is obtained
from chiller selection results or catalog data.
Page 35 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Template Full Load Steam Input
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load Burner Input
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Template Full Load Engine Input
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Minimum ECWT, EACWT, or OAT
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Input power can be defined as kW/Ton (ikW/kW) or as total kW. To change the units of measure, select the desired units label in the
drop-down list to the right of this input item.
This input item only applies to electric-drive chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load Steam Input
This item defines the chiller steam input at its full load design point. It corresponds to the full load LCHWT, entering absorber/condenser
temperature (EACWT) and the full load capacity conditions specified earlier on this tab. Typically full load steam data is obtained from
chiller selection results or catalog data.
Steam input can be defined as lb/ton-hr (kg/kWh) or as total lb/hr (kg/hr). To change the units of measure, select the desired units label in
the drop-down list to the right of this input item.
This item only applies to steam absorption chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load Burner Input
This item defines the burner energy input for the chiller at its full load design point. It corresponds to the full load LCHWT, entering
absorber/condenser temperature (EACWT) and the full load capacity conditions specified earlier on this dialog. Typically full load burner
input data is obtained from chiller selection results or catalog data.
Burner input can be defined as MBH/ton (ikW/kW) or as total MBH (ikW) energy input. To change the units of measure, select the desired
units label in the drop-down list to the right of this input item.
This item only applies to direct-fired absorption chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Full Load Engine Input
This item defines the energy input to the chiller at its full load design point. It corresponds to the full load LCHWT, entering condenser
temperature (ECWT) and the full load capacity conditions specified earlier on this dialog. Typically full load engine input data is obtained
from chiller selection results or catalog data.
Engine energy input can be defined as MBH/ton (ikW/kW) or as total MBH (ikW) energy input. To change the units of measure, select the
desired units label in the drop-down list to the right of this input item.
This item only applies to engine chillers.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum ECWT, EACWT, or OAT
This item defines the minimum entering condenser temperature permitted for the chiller. It establishes the lower boundary for the
performance map that will be generated from your template data.
1. For a water-cooled electric-drive chiller, the entering condenser water temperature (ECWT) is defined.
2. For a water-cooled absorption chiller, the entering absorber/condenser water temperature (EACWT) is entered.
3. For an air-cooled chiller, the entering outdoor air temperature (OAT) for the condenser is defined.
Page 36 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Template Minimum Load
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Number of Part Load Points
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
Part Load Performance Data
23.0 Entering Chillers ›› 23.4 Creating Chillers from Templates ››
23.5 Importing Chiller Data
23.0 Entering Chillers ››
Overview for Chiller Import Dialog
23.0 Entering Chillers ›› 23.5 Importing Chiller Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Template Minimum Load
This item defines the minimum load condition at which either cycled operation begins or hot gas bypass operation begins. It is specified
as a percent of the full load chiller capacity. It also defines the minimum percent load boundary for the performance map that is
generated from your template inputs.
For packaged chillers, this minimum load point is typically determined by the capacities of compressors in the chiller and is often
published in the manufacturer’s literature. For applied chillers it tends to vary with operating conditions and therefore an average value
must be estimated for use in the program.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Number of Part Load Points
This item defines the number of part-load performance points you will supply with your template inputs. A "data point" refers to one group
of related % load, condenser temperature and input power data.
In many applications the performance data you have for the chiller will be limited to four IPLV or NPLV data points. In this case the
"number of part load points" is four. In other cases a larger set of data points may exist in which case that number should be entered
instead.
When you specify a number of data points, the Part Load Performance table on the right side of the dialog will expand or contract to
accommodate your data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Part Load Performance Data
The Part Load Performance Data table on the right-hand side of the dialog is used to enter part-load performance information for the
chiller. In this table each row contains data for a different chiller operating condition. Each column contains a different value describing
the operating condition. Three columns of data are provided:
1. % Load defines the chiller load as a percentage of the Full Load Capacity defined earlier on this dialog. For example, if the full load
capacity is 500 Tons and the % Load is 75%, this refers to a load of 375 Tons.
2. Condenser Temperature specifies the entering condenser temperature for each operating condition. The entering condenser water
temperature (ECWT) is entered for water-cooled electric-drive chillers; the entering absorber/condenser water temperature (EACWT)
is entered for absorption chillers; the entering outdoor air temperature (OAT) is defined for air-cooled chillers.
3. Input Power defines the chiller performance at each operating condition. The units of measure for this column will match the units you
used to define full load input power. Depending on the chiller type, this item describes full load electrical input, full load steam input, full
load burner input or full load engine input.
Values in the 100% load row of the table are established by your full load inputs on the left side of the dialog and may not be changed. All
subsequent rows in the table can be edited.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains how to import chiller performance data from Carrier Electronic Catalog.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 37 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
23.6 Common Tasks
23.0 Entering Chillers ››
Creating a New Chiller
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Overview for Chiller Import Dialog
The Import button on the Chiller Properties window is used to read chiller or heat pump performance data from a file produced by one of
the Carrier Electronic Catalog (E-CAT) Chiller Builder tools. Using this feature you can import performance data for an actual chiller or
heat pump selection.
The following steps are required to import chiller or heat pump data into HAP:
1. Obtain an import data file from your Carrier sales engineer. Save this data file to your computer’s hard disk. You can save the file in
any folder, but you can save time by placing it in the \E20-II\TEMP folder on the drive containing HAP.
2. Run HAP, choose the Chillers data category, and click on the  option to create a new chiller. Then press the
Import button.
3. The Open window will appear as shown below. Use this window to locate the import file that was saved to disk in step #1 and then
select the file.
The window initially shows import files in the \E20-II\Temp folder. If the file is in a different folder you can browse using your mouse by
clicking on command buttons and on folder names which appear. This allows you to move up and down the folder tree structure of
your hard disk. As an alternative, you can enter the path leading to your import file in the "File Name" item toward the bottom of the
dialog.
Once you locate your import data file, you can select the file by double-clicking on the file name, or by highlighting the name and then
pressing the Open button. Equipment performance data will be read from the file you choose and will be displayed in the Chiller
Properties window.
At any time if you wish to exit without importing data, simply press the Cancel key.
4. After data has been imported into the Chiller Properties window, review the data before saving it.
Note that many of the input items will now be shown as display-only. This is because the program preserves performance data
obtained from a E-CAT program as is. The only way to change it is to rerun the E-CAT program, make a new file and then import it.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with chiller input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 38 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm
Editing an Existing Chiller
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Printing Chiller Inputs
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Deleting Chiller Inputs
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Copying a Chiller
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Duplicating a Chiller
23.0 Entering Chillers ›› 23.6 Common Tasks ››
Creating a New Chiller
Please see Creating a New Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Chiller
Please see Editing an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Chiller Inputs
Please see Generating Input Data Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Chiller Inputs
Please see Deleting Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Chiller
Please see Copying Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Chiller
Please see Duplicating an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 39 of 39
23.0 Entering Chillers
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh155F.htm