27.0 Weather Calculations
27.1 Weather Calculation Overview
27.0 Weather Calculations ››
Weather Data Calculation Overview
27.0 Weather Calculations ›› 27.1 Weather Calculation Overview ››
27.2 Time Conventions for Weather and Load Calculations
27.0 Weather Calculations ››
Time Conventions for Weather and Load Calculations
27.0 Weather Calculations ›› 27.2 Time Conventions for Weather and Load Calculations ››
This chapter explains calculations involving weather data for system design calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section provides an overview of weather data calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Weather Data Calculation Overview
This and the following series of help topics document the design weather data calculations in HAP.
About Design Weather Data. In order to determine the maximum cooling loads for a building, 24-hour profiles
of warmer than normal temperatures and corresponding humidities are considered for each month. Clear sky
solar fluxes and heat gains are also required to determine maximum solar loads on walls, roofs and windows.
Therefore, HAP calculates temperature, humidity, solar flux and solar heat gain profiles for one design day in
each month of the year. One of the basic considerations for all these calculations is the convention used to
measure time. For further information on these calculations, please click on the desired topic below.
Time conventions for weather and load calculations.
Calculating design temperature and humidity profiles.
Calculating clear sky solar flux profiles.
Calculating clear sky solar heat gain profiles.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains time conventions used for weather data and load calculations.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Time Conventions for Weather and Load Calculations
Page 1 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
This help topic explains the time conventions HAP uses for weather and load calculations.
About Local Time. Local time (LT) is clock time. This is the time indicated by the clock on your wall and by
which we all conduct our businesses and daily lives. All calculations in HAP are performed according to local
time. This is the most logical and accurate approach since schedules for building occupancy, heat gains and
equipment operation are specified in terms of local time.
About Apparent Solar Time. Many readers may be surprised that there is any other way of measuring time
than local time. For purposes of weather and load calculations, however, apparent solar time (AST) is an
important concept. Apparent solar time is related to the movement of the Sun across the sky. Noon according
to AST is when the Sun reaches its highest point or zenith in the sky. AST for the rest of the day is measured
with respect to this "solar noon". Because the Earth rotates 15 degrees each hour, 1pm AST is when the Earth
has rotated 15 degrees past the zenith position of the Sun. In order to calculate solar fluxes and solar heat
gains for a building, the position of the Sun in the sky must be determined using the AST. When calculating
loads for a certain hour according to local time, the corresponding apparent solar time must be determined so
solar loads can be calculated. This is because AST is not the same as local time.
Local versus Apparent Solar Time. The best way to understand why apparent solar time and local time are
different is with an example. Consider Boston and Detroit, two cities located in the Eastern Time Zone of North
America, but separated by several hundred miles and 12 degrees of longitude. When clocks in Boston read
12:00 noon, clocks in Detroit read the same time. Local time is always the same in both cities. However, when
the Sun is at its zenith over Boston, it is not yet at its zenith over Detroit. It will take the Earth 48 minutes to
rotate 12 degrees needed for the Sun to reach its zenith position over Detroit. Consequently, solar radiation
striking buildings at the same local time in Boston and Detroit will differ because the Sun is in a different
position in the sky in each city. While local time is the always the same in Boston and Detroit, apparent solar
time will never be same. Further, to calculate accurate solar loads for 12 noon local time, the difference
between local and apparent solar time must be accounted for.
Expanding this example to a more general discussion, all cities in the same time zone always have the same
local time. However, only cities at the same longitude have the same apparent solar time. Further, local time
and apparent solar time differ for all but a few days each year. The differences between LT and AST are due
to three factors:
a. The fact that the Earth's orbit is elliptical rather than circular and that the Earth travels along its orbit while
rotating rather than standing still. This causes varying differences between LT and AST each day of the
year. Differences range between 0 minutes and 16.5 minutes as shown in Figure 1 below.
b. The difference between the longitude of a city and the central longitude for the time zone. This is usually
responsible for differences up to 30 minutes between LT and AST, but in some time zones the difference
can be larger.
c. The use of daylight savings time introduces a further 1 hour difference between LT and AST.
Apparent solar time is calculated from local time using the following equations:
AST = LT + [4(Lstd - Lloc) + E] / 60 - D
E = 9.87sin(2B) - 7.53cos(B) - 1.5sin(B)
B = 360(N - 81) / 364 , degrees
where:
AST
=
Apparent solar time, hours.
LT
=
Local time, hours.
Lstd
=
Central longitude for local time zone, degrees. This
longitude is computed by multiplying the
number hours difference between local time
and Greenwich Mean Time (GMT) by 15
degrees/hour. For example, the Eastern Time
Zone in North America is GMT + 5 hours.
Therefore, the central longitude is 75 degrees
east.
Lloc
=
Longitude for city, degrees.
Page 2 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
E
=
"Equation of Time" factor which accounts for the difference
between LT and AST due to Earth orbital
effects, hours.
D
=
Daylight savings time factor, hours. Zero hours when
daylight savings time is not in effect. 1 hour
when daylight savings time is in effect.
N
=
Day of year. For example: 1 = January 1; 152 = June 1,
etc...
For a city located on the central longitude of a time zone, and without considering daylight savings time, the
differences between local and solar time would only be due to orbital effects and are shown in Figure 1.
Maximum differences of about 14 to 16.5 minutes occur in mid-February and late October.
For a more realistic example, consider the differences between LT and AST for Detroit, assuming daylight
savings time in effect between April 1 and October 31. These differences are shown in Figure 2 and reach a
maximum value of 98 minutes in late July.
Page 3 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
27.3 Calculating Design Temperature Profiles
27.0 Weather Calculations ››
Calculating Design Temperature Profiles
27.0 Weather Calculations ›› 27.3 Calculating Design Temperature Profiles ››
Program Time Conventions. As stated before, HAP performs all weather and load calculations according to
local time. To calculate solar fluxes and heat gains for a specific local time, the corresponding AST is
computed and used to determine the position of the sun in the sky. Thus, solar radiation profiles will match
local time correctly. As illustrated above, this adjustment can be significant at certain times of year.
Throughout the program weather conditions, loads and energy simulation results are referred to using hours
0000 through 2300. Further, each hour refers to the 60 minute period following the hour. For example, hour
0000 refers to the period between 12:00am and 12:59am local time. Weather conditions, and loads are
calculated at the midpoint of the hour to determine conditions representative of the entire hour. Thus, for hour
0000, calculations are performed for 12:30am local time.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculation of design day temperature profiles.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 4 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
Calculating Design Temperature Profiles
For cooling design calculations, hourly dry bulb and wet bulb profiles are constructed for one 24 hour period in
each month. These profiles are based on cooling design temperature values and represent warmer than
normal conditions. In this help topic the procedures used to derive the design dry-bulb and wet-bulb profiles
are described.
A. Calculation of Dry-Bulb Profiles
For the design day in each month, the dry-bulb temperature profile is constructed using the design dry-bulb
temperature for that month and a pattern for the hourly variation of temperatures recommended by ASHRAE.
This ASHRAE method produces smooth profiles with maximum temperatures at 3pm and minimum
temperatures at 5am. To suit HAP’s time conventions, profiles are adjusted so that maximum temperatures
occur at 3:30pm local time and minimum temperatures occur at 5:30am local time. This is allowable because
the design data represents idealized profiles and are therefore approximate rather than exact. If daylight
savings time is used, the temperature profiles will be shifted for the months during which daylight savings time
is in effect. For these months maximum temperatures occur at 4:30pm and minimum temperatures occur at
6:30am local time.
Individual hourly dry-bulb temperatures for a design day are computed using the following equation.
Ta,h = Tdb,m ΔT Fh
where:
Ta,h
=
Dry bulb temperature for hour h (F or C).
Tdb,m
=
Cooling design dry-bulb for month (F or C).
ΔT
=
Daily temperature range (F or K).
Fh
=
Hourly temperature factor (dimensionless). See Table 1.
Table 1. Hourly Factors (Fh) For Design Dry Bulb Profiles
Time
Fh
Time
Fh
Time
Fh
Time
Fh
0030
0.82
0630
0.98
1230
0.23
1830
0.21
0130
0.87
0730
0.93
1330
0.11
1930
0.34
0230
0.92
0830
0.84
1430
0.03
2030
0.47
0330
0.96
0930
0.71
1530
0.00
2130
0.58
0430
0.99
1030
0.56
1630
0.03
2230
0.68
0530
1.00
1130
0.39
1730
0.10
2330
0.76
Data adapted from Table 2, pg 28.6, 1997 ASHRAE Handbook of Fundamentals [1]
For the warmest month of the year, the design dry-bulb temperature is equal to the summer design dry-bulb
specified for the city. For all other months, the design dry-bulb for the month is either estimated using an
empirical method described in the Carrier System Design Manual [2]. With this Carrier System Design Manual
method, design dry-bulbs are computed using the equation:
Tdb,m = Tsdb Fm
where:
Tsdb
=
Summer design dry-bulb temperature (F or C).
Fm
=
Monthly design temperature factor for month m (F or K).
Fm values are listed in Table 2. Columns in this table are provided for each month. Data in each row
corresponds to a different annual temperature range. The annual range is the difference between the summer
and winter design dry bulbs. Depending on the annual temperature range for a site, data is either read directly
from the table or determined by interpolation between rows.
Page 5 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
Table 2. Monthly Factors for Design Dry Bulb Profiles.
Annual
Monthly Design Temperature Factors (F)
Range
Month (for Northern Hemisphere)
(F)
Jan
Feb
Mar
Apr
May
Jun
Jul
Aug
Sep
Oct
Nov
Dec
50
10
8
5
4
3
1
0
0
2
4
7
9
55
11
9
6
5
3
1
0
0
2
4
8
10
60
15
13
9
7
3
1
0
0
2
5
10
14
65
18
16
11
8
4
1
0
0
2
6
12
17
70
22
19
13
9
4
1
0
0
2
7
14
20
75
23
20
14
9
4
1
0
0
3
7
15
21
80
35
33
24
16
8
3
0
0
4
12
20
30
85
43
40
29
19
9
3
0
0
5
16
25
38
90
44
40
29
19
10
3
0
0
6
16
26
38
95
45
41
29
19
10
3
0
0
6
16
27
39
100
45
41
29
19
10
3
0
0
6
16
27
39
105
47
42
30
20
11
4
0
0
6
17
29
42
110
49
43
30
20
11
4
0
0
6
17
31
44
115
55
49
33
22
11
4
0
0
8
20
36
50
120
66
58
39
22
11
4
0
0
9
24
44
61
Jul
Aug
Sep
Oct
Nov
Dec
Jan
Feb
Mar
Apr
May
Jun
Month (for Southern Hemisphere)
Data adapted from Table 3, pg 1-19, Carrier System Design Manual [2].
Readers should note two limitations of the monthly design temperature calculation. First, data in Table 2 is
limited to annual temperature ranges between 50 F and 120 F (27.8 K to 66.7 K). This range covers most of
the weather conditions encountered in the world. For those sites with annual ranges less than 50 F, the 50 F
values from the table are used. For those sites with annual ranges greater than 120 F, 120 F values from the
table are used.
Second, assumptions about the variation of monthly design dry bulbs during the year, and about when
maximum and minimum design values occur may not apply for all sites. These assumptions are generally
reliable for mid and high latitude sites. For sites near the equator, however, maximum temperatures
sometimes occur in September and March, instead of July or January.
For any situation in which the assumptions are not realistic, profile data should be modified to account for local
conditions. The program provides the ability to quickly modify profile data as necessary.
B. Calculation of Wet-Bulb Profiles
For the design day in each month, the wet-bulb temperature profile is constructed using two different, but very
similar, procedures. Which procedure is used depends on how weather data for a city is specified.
If you select a city from HAP’s weather database and use the default weather data for the city, wet-bulb
temperatures are derived from a specific humidity profile for the day. The peak humidity in this profile is
calculated from the design dry-bulb and coincident wet-bulb temperature for the month. The minimum humidity
is set equal to the peak humidity, unless this humidity condition crosses the saturation line. If it does, the
minimum humidity is based on a wet-bulb temperature equal to dry-bulb temperature minus 0.5 F (0.28 K).
Example #1: For a city having low humidity conditions, the peak humidity is calculated from the design dry-
bulb and coincident wet-bulb temperatures for the month. The minimum humidity is equal to the peak humidity
Page 6 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
because this humidity level is below the saturation level at the time of the minimum dry-bulb. Therefore, the
humidity level is constant for all 24 hours. Hourly wet-bulb temperatures are derived from the dry-bulb and
specific humidity for each hour.
Example #2: For a city having high humidity conditions, the peak humidity is calculated from the design dry-
bulb and coincident wet-bulb temperatures for the month. This specific humidity will result in a condition above
saturation if used at the time of the minimum dry-bulb temperature. Therefore the minimum specific humidity is
computed from the minimum dry-bulb and a wet-bulb which is equal to dry-bulb minus 0.5 F (0.28 K). In this
situation, the maximum and minimum specific humidities differ. Hourly humidities follow a sinusoidal profile
between maximum and minimum values. Hourly wet-bulb temperatures are derived from the dry-bulb and
specific humidity for each hour.
When you modify the default weather data for a city or enter data for a new city, HAP first uses the design dry-
bulb and coincident wet-bulb temperatures to compute the specific humidity for the warmest hour of the day.
This specific humidity is held constant for all 24 hours unless it results in wet-bulb temperatures within 0.5 F
(0.28 K) of the corresponding dry-bulb or wet-bulbs that exceed the corresponding dry-bulb. In these cases,
the wet-bulb temperature for the hour will equal dry-bulb minus 0.5 F (0.28 K). While this method will yield the
same wet-bulb temperatures for the time of maximum and minimum dry-bulb temperatures, there can be a
subtle difference between wet-bulbs between maximum and minimum times for the two methods.
For the warmest month of the year, the summer coincident wet-bulb temperature is used for these
calculations. For the other months coincident wet bulb temperatures are estimated using an empirical method
described in the Carrier System Design Manual [2]. With this method, monthly coincident wet bulbs are
computed using the equation:
Twb,m = Tswb Fw
where:
Twb,m
=
Coincident wet bulb temperature for month (F or C).
Tswb
=
Coincident summer wet bulb temperature (F or C).
Fw
=
Monthly design wet bulb factor for month (F or K).
Fw values are shown in Table 3. Columns in this table are provided for each month. Rows contain Fw values
for different annual temperature ranges. The annual range is the difference between summer and winter
design dry bulb temperatures. Depending on the annual range for a site, Fw data is either read directly from
the table or determined via interpolation between rows.
Readers should note that this method has the same limitations described previously for dry-bulb profiles. For
any situations in which the assumptions used to construct wet bulb profiles are not appropriate, profile data
should be modified to account for local conditions. The program provides the ability to quickly modify profile
data as necessary.
Table 3. Monthly Factors for Design Wet Bulb Profiles.
Annual
Monthly Design Temperature Factors (F)
Range
Month (for Northern Hemisphere)
(F)
Jan
Feb
Mar
Apr
May
Jun
Jul
Aug
Sep
Oct
Nov
Dec
50
6
5
3
2
1
0
0
0
1
2
3
5
55
7
6
3
3
2
0
0
0
1
2
4
6
60
9
8
4
3
2
0
0
0
1
3
5
7
65
12
10
6
4
2
0
0
0
1
3
6
10
70
12
10
6
4
2
0
0
0
1
4
6
10
75
15
12
7
5
2
0
0
0
2
4
8
13
80
24
20
13
9
4
2
0
0
2
6
11
19
85
28
23
14
10
5
2
0
0
3
8
14
23
90
28
23
14
10
5
2
0
0
3
8
14
23
Page 7 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
27.4 Calculating Design Solar Flux Profiles
27.0 Weather Calculations ››
Calculating Design Solar Flux Profiles
27.0 Weather Calculations ›› 27.4 Calculating Design Solar Flux Profiles ››
95
28
23
14
10
5
2
0
0
3
8
14
23
100
28
23
14
10
5
2
0
0
3
8
14
23
105
29
24
15
10
5
2
0
0
3
8
14
24
110
31
25
15
10
5
2
0
0
3
8
16
26
115
39
31
18
11
5
2
0
0
4
10
21
33
120
50
40
23
12
5
2
0
0
4
13
27
42
Jul
Aug
Sep
Oct
Nov
Dec
Jan
Feb
Mar
Apr
May
Jun
Month (for Southern Hemisphere)
Data adapted from Table 3, pg 1-19, Carrier System Design Manual [2].
C. References
1. 1997 ASHRAE Handbook of Fundamentals, American Society of Heating, Refrigerating and Air
Conditioning Engineers, Inc., 1997.
2. Carrier System Design Manual, Part 1: Load Estimating, Carrier Corporation, 1960.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculation of design day solar flux profiles.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Calculating Design Solar Flux Profiles
This help topic explains how solar flux profiles are calculated for design cooling studies. Clear sky conditions
are assumed so the maximum effects of solar heat can be considered. For each month, hourly profiles of solar
flux are constructed using procedures outlined in the ASHRAE Handbook of Fundamentals. Separate sections
below describe fundamental solar energy concepts and how design solar fluxes are calculated.
A. Solar Energy Fundamentals
Before describing design solar calculation procedures, several fundamental solar energy concepts must be
understood. These are presented in the paragraphs below.
Solar Flux is the rate of solar energy striking the exterior surfaces of a building. The direction and intensity of
solar flux influence wall, roof and window load calculations.
Solar Heat Gain refers to the rate of solar energy reaching the interior of a building after passing through a
window. It is used in calculating window solar loads. The solar heat gain differs from the solar flux because the
glass panes, framing and interior shades in a window reflect, absorb and transmit portions of the solar flux that
strikes the exterior surface of the window. Thus, the total solar heat gain is always smaller than the total solar
flux outside the window.
Extraterrestrial Solar Flux. To determine the intensity of solar flux at the Earth's surface, characteristics of
solar flux outside the Earth's atmosphere must be known. This is referred to as the extraterrestrial solar flux.
Because the distance between the Earth and the Sun varies throughout the year, the intensity of the
Page 8 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
extraterrestrial flux varies. In solar energy calculations, the extraterrestrial flux on a surface perpendicular to
the Sun's rays, Ion, is commonly used. Values of Ion listed in Table 1 show the general seasonal variation of
the extraterrestrial flux. These values based the solar constant, Isc. The solar constant is the value of Ion when
the Earth is at its average distance from the Sun. According to the 1997 ASHRAE Handbook of Fundamentals
[1], the currently accepted value for Isc is 433.34 BTU/hr sqft or 1367 W/sqm.
Components of Solar Flux. The solar flux striking a building is composed of three separate components:
1. Beam Solar Flux is the portion of the extraterrestrial solar flux that passes through the Earth's atmosphere
unaltered. Beam solar continues to travel in the original direction of the extraterrestrial flux. Thus, its
direction when it reaches the Earth's surface is dependent on the position of the sun in the sky.
2. Diffuse Solar Flux is the portion of the extraterrestrial flux which reaches the Earth's surface after being
scattered by molecules of air, water vapor, other atmospheric gases and dust in the atmosphere. On
overcast days the intensity of the diffuse flux is nearly uniform over the entire dome of the sky. On clear
days, the diffuse flux is less uniform, with higher intensities in the area of the sky where the sun is located.
3. Reflected Solar Flux is solar energy striking a building after being reflected by ground surrounding the
building. Both direct and diffuse solar fluxes reach the ground. The ground absorbs a portion of this flux and
reflects another portion. Vertical and tilted surfaces of a building will receive a portion of the total ground-
reflected flux.
Solar Angles. Finally, in order to calculate solar flux quantities, a variety of angles describing Sun Earth
geometry and the direction of the beam solar flux must be defined. Each is listed separately below. The
notation used duplicates that found in the ASHRAE Handbook of Fundamentals.
Declination (δ): The angular position of the Sun relative to the plane of the Earth's equator. See values in
Table 1.
Hour Angle (H): An angular expression of the apparent solar time , measured from solar noon.
H = 15 ( 12 AST )
where:
H
=
Hour angle, degrees.
AST
=
Hour of day, apparent solar time. AST=0 for midnight,
AST=12 for solar noon, AST=23 for 11pm.
Solar Altitude Angle (β): The angle between the beam solar flux and a horizontal surface.
sin(β) = cos(L)cos(δ)cos(H) + sin(L)sin(δ)
where:
β
=
Solar altitude angle, degrees.
L
=
Site latitude, degrees.
Solar Azimuth Angle (ϕ): The Sun's angular distance from due south. Positive angles are measured counter
clockwise from south. Thus when the Sun is east of due south, the solar azimuth angle is positive; when west
of due south the azimuth is negative.
cos(ϕ) = [ sin(β)sin(L) - sin(δ) ] / cos(β)cos(L)
Surface Azimuth Angle (ψ): The angle between a line perpendicular to a vertical wall and due south. As with
solar azimuths, positive angles are measured counter clockwise from south. Thus, angles for the principal
exposures are as follows: north : ψ = 180, east : ψ = 90, south : ψ = 0, west : ψ = 90.
Surface Solar Azimuth Angle (γ): The Sun's angular distance from a line perpendicular to a vertical wall.
γ = ϕ ψ
Angle of Incidence (θ) For Beam Solar: The angle between the direction of the beam solar flux and a line
perpendicular to a building surface. The general equation for the angle of incidence is:
cos(θ) = cos(β)cos(γ)sin(Σ) + sin(β)cos(Σ)
Page 9 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
where:
Σ
=
Tilt angle for building surface, degrees. Measured from
horizontal. For horizontal surfaces Σ = 0; for
vertical surfaces Σ = 90.
For vertical surfaces this equation reduces to:
cos(θ) = cos(β)cos(γ)
For horizontal surfaces the equation reduces to:
cos(θ) = sin(β)
B. Calculation of Clear Sky Solar Flux Profiles
The procedure used to compute hourly clear sky solar flux profiles is taken from the 1997 ASHRAE Handbook
of Fundamentals [1]. The goal of the procedure is to determine hourly values of the beam, diffuse and
reflected components of solar flux on each of the building exposures for clear sky conditions. Fluxes are
computed for the twenty first day of each month according to ASHRAE procedures. The resulting flux values
represent estimates for typical clear sky conditions. Procedures for computing each component of the solar
flux are described below.
Beam Solar Flux. First compute the beam solar flux on a surface perpendicular to the direction of the flux:
Ibn = ACN [ A / exp (B/sin(β)) ]
where:
Ibn
=
Beam solar flux on surface perpendicular to direction of flux,
BTU/hr sqft or W/sqm.
A
=
Apparent solar irradiation at air mass of zero, BTU/hr sqft or
W/sqm. See values in Tables 1 and 2.
B
=
Atmospheric extinction coefficient, dimensionless. See
values in Table 1 and 2.
ACN
=
Atmospheric clearness number, dimensionless. See
discussion below.
The procedure for computing Ibn was developed for a set of monthly reference atmospheric conditions. These
reference conditions define the quantities of ozone, moisture and dust in the atmosphere for a site at sea level.
For sites with unusually dry, wet, dusty, or clear atmospheres or sites at high elevations, the atmospheric
clearness number (ACN) is used to increase or decrease Ibn values. For sites at which conditions are close to
the reference conditions, a clearness number of 1.00 is used. Clearness numbers can be determined for U.S.
and Canadian sites from Figure 7, pg 27.12 of the 1993 ASHRAE Handbook of Fundamentals.
Table 1 Clear Sky Solar Flux Parameters, Northern Hemisphere
Month
&
Day
Ion
δ
A
Day
Number
(BTU/h-sqft)
(degrees)
(BTU/h-sqft)
B
C
Jan 21
21
448.8
-20.0
390
0.142
0.058
Feb 21
52
444.2
–10.8
385
0.144
0.060
Mar 21
80
437.7
0.0
376
0.156
0.071
Apr 21
111
429.9
11.6
360
0.180
0.097
May 21
141
423.6
20.0
350
0.196
0.121
Jun 21
172
420.2
23.45
345
0.205
0.134
Jul 21
202
420.3
20.6
344
0.207
0.136
Aug 21
233
424.1
12.3
351
0.201
0.122
Page 10 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
Sep 21
264
430.7
0.0
365
0.177
0.092
Oct 21
294
437.3
-10.5
378
0.160
0.073
Nov 21
325
445.3
-19.8
387
0.149
0.063
Dec 21
355
449.1
-23.45
391
0.142
0.057
Data from Table 8, pg 29.14, 1997 ASHRAE Handbook of Fundamentals [1]
Table 2 Clear Sky Solar Flux Parameters, Southern Hemisphere
Month
&
Day
Ion
δ
A
Day
Number
(BTU/h-sqft)
(degrees)
(BTU/h-sqft)
B
C
Jan 21
21
448.8
-20.0
390
0.207
0.136
Feb 21
52
444.2
–10.8
385
0.201
0.122
Mar 21
80
437.7
0.0
376
0.177
0.092
Apr 21
111
429.9
11.6
360
0.160
0.073
May 21
141
423.6
20.0
350
0.149
0.063
Jun 21
172
420.2
23.45
345
0.142
0.057
Jul 21
202
420.3
20.6
344
0.142
0.058
Aug 21
233
424.1
12.3
351
0.144
0.060
Sep 21
264
430.7
0.0
365
0.156
0.071
Oct 21
294
437.3
-10.5
378
0.180
0.097
Nov 21
325
445.3
-19.8
387
0.196
0.121
Dec 21
355
449.1
-23.45
391
0.205
0.134
Data from Table A-5, pg 24, reference [2].
Next, the beam solar flux on a wall or roof exposure is computed using the equation:
Ib = Ibn cos(θ)
where:
Ib
=
Beam solar flux on a surface, BTU/hr sqft or W/sqm.
θ
=
Angle of incidence for direct solar flux, degrees.
Diffuse Solar Flux. Before computing the diffuse solar flux on an exposure, the factor "Y" must be calculated.
"Y" is the ratio of diffuse solar flux on a vertical surface to the diffuse flux on a horizontal surface. This factor
must be used because for clear sky conditions the intensity of the diffuse solar flux is not uniformly distributed
over the dome of the sky. The diffuse flux from the area surrounding the Sun is most intense, while the flux
originating from other portions of the sky is less intense. Hence, whether a surface is exposed to the Sun to
some extent affects the amount of diffuse solar it receives. "Y" is computed using the following equations:
For cos(θ) greater than 0.2:
Y = 0.55 + 0.437cos(θ) + 0.313cos2(θ)
For cos(θ) less than or equal to 0.2:
Y = 0.45
where:
Y
=
Ratio of diffuse flux on vertical surface to diffuse flux on
horizontal surface, dimensionless.
θ
=
Angle of incidence for beam solar flux, degrees.
Page 11 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
27.5 Calculating Design Solar Heat Gain Profiles
27.0 Weather Calculations ››
Calculating Design Solar Heat Gain Profiles
27.0 Weather Calculations ›› 27.5 Calculating Design Solar Heat Gain Profiles ››
Next, the diffuse solar flux is calculated. For a surface of any orientation the general equation is:
Id = C Y Ibn
For horizontal surfaces the following equation is used:
Idh = C Ibn
where:
Id
=
Diffuse solar flux on a tilted surface, BTU/hr sqft or W/sqm.
Idh
=
Diffuse solar flux on a horizontal surface, BTU/hr sqft or
W/sqm.
C
=
Sky diffuse factor, dimensionless. See Tables 1 and 2 for
values.
Reflected Solar Flux. Solar energy which strikes a tilted building exposure after being reflected by the
surrounding ground is determined with the following equation:
Ir = ρg Ibn(C + sin(β))(1 - cos(Σ)) / 2
For vertical surfaces this reduces to:
Irv = ρg Ibn(C + sin(β)) / 2
For horizontal surfaces there is no reflected solar flux:
Irh = 0
where:
Ir
=
Ground reflected solar flux on a surface of any orientation,
BTU/hr sqft or W/sqm.
Irv
=
Ground-reflected solar flux on a vertical surface, BTU/hr/sqft
or W/sqm.
Irh
=
Ground-reflected solar flux on a horizontal surface,
BTU/hr/sqft or W/sqm.
ρg
=
Ground reflectance, dimensionless.
C. References
1. 1997 ASHRAE Handbook of Fundamentals, American Society of Heating, Refrigerating and Air
Conditioning Engineers, Inc., 1997.
2. Energy Calculations 1: Procedure for Determining Heating and Cooling Loads for Computerizing Energy
Calculations, Algorithms for Building Heat Transfer Subroutines, American Society of Heating, Refrigerating
and Air Conditioning Engineers, Inc., 1976.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains calculation of design day solar heat gain profiles.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 12 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
Calculating Design Solar Heat Gain Profiles
This help topic explains how solar heat gain profiles are calculated for design cooling studies. Clear sky
conditions are assumed so the maximum effects of solar heat can be considered. For each month, hourly
profiles of solar flux are used to derive solar heat gain data using procedures outlined in the ASHRAE
Handbook of Fundamentals. These procedures are described below
A. Calculation of Clear Sky Solar Heat Gain Profiles
Solar heat gain (SHG) profiles for design cooling days are computed using the clear sky solar flux profiles and
an ASHRAE-recommended procedure. As discussed previously, the solar heat gain is the amount of solar
heat reaching the interior of the building after passing through the window. Standard ASHRAE procedures
require that reference SHGs be calculated first using the optical properties of "reference glass". Reference
glass is single-pane, 1/8" double strength sheet glass (α=.06, ρ=08, τ=.86). Then, when computing solar loads
for a specific window type, the reference SHGs are multiplied by a "shading coefficient" factor to adjust for the
optical properties of the specific window type. The help topic dealing with solar load calculations describes the
use of shading coefficients in greater detail.
Reference solar heat gains are computed separately for the following four components:
1. Beam solar, portion absorbed by glass (ASHGFb).
2. Beam solar, portion transmitted through window (TSHGFb).
3. Diffuse plus ground-reflected solar, portion absorbed by glass (ASHGFd).
4. Diffuse plus ground-reflected solar, portion transmitted through window (TSHGFd).
Separate beam and diffuse calculations are required because transmission of solar heat through glass
depends on the angle at which solar radiation strikes the glass. The beam solar flux strikes window glass at a
specific angle, while diffuse and ground-reflected solar is multi-directional. Separate calculations for the
absorbed and transmitted components of the SHG are required due to the transfer function procedure for
calculating loads from SHG values.
Reference solar heat gain calculations are based on equations from page 29.37 of the 1997 ASHRAE
Handbook of Fundamentals [1] and are as follows:
TSHGFb = Ib [ Σ tjcosj(θ) ] for j=0 to 5
ASHGFb = Ib [Σ ajcosj(θ) ] for j=0 to 5
TSHGFd = 2(Id)[Σ ( tj / (j+2) ) ] for j=0 to 5
ASHGFd = 2(Id)[Σ ( aj / (j+2) ) ] for j=0 to 5
where:
Ib
=
Beam solar flux on window surface, BTU/hr/sqft or W/sqm.
Id
=
Diffuse plus ground-reflected solar flux striking window
surface, BTU/hr/sqft or W/sqm.
tj
=
Transmission coefficients for reference glass,
dimensionless. See Table 3.
aj
=
Absorption coefficients for reference glass, dimensionless.
See Table 3.
θ
=
Angle of incidence for beam solar flux striking window
surface, degrees.
Table 3 Transmission and Absorption Coefficients for Reference Glass
j
aj
tj
0
0.01154
-0.00885
1
0.77674
2.71235
2
-3.94657
-0.62062
3
8.57881
-7.07329
Page 13 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm
4
-8.38135
9.75995
5
3.01188
-3.89922
B. Reference
1. 1997 ASHRAE Handbook of Fundamentals, American Society of Heating, Refrigerating and Air
Conditioning Engineers, Inc., 1997.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 14 of 14
27.0 Weather Calculations
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh18E.htm