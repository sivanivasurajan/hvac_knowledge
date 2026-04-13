9.0 Entering Weather Data
9.1 Overview for Weather and the Weather Form
9.0 Entering Weather Data ››
Overview for Weather and the Weather Form
9.0 Entering Weather Data ›› 9.1 Overview for Weather and the Weather Form ››
This chapter explains weather input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of weather input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Weather and the Weather Form
About Weather Data. "Weather Data" refers to the temperature, humidity and solar radiation conditions
experienced by the building and its HVAC equipment. In HAP this term is also used to refer to information
about the geographical location of the building, the nature of local time and local soil properties. Weather data
has a significant effect on building loads and equipment operation. It therefore plays a key role in load
calculations and system performance calculations.
HAP deals with two distinct kinds of weather data:
1. Design Weather Data is used to perform cooling and heating design load estimates. Cooling design
weather data consists of 24-hour profiles of temperature and humidity representing warmer than normal
conditions, and clear sky solar radiation profiles representing maximum sunshine conditions for each
month. This data is used to estimate design cooling loads according to standard industry practices. Heating
design weather data consists of information about the winter design temperature and humidity. This data is
used to determine design heating loads according to standard industry practices.
2. Simulation Weather Data is required when performing 8,760 hour energy simulations. Simulation weather
data refers to the 8,760 hour sequence of actual weather data used to simulate building loads and HVAC
equipment operation over the course of a year. Results of these simulations are used to compute annual
energy use and energy costs. This data is only used in HAP and not in HAP System Design Load.
In HAP a project only uses one set of weather data at a time. This is in contrast to data such as spaces,
systems and plants for which multiple items can exist in each category of data. Rather, one set of weather
data exists and the current weather data that has been defined is used for all program calculations.
Page 1 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
The Weather Form, shown above, is used to define design weather data for a project. The Weather Form
contains three key components:
1. The Title Bar appears across the top of the form. It lists the name of the city whose weather data is
displayed in the form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains multiple categories of weather information
represented as separate tabs in a notebook. To move from one tab to another, simply click on the desired
tab. There are four tabs for the four categories of weather data:
a. Design Parameters contains information about the geographic location of the building, its summer and
winter design conditions, local soil conditions, local time specifications and the range of months to be
used in design cooling calculations.
b. Design Temperatures contains information about cooling design day temperature and humidity profiles.
Features on this tab can be used to view and to modify the design day profiles.
c. Design Solar summarizes the peak solar heat gains for cooling design days. Features on this tab can be
used to view peak solar heat gain data as well as adjust the profiles.
d. Simulation contains information about simulation weather data used in the project. It also is used to
define the operating calendar for the energy simulation.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the weather data and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the weather data.
c. Press Help to display this overview topic.
Weather Features. Finally, HAP provides useful features for:
Editing weather data.
Page 2 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.2 Design Parameter Data
9.0 Entering Weather Data ››
Design Parameters Tab / Weather Form
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Printing or viewing weather reports.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains inputs on the Design Parameters tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Parameters Tab / Weather Form
About Design Parameters. Items on the Design Parameters tab are used to specify design weather
conditions for the building site. This tab contains information about the geographic location of the building, its
summer and winter design conditions, soil conditions, local time specifications and the range of months to be
used in design cooling calculations. Once defined, this data is used to calculate cooling design temperature,
humidity and solar radiation profiles. The month range governs the months considered in a design cooling
analysis. The soil conductivity is used for slab floor, basement floor and basement wall heat flow calculations.
The Design Parameters Tab contains nineteen input items:
1. Region, Location and City are used to define design weather data by choosing a city from HAP’s weather
database. As an alternative the city name and the design data can be directly specified by the user.
Page 3 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Region / Location / City
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
2. Latitude and Longitude define the geographic coordinates for the building’s locale. These values are used in
solar calculations.
3. Elevation influences psychrometric calculations for the building site, since air density and psychrometric
properties vary with elevation above sea level.
4. Summer Design DB , Summer Coincident WB and Summer Daily Range are used to construct temperature
and humidity profiles for cooling design calculations.
5. Winter Design DB and Winter Coincident WB define temperature and humidity conditions for heating design
calculations.
6. Atmospheric Clearness Number is used to adjust standard design day solar data for conditions that are
unusually clear or unusually hazy.
7. Average Ground Reflectance is used to calculate the ground-reflected component of solar heat gain for a
building.
8. Soil Conductivity is used when calculating heat flow through slab floors, basement floors and basement
walls.
9. Design Cooling Calculation Months specifies the range of months to be used in all cooling design analyses
performed for the project.
10. Time Zone is used to adjust solar profiles for local time.
11. Daylight Saving Time, DST Begins, and DST Ends are used to define whether daylight savings time is
used and if so, when during the year it begins and ends. The use of daylight savings time affects the
relationship between solar profiles and local time.
12. Data Source indicates the source of HAP’s default weather data for latitude, longitude, elevation, summer
dry-bulb, summer wet-bulb, summer daily range, and winter dry-bulb. This is not an input item. It is for
reference only. When weather data is directly specified by the user, or is adjusted by the user, the source
indicates data is "user-defined".
Special Features. If you choose a new city or adjust existing values on the Design Parameters tab, HAP will
recalculate the cooling design temperature and solar profiles when you leave the tab either by moving to a
different tab in the Weather Form or by pressing the OK button to exit from the Weather form. The results of
the weather profile calculations will appear on the Design Temperatures tab and the Design Solar tab . Results
can also be viewed and printed via the Print/View Input Data option for weather data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Region / Location / City
The Region, Location and City items are used together to select weather data for a city from HAP’s weather
database. When a city is selected, design weather parameters for the city will be retrieved from HAP’s
database and will be displayed on the screen. This serves as a fast, efficient method of defining weather data.
However, if it is necessary, you can also specify your weather data directly rather than using data from HAP’s
database.
Because there are several hundred cities in HAP’s database, the city selection process is divided into three
steps to make it more manageable:
1. First use the Region drop-down list to select the geographic region of the world containing your city.
2. Next use the Location drop-down list to select the state, province or country containing your city. When
working with cities in the United States, the drop down list contains state names. When working with cities
in Canada, the list contains province names. When working with cities elsewhere, the list contains country
names.
3. Finally, use the City drop-down list to select the desired city.
Page 4 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Latitude
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Longitude
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Elevation
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Design weather parameters for the city you select will be retrieved from HAP’s database and will be displayed
on the screen.
Application Information:
1. When you select a city from HAP’s weather database, the following values are read from the database:
latitude, longitude, elevation, summer design dry-bulb, summer coincident wet-bulb, summer daily range,
winter design dry-bulb, atmospheric clearness number, and time zone. The remaining values on the Design
Parameters tab are set to standard default values. All values on the form should be inspected and adjusted
if necessary.
2. If the desired city is not in HAP’s database and therefore does not appear in the city drop-down list, design
weather data can be directly specified. Instead of choosing a location and city, simply type in the location
and city names. Then directly enter the design parameters that appear on the remainder of the screen using
data you have obtained from a reference handbook.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Latitude
The site latitude is used in solar radiation calculations. It has an important effect on the direction and intensity
of solar radiation hour-by-hour through the day and throughout the year. Positive latitude values are used for
cities north of the equator. Negative values are used for cities south of the equator.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Longitude
The site longitude influences solar radiation calculations. All program calculations are performed according to
local time (LT). The direction and intensity of solar radiation depend on the position of the sun in the sky.
Because solar position angles are determined according to apparent solar time (AST), it is necessary to use
the longitude and time zone inputs to convert this data from AST to LT.
Positive longitude values are used to represent west longitude. Negative values are used to represent east
longitude.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Elevation
The site elevation is required for air property and psychrometric calculations since properties of air vary with
altitude. Positive values indicate the distance above sea level. Negative values define the distance below sea
level.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 5 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Summer Design Temperatures
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Winter Design Temperatures
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Atmospheric Clearness Number
Summer Design Temperatures
Three items define characteristics of cooling design temperature profiles:
1. Summer Design Dry-Bulb defines the warmest outdoor air dry-bulb temperature considered for cooling
design conditions. For weather data obtained from the ASHRAE Handbook of Fundamentals, 0.4% design
values are used. This means the warmer temperatures occur in only 0.4% or about 35 hours during the
year. Data obtained from other sources often uses different design criteria, as explained in the Data Source
help topic.
The summer design dry-bulb is the basis for constructing cooling design day temperature profiles . It is the
peak temperature in the warmest month of the year. Design temperature profile calculations are described
in a separate help topic.
2. Summer Coincident Wet-Bulb is the average wet-bulb temperature coincident with the summer design
dry-bulb. For weather data obtained from the ASHRAE Handbook of Fundamentals, 0.4% design values are
used since 0.4% dry-bulb values are used. This coincident wet-bulb is used to generate humidity profiles for
design cooling days.
3. Summer Daily Range represents the difference between maximum and minimum dry-bulb temperatures on
an average day during the warmest month of the year. The daily range is used together with the summer
design dry-bulb when constructing cooling design temperature profiles.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Winter Design Temperatures
According to industry practice, design heating loads are calculated for a single ambient condition, not related
to a specific month or time of day. For this design condition, HAP uses the following values to represent
ambient temperature and humidity:
1. Winter Design Dry-Bulb defines the coldest outdoor air temperature considered for heating design
conditions. For weather data obtained from the ASHRAE Handbook of Fundamentals, 99.6% design values
are used. This means the colder temperatures occur in only 0.4% or about 35 hours of the year. Data
obtained from other sources often uses different design criteria, as explained in the Data Source help topic.
The winter design dry-bulb is used to calculate transmission, infiltration and ventilation loads for the heating
design condition. In certain situations, it is also involved indirectly in constructing cooling design
temperature profiles . These design temperature profile calculations are described in a separate help topic.
2. Winter Coincident Wet-Bulb is the average wet-bulb temperature coincident with the winter design dry-
bulb. It is used only for humidification design calculations. Currently winter coincident wet-bulb data is not
tabulated in handbooks such as the ASHRAE Handbook of Fundamentals. It is important to recognize that
HAP’s default winter wet-bulb data is not an ASHRAE value. Instead, default data provided by HAP
corresponds to 50% relative humidity at the winter design dry-bulb temperature. If you have access to
locally observed winter design humidity data, we encourage you to use it to replace HAP’s default data.
However, in the absence of locally observed data, we feel the estimate using 50% RH is reasonable for
sites with cold winter design conditions, since there is very little change in specific humidity (lb/lb or kg/kg)
for large changes in RH at cold conditions.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Average Ground Reflectance
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Soil Conductivity
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Atmospheric Clearness Number
Atmospheric Clearness Number (ACN) is a factor used to correct clear sky solar radiation profiles for
unusually clear or hazy conditions. HAP’s design day solar radiation profiles are calculated using ASHRAE
procedures which assume specific sky clearness conditions. When your local conditions deviate from this
ASHRAE assumption, solar profiles should be corrected using the an Atmospheric Clearness Number. A chart
is provided on Figure 5, Chapter 33 of the 2003 ASHRAE Handbook - HVAC Applications. ACN values
typically range from 1.15 for very clear conditions, to 1.00 for typical conditions, to 0.85 for very hazy
conditions.
Further information about the use of ACN values in calculations can be found in the solar calculation help
topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Average Ground Reflectance
Average Ground Reflectance defines how much solar radiation is reflected by ground surfaces surrounding
the building. Solar heat striking vertical and tilted surfaces of a building is comprised of beam, diffuse and
ground-reflected components. One ground reflectance value is used for all exposures of the building and all
months of the year. Reflectance varies depending on the type of surface surrounding the building. Typical
values are shown in the table below. The standard default value used by HAP for all cities is 0.20.
Surface Type
Reflectance
New Concrete
0.31 to 0.34
Old Concrete
0.22 to 0.25
Bright Green Grass
0.21 to 0.31
Crushed Rock
0.20
Bitumen and Gravel Roof
0.14
Bituminous Parking Lot
0.09 to 0.12
Notes:
1. Reflectance varies with angle of incidence.
2. Data from 2001 ASHRAE Handbook of Fundamentals, Table 10, pg 30.16.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Soil Conductivity
Soil Conductivity refers to the thermal conductivity of soil surrounding a building. The conductivity affects
calculation of heat transfer through basement walls, basement floors and slab floors. Thermal conductivity
varies depending on the composition of local soil and its moisture content.
When a new city is selected, HAP sets the soil conductivity to a standard default value of 0.8 BTU/hr/ft/F (1.38
W/m/K). Users should override this default if more accurate, site-specific data is available. Sample
conductivities for common soil types in North America are provided in the table below.
Page 7 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Design Cooling Calculation Months
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Time Zone
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Apparent Thermal Conductivity Values for Soils (BTU/hr-ft-F)
Recommended Values
for Design(2)
Classification
Normal
Range
Low(3)
High(4)
Sands
0.35 to 1.45
0.45
1.30
Silts
0.50 to 1.45
0.95
1.30
Clays
0.50 to 0.95
0.65
0.90
Loams
0.50 to 1.45
0.55
1.30
Notes:
1. Derived from 2001 ASHRAE Handbook of Fundamentals, Table 7, page 25.15.
2. Reasonable values for use when no site-specific data are available.
3. Moderately conservative values for minimum heat loss through soil.
4. Moderately conservative values for maximum heat loss through soil.
5. Multiply by 1.731 to convert to W/m/k for SI Metric units.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Cooling Calculation Months
This item defines the range of months considered when performing cooling design calculations for systems
and plants. Once you choose start and end months, your specification will be used for all subsequent system
and plant design calculations in the current project.
To be absolutely sure maximum space loads, zone loads, system loads and plant loads are identified during
sizing calculations, January thru December should be selected. However, based on prior experience, you may
be able to select a smaller range of months and still be confident that peak loads will fall within this period. For
example, for a certain building type and building location choosing summer and fall months might ensure that
all possible peak load times are considered in the analysis. The benefit of choosing fewer months is that
system and plant sizing calculations will run faster. The risk is that peak load times might be excluded from the
analysis resulting in unreliable sizing data. When in doubt, choose January thru December to ensure all peak
load conditions are included in your analysis.
Note: Your choice of design cooling calculation months has no effect on design heating calculations. Design
heating calculations will always be performed for the winter design condition no matter what design cooling
months are selected. For example, in the northern hemisphere it is not necessary to include January in your
range of months just to ensure heating calculations are properly performed. In the southern hemisphere, it is
not necessary to include July in your range of months to ensure heating calculations are properly performed.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Time Zone
This item defines the difference between Local Standard Time (LST) and Greenwich Mean Time (GMT) in
hours. The time zone value and the site longitude are used to convert between apparent solar time (AST) and
local time (LT) when performing solar radiation calculations. The direction and intensity of solar flux depends
Page 8 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Daylight Savings Time
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
upon solar position which is a function of AST. However, building operation is scheduled according to LT.
Therefore, a conversion between the two systems of measuring time is necessary.
Positive time zone values indicate the time zone is to the west of the Greenwich Meridian. Negative values
indicate the time zone is to the east. Sample time zone values for North America are shown in the table below.
Further information about the use of the time zone input in calculations can be found in the time calculation
help topic.
Time Zone
Hours Difference Between GMT &
LST
Newfoundland
GMT + 3.5 hours
Atlantic
GMT + 4 hours
Eastern
GMT + 5 hours
Central
GMT + 6 hours
Mountain
GMT + 7 hours
Pacific
GMT + 8 hours
Yukon
GMT + 9 hours
Hawaii
GMT + 10 hours
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Daylight Savings Time
HAP provides the option of considering daylight savings time during a portion of the year. "Daylight Savings
Time" is the portion of the year when local time is shifted forward by one hour. The term "daylight savings" is
used in the United States. In other countries this is referred to by other names such as "summer time."
Use of daylight savings time affects the timing of solar heat gains and ambient temperatures. In the case of
solar gains, the direction and intensity of solar flux depends upon solar position which is a function of apparent
solar time (AST). However, building operation is scheduled according to local time (LT). Therefore, a
conversion between the two systems of measuring time is necessary to calculate the correct solar gains at the
correct times of day as measured in local time. Daylight savings time is one consideration in this conversion
from solar to local time. In the case of ambient temperatures, the maximum temperature is assumed to occur
at 1500 local time for design cooling profiles. When daylight savings time is in use, the profile is shifted so the
peak temperature occurs at 1600 local time.
Three input items are used to describe daylight savings time:
1. Daylight Savings Time. This item is used to specify whether daylight savings time should be considered.
Click on the desired item (Yes or No).
2. DST Begins defines the month and day for the beginning of the daylight savings period. The program
assumes daylight savings time begins at 12:01 am on this day.
3. DST Ends defines the month and day for the end of the daylight savings period. The program assumes
daylight savings time ends at 11:59 pm on this day.
Application Information. When specifying daylight savings time for system design applications, remember
that the convention is that the cooling design day occurs on the 21st of each month.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 9 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Data Source
9.0 Entering Weather Data ›› 9.2 Design Parameter Data ››
Data Source
This item on the Design Parameters tab indicates the source of HAP’s default weather data for latitude,
longitude, elevation, summer dry-bulb, summer wet-bulb, summer daily range, and winter dry-bulb. As shown
below, the source also conveys information about the meaning of summer and winter design temperatures.
This is not an input item; it is provided for reference only.
Design Weather Data Sources in HAP
1. 2001 ASHRAE Handbook. Data obtained from Chapter 27 of the 2001 ASHRAE Handbook of
Fundamentals. Summer temperatures are 0.4% design values. The winter design dry-bulb is the 99.6%
design value. Percentages are in relation to the entire year.
2. 1997 ASHRAE Handbook. Data obtained from Chapter 26 of the 1997 ASHRAE Handbook of
Fundamentals. Summer temperatures are 0.4% design values. The winter design dry-bulb is the 99.6%
design value. Percentages are in relation to the entire year.
3. 1993 ASHRAE Handbook. Data obtained from Chapter 24 of the 1993 ASHRAE Handbook of
Fundamentals. Summer temperatures are the 1% design dry-bulb and mean coincident wet-bulb, where
available. Otherwise summer temperatures are the 1% design dry-bulb and 1% design wet-bulb. The winter
design dry-bulb is the 99% design value. Percentages are in relation to summer or winter months only.
4. 1989 ASHRAE Handbook. Data obtained from Chapter 24 of the 1989 ASHRAE Handbook of
Fundamentals. Summer temperatures are the 1% design dry-bulb and mean coincident wet-bulb, where
available. Otherwise summer temperatures are the 1% design dry-bulb and 1% design wet-bulb. The winter
design dry-bulb is the 99% design value. Percentages are in relation to summer or winter months only.
5. 1982 Climatic Data, Region X. Data obtained from "Climatic Data for Region X, Arizona, California, Hawaii,
Nevada", ASHRAE, 5th Edition, May 1982. Summer temperatures are the 0.1% design dry-bulb and mean
coincident wet-bulb. The winter design dry-bulb is the 0.2% value. Percentages are in relation to the entire
year.
6. 1994 Environment Canada. Design data was obtained from Environment Canada in 1994. Details
regarding the design criteria for summer and winter temperatures are not available.
7. 1978 USAF Weather Manual. Data obtained from "Facility Design and Planning Engineering Weather
Data", AFM 88-29, July 1978. Summer temperatures are the 1% design dry-bulb and mean coincident wet-
bulb. The winter design dry-bulb is the 99% value. Percentages are in relation to summer or winter months
only.
8. China Design Criteria GBJ19-87. Data provides the standard values used by design engineers in China.
9. 1993 NIWAR. Data obtained from the National Institute of Water & Atmospheric Research, Ltd in New
Zealand. No details available about design temperature criteria.
10. 2002 Carrier CIAC. Data for Caracas, Venezuela was supplied by Carrier Inter-America after consultation
with engineers in Caracas. This data was used because Caracas data is not available in current
handbooks.
11. 1993 Carrier SA (France). Data obtained from Carrier SA in France and is meant to represent design
values commonly used by local engineers. No details available about design criteria.
12. 1993 Carrier Gmbh (Germany). Data obtained from Carrier Gmbh in Germany and is meant to represent
design values commonly used by local engineers. No details available about design criteria.
13. 1993 Carrier BV (Netherlands). Data obtained from Carrier BV in the Netherlands and is meant to
represent design values commonly used by local engineers. No details available about design criteria.
14. 1993 Carrier Interclisa (Spain). Data obtained from Carrier Interclisa in Spain and is meant to represent
design values commonly used by local engineers. No details available about design criteria.
15. 1993 Carrier AB (Sweden). Data obtained from Carrier AB in Sweden and is meant to represent design
values commonly used by local engineers. No details available about design criteria.
Page 10 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.3 Design Temperature Profiles
9.0 Entering Weather Data ››
Design Temperatures Tab / Weather Form
9.0 Entering Weather Data ›› 9.3 Design Temperature Profiles ››
16. 1993 Carrier AC Ltd (UK). Data obtained from Carrier Air Conditioning, Ltd in the United Kingdom and is
meant to represent design values commonly used by local engineers. No details available about design
criteria.
17. 1993 Carrier Delchi (Italy). Data obtained from Carrier Delchi in Italy and is meant to represent design
values commonly used by local engineers. No details available about design criteria.
18. 1993 Carrier Australia. Data obtained from Carrier Australia and is meant to represent design values
commonly used by local engineers. No details available about design criteria.
19. 1993 Carrier Asia/Pacific. Data obtained from Carrier Asia/Pacific Operations and is meant to represent
design values commonly used by local engineers. No details available about design criteria.
20. 1984 Toyo Carrier (Japan). Data obtained from Toyo Carrier of Japan and is meant to represent design
values commonly used by local engineers. No details available about design criteria.
21. User-Defined. Indicates that the user has directly entered design parameters for this city or has modified
default data from HAP’s weather database.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes inputs on the Design Temperature Profiles tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Temperatures Tab / Weather Form
About Design Temperature Data. The Design Temperatures tab contains information about cooling design
day temperature and humidity profiles for the currently selected city. Based on the design parameters for the
city you selected, HAP constructs 24-hour profiles of temperature and humidity for all 12 months. Each profile
represents warmer than normal conditions and typical humidity levels that coincide with these temperatures.
Temperature and humidity profiles form the basis for cooling design load calculations and system performance
calculations.
Note: Profiles for all 12 months represent warmer than normal conditions. A common misunderstanding is
the belief that profiles in winter months represent colder than normal conditions. This is not the case. All 12
profiles represent design cooling conditions. The availability of cooling design profiles for all 12 months is
mainly important in tropical sites where peak cooling loads can occur at any time of year. In addition, cooling
design data for winter months is sometimes needed for special applications outside of tropical regions.
Page 11 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.4 Design Solar Profiles
9.0 Entering Weather Data ››
The Design Temperatures Tab allows you to view and edit the cooling design temperature and humidity
profiles. The tab contains two tables:
1. The Monthly Max/Min table on the left-hand side of the tab summarizes the design temperature and
humidity profiles by listing the maximum and minimum dry-bulb and wet-bulb temperatures in each profile.
This summary of data is useful for quickly reviewing the variation of design temperatures and humidities
during the year. It can also be used to shift the entire profile up or down, or to expand or compress its
range.
In the Monthly Max/Min table each row contains data for a different month. Columns contain the maximum
and minimum dry-bulbs and wet-bulbs for each month. To adjust the profiles, simply modify the desired
maximum and minimum values. The design profile will be updated immediately to span the range between
the new maximum and minimum values, but will preserve the original shape of the profile. Data for the
updated profile can be reviewed in the Hourly Detail View table on the right-hand side of the tab.
2. The Hourly Detail View table on the right-hand side of the tab lists the complete cooling design dry-bulb
and wet-bulb profiles for all 12 months. This table allows the hourly profiles to be viewed and to be changed
on an hour-by-hour basis.
In the Hourly Detail View table rows contain data for the 24 hours of the day. Columns contain dry-bulb and
wet-bulb profiles for each month. To edit data use the scroll bars to move to a month and hour and then
modify the desired values.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes inputs on the Design Solar Profiles tab.
Page 12 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Design Solar Tab / Weather Form
9.0 Entering Weather Data ›› 9.4 Design Solar Profiles ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Design Solar Tab / Weather Form
About Design Solar Data. The Design Solar tab contains information about solar heat gain profiles for the
currently selected city. Based on the design parameters for the city you selected, HAP constructs 24-hour
profiles of solar flux and solar heat gain for all 12 months using ASHRAE procedures. Each profile represents
clear sky solar conditions. Solar profiles are used for wall, roof and window load calculations.
The Design Solar Tab allows you to view and edit the solar profiles. The tab contains a single table in which
each row contains data for one month. Columns contain the peak solar heat gain for the seventeen principal
wall and roof orientations. Note that the peak solar heat gains shown here represent only a small fraction of
the 19,584 flux and heat gain values contained in the solar profiles. The complete profiles can be reviewed
using the Design Solar Profiles report.
Peak solar heat gain data can be viewed by scrolling horizontally through the table. Profiles can be modified
by specifying a profile multiplier found toward the left end of each row. When you enter a multiplier, all hourly
flux and heat gain profiles for the month will be adjusted accordingly. Multipliers greater than 1.0 increase the
solar values. Multipliers smaller than 1.0 decrease the solar values.
Example: A multiplier factor of 1.10 is specified for the month of July. The program will immediately increase
all 4,896 design day solar flux and solar heat gain values for the month of July by 10% from their original
values. The 17 peak solar heat gain values shown for July on this tab will be updated to reflect the change.
Adjustments are always made with respect to the originally calculated values. Thus, if you wish to change data
back to the original calculated values, simply enter a multiplier of 1.00.
Page 13 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.5 Simulation Weather Data
9.0 Entering Weather Data ››
Simulation Tab / Weather Form
9.0 Entering Weather Data ›› 9.5 Simulation Weather Data ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains inputs on the Simulation Weather tab.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Simulation Tab / Weather Form
Items on the Simulation Tab are used to select the simulation weather data used for energy simulations for the
current project, and to define the operating calendar for the energy simulation.
Inputs on this tab divide into two groups:
1. Simulation Weather - Simulation weather data refers to the 8,760 hour sequence of actual weather data
(temperature, humidity, solar radiation) used to simulate building loads and HVAC equipment operation
over the course of a year. Simulation weather for your project can be loaded from one of two sources:
a. HAP Library - HAP offers a library of pre-processed, quality checked simulation weather files for over
500 cities worldwide. The Select from HAP Library button is used to load data from this source.
b. Importing Data from an External File - Data can also be loaded directly from an external file from
common weather libraries and web sources. The file formats currently supported include EnergyPlus
Page 14 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Selecting From HAP Library
9.0 Entering Weather Data ›› 9.5 Simulation Weather Data ››
EPW, ASHRAE International Weather for Energy Calculations (IWEC), ASHRAE IWEC version 2
(IWEC2), USA TMY2 and USA TMY3. The Import a Weather File button is used to load this type of data.
2. Operating Calendar - The operating calendar defines the sequence of days during the year. Because
energy simulations are dynamic, thermal performance on one day affects performance on one or more
subsequent days. Internal heat gains and equipment operation are usually closely tied to human activity in
the building, which in turn is tied to the day of the week and holidays. Therefore, it is important to define the
sequence of days for the 365-day simulation year.
The Day of Week for January 1st establishes the day of the week which starts the day sequence for the
year. This establishes which days of the week match up with the 365 days in the year.
The Holiday Calendar establishes which days of the year are exceptions to the normal Monday thru Sunday
scheduling cycle because they are holidays.
Note that this tab only appears when running HAP in full HAP mode. It does not appear for HAP System
Design Load.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Selecting from HAP Library
The "Select From HAP Library" button is used to select a simulation weather file from HAP's library of pre-
processed, quality checked data files. When this button is pressed the Select From HAP Library window will
appear, as shown below. This is a standard Windows file selection window that allows you to locate and select
the desired simulation weather file.
When the dialog initially appears, it displays HAP simulation weather files contained in the \E20 II\Weather
folder on the drive HAP is installed on. HAP automatically installs the full library of simulation weather files in
this folder. Simply highlight the desired file and press the Open button. The file and its data will be loaded into
your project. You will then be returned to the Weather Properties window.
Page 15 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
About Simulation Weather Data Files. Simulation weather data refers to the 8,760 hour sequence of actual
weather data (temperature, humidity, solar radiation) used to simulate building loads and HVAC equipment
operation over the course of a year. A library of data files containing simulation weather for more than 500
cities worldwide is provided with HAP. Each file contains data for a different city. The file name indicates the
contents of the file and the type or source of data. For example: USA\_ILLINOIS\_CHICAGO\_TMY2.HW1
contains data for Chicago whose source was the US NREL TMY2 weather data. The library is automatically
installed with install HAP.
Application Information. Simulation weather data is provided for many, but not all, of the cities in HAP’s
design weather database. While temperature and humidity data is measured at nearly every weather station,
solar radiation measurements are only taken at a limited number of stations. Recently, reliable methods for
estimating solar radiation from cloud cover data have come into use. Since cloud cover is measured at many
weather stations, this has expanded the sites for which simulation weather data can be derived.
In those cases where a simulation weather file is not available for your building site, first check for weather
from external sources which can be loaded via the Import a Weather File option. In recent years availability of
simulation weather data has grown rapidly and certain sources such as the US Department of Energy's
EnergyPlus web site now offer data for thousands of cities worldwide.
If a simulation weather file for the building site can't be found, a nearby location should be chosen. For best
results, this nearby site should be:
1. Geographically close to the building site. Latitude and longitude affect the angles of incidence for solar
radiation. The farther the simulation data site is from the actual building site, the larger the margin of error in
solar heat gains and loads.
2. Climatically similar to the building site. If temperature, humidity and cloudiness conditions are similar to
those at the building site, the simulation data can provide accurate results.
3. At a similar elevation. Elevation affects psychrometrics and airflow calculations. The closer the simulation
data elevation is to the building site elevation, the more accurate the results.
When simulation weather data is for a site different from the building site, readers should note that the latitude,
longitude, time zone and elevation from the simulation weather data file will be used in calculations rather than
Page 16 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Importing\_Weather\_Data
9.0 Entering Weather Data ›› 9.5 Simulation Weather Data ››
the values specified on the Design Parameters tab. This is required for valid solar radiation and humidity
calculations for the simulation data. Note that the ground reflectance and daylight savings time values
specified on the Design Parameters tab are used in simulation calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Importing Weather Data
The "Import a Weather File" option is used to import simulation weather data from an external file. While HAP
offers a library of data for over 500 cities worldwide, other extensive sources of data exist and can be utilized
via this "Import" feature. The procedure for importing data is described first below. Next application
information is provided regarding how to determine your data format, how to find weather from external
sources and how to validate imported weather data.
Procedure. When the "Import a Weather File" button is pressed, the Import a Weather File selection window
shown above appears. Using this window importing a weather file requires three steps:
1. Choose File Format Type - At the bottom of the window select your file format in the "Files of Type" drop-
down list. File format is determined by your source of data. The Application Information section below
describes how to determine your file format. Choices in the drop-down list include EnergyPlus EPW,
ASHRAE IWEC, ASHRAE IWEC2, USA TMY2 and USA TMY3. Once a file format is selected, the window
will only display files of that type.
2. Browse to Locate File - Next use the file navigation features at the top of the window to navigate to the
folder on your computer containing the desired weather file. If you obtained the file from a web site, you will
previously have downloaded and the file into a specific folder on your computer. If you are working from
data on a CD, in some cases you can navigate to the proper folder and read data directly from the CD..
Page 17 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
3. Select File - Once you have your desired weather file displayed in the file list on the window, click it once to
select it. Then press the Open button in the lower right. HAP will translate data from your chosen file and
store it in the proper format in your project. When translation is complete, a message is displayed
explaining how to quality check the data. The Application Information section below also contains
information about quality checking imported data.
Application Information.
1. What is My Data Format? The first question when importing data from an external source is "what format
do I have?"
"Format" refers to how weather data is arranged in the data file. HAP is programmed to recognize several
common weather data file formats. When you specify the format, HAP knows where to find data within that
specific kind of file. Each format arranges data differently so it is critical to properly identify the format of
your file. Otherwise, HAP will not be able to read the data.
File format is indicated by the "extension" of the file name. File names are comprised of two parts - the
body and the extension. In the sample file name below, the file extension is ".epw". The body is everything
that comes before the ".epw".
USA\_IL\_Chicago-OHare.Intl.AP.725300.epw
The extensions for file formats currently supported by HAP are:
.EPW = EnergyPlus EPW format
.IWC = ASHRAE IWEC format
.CSV = ASHRAE IWEC2 format
.TM2 = USA TMY2 format
.CSV = USA TMY3 format
The file extension is a reliable indicator of file format if you obtained the file from a primary source such as
the DOE EnergyPlus web site, or an ASHRAE IWEC CD for example. Identifying the file format can
sometimes be tricky, however. Common pitfalls are described below:
a. Pitfall 1 - Secondary Source - If you obtained the file from a secondary source - a colleague e-mailed
you the data for example - there is a risk the file has been renamed and the extension may no longer be
a reliable indicator of the format. If the file has an .EPW extension but is not in EnergyPlus format, for
example, HAP will not be able to read the data and will display a message indicating the file format is not
correct.
b. Pitfall 2 - Format Determined from Body of File Name - In some situations the body of the file name
includes information that might be mistaken for the file format. For example the file
USA\_PA\_Philadelphia.Intl.AP.TMY3.epw contains "TMY3" in the body of the file name. However, this
only means the original source of the data is the TMY3 library. The file extension says this file is in
EnergyPlus EPW format.
c. Pitfall 3 - Not All .CSV Files are TMY or IWEC2 - Files using the TMY3 and IWEC2 formats both have
a .CSV file extension. However, this file extension is shared with a vast number of Excel spreadsheet
files saved in comma separated value (CSV) format. Therefore, just because you have a file with a .CSV
extension does not necessarily mean it is in TMY3 or IWEC2 format. The key is to make sure you
obtained the file from a primary source - the ASHRAE IWEC2 CD-ROM or the NREL TMY3 web site.
d. Pitfall 4 - Renaming a File Does Not Format It - If you have weather data in one format, renaming the
file to use one of the extensions HAP recognizes does not automatically make it formatted. For example,
suppose a colleague e-mails you some weather data in Excel XLSX format. You notice HAP does not
offer XLSX as a file format, so you rename the file with the .EPW extension and try to import it as an
EnergyPlus EPW file. This will fail because the data is still in Excel format. Giving the file a .EPW
extension did not change its format.
2. How Do I Obtain Weather Files from External Sources? There are many primary sources for simulation
weather data files. The most common sources are noted below.
a. EnergyPlus Web Site - One of the most widely used sources of data is the US Department of Energy
(DOE) EnergyPlus web site. The DOE has collected simulation weather data from many sources and
converted them to a single standard format. As a result this web site serves as a single repository of
Page 18 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
data for thousands of cities worldwide. You can find this site by a web search using the phrase
"EnergyPlus weather".
Files downloaded from this site are in ZIP format. The ZIP file contains multiple files. The file you need
to extract to use with HAP is the one with the .EPW file extension.
b. ASHRAE - ASHRAE offers for sale CD-ROMs containing the International Weather for Energy
Calculations (IWEC) or IWEC version 2 (IWEC2) weather libraries. For IWEC, files can be read directly
from the CD-ROM. For IWEC2 files on the CD are zipped, so the file must be copied to your hard disk
and unzipped to produce a .CSV file before it can be imported into HAP.
c. TMY3 - Typical Meteorological Year version 3 (TMY3) files for cities in the United States can be
downloaded from a National Renewable Energy Laboratory (NREL) web site. You can find this site by a
web search using the phrase "NREL TMY3 weather data". Files downloaded from the web site are not
zipped and can be used directly once saved on your hard disk.
d. Other - Other organizations and governments have created their own weather files in one of the formats
supported by HAP. Most frequently the .EPW format is used. These files can be obtained from the
organization or government body that created the files.
3. How Do I Quality Check Imported Data? Users should always be skeptical about the quality of data
imported from an external source. Even if it comes from the EnergyPlus web site, ASHRAE or a
government source, it can contain erroneous data.
Erroneous data exists either due to a malfunction of weather station equipment when data was recorded or
errors in data processing afterwards. Erroneous data is unusually high or low values of temperature,
humidity or solar radiation for the given location, time of year or time of day. Erroneous data can have
adverse effects on the accuracy of your simulation. For example, suppose a data processing error for
results in little or no beam solar radiation being included in the file. This will result in summer cooling loads
being smaller than actual, and will result in winter heating loads being larger than actual. Simulation results
will be significantly skewed using this weather data.
After importing weather from an external source Carrier recommends quality checking the data as follows:
a. After the data is imported click OK to save and return to the HAP main window. From the main window
generate the following two weather reports: (i) Simulation Weather Summary and (ii) Simulation
Temperature Profile Graph for Jan 1 thru Dec 31.
b. Inspect the Simulation Weather Summary Report. Table 2 provides statistics for the maximum and
minimum temperatures each month. Compare this data with your summer and winter design points for
the city. It is normal for the simulation weather file to have temperatures that exceed the summer and
winter design values by several degrees. But if maximum or minimum temperature are significantly out
of line, this may indicate a problem. Further, look for unusual temperatures based on time of year. For
example, a maximum of 95 F (35 C) in a mid-winter month in a cold climate city should be raise
suspicion. When odd data is found, the Simulation Temperature Profile Graph report can be used to
identify when the odd data occurs and whether it is reasonable or not.
Table 3 in this report contains solar radiation statistics. The data to inspect is the monthly clearness
indexes on the right side of the table. Clearness index is the ratio of daily total solar on a horizontal
surface at ground level divided by total daily solar on a horizontal surface at the outer edge of earth's
atmosphere. Maximum values should be in the 0.6s or 0.7s. Any values in the 0.8s or 0.9s indicates
solar is too high. Maximums in the 0.5s or lower may indicate solar is underestimated. However you
should also consider local climates with persistent cloudiness such as a monsoon season that could
explain unusually low values. For the minimum clearness index data look for values of 0.00. Even when
it is very cloudy, there is a little bit of diffuse solar radiation reaching the ground, so values of 0.00 should
not occur. This tends to indicate a problem with underestimated solar. If problems with solar data are
indicated the Simulation Solar Profile Graph report can be used to investigate further.
c. Inspect the Simulation Temperature Profile Graph report. When this report is generated for the full year
you can quickly identify questionable data. It will appear as sharp upward or downward spikes in the
profile. Note that temperature and humidity can be highly variable so a certain amount of up and down
spikes is reasonable. Spikes to unreasonable levels, such as to 95 F (35 C) in a cold mid-winter month,
however should be investigated further.
Page 19 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
Day of Week for January 1st
9.0 Entering Weather Data ›› 9.5 Simulation Weather Data ››
List of Holidays
9.0 Entering Weather Data ›› 9.5 Simulation Weather Data ››
If you find what appears to be erroneous data, engineering judgement must be used to determine whether
to use the data or discard it. Three spikes in temperature data during the year each over a short duration of
time may be judged insufficient to compromise accuracy of simulation results. Persistent underestimating
of beam solar radiation, on the other, hand may be judged so serious the data cannot be used for
simulation.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Day of Week for January 1st
The "Day of Week for January 1st" item defines the starting point for the operating calendar for an energy
simulation. This is the first of two inputs that define the operating calendar for an energy simulation.
The sequence of days in the simulation is important because dynamic heat flow in the building causes thermal
behavior and equipment operation on successive days to be related. Therefore it is necessary to define the
day of the week for the first day in the 365-day sequence of days used in an energy simulation.
Select the desired day from the drop-down list. When a day is selected, the calendar image used to select
holidays will adjust to your selection.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
List of Holidays
The "Holidays List" item defines when holidays occur in the operating calendar for the energy simulation. This
is the second input that determines the operating calendar for the simulation.
Holidays are selected or deselected using the calendar image on the right side of the tab. A list of all holidays
currently selected is shown on the left. To select holidays:
a. Use the Previous and Next buttons beneath the calendar to scroll to the desired month.
b. Double-click on a day number to select it as a holiday. The day will be darkened in the calendar to indicate it
is selected. The day will also be added to the holiday list on the left.
c. To de-select a holiday, double-click on a day that is already selected. The day will return to normal color to
indicate it is no longer selected. The day will also be removed from the holiday list on the left.
Page 20 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
9.6 Common Tasks
9.0 Entering Weather Data ››
Editing Weather Data
9.0 Entering Weather Data ›› 9.6 Common Tasks ››
Printing and Viewing Weather Reports
9.0 Entering Weather Data ›› 9.6 Common Tasks ››
Why the Operating Calendar and Holidays are Important. Loads and equipment operation in a building are
strongly related to human activity. Activity is usually related to days of the week. Holiday or shutdown periods
often have a pattern of internal heat gains and equipment operation different from other days of the week.
Dynamic heat transfer causes thermal behavior and equipment operation on successive days to be related.
Therefore the sequence of days in the operating calendar has an important effect on simulation results.
The sequence of days of the week (Sunday, Monday, etc...) is determined by the "Day of Week for January
1st" input and repeats every 7 days. Holidays occur at irregular intervals and therefore need to be separately
identified. Profiles that you define later for your internal heat gain and equipment operation schedules can be
linked to specific days of the week and also to holidays. While simulating building loads and equipment
operation for each day of the year, the program the program will use the proper profile from your schedules
depending on the day of the week and whether the current day is a holiday.
Application Information. The holiday feature of the program can be used both for conventional holidays, and
for any other situation where heat gains or operation is independent of the day of the week. This can include
shutdown periods for manufacturing facilities and schools.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains common tasks involving weather input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing Weather Data
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing and Viewing Weather Reports
About Weather Reports. HAP provides four ways to generate weather data reports. These methods use
various menu options and toolbar buttons as described in the Generating Weather Reports help topic. All four
procedures require selection of weather report options using the Weather Report form shown below.
Page 21 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
The Weather Report Form is divided into three sections:
1. Design Reports. The upper section contains a checklist of design weather reports. To choose reports, first
place a check mark next to the desired report options. Once reports have been selected, press the Print
button to print the report, or press the Preview button to view the report. Four design reports are offered:
a. Design Parameters and MSHGs is a one page report listing the design parameters for the current city
as well as the table of maximum solar heat gains.
b. Design Temperature Profiles is a one page report containing the cooling design dry-bulb and wet-bulb
temperature profiles for all 12 months.
c. Design Temperature Profile Graph is a one-page report which provides a graph of the cooling design
dry-bulb and wet-bulb temperature profile for one month. This month must be selected from the drop-
down list opposite this report option.
d. Design Solar Profiles tabulates solar flux and heat gain profiles for one month. The month is selected in
the drop-down lists opposite this report option. The report contains four pages. Each page lists hourly
profiles for a different solar component for the seventeen principal wall and roof orientations. The solar
components are solar flux, the beam component of solar heat gain, the diffuse component of solar heat
gain and the total solar heat gain.
2. Simulation Reports. The second section contains a checklist of simulation weather reports. This section of
the dialog does not appear if you are running in System Design Load mode.
To choose reports, first place a check mark next to the desired report options. Once reports have been
selected, press the Print button to print the report, or press the Preview button to view the report. Four
simulation weather reports are offered:
a. Simulation Weather Summary is a two page report which summarizes conditions from the 8,760-hour
simulation weather file used for energy simulations. Because the weather data consists of 508,445
values defining hourly temperature, humidity and solar radiation conditions, it is sometimes helpful to use
statistics to make sense of this quantity of data. For each month the report lists the absolute maximum,
average daily maximum, average, average daily minimum and absolute minimum temperature, plus the
times when absolute maximums and minimums occur. The report also lists maximum, average and
minimum daily solar radiation totals and the days on which each occurs. Finally, the report lists site data
such as the latitude, longitude and elevation, and the holiday selections from the Simulation tab on the
Weather form.
Page 22 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm
b. Simulation Weather Profiles is a tabular report that lists hourly temperature, humidity and solar
radiation data for one or more days. The start and end days for the reporting period are specified using
items to the right of this report option. When you click on the From or To item, a calendar image appears
and allows you to select the start or end day.
Note #1: Readers should note that this calendar image is not synchronized with your operating calendar
for the project, so the position of day numbers in the calendar DO NOT correspond to specific days of the
week. For example, January 1st always appears as a Sunday in this calendar image.
Note #2: We recommend only selecting short sequences of days when using this report. When selecting
more than 4 or 5 days, this report often takes a long time to be generated. When you need to review
longer sequences of weather data, we recommend using the two graph options below. Both graphical
reports always generate quickly, even when the entir year is selected.
c. Simulation Temperature Profile Graph provides a line graph of hourly dry-bulb and wet-bulb
temperatures from the simulation weather file. This report is often useful for quickly identifying times of
year with extreme hot or cold conditions. As with the Simulation Weather Profiles report above, users
select the start and end days for the reporting period. Periods from 1 day to 365 days in length can be
selected.
d. Simulation Solar Profile Graph provides a line graph of hourly solar radiation profiles from the
simulation weather file. This report can be useful for identifying times of intense solar radiation when high
building loads may occur. As with the Simulation Weather Profiles report above, user select the start and
end days for the reporting period. Periods from 1 day to 365 days in length can be selected.
3. Command Buttons appear along the bottom of the form. Five buttons are provided on this form:
a. Restore Defaults is used to reset data on this form to the standard default set of selections. This is often
done when users wish to clear existing selections and begin selecting options all over again.
b. Print is used to print the selected reports.
c. Preview is used to display the selected reports. Once the reports have been displayed they can be
printed, saved as bitmaps or copied to the clipboard using options in the HAP report viewer.
d. Cancel is used to exit from the form without generating reports.
e. Help is used to display this help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 23 of 23
9.0 Entering Weather Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh38A2.htm