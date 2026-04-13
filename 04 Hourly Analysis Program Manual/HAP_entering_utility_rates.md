26.0 Entering Utility Rates
Utility Rate Form Overview
26.0 Entering Utility Rates ››
This chapter explains input data for electric and fuel utility rates.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Utility Rate Form Overview
The Electric Rate form is used to define the pricing structure for electrical energy use in a building. The Fuel Rate form is used to
define the pricing structure for use of one type of fuel in a building. Electric and fuel pricing data is used to determine annual costs in
an energy simulation. Both are used in the full HAP edition but not in HAP System Design Load.
Quick Reference: EIA Electric and Fuel Prices
While Electric Rates and Fuel Rates are two categories of data in a HAP project, both use the same user interface for entering data.
Features of this common user interface will be described in this and the following series of help topics. In cases where features are
identical, examples for an electric rate will be given. In cases where features differ slightly, examples for both electric and fuel rates
will be provided.
The Electric Rate and Fuel Rate forms contain three key components:
1. The Title Bar appears across the top of the form. It lists the name of the electric rate or fuel rate whose data is being defined. At
the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains four categories of information represented as four separate tabs in a
notebook. To move from one tab to another simply click on the desired tab name. The four tabs are as follows:
Page 1 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Basic Rules for Entering Energy, Fuel and Demand Charges
26.0 Entering Utility Rates ››
a. General contains basic information about units of measure, customer charges, scheduling and emissions. If a "simple" rate
structure is being defined, this is the only tab that will be available for data entry. When a "complex" rate structure is defined,
the other three tabs in the form become active.
b. Energy or Fuel Charges is used to define the pricing structure for the energy charge component of an electric rate or the fuel
charge component of a fuel rate.
c. Demand Charges contains pricing information for the demand charge component of the rate.
d. Demand Clauses provides inputs for any clauses used to define the calculation of billing demand. Billing demand is used for
both demand charges and any demand-related energy charges.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the utility rate inputs and return to the main program window.
b. Press Cancel to return to the main program window without saving changes. If you press Cancel while creating a new rate
structure, the new rate will not be added to your project.
c. Press Help to display this overview topic.
Further Information. For more information about the tabs on this form click the desired item below.
General Tab
Energy and Fuel Charge Tabs
Demand Charge Tab
Demand Clause Tab
Application Information. Individual utility companies charge for energy use, fuel use and demand in widely different ways and use
vastly different terminology in stating their pricing structures. This presents a challenge for developing one consistent approach to
modeling utility rate structures in the program. HAP uses a modular approach to meet this challenge. The program provides building
blocks representing the common billing mechanisms for energy, demand, demand determination and miscellaneous charges. The
user is able to pick and choose among these building blocks to assemble a utility rate model that best represents the pricing
structure used for their building. The following topics explain how to apply program features to define electric and fuel rates.
Utility Rate Applications
Basic Rules for Defining Energy, Fuel and Demand Charges
Utility Rate Features. Finally, HAP provides useful features for:
Creating new utility rates
Editing an existing utility rate.
Printing utility rate data.
Deleting utility rates.
Copying a utility rate.
Duplicating a utility rate.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Basic Rules for Entering Energy, Fuel and Demand Charges
The Electric Rate and Fuel Rate forms provide the flexibility to enter many different pricing structures. However certain rules must
be observed when organizing the input data to avoid situations where the data is ambiguous or incomplete. This topic explains
these rules. Separate discussions are provided below for electric energy charges, fuel charges, demand charges and a special type
of electric energy charge called a "Compound Block" charge.
Electric Energy Charges
Rules for entering electric energy charge data are provided below. Information about terminology used in this discussion can be
found in the application discussion for energy charges.
1. Every electric rate must include an energy charge. Therefore at least one step on the energy charge tab must be defined.
2. Energy prices must cover energy use for all time periods during the year. If seasonal scheduling and/or time-of-day scheduling
are used, energy prices must cover all seasons and all time-of-day periods. Time periods when energy use is unbilled are not
permitted.
3. Energy prices in a stepped charge structure must cover all energy use. The last step in a group of related steps must be
9999999. "9999999" is interpreted by the program as meaning "all additional energy use". A stepped charge structure imposes
Page 2 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
26.1 General Inputs
26.0 Entering Utility Rates ››
prices for different quantities of energy use. For example, the first 10,000 kWh has one price, the next 30,000 kWh has a different
price, and so on.
4. Overlapping energy prices are not permitted. Overlapping prices are two separate price items referring to the same energy use
during the same time period. Typically overlapping charges are created by defining one price item for a specific season and/or
time-of-day period and a separate price item assigned to all seasons or all periods.
5. Related items in a stepped charge structure must be consecutive items in the energy charge table. When prices are defined for
different quantities of energy use (e.g., first 10,000 kWh, next 30,000 kWh, etc...), these price items must be in consecutive rows
of the energy charge table.
Fuel Charges
Rules for entering fuel charge data are the same as for electric energy charges. In the discussion of energy charges above, simply
substitute "fuel" for "electric energy".
Demand Charges
Rules for entering demand charge data are provided below. Information about terminology used in this discussion can be found in
the application discussion for demand charges. Note that the following rules apply to both electric and fuel demand charges.
1. The demand charge is an optional component of the utility rate. Some rate structures include a demand charge and some don’t.
2. Demand prices are not required to cover all time periods during the year. Frequently demand charges only apply to peak
demands during certain times of day or times of year.
3. Demand prices in a stepped charge structure must cover all demand levels. The last demand step in a group of steps must be
9999999. "9999999" is interpreted by the program as meaning "all additional demand". A stepped charge structure imposes
prices for different quantities of demand. For example, the first 100 kW has one price, the next 500 kW has another price, and so
on.
4. Overlapping demand prices are permitted. Overlapping prices are two separate price items referring to the demand measured
during the same period of time. Typically overlapping charges occur when the rate schedule includes a "non-time-related" or
"NTR" demand charge. For example a rate might impose one demand charge for maximum demand measured only during "on-
peak" hours, and a second demand charge for maximum demands measured considering all 24 hours in the day.
5. Related items in a stepped charge structure must be consecutive items in the demand charge table. When prices are defined for
different quantities of demand (e.g., first 100 kW, next 500 kW, etc...), these price items must be in consecutive rows of the
demand charge table.
Compound Block Energy Charges
A "Compound Block" energy charge is a special type of electrical energy charge that involves a two-tier structure. The first tier is a
series of demand blocks having units of kWh/kW. Each demand block is subdivided into individual energy blocks having units of
kWh. Because this type of energy charge differs from all others, a different set of rules is used when entering its data. For further
information on Compound Block charges and the terminology used below, please refer to the application discussion for energy
charges.
1. The Compound Block energy charge must contain two or more demand blocks.
2. There must be at least one energy step per demand block.
3. All energy steps must be related to a demand block. No independent energy steps are permitted.
4. The Season and Period specified for energy steps in a demand block must match those for the demand block. For example, if
"Summer" is specified for the demand block, all energy steps associated with this demand block must also use specify "Summer".
5. Demand Blocks in a related group must be positioned consecutively. When seasonal or time-of-day scheduling is used, there will
be two or more groups of demand blocks in the structure (for example, one for summer and one for winter). The demand blocks
in each related group, plus the associated energy steps must be in consecutive rows of the energy charge table.
6. The last energy step in a demand block must be 9999999 kWh. The program interprets "9999999" as meaning "all additional
kWh".
7. Demand blocks must cover all levels of demand. The last demand block in a group of related demand blocks must be 9999999
kWh/kW. The program interprets "9999999" as meaning "all additional kWh/kW".
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the General tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 3 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
General Tab / Utility Rate Form
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
General Tab / Utility Rate Form
The General tab on the Electric Rate and Fuel Rate forms contains basic information about the rate such as units of measure,
customer charges, scheduling and emissions.
Quick Reference: EIA Electric and Fuel Prices
The tab is divided into four sections:
1. The General section on the left side of the tab contains a series of inputs defining various aspects of the rate:
a. Rate Name is a reference label for the utility rate.
b. Rate Type defines whether the rate is "simple" containing only a flat energy or fuel price and a customer charge, or is
"complex". Complex charges can contain energy charges, demand charges and demand determination clauses, and can make
use of seasonal and time of day scheduling features.
c. Energy Units and Conversion items specify the units of measure for the energy or fuel and the relationship between those units
and standard energy unit such as kWh or kBTU.
d. Demand Units defines the units of measure for billing demand. For electric rates demand can be measured as kW or kVA. For
fuel rates demand can represent peak hourly consumption or peak daily consumption.
e. Flat Price only applies when a "simple" type of rate is being entered. It is the single energy or fuel price that applies to all
consumption.
f. Customer Charge is a fixed charge imposed each month, regardless of energy or demand levels.
g. Minimum Charge defines the minimum charge imposed each month. In some cases this is equal to the customer charge and in
others is equals the charge for a minimum energy consumption level.
h. Tax Rate is used to calculate the tax on the energy or fuel bill. This item is optional.
Page 4 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Rate Name
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Rate Type
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Energy Units and Conversion
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
2. The Seasonal Scheduling section is used to assign billing seasons to the months of the year. It is used when separate prices are
defined for different times of year. It only applies when defining a "complex" type of rate.
3. The Time-Of-Day Scheduling section is used to link a schedule to the utility rate which specifies hours included in the various
time-of-day periods such as Peak and Off-Peak. This section is only used when separate prices are specified for different time-of-
day periods, or when demand determination requires use of time-of-day periods. It only applies when defining a "complex" type of
rate.
4. The Emissions Analysis section allows greenhouse gas emission rates to be defined for electrical energy or the particular fuel
source for this utility rate. This is an optional section. If emissions data is supplied, the program will estimate total CO2 equivalent
(CO2e) emissions based on the total energy or fuel consumption for the year. This data is often required for green building design
applications.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Rate Name
This item is a reference name for the electric rate or fuel rate. It will appear elsewhere in the program on selection lists and reports.
The reference name appears:
a. In the list of available electric rates or fuel rates on the HAP main window.
b. In the list of available utility rates when linking utility rates to a building.
c. In input data reports for electric rates, fuel rates and building data.
Therefore, it is important to use a descriptive name. Typically the name includes information about the utility company, the rate
schedule designation and the fuel source.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Rate Type
HAP provides options for entering a simple rate structure or a complex structure.
1. A "simple" rate structure contains one flat energy or fuel price, which applies to all consumption, and a customer charge. All
information for the simple rate is entered on the General tab. When a "simple" rate is chosen the Energy (or Fuel), Demand and
Demand Clause tabs are not used and are therefore disabled. This option is used both for those cases where the local utility
company’s rate structure is very simple, and for conceptual studies where it is not yet necessary to model all the details of the
actual rate.
2. A "complex" rate allows all the aspects of an actual rate structure to be defined. These include various kinds of energy or fuel
charges, demand charges and demand determination clauses as well as seasonal and time-of-day scheduling. When a
"complex" charge is chosen the Energy (or Fuel), Demand and Demand Clause tabs will be reactivated and can be used to enter
data.
To choose a rate type, click the button opposite the desired item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy Units and Conversion
These items allow the units of measure for a fuel source to be defined. In the Energy Units item enter a label for fuel units of
measure. In the Conversion item, enter a conversion factor relating the units of measure to standard energy units such as kBTU or
kWh.
The units of measure for fuel will be dictated by the utility company’s rate sheet. When the unit of measure is energy based, the
conversion factor will be known from basic engineering principles. For example, if the unit of measure for a gas rate is "Therms",
standard principles dictate that a Therm equals 100,000 BTU or 100 kBTU. When the unit of measure is mass-based or volume-
based, the conversion factor will depend on the heating value of the fuel. For example, if the unit of measure for a gas rate is 100
cubic feet (CCF), the conversion factor from CCF to kBTU will depend on its heating value per cubic foot. This information should be
available from the utility company.
Page 5 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Demand Units
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Flat Price
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
EIA Electric and Fuel Prices
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Note that when you are entering data for an electric rate, both of these items are defaulted and may not be changed. Energy Units
will be "kWh" and the conversion factor will be 1.0 kWh/kWh.
Finally, a conversion factor is required because system and plant simulations produce energy use data in standard units of kWh for
electrical energy and kBTU (kWh in SI Metric) for fuel use. The fuel use data must be converted into billing units in order to calculate
fuel costs.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Demand Units
For electric rates, users can choose between kW and kVA as the units of measure. kW is the working power measured by a
wattmeter. kVA is the apparent power which includes both the working and reactive components of power, and is a more complete
representation of power use. However, buildings typically use wattmeters so kW is more frequently measured than kVA. The units of
measure for demand will be listed on the electric rate sheet and will dictate your choice for this input.
For fuel rates, users have a choice of fuel demand being based on peak hourly consumption or peak daily consumption for a month.
This convention for determining demand will be listed on the fuel rate sheet and will dictate your choice for this input.
For both fuel and electric rates, the demand units are only relevant if the rate structure includes a demand charge or demand-related
energy charges. The latter refers to an energy charge whose energy block sizes depend on the monthly billing demand.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Flat Price
This item only applies when entering a "simple" type of rate. It defines the flat price for energy or fuel applying to all consumption
each month. The price units depend on the Energy Units defined earlier and the Currency defined in project preferences. For
example, if Therms and Dollars were entered earlier, the flat price will be in terms of $/Therm.
Often users will model a flat price based on Energy Information Administration (EIA) average price data. The EIA tabulates average
prices for each of the 50 US states: Read More.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
EIA Electric and Fuel Prices
Often users choose to model an average flat price for electricity or fuel rather than modeling the specific details of an actual utility
rate structure. For applications in the United States, average price data can be obtained from the Energy Information Administration
(EIA) web site. The EIA tabulates average prices all 50 US states and the District of Columbia. The tables below show average
commercial sector prices for electricity and natural gas for 2015. This data in HAP is updated as new data becomes available. This
data below was the latest available as of July, 2017.
EIA Electric and Natural Gas Prices by US State
State
2015 Average Price of
Electricity ($/kWh)
2015 Average Price of
Natural Gas ($/MCF)1
Alabama
0.1083
11.26
Alaska
0.1744
8.01
Arizona
0.1039
10.53
Arkansas
0.0832
8.43
California
0.1573
8.04
Page 6 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Colorado
0.0988
7.47
Connecticut
0.1597
8.60
Delaware
0.1025
10.70
District of Columbia
0.1201
11.07
Florida
0.0950
10.92
Georgia
0.0989
8.58
Hawaii
0.2693
31.17
Idaho
0.0780
7.59
Illinois
0.0902
7.29
Indiana
0.0978
7.61
Iowa
0.0892
6.50
Kansas
0.1010
8.87
Kentucky
0.0944
8.75
Louisiana
0.0866
8.07
Maine
0.1247
14.16
Maryland
0.1100
9.80
Massachusetts
0.1579
10.81
Michigan
0.1055
7.51
Minnesota
0.0944
7.31
Mississippi
0.1055
7.86
Missouri
0.0916
9.14
Montana
0.1023
8.13
Nebraska
0.0867
6.40
Nevada
0.0925
8.66
New Hampshire
0.1496
13.63
New Jersey
0.1297
8.50
New Mexico
0.1030
6.32
New York
0.1531
6.85
North Carolina
0.0873
8.27
North Dakota
0.0883
6.62
Ohio
0.1007
6.39
Oklahoma
0.0768
8.12
Oregon
0.0880
10.09
Page 7 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Customer Charge
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Minimum Charge
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Tax Rate
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Pennsylvania
0.0960
9.32
Rhode Island
0.1578
11.99
South Carolina
0.1021
8.49
South Dakota
0.0916
6.22
Tennessee
0.1016
8.46
Texas
0.0815
6.95
Utah
0.0862
7.97
Vermont
0.1454
7.89
Virginia
0.0821
8.13
Washington
0.0822
9.77
West Virginia
0.0861
9.14
Wisconsin
0.1089
6.78
Wyoming
0.0912
7.43
US Overall Average
0.1064
7.91
Notes:
1 = One MCF = 1000 cubic feet of gas.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Customer Charge
Many utilities impose a fixed charge each billing period to cover the cost of providing service or for rendering the bill. This may be
referred to as a "customer charge", a "service charge" or a "fixed charge". If a customer charge is not imposed, enter zero for this
item.
This input item can also be used to account for any miscellaneous charges on the rate sheet that are fixed quantities each month
and cannot be modeled by other means. An example is a contract demand charge made in addition to the normal demand charge.
Because a contract demand charge typically remains fixed for a year or more at a time, it cannot be included in the normal demand
charge inputs. However it can be included by adding it to the monthly customer charge.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum Charge
This item defines the minimum allowable charge each billing period. If the sum of energy, demand and customer charges is lower
than the minimum charge, the customer is billed for the minimum charge instead. If a minimum is imposed it will be listed on the
utility rate sheet.
When a minimum charge is not imposed, enter a zero value for this item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Seasonal Scheduling
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Time-Of-Day Scheduling
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
Tax Rate
Taxes are often levied on electric and fuel charges. Users can account for tax charges by defining a tax rate with this input item. Tax
will be computed based on the total of energy, demand and customer charges each month.
If taxes are not imposed or you do not wish to consider them, enter a tax rate of 0%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Seasonal Scheduling
When separate energy, fuel or demand prices are defined for different times of year, or when demand determination clauses require
different calculations based on time of year, the utility rate will specify which months of the year fall in different billing "seasons".
Typically two billing seasons referred to as "Summer" and "Winter" are used. In some cases a third billing season is used. HAP
provides an option for a third season which it refers to as the "Mid-Season".
When seasonal scheduling is used, first mark the check box for seasonal scheduling. This activates the inputs for assigning
seasons to months. This portion of the General tab is organized as a grid where rows contain data for each season and columns
contain data for each month. To assign a month to a particular season, click the button in the cell opposite the desired season and
month. In the figure above, January through May and October through December have been assigned to the "Winter" billing season.
June through September have been assigned to the "Summer" billing season. The "Mid Season" option has not been used in this
example.
Once seasons have been defined, options will be provided on the Energy Charges, Fuel Charges, Demand Charges and Demand
Clause tabs for specifying that prices or data that apply during particular seasons.
Finally, note that seasonal scheduling is only available for complex rates.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Time-Of-Day Scheduling
When separate energy, fuel or demand prices are defined for different times of day, or when demand determination clauses require
different calculations based on time of day, the utility rate will specify which hours of the day fall in different time-of-day periods.
When time-of-day scheduling is used, first mark the check box for time-of-day scheduling. This activates the schedule input section
of the General tab. If you previously defined a time-of-day schedule, use the drop-down list to select that schedule. If you have not
yet created a time-of-day schedule, use the  option.
When entering time-of-day schedule data:
1. In the Schedule form, always specify the schedule type as "time-of-day utility rate".
2. Decide which of HAP’s time of day periods to associate with your utility rate’s schedule. Typically the utility rate will use the terms
"Peak" and "Off-Peak" so these can be directly associated with the HAP time of day periods of the same names. When additional
periods are used, your utility may refer to them by various names such as "shoulder peak", "partial peak", and "mid peak".
Because names used by utilities vary so widely, you will need to decide which of HAP’s other two time-of-day periods (Mid-Peak
and Normal-Peak) to associate with your utility’s additional time-of-day periods.
3. Use care when translating the utility’s time specifications into program inputs. For example, the rate sheet may specify that the
Peak period runs from 11:00 AM to 5:00 PM. This means from 11:00 AM to and including 5:00 PM, but not beyond 5:00 PM. The
proper HAP schedule inputs would assign hours 11 through 16 to the peak period, but not hour 17. Hour 16 covers the period
from 4:00 PM to 4:59:59 PM. If you added hour 17, this would extend the peak period to 5:59:59 PM which is not correct.
4. If both seasonal and time-of-day scheduling is used, make sure your time-of-day schedule data is synchronized with the schedule
of seasons. For example, if the peak and off-peak times differ in summer and winter, make sure you use the Assignments tab in
Page 9 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Emissions Analysis
26.0 Entering Utility Rates ›› 26.1 General Inputs ››
26.2 Energy or Fuel Charge Inputs
26.0 Entering Utility Rates ››
Energy or Fuel Charge Tab / Utility Rate Form
26.0 Entering Utility Rates ›› 26.2 Energy or Fuel Charge Inputs ››
the Schedule form to assign your schedule profiles in a way that matches your designation of months for summer and winter
billing seasons on the Electric Rate or Fuel Rate forms.
Once a time-of-day schedule is linked to your utility rate, options will be provided on the Energy Charges, Fuel Charges, Demand
Charges and Demand Clause tabs for specifying that prices or data that apply during particular time-of-day periods.
Finally, note that time-of-day scheduling is only available for complex rates.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Emissions Analysis
The Emissions Analysis section of the General tab allows greenhouse gas emission rates to be defined for electrical energy or a
particular fuel source. This is an optional section. If emissions data is supplied, the program will estimate total CO2 equivalent
(CO2e) emissions based on the total energy or fuel consumption for the year. Results are shown on the Annual Energy Use and
Emissions Summary report. This data is often required for green building design applications.
To include emissions calculations in your analysis, first mark the check box for this section. Then enter the CO2e emission factor.
Many different gaseous emissions from the generation of electricity or burning of fossil fuels contribute to atmospheric greenhouse
warming. The CO2 equivalent (CO2e) emission factor represents the equivalent lb or kg of CO2 per unit of energy or fuel that has
the same greenhouse warming effect as all of the different gaseous emissions combined. This provides a single point of reference
for evaluating the greenhouse warming effect of energy consumption.
Emission data for electrical energy is based on assumptions about the type of power plants used to generate the electricity, and the
efficiency of transmitting energy to the building site. For example, a utility that relies heavily on coal-fired power plants will have
higher CO2e emission rates than one that uses hydroelectric power, nuclear plants or gas-fired power plants.
Emissions data for fuel sources will depend on the type and quality of the fuel.
Emission rate data is often available from government reports. For applications in the United States, one useful source of this data is
Source Energy and Emission Factors for Energy Use in Buildings, Deru and Torcellini, National Renewable Energy Laboratory
Technical Report NREL/TP-550-38617, June 2007. This report is available for download from the NREL web site.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains data found on the Energy Charge or Fuel Charge tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Energy or Fuel Charge Tab / Utility Rate Form
In an electric rate the Energy Charges tab contains information about the energy charge component of the electric bill. For a fuel
rate the Fuel Charges tab contains information about the fuel charge component of the bill. Both tabs have similar format and
content which is discussed below.
Page 10 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Entering Standard Energy Charges
26.0 Entering Utility Rates ›› 26.2 Energy or Fuel Charge Inputs ››
The tab contains an expandable table of energy or fuel charge data. Each row in the table contains data for one item in the charge.
Each item defines a price for a particular period of time and a particular quantity of energy use. Columns in the table provide
information describing the energy or fuel price and the time period and energy quantity it applies to.
The number of row items in the table is controlled by marking and unmarking the check boxes at the left end of each row:
a. To add a row to the end of the table, mark the check box for the last row in the table.
b. To remove a row from the table, remove the check from the check box for any row. That row will be deleted and rows beneath it
will move up one position.
The column data and extra inputs found on this tab vary slightly between the following three applications. For further information on
each, click on the desired item below
Entering standard electric energy charges.
Entering compound block electric energy charges.
Entering fuel charges.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Entering Standard Energy Charges
This topic describes inputs on the Energy Charges tab when entering a "standard" type of energy charge. "Standard" covers flat
price, declining block, demand block and mixed block types of energy charges. It does not apply to the two-tier Compound Block
type of charge. For information on these types of energy charges, please refer to the applications discussion for energy charges.
Inputs for a "Standard" type of electrical energy charge are shown above. Required input items are as follows:
1. Type of Energy Charge. For any energy charge that qualifies as a flat price, declining block, demand block or mixed block
charge, choose the "Standard" option. This selection imposes a specific set of validation rules for the data you enter. For
information on these rules, click here: Basic Rules for Entering Energy Charge Data.
Page 11 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Entering Compound Energy Charges
26.0 Entering Utility Rates ›› 26.2 Energy or Fuel Charge Inputs ››
2. Step Type. For a "Standard" type of energy charge, step type is always set to "Energy" and is display-only. It cannot be changed.
Step Type only is used when entering a Compound Block energy charge.
3. Season specifies the season during which price data in this row of the table applies. If seasonal scheduling was selected on the
General tab, the seasons you specified will appear in the drop-down list plus an option for "All" seasons. If seasonal scheduling is
not used, "All" will be the only choice in the drop-down list.
4. Period defines the time-of-day period during which price data in this row applies. If time-of-day scheduling was selected on the
General tab, then the time-of-day periods you defined will appear in the drop-down list plus an option for "All" periods. If time-of-
day scheduling is not used, "all" will be the only choice in the list.
5. Block Size defines the quantity of energy the energy price applies to. In a flat price structure, one price item applies to all energy
use so the block size should be 9999999. HAP interprets a "9999999" value as meaning "all energy". When a declining block,
demand block or mixed block structure is being entered, you will define a series of price items each for a specific quantity of
energy. The "Block Size" specifies this quantity of energy. Note that the last step in a series of related steps must use a block size
of 9999999 to designate "all additional energy use".
6. Block Units specifies the units of measure for the energy block defined in this row of the table. In a flat price or declining block
structure, all energy blocks have units of kWh. In a demand block structure, all rows have units of kWh/kW. This is also referred
to as "hours use" by some utility companies. Finally, for a mixed block type of structure, block units will vary between kWh/kW
and kWh units. To specify the block units, select the desired units label from the drop down list.
7. Price defines the cost of energy for this item in the energy charge. The price will apply to the season, period and energy block
specified in the other columns of this row. When entering this data be careful about the currency units. For example, if you
specified currency as "Dollars", energy prices must be entered in Dollars/kWh. In many situations utility companies will specify
prices in Cents/kWh, so the price must be converted to dollars when entering the data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Entering Compound Energy Charges
This topic describes inputs on the Energy Charges tab when entering a "compound block" type of energy charge. This is a special
two-tier type of electric energy charge, explained in further detail in the applications discussion for energy charges.
Inputs for a "compound block" type of electrical energy charge are shown above. Required input items are as follows:
1. Type of Energy Charge. When modeling a compound block energy charge, choose the "Compound" option. This selection
imposes a specific set of validation rules for the data you enter. For information on these rules, click here: Basic Rules for
Entering Energy Charge Data.
Page 12 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Entering Fuel Charges
26.0 Entering Utility Rates ›› 26.2 Energy or Fuel Charge Inputs ››
2. Step Type. The compound block charge consists of a number of demand blocks (having units of kWh/kW) which are subdivided
into energy steps (with units of kWh). The "Step Type" is used to designate whether each row in the table is a demand block or
an energy step. Choose "Demand" when entering a demand block. Choose "Energy" when entering an energy step.
3. Season specifies the season during which price data in this row of the table applies. If seasonal scheduling was selected on the
General tab, then the seasons you specified will appear in the drop-down list plus an option for "All" seasons. If seasonal
scheduling is not used, "All" will be the only choice in the drop-down list.
4. Period defines the time-of-day period during which price data in this row applies. If time-of-day scheduling was selected on the
General tab, then the time-of-day periods you defined will appear in the drop-down list plus and option for "All" periods. If time-of-
day scheduling is not used, "All" will be the only choice in the list.
5. Block Size defines the size of a demand block or the size of an energy step in the charge structure. As described in the Basic
Rules topic, the last energy step in a demand block must use the block size of 9999999 kWh to indicate "all additional kWh". The
last demand block in a group of related blocks must use a block size of 9999999 kWh/kW to indicate "all additional kWh/kW".
6. Block Units is a display-only item which indicates the units of measure for the block defined in each row. It is set by the "Step
Type" for the row. When the Step Type is "Demand", the units of measure will be "kWh/kW". When the Step Type is "Energy" the
units of measure will be "kWh".
7. Price defines the cost of energy for each energy step in the structure. The price will apply to the season, period and energy block
specified in the other columns of this row. Prices are only defined for energy steps in the structure. For a demand block, the price
cell in the table will be disabled.
When entering this data be careful about the currency units. For example, if you specified currency as "Dollars", energy prices
must be entered in Dollars/kWh. In many situations utility companies will specify prices in Cents/kWh, so the price must be
converted to dollars when entering the data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Entering Fuel Charges
This topic describes inputs on the Fuel Charges tab. Required input items are as follows. Terminology used in this discussion is
explained in the applications discussion for fuel charges. Rules for organizing data are explained in the basic rules topic.
1. Step Type. This is a display-only item which is always set to "Fuel".
2. Season specifies the season during which price data in this row of the table applies. If seasonal scheduling was selected on the
General tab, then the seasons you specified will appear in the drop-down list plus an option for "All" seasons. If seasonal
scheduling is not used, "All" will be the only choice in the drop-down list.
3. Period defines the time-of-day period during which price data in this row applies. If time-of-day scheduling was selected on the
General tab, then the time-of-day periods you defined will appear in the drop-down list plus and option for "All" periods. If time-of-
day scheduling is not used, "all" will be the only choice in the list.
4. Block Size defines the quantity of consumption the fuel price applies to. In a flat price structure, one price item applies to all fuel
use so the block size should be 9999999. HAP interprets a "9999999" value as meaning "all fuel use". When a declining block,
demand block or mixed block structure is being entered, you will define a series of price items each for a specific quantity of fuel
use. The "Block Size" specifies this quantity of fuel. Note that the last step in a series of related steps must use a block size of
9999999 to designate "all additional fuel use".
Page 13 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
26.3 Demand Charge Inputs
26.0 Entering Utility Rates ››
Demand Charge Tab / Utility Rate Form
26.0 Entering Utility Rates ›› 26.3 Demand Charge Inputs ››
5. Block Units specifies the units of measure for the consumption block defined in this row. This item is display-only and will always
contain the fuel unit of measure you defined on the General tab.
6. Price defines the cost of fuel for this item in the fuel charge. The price will apply to the season, period and consumption block
specified in the other columns of this row. When entering this data be careful about the currency units. For example, if you
specified currency as "Dollars", fuel prices must be entered in Dollars/fuel unit. In many situations utility companies will specify
prices in Cents/fuel unit, so the price must be converted to dollars when entering the data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data on the Demand Charge tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Demand Charge Tab / Utility Rate Form
The Demand Charges tab contains information about the demand charge component of the utility bill. This is an optional component
of the utility rate that charges for peak use of energy or fuel.
The tab contains an expandable table of demand charge data. Each row in the table contains data for one item in the charge. Each
item defines a price for a demand occurring during a particular period of time and for a particular quantity of demand. Columns in the
table provide information describing the demand price, and the time period and demand quantity it applies to.
The number of row items in the table is controlled by marking and unmarking the check boxes at the left end of each row:
a. To add a row to the end of the table, mark the check box for the last row. The last row is normally disabled. Marking the check
box enables it.
b. To remove a row from the table, remove the check from the check box for any row. That row will be deleted and rows beneath it
will move up one position.
The column data on this tab is as follows. For information on the terminology used below, please refer to the application discussion
for demand charges. For a discussion of the basic rules for entering demand charges, refer to the Basic Rules topic.
1. Season specifies the season during which price data in this row of the table applies. If seasonal scheduling was selected on the
General tab, then the seasons you specified will appear in the drop-down list plus an option for "All" seasons. If seasonal
scheduling is not used, "All" will be the only choice in the drop-down list.
2. Period defines the time-of-day period during which price data in this row applies. If time-of-day scheduling was selected on the
General tab, then the time-of-day periods you defined will appear in the drop-down list plus an option for "All" periods. If time-of-
day scheduling is not used, "all" will be the only choice in the list.
3. Block Size defines the quantity of demand the price item applies to. In a flat price structure, one price item applies to all demand
so the block size should be 9999999. HAP interprets a "9999999" value as meaning "all demand". When a stepped demand
charge is being entered, you will define a series of price items each for a specific quantity of demand. The "Block Size" specifies
this demand quantity. Note that the last step in a series of related steps must use a block size of 9999999 to designate "all
additional demand".
Page 14 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
26.4 Demand Determination Inputs
26.0 Entering Utility Rates ››
Demand Clause Tab / Utility Rate Form
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
4. Block Units specifies the units of measure for demand. This item is display-only. For electric rates it will display "kW" or "kVA"
depending on your choice of demand units on the General tab. For fuel rates it will display the fuel unit of measure you specified
on the General tab.
5. Price defines the price for demand for this item in the demand charge. The price will apply to the season, period and demand
block specified in the other columns of this row.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This chapter explains input data found on the Demand Determination tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Demand Clause Tab / Utility Rate Form
The Demand Clauses tab contains information about demand determination clauses in the rate structure. When a utility rate
includes a demand charge or demand-related energy charges, the rate structure will define rules for determining the billing demand
used to calculate these charges. In the simplest case, the billing demand will be the measured peak demand each month. In other
cases, one or more clauses will be specified to adjust the measured peak to obtain billing demand. Inputs on this tab are described
below. The principles of demand determination clauses are discussed in a separate application discussion topic.
Page 15 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Rachet Clause
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
Trailing Window Clause
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
For electric rates, this tab is divided into five sections, one for each of the five possible demand determination clauses. For fuel
rates, the "Power Factor Multiplier" clause shown above does not apply, so only four sections are provided. For a description of
demand determination inputs, click on any of the following:
Rachet Clause
Trailing Window Clause
Power Factor Multiplier Clause
Minimum Demand Clause
Demand Multiplier Clause
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Rachet Clause
A rachet clause introduces a penalty for large changes between monthly demands.
Example: A rachet clause might specify that the billing demand shall be the measured peak demand or 80% of the largest peak
demand in the preceding summer months of June, July, August and September, whichever is greater. If the measured peak demand
in any month is less than 80% of the summer peak, the 80% summer peak will be used instead of the measured peak to calculate
demand charges for that month. Therefore, changes in peak demand of more than 20% of the summer peak will be penalized.
To define a rachet clause, mark the check box for the clause and then enter the following values:
1. king Months define a group of months during which the largest peak demand is identified. Typically the Peaking Months will be
summer months when the highest demands during the year are expected. Note that this specification is inclusive. For example
"Jun to Sept" includes June, July, August and September.
2. Multiplier is the multiplier factor applied to the largest demand found during the Peaking Months. In the example above, 80% was
used as the multiplier.
3. Applies defines the group of months during which the rachet clause applies. In some cases this will be all months other than the
peaking months. In other cases it will be all months of the year (specify Jan to Dec in this case). As with the peaking months, this
specification is inclusive.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Trailing Window Clause
A "trailing window" clause introduces a penalty for large changes between monthly demands. It does this by comparing the
measured demand in the current month with a percentage of the largest demand in a number of preceding months.
Example: A trailing window clause might specify that the billing demand for each month shall be the measured peak demand or 75%
of the largest measured peak in the previous 6 months, whichever is larger.
To define a trailing window clause, mark the check box for the clause and then enter the following values:
1. Window is the number of prior months specified in the clause. In the example above, the window was 6 months. Note that if the
clause specifies 12 months, a value of 11 should be entered. When performing an energy simulation we are only working with a
12 month period. So, excluding the current month, there are only 11 other months to consider in the trailing window calculation.
Page 16 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Power Factor Multiplier Clause
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
Minimum Demand Clause
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
Demand Multiplier Clause
26.0 Entering Utility Rates ›› 26.4 Demand Determination Inputs ››
2. Multiplier is the multiplier factor applied to the largest demand found during the series of previous months. In the example above
75% was the multiplier.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Power Factor Multiplier Clause
This clause introduces an indirect charge for excessive reactive power use. It is only used in electric rate structures. Power used in
alternating current circuits is classified as "working" and "reactive". "Apparent" power is the vector sum of working and reactive
power. Working power can be measured by a wattmeter. Reactive power is used to generate the magnetic flux in inductive
machinery such as electric motors. It must be measured with separate metering equipment. Rather than measure it directly, utilities
sometimes spot check buildings and impose a penalty if reactive power use is excessive. The reference value for the penalty is the
"power factor" which is the ratio of working power to apparent power and therefore indirectly indicates the magnitude of the reactive
power component. The lower the power factor, the larger the reactive power use.
Example: A power factor multiplier clause might state that customers shall maintain a lagging power factor of 90% or higher. For
each 1% by which the average power factor lags below 90%, the billing demand shall be increased by 1%.
To define a power factor multiplier clause, mark the check box for the clause and then enter the power factor multiplier. If a
building’s power factor is 85% lagging in the example above, then a multiplier of 105% would be used since the power factor is 5
percentage points below 90%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Minimum Demand Clause
Utilities often specify that billing demand may not be less than a certain demand level. For example, a minimum demand clause
might state that the billing demand shall be the measured peak demand or 50 kW, whichever is larger.
To enter this clause, mark the check box for the clause and then enter the minimum demand value. In the example above, the
minimum demand was 50 kW.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Demand Multiplier Clause
This type of clause typically provides a discount for demand measured during certain times of day or times of year. This is done to
encourage shifting of demand to those periods.
Example: A demand multiplier clause might state that billing demand during the winter months shall be 60% of the measured
demand.
To define a demand multiplier clause, first mark the check box for the clause and then enter the following values:
Page 17 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
26.5 Common Tasks
26.0 Entering Utility Rates ››
Creating a New Utility Rate
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
Editing an Existing Utility Rate
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
Printing Utility Rate Inputs
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
Deleting Utility Rate Inputs
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
Copying a Utility Rate
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
1. Season defines the season during which the multiplier applies. If you selected seasonal scheduling on the General tab, this drop
down list will include all the seasons you defined plus an option for "All" seasons. If seasonal scheduling was not specified, "All"
will be only choice.
2. Period defines the time-of-day period during which the multiplier applies. If you selected time-of-day scheduling on the General
tab, this drop-down list will include the time-of-day periods from the schedule you linked to this utility rate plus an option for "all"
periods. If time-of-day scheduling was not specified, "All" will be the only option.
3. Multiplier is the factor applied to all measured demands in the season and time of day period covered by the clause.
In the example above Season=Winter, Period=All and Multiplier=60%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with utility rate input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Utility Rate
Please see Creating a New Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Utility Rate
Please see Editing an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Utility Rate Inputs
Please see Generating Input Data Reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Utility Rate Inputs
Please see Deleting Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 18 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm
Duplicating a Utility Rate
26.0 Entering Utility Rates ›› 26.5 Common Tasks ››
Copying a Utility Rate
Please see Copying Items.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Utility Rate
Please see Duplicating an Existing Item.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 19 of 19
26.0 Entering Utility Rates
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh817D.htm