7.0 Utility Rate Applications
Overview for Utility Rate Applications
7.0 Utility Rate Applications ››
Modeling Utility Rates - Energy and Fuel Charges
7.0 Utility Rate Applications ››
This chapter provides guidance for using modeling utility rate structrures in HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Utility Rate Applications
The following series of help topics explains how to model utility rate structures in energy simulations. The term
"utility rate" refers to the pricing structure a utility uses when billing for electric energy use or fuel use in a
building. Utility rate data is used by HAP when calculating energy costs. HAP deals with two distinct types of
utility rates:
1. Electric Rates define pricing structures for electric energy use and demand.
2. Fuel Rates define the pricing structures for natural gas, fuel oil, propane, remote chilled water, remote hot
water and remote steam.
While data is defined in the program in two separate data categories (one for electric and one for fuel), both
types of utility rates use the same terminology and input items and the same application concepts. The
following discussions will use electric rates for examples, but the concepts apply equal to electric and fuel
rates.
Basic Concepts
Individual utility companies charge for energy use, fuel use and demand in widely different ways and use
vastly different terminology in stating their pricing structures. This presents a challenge for developing one
consistent approach to modeling utility rate structures in the program. HAP uses a modular approach to meet
this challenge. The program provides building blocks representing the common billing mechanisms for energy,
demand, demand determination and miscellaneous charges. The user is able to pick and choose among these
building blocks to assemble a utility rate model that best represents the pricing structure used for their building.
The key elements in successfully using the utility rate modeling features in HAP are:
1. Recognizing the separate billing mechanisms used in your utility rate structure and matching them to the
corresponding building blocks offered by HAP.
2. Understanding the common terminology used by HAP and relating this to the specific terminology used by
your utility company.
The following topics discuss terminology and building blocks involved with the three common components of a
commercial building utility bill:
Energy and Fuel Charges.
Demand Charges
Demand Determination
Each topic will define terms, provide examples of the common billing mechanisms and show examples of how
data would be input in HAP. Related information on these subjects can be found in the discussion of utility rate
inputs and energy cost calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 1 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
Modeling Utility Rates - Energy and Fuel Charges
An "energy charge" is the component of the electric bill that charges for energy consumption measured in
kWh. In a fuel bill, it is the component that charges for fuel consumption measured in units defined by the
utility. Nearly all utility rates include an energy or fuel charge; many include nothing but an energy or fuel
charge.
HAP is able to model the five most common types of energy and fuel charges. Utility rates will never refer to
the charges using the names shown below. Instead these are simply descriptive names that are handy when
explaining the pricing structures. To decide which kind of energy or fuel charge you have, match the charge
defined on your utility rate sheet with one of the following.
Flat Price. This pricing structure uses a flat cost/kWh price for all times, or specific periods such as seasons or
time-of-day periods.
Sample Utility Rate Statement:
All kWh during summer billing months................... 0.077 $/kWh
All kWh during winter billing months...................... 0.049 $/kWh
Example: During one summer billing month 40000 kWh is used. The energy charge is calculated as:
kWh Range
Block Size
x
Price
=
Cost
All
40000 kWh
x
0.077 $/kWh
=
$3080
Total
=
$3080
Program Input: Use the "Standard" energy charge type. For fuel rates, all fuel charges are "standard". Specify
one step for each fixed price item. For this example, the inputs would be as follows. Note that in HAP the
energy or fuel quantity "9999999" is used to designate "all".
Season
Period
Block Size
Block Units
Price
Summer
All
9999999
kWh
0.07700
Winter
All
9999999
kWh
0.04900
Declining Block. This pricing structure uses different energy or fuel prices for different "blocks" of energy or
fuel that are consumed. Generally the price declines with each succeeding block, hence the name "declining
block".
Sample Utility Rate Statement:
For the first 8000 kWh........................................... 0.101 $/kWh
For the next 15000 kWh......................................... 0.063 $/kWh
For all remaining kWh............................................ 0.044 $/kWh
Example: During one billing month 40000 kWh is used. The energy charge is calculated as:
kWh Range
Block Size
x
Price
=
Cost
1-8000
8000 kWh
x
0.101 $/kWh
=
$808
8001-23000
15000 kWh
x
0.063 $/kWh
=
$945
23001-40000
17000 kWh
x
0.044 $/kWh
=
$748
Total
=
$2501
Program Input: Use the "Standard" energy charge type. For fuel rates, all fuel charges are "standard". Specify
one step for each block in the pricing structure. For this example, the inputs would be:
Season
Period
Block Size
Block Units
Price
All
All
8000
kWh
0.101
All
All
15000
kWh
0.063
Page 2 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
All
All
9999999
kWh
0.044
Demand Block. This pricing structure is the same as "Declining Block" above, except that the block sizes vary
each month based on the billing demand for that month. Therefore the block sizes have units of
energy/demand such as kWh/kW. In some cases the units are referred to as "hours use". This pricing structure
is rarely seen for fuel charges
Sample Utility Rate Statement:
For the first 150 kWh/kW demand............................ 0.085 $/kWh
For the next 100 kWh/kW demand........................... 0.062 $/kWh
For all additional kWh............................................. 0.038 $/kWh
Example: During one billing month the billing demand is 200 kW and 60000 kWh is used. The energy charge
is calculated as:
kWh Range
Block Size
x
Price
=
Cost
1-30000
30000 kWh
x
0.085 $/kWh
=
$2550
30001-50000
20000 kWh
x
0.062 $/kWh
=
$1240
50001-60000
10000 kWh
x
0.038 $/kWh
=
$380
Total
=
$4170
Program Input: Use the "Standard" energy charge type. For fuel rates, all fuel charges are "standard". Specify
one step for each block in the pricing structure. For this example, the inputs would be:
Season
Period
Block Size
Block Units
Price
All
All
150
kWh/kW
0.085
All
All
100
kWh/kW
0.062
All
All
9999999
kWh/kW
0.038
Mixed Block. The "Mixed Block" charge combines elements of both "Declining Block" and "Demand Block". It
contains a mixture of blocks of fixed size and blocks with size varying based on billing demand. Therefore, in
an electric rate, some blocks have kWh units and others have units of kWh/kW or "hours use". This pricing
structure is sometimes used for electric energy charges but is uncommon for fuel charges.
Sample Utility Rate Statement:
For the first 150 kWh/kW demand.................................. 0.075 $/kWh
For the next 15000 kWh................................................. 0.050 $/kWh
For the next 100 kWh/kW demand.................................. 0.047 $/kWh
For all additional kWh.................................................... 0.042 $/kWh
Example: During one billing month the billing demand is 120 kW and 50000 kWh is used. The energy charge
is calculated as:
kWh Range
Block Size
x
Price
=
Cost
1-18000
18000 kWh
x
0.075 $/kWh
=
$1350
18001-33000
15000 kWh
x
0.050 $/kWh
$750
33001-45000
12000 kWh
x
0.047 $/kWh
=
$564
45001-50000
5000 kWh
x
0.042 $/kWh
=
$210
Total
=
$2874
Program Input: Use the "Standard" energy charge type. For fuel rates, all fuel charges are "standard". Specify
one step for each block in the pricing structure. For this example, the inputs would be:
Page 3 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
Season
Period
Block Size
Block Units
Price
All
All
150
kWh/kW
0.075
All
All
15000
kWh
0.050
All
All
100
kWh/kW
0.047
All
All
9999999
kWh
0.042
Compound Block. The "Compound Block" charge uses a two-tier block structure shown in the example
below. The first tier contains demand blocks which are used with the billing demand each month to establish a
series of large energy blocks. These first tier blocks are subdivided into smaller energy blocks each with a
separate price. Compound Block charges are infrequently seen in electric rate structures. They are currently
not used for fuel charges.
Sample Utility Rate Statement:
For the first 125 kWh/kW demand
For the first 3000 kWh................................................... 0.087 $/kWh
For the next 87000 kWh................................................. 0.043 $/kWh
For the all additional kWh............................................... 0.034 $/kWh
For the next 200 kWh/kW demand
For the first 6000 kWh................................................... 0.060 $/kWh
For the next 85000 kWh................................................. 0.044 $/kWh
For the all additional kWh............................................... 0.042 $/kWh
For all over 325 kWh/kW demand
For all kWh.................................................................... 0.039 $/kWh
Example: During one billing month the billing demand is 500 kW and 200000 kWh is used. The energy charge
is calculated as:
kWh Range
Block Size
x
Price
=
Cost
First 125 kWh/kW
62500 kWh
1-3000
3000 kWh
x
0.087 $/kWh
=
$261.00
3001-62500
59500 kWh
x
0.043 $/kWh
=
$2558.50
Next 200 kWh/kW
100000 kWh
1-6000
6000 kWh
x
0.060 $/kWh
=
$360.00
6001-100000
94000 kWh
x
0.044 $/kWh
=
$4136.00
All Above 325 kWh/kW
37500 kWh
1-37500
37500 kWh
x
0.039 $/kWh
=
$1462.50
Total
=
$8778.00
Program Input: Use the "Compound Block" energy charge type. Specify one step for each first tier and second
tier line item in the in the pricing structure. For this example, the inputs would be:
Block Type
Season
Period
Block Size
Block Units
Price
Demand
All
All
125
kWh/kW
-
Energy
All
All
3000
kWh
0.087
Energy
All
All
87000
kWh
0.043
Energy
All
All
9999999
kWh
0.034
Demand
All
All
200
kWh/kW
-
Energy
All
All
6000
kWh
0.060
Energy
All
All
95000
kWh
0.044
Page 4 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
Modeling Utility Rates - Demand Charges
7.0 Utility Rate Applications ››
Energy
All
All
9999999
kWh
0.042
Demand
All
All
9999999
kWh/kW
-
Energy
All
All
9999999
kWh
0.039
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modeling Utility Rates - Demand Charges
A "demand charge" is imposed for the peak power use during a month rather than for total energy
consumption. Utility companies typically impose a demand charge in addition to the energy charge. While
nearly all electric and fuel rate structures contain an energy or fuel charge, only certain rates include a demand
charge. Demand charges are simpler than energy charges in that there are only two types. Each is described
below
Flat Price. This demand charge structure uses a flat cost/demand price for all times, or specific periods such
as seasons or time-of-day periods.
Sample Utility Rate Statement:
All kW of on-peak demand during summer months.............. 10.45 $/kW
All kW of mid-peak demand during summer months............ 8.65 $/kW
All kW of on-peak demand during winter months................. 7.40 $/kW
Example: During one summer billing month the demand for on-peak hours is 370 kW and demand for mid-
peak hours is 207 kW. The demand charge is calculated as:
kW Range
Block Size
x
Price
=
Cost
All
370 kW
x
10.45
=
$3866.50
All
207 kW
x
8.65
=
$1790.55
Total
=
$5657.05
Program Input: The number of steps entered in the demand charge is determined by the number of flat price
periods. In this example, three steps are required:
Season
Period
Block Size
Block Units
Price
Summer
Peak
9999999
kW
10.45
Summer
Mid-Peak
9999999
kW
8.65
Winter
Peak
9999999
kW
7.40
Stepped. This pricing structure uses different demand prices for successive "blocks" of demand. This pricing
structure is similar to the declining block energy charge.
Sample Utility Rate Statement:
For the first 50 kW of billing demand......................... 10.18 $/kW
For the next 100 kW of billing demand....................... 7.00 $/kW
For all remaining billing demand................................ 5.44 $/kW
Example: During one billing month the billing demand is 400 kW. The demand charge is calculated as:
kW Range
Block Size
x
Price
=
Cost
1-50
50 kW
x
10.18 $/kW
=
$509
51-150
100 kW
x
7.00 $/kW
=
$700
Page 5 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
Modeling Utility Rates - Demand Determination
7.0 Utility Rate Applications ››
151-400
250 kW
x
5.44 $/kW
=
$1360
Total
=
$2569
Program Input: The number of steps entered in the demand charge is determined by the number of "steps" or
"blocks" in the demand charge. In this example, three steps are required:
Season
Period
Block Size
Block Units
Price
All
All
50
kW
10.18
All
All
100
kW
7.00
All
All
9999999
kW
5.44
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modeling Utility Rates - Demand Determination
Whenever demand charges or demand block energy charges are used in a rate structure, the peak demand
must be determined for each billing period. For electric rates the integrated power use over a 15, 30 or 60
minute period is typically used. For fuel rates, the peak hourly fuel consumption, or peak daily fuel
consumption is used. In the simplest cases the measured peak demand is used directly to compute the
demand charge. In other cases, however, the measured demand is adjusted by one or more clauses to
determine a "billing" demand used to calculate the charge. For example, some rate structures impose a
minimum demand clause. The billing demand is either the measured demand or the minimum demand,
whichever is larger.
Clauses used to derive "billing" demand from the measured demand are referred to as "Demand
Determination" clauses. Usually the utility rate sheet will include a "Demand Determination" section that spells
out these clauses. In other cases the clauses are provided as fine print below the demand charge statement
Each utility company defines clauses in different ways, but most fall into one of the following five categories:
a. Minimum demand clauses
b. Rachet clauses
c. Trailing window clauses
d. Demand multiplier clauses
e. Power factor multiplier clauses (electric rates only).
Utilities will never refer to the clauses by these names. Instead, these are simple descriptive names that make
explaining the clauses easier. To determine which kind of demand clauses are used in your rate structure,
match the clause defined on your utility rate sheet with the following descriptions.
Minimum Demand Clause. Utilities often specify that billing demand may not be less than a certain demand
level.
Sample Demand Clause:
The billing demand shall be the larger of:
a. The maximum 30-minute integrated demand measured, or
b. 50 kW.
Example: In a particular month the measured demand is 35 kW. Using the sample clause above, billing
demand would be determined as:
Measured Demand
Minimum Demand
Billing Demand
35 kW
50 kW
50 kW
Page 6 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
Program Input: To model this clause in HAP, select the Minimum Demand Clause option and specify the
minimum demand value.
Rachet Clause. A rachet clause introduces a penalty for large swings between monthly demands. The key to
recognizing the rachet clause is that it compares measured demands with a percentage of the highest demand
found during a fixed set of months.
Sample Demand Clause:
The billing demand shall be the larger of:
a. The maximum 30-minute integrated demand measured, or
b. 75% of the highest demand determined during the billing months of June through August
Example: The measured demand for November is 100 kW. The highest measured demand during the months
of July through August was 200 kW. Using the rachet clause above billing demand is determined as follows:
Measured Demand
Rachet Demand
Billing Demand
100 kW
0.75 x 200 = 150 kW
150 kW
Program Input: To model this clause in HAP select the Rachet Clause option and then specify the months
during which the rachet peak is determined ("peaking months"), the months in which the rachet applies
("Applies In") and the multiplier factor. For the sample rachet clause the following inputs would be used:
a. Peaking months = June to August
b. Applies in months = January to December
c. Multiplier = 75%.
Trailing Window Clause. A "trailing window" clause also introduces a penalty for large swings between
monthly demands. The key to recognizing the trailing window clause is that it compares the measured demand
in the current month with a percentage of the highest demand found within a series of preceding months. This
series of months is referred to as the "trailing window".
Sample Demand Clause:
The billing demand shall be the larger of:
a. The maximum 30-minute integrated demand measured, or
b. 50% of the highest demand measured during the preceding 6 months.
Example: The measured demand for November is 100 kW. The highest measured demand during the
previous 6 months was 250 kW in July. Using the trailing window clause above billing demand is determined
as follows:
Measured Demand
Rachet Demand
Billing Demand
100 kW
0.50 x 250 = 125 kW
125 kW
Program Input: To model this clause in HAP select the Trailing Window Clause option and then specify the
size of the trailing window and the multiplier factor. For the sample rachet clause the following inputs would be
used:
a. Window = 6 months
b. Multiplier = 50%.
Demand Multiplier Clause. This clause provides a discount on demand measured during certain times of day
or times of year to encourage shifting of demand to those periods.
Sample Demand Clause:
Billing demand during the winter months shall be 60% of the maximum 30-minute integrated demand
measured.
Example: The measured peak demand for one of the winter billing months is 140 kW. Using the demand
multiplier clause shown above, the billing demand would be determined as follows:
Measured Demand
Demand Multiplier
Adjustment
Billing Demand
Page 7 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm
140 kW
140 kW x 0.60 = 84 kW
84 kW
Program Input: To model this clause in HAP, select the Demand Multiplier option and specify the multiplier
factor and the season and period in which the multiplier applies. For the example clause above the inputs
would be:
a. Multiplier = 60%
b. Season = Winter
c. Period = All
Power Factor Multiplier Clause. This clause introduces an indirect charge for excessive reactive power use.
It is only used in electric rate structures. Power used in alternating current circuits is classified as "working"
and "reactive". "Apparent" power is the vector sum of working and reactive power. Working power can be
measured by a wattmeter. Reactive power is used to generate the magnetic flux in inductive machinery such
as electric motors. It must be measured with separate metering equipment. Rather than measure it directly,
utilities sometimes spot check buildings and impose a penalty if reactive power use is excessive. The
reference value for the penalty is the "power factor" which is the ratio of working power to apparent power and
therefore indirectly indicates the magnitude of the reactive power component. The lower the power factor, the
larger the reactive power use.
Sample Demand Clause:
Customers shall maintain a lagging power factor of 90% or higher. For each 1% by which the average
power factor lags below 90%, the demand charge shall be increased by 1%.
Example: For a certain month the measured peak demand is 200 kW. A spot check indicates the building
power factor is 80% lagging. Using the demand clause above, the building would be penalized by increasing
the demand charge by 1% for each 1% the power factor is below 90%, or a total of 10%.
Measured Demand
Power Factor Multiplier
Adjustment
Billing Demand
200 kW
200 kW x 1.10 = 220 kW
220 kW
Program Input: To model this clause in HAP, select the Power Factor Multiplier option and then specify the
multiplier factor. For the example clause above the multiplier would be 110%.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 8
7.0 Utility Rate Applications
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh97B2.htm