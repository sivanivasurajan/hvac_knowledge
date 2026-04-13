13.0 Entering Buildings
13.1 Overview for Building Form
13.0 Entering Buildings ››
Overview for Building Form
13.0 Entering Buildings ›› 13.1 Overview for Building Form ››
This chapter explains input data for Building alternatives.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of the organization of Building data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Building Form
About Buildings. A Building is the container holding all the HVAC and non-HVAC systems for one design scenario being studied in
an energy analysis. Taken literally, a building represents one individual structure. However, the definition of a building is flexible. It
can represent a portion of an actual building such as a renovation or addition. It can also represent a group of structures. For
example, a "building" could represent a campus in which all the structures are served by a common set of plant equipment.
The Building Form, shown above, is used to define the plants, systems and non-HVAC equipment included in the energy analysis.
It also defines the utility rate structures used to calculate energy and fuel costs. The Building form contains three key components:
1. The Title Bar appears across the top of the form. It lists the name of the building whose data is being defined. At the right end of
the title bar is a button for closing the form.
Page 1 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
13.3 Plant Selection Data
13.0 Entering Buildings ››
Plants Tab / Building Form
13.0 Entering Buildings ›› 13.3 Plant Selection Data ››
2. The Working Area is in the center of the form and contains four categories of information represented as four separate tabs in a
notebook. To move from one tab to another simply click on the desired tab name. The four tabs are as follows:
a. Plants is used to define the chilled water, hot water and steam plants included in the building. It is also used to enter the
reference name for the building.
b. Systems specifies the air systems included in the building.
c. Misc. Energy contains information about non-HVAC systems in the building that have not already been accounted for. For
example energy use for lighting and electrical equipment in conditioned areas has already been accounted for in space inputs,
but energy use for such things as exterior lighting has not been accounted for and must be defined here.
d. Meters defines the utility rate structures used to calculate energy and fuel costs for the building. It also includes three
additional inputs used in cost and energy calculations.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the building inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes. If you press Cancel while creating a new building,
the new building will not be added to your project.
c. Press Help to display this overview topic.
Further Information. For more information about the tabs on this form click the desired item below.
Plants Tab.
Systems Tab.
Misc. Energy Tab.
Meters Tab
Building Features. Finally, HAP provides useful features for:
Creating new buildings.
Editing an existing building.
Printing building data.
Deleting building.
Copying a building.
Duplicating a building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Plant Selection tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Plants Tab / Building Form
The Plants tab is used to define the chilled water, hot water and steam plants included in the building. It is also used to enter the
reference name for the building.
Page 2 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
13.4 System Selection Data
13.0 Entering Buildings ››
Systems Tab / Building Form
13.0 Entering Buildings ›› 13.4 System Selection Data ››
The tab is divided into two sections:
1. General contains the reference name for the building. This reference name will appear elsewhere in the program on selection
lists and reports. The reference name appears i the list of available buildings on the HAP main window and on reports containing
building input data and building simulation results.
Therefore, it is helpful to use a descriptive name. Typically the name includes information about the design case or energy
conservation measures being studied.
2. Plants Included in Building is used to select the chilled water, hot water and steam plants included in the building. This section
contains a list of all plants in your project. To include a plant, mark the check box next to its name. To remove a plant, uncheck
the check box next to its name.
When plants are selected, the program will automatically include systems served by the plants in the building. These systems
and their system multipliers will appear on the Systems tab. In addition, if you remove a plant, the systems served by the plant
will be removed from the list shown on the Systems tab.
Note that inclusion of plants in the building is optional. Many applications use only packaged or split DX equipment and
therefore do not involve chilled water, hot water or steam equipment. In these cases no plants in the list should be selected.
DX equipment will be linked to the building on the Systems tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input dat aon the System Selection tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 3 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
Systems Tab / Building Form
The Systems tab is used to define the air system equipment included in the building. The tab has three key components:
1. Systems in Current Project. The box on the left side of the tab lists all systems in the current project.
2. Systems Included in This Building. The box on the right side of the tab lists the systems that have been included in the
building. This box also lists the system multipliers.
3. Add and Remove Buttons appear between the two boxes. The Add button is used to include systems in the building. The
Remove button is used to delete systems from the list of included systems.
Use of these features is described below.
Including Systems in the Building. To include systems in a building:
1. First select one or more systems in the "Systems in Current Project" box on the left.
2. Then press the Add button. All systems you selected will appear in the "Systems Included in this Building" box on the right. Note
that this does not remove the system names from the box on the left. The box on the left always contains a complete list of all
systems in your project. The box on the right only lists those systems you have included in the building.
Removing Systems from the Building. To remove a system that was previously included in the building:
1. First select one or more systems in the "Systems Included in This Building" box on the right.
2. Then press the Remove button. The selected systems will be removed from the box on the right.
Specifying System Multipliers. In some situations a building will contain two or more identical air systems. In the figure above, a
multi-story office building has five intermediate floors with identical load patterns and air handling equipment. Therefore, one air
system serving a typical intermediate floor has been defined and is used with a multiplier of 5 to account for the total loads and
energy use for the five intermediate floors. System multipliers can be defined in two ways:
a. When a system is included in the building by pressing the Add button, you can press the Add button multiple times to increment
the multiplier. For example, if you click the Add button five times, the multiplier will change to "5".
b. After including a system in the building you can edit its multiplier. Click on the system name in the "Systems Included in this
Building" box on the right. Then enter the multiplier. Note that the multiplier must be a two digit number. Therefore if you are
entering a multiplier of 5, enter the value "05".
Application Information. All systems included in a building must be defined. Therefore, packaged or split DX systems as well as
systems using chilled water cooling and hot water or steam heating must be defined here.
Page 4 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
13.5 Miscellaneous Energy Data
13.0 Entering Buildings ››
Misc. Energy Tab / Building Form
13.0 Entering Buildings ›› 13.5 Miscellaneous Energy Data ››
When chilled water, hot water or steam plants are used in the building, selection of these plants on the Plants tab will automatically
generate system selections and multipliers on this tab. For example, in the figure above AHU-1, AHU-2 and AHU-3 are chilled
water / hot water systems that are served by chilled water plant and hot water plants selected earlier on the Plants tab. The program
will automatically include these three as selected systems and will automatically determine their system multipliers.
Systems which are not associated with chilled water, hot water or steam plants must be directly specified on this tab. In the figure
above, AHU-4 and AHU-5 use DX cooling equipment and were directly specified on this tab.
In many applications all systems in the building will use DX cooling equipment. Therefore no plants will be selected on the Plants
tab, and all systems included in the building must be directly selected on the Systems tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Miscellaneous Energy Data tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Misc. Energy Tab / Building Form
The Miscellaneous Energy tab contains information about non-HVAC systems in the building that have not already been accounted
for. This is optional information. Whether miscellaneous energy use needs to be defined depends on the scope of your energy
analysis study. The application section below discusses this in further detail.
This tab allows up to 10 miscellaneous energy uses to be defined. The tab is arranged as a table in which each row contains data
for one energy use item, and columns describe the different characteristics of the energy use. Columns in this table contain the
following information:
Page 5 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
13.6 Utility Meters Data
13.0 Entering Buildings ››
Meters Tab / Building Form
13.0 Entering Buildings ›› 13.6 Utility Meters Data ››
1. Name is a reference name for the energy item. It appears here, on the input data report for the building, and on the LEED NC 2.2
EA Credit 1 Summary report where each miscellaneous energy use item is tabulated separately in tables 1.8.1 and 1.8.2.
2. Process is an optional input that defines whether the item qualifies as process energy for purposes of a LEED Energy and
Atmopshere Credit 1 analysis. If it is a process energy use, place a check in the box. Otherwise leave the box blank. If you are
not performing a LEED analysis, then this item is not relevant and can be left blank.
3. Energy or Fuel Type defines what energy or fuel source is used for the item. Choose the desired option in the drop-down list.
During the simulation this information will be used to assign energy or fuel use to the proper category. For example, if the fuel
type is natural gas, fuel use for this item will be added to the building’s natural gas consumption profile.
4. Peak Use specifies the maximum energy or fuel rate for the item. Electrical energy items are defined in units of kW. Fuel use
items are defined in terms of MBH (or kW in SI Metric).
5. Schedule defines the fractional schedule used for this energy item. This schedule describes how energy or fuel use varies hour
by hour. For example, if the 8 AM value in one of the schedule profiles is 80%, that means that 80% of the peak energy use
occurs during this hour.
If you defined a schedule for your miscellaneous energy use ahead of time, simply select it from the drop-down list. Otherwise,
use the  item in the drop-down list to create a new schedule. When entering schedule data, be sure to
specify the schedule type as "fractional".
Existing schedules can also be modified from the Misc. Energy Tab by pressing the Edit button next to the schedule name.
Application Information. HAP automatically accounts for certain types of non-HVAC energy use:
a. Lighting energy use in conditioned areas was specified in space inputs and is automatically calculated as part of system
simulation calculations.
b. Electrical equipment energy use in conditioned areas was also specified in space inputs and is automatically calculated as part of
system simulation calculations.
Whether additional categories of non-HVAC energy use need to be accounted for depends on the scope of the energy analysis
study. Some studies focus mainly on the HVAC equipment. Others focus on energy consuming systems only within the building. Still
others focus on energy use by both systems inside and outside the building. Application tips:
a. If miscellaneous heat gains from equipment were defined in space inputs, this data only accounts for the effect of the heat gain on
building loads. If heat gains are associated with energy or fuel use, this use should be specified on the Miscellaneous Energy tab.
For example, heat gain from gas cooking appliances in a kitchen space might have been defined in space inputs. This permitted
calculation of the load for the kitchen space, but does not account for gas consumption and cost. The gas consumption must be
defined on the Misc. Energy tab in order for it to be included in cost calculations.
b. Energy consuming systems which do not contribute heat gain to conditioned areas and those which are outside the building are
also candidates for consideration as miscellaneous energy items. Examples include entrance, facade and parking lot lighting, and
elevator motors.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Utility Meters tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Meters Tab / Building Form
The Meters Energy tab defines the utility rate structures used to calculate energy and fuel costs for the building. It also includes
three additional inputs used in cost and energy calculations.
Page 6 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
Meter Selections
13.0 Entering Buildings ›› 13.6 Utility Meters Data ››
The tab is divided into two sections:
1. The Meters section is used to select electric and fuel rate structures that will be used to calculate energy and fuel costs for the
building.
2. The Miscellaneous Data section contains additional inputs involved with calculating energy costs and check figures on the
building reports. These items include:
Average Building Power Factor
Source Electric Generating Efficiency
Additional Floor Area
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Meter Selections
Page 7 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
Average Building Power Factor
13.0 Entering Buildings ›› 13.6 Utility Meters Data ››
Source Electric Generating Efficiency
13.0 Entering Buildings ›› 13.6 Utility Meters Data ››
The Meters section of this tab allows selection of the utility rates that will be used to calculate energy and fuel costs for the building.
Separate items are provided for defining the electric rate and a fuel rate for each possible fuel source used in the building. A utility
rate can be linked to the building in two ways.
1. Selecting an Existing Rate. If you previously created and stored electric rates or fuel rates in your project you can simply select
the desired rate from the drop-down list.
2. Creating a New Rate. If you have not yet created an electric rate or fuel rate, choose the "" item in the drop-
down list. For example, when this is done for the electric rate item, the Electric Rate form will appear and will allow you to enter
data for a new rate. When you press OK to exit the Electric Rate form, your rate data will be saved and the rate will be linked to
the building automatically. A similar procedure can be used to create new fuel rates.
In addition, you can modify existing rate data directly from the Building form by pressing the button to the left of the drop-down list.
For example, if you press the Natural Gas button, the Fuel Rate form will appear and will display data for the currently selected fuel
rate for natural gas. After modifying data, press the OK button to return to the Building form.
Notes:
a. An electric rate must be selected for every building.
b. Fuel rates only need to be selected for those fuel sources used in the building.
c. If a fuel source is used in the building but no fuel rate is selected, a fuel cost of zero will be calculated for that fuel source.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Average Building Power Factor
This item defines an average building power factor used to convert electric power data from units of kW to kVA. It is only applicable
when the electric rate chosen for the building uses units of kVA for demand-related charges. If units of kVA are not used, the power
factor is not relevant. Its value can be left at 100%.
Further Details. When entering electric rate data, the user has the option of defining demand-related charges in terms of working
power measured in kW or apparent power measured in kVA. When the kVA option is used, the program computes a simple
estimate of building kVA each hour by dividing kW power data by the average building power factor. The power factor is the average
ratio of working power divided by apparent power for the building.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Source Electric Generating Efficiency
This item defines the average generating efficiency for electric power plants that provide energy to the building. This value is used to
calculate "source" energy totals on the two Energy Budget reports. This input is only required if the program will be used to generate
the Energy Budget reports and local energy codes require that both "site" and "source" energy totals be provided. If this feature is
not needed, set the efficiency to 100%.
Further Details. Energy Budget reports generated by HAP list the "site" and "source" energy use for a building. Site energy is the
actual energy consumed by equipment in the building. Source energy is an estimate of the energy required to generate electricity
provided to the building. The difference between site and source energy quantities is due to inefficiencies in generating electricity
and transmitting it to the building site. When this is required by energy codes, the codes usually mandate the efficiency value to be
Page 8 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
Additional Floor Area
13.0 Entering Buildings ›› 13.6 Utility Meters Data ››
13.7 Common Tasks
13.0 Entering Buildings ››
Creating a New Building
13.0 Entering Buildings ›› 13.7 Common Tasks ››
Editing an Existing Building
13.0 Entering Buildings ›› 13.7 Common Tasks ››
Printing Building Inputs
13.0 Entering Buildings ›› 13.7 Common Tasks ››
Deleting Building Inputs
13.0 Entering Buildings ›› 13.7 Common Tasks ››
used. It typically varies between 25% and 33%. For fuels and non-electric energy sources, site and source energy values are equal
since the fuel is consumed at the building site.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Additional Floor Area
This item defines the non-conditioned floor area in the building, not already accounted for. This input is used together with the
conditioned floor area to calculate cost per sqft (cost per sqm) or energy per sqft (energy per sqm) check figures on the building
simulation reports. In certain cases local energy codes may require that these check figures be based on the gross floor area of the
building rather than just the conditioned floor area. If this is not required, specify zero as the additional floor area.
Further Details. Earlier in the energy analysis, spaces were defined to describe the conditioned regions of the building. During
energy simulations, the program sums the floor area for all spaces in the building to determine a conditioned floor area total. Annual
Cost, Annual Energy and Energy Budget reports generated by the program provide data both on a gross basis (Total Cost, Total
Energy) and on a per sqft or per sqm basis. Certain energy codes require that the per sqft or per sqm figures be based on the gross
building floor area rather than the conditioned floor area. For these situations, additional floor area for such regions as unconditioned
storerooms, stairwells and corridors must be defined. HAP will combine the additional floor area with the conditioned floor area to
determine the gross building floor area. This gross area will be used to calculate per sqft and per sqm check figures.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with Building input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Building
Please see Creating a New Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Building
Please see Editing an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Building Inputs
Please see Generating Input Data Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm
Copying a Building
13.0 Entering Buildings ›› 13.7 Common Tasks ››
Duplicating a Building
13.0 Entering Buildings ›› 13.7 Common Tasks ››
Deleting Building Inputs
Please see Deleting Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Building
Please see Copying Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Building
Please see Duplicating an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 10 of 10
13.0 Entering Buildings
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh5071.htm