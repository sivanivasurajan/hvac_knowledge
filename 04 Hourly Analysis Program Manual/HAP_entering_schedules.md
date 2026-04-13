17.0 Entering Schedules
Overview for Schedules and the Schedule Form
17.0 Entering Schedules ››
This chapter explains schedule input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Schedules and the Schedule Form
About Schedules. Schedules define the hourly and daily behavior of various characteristics of a building and
its HVAC equipment. HAP deals with three distinct kinds of schedules, all defined using the same procedures
on the Schedule form:
1. Fractional Schedules define hourly and daily variation in percentages. Fractional schedules are most often
used to describe the variation of internal heat gains. For example, percentages in a lighting schedule define
the fraction of lights in use each hour of the day. Fractional schedules can also be used to define the hourly
control of outdoor ventilation air in an HVAC system or the use of hot water in a service hot water system.
2. Fan/Thermostat Schedules define the hours in each HVAC equipment operating period. Hours of a day
are designated as "occupied" or "unoccupied." During occupied hours, the occupied thermostat setpoints
are used and systems generally operate to ventilate and condition the building. During unoccupied hours,
the unoccupied thermostat setpoints are used and systems general operate in an on-demand mode to
condition the building.
3. Utility Rate Schedules define on-peak and off-peak pricing periods for electricity.
A schedule consists of up to 8 profiles. Each profile contains data for one 24-hour period. Profiles are
assigned to the different days of the week and months of the year. For most system design applications, only
one profile for the design day is needed. For special applications, you may need to specify separate profiles to
model behavior in summer and winter months. For energy analyses, profiles for different days of the week or
months of the year can be defined.
Each project you create can contain many different schedules. This allows the unique hourly variation of each
heat flow component, HVAC equipment control, or utility rate to be modeled with a separate schedule.
Schedules are entered and stored in the project database. They are later linked to spaces, air systems or
utility rates before being used in program calculations.
Page 1 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
The Schedule Form, shown above, is used to define data for one schedule. The Schedule Form contains
three key components:
1. The Title Bar appears across the top of the form. It lists the name of the schedule whose data is displayed
in the form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains multiple categories of schedule information
represented as separate tabs in a notebook. To move from one tab to another, simply click on the desired
tab. There are three tabs for the three categories of schedule data:
a. Schedule Type defines the name of the schedule and specifies what kind of schedule it is: fractional,
fan/thermostat or utility rate.
b. Profiles contains information about individual 24-hour profiles which comprise the schedule.
c. Assignments defines which profiles are used for different months of the year.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the weather data and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the weather data.
c. Press Help to display this overview topic.
Schedule Features. Finally, HAP provides useful features for:
Creating a new schedule.
Editing an existing schedule.
Printing schedule.
Deleting schedules.
Copying schedules.
Duplicating schedules.
Page 2 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
17.1 Inputs
17.0 Entering Schedules ››
Schedule Type Tab / Schedule Form
17.0 Entering Schedules ›› 17.1 Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data in the Schedule Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Schedule Type Tab / Schedule Form
The Schedule Type Tab contains the name of the schedule and defines the type of schedule data being
entered:
1. Schedule Name is a reference name used to identify the schedule. It appears on selection lists when
linking schedules to spaces, systems or utility rates. It also appears on reports listing schedule, space,
system or utility rate data. The schedule name should be descriptive so you can recognize what it
represents when it appears later on selection lists and reports.
2. Schedule Type defines the kind of schedule being entered. HAP deals with three distinct kinds of
schedules:
a. Fractional schedules define hourly and daily behavior in percentages. Fractional schedules are most
often used to describe the hourly variation of internal heat gains. For example, percentages in a lighting
schedule define the fraction of lights in use each hour of the day. Fractional schedules can also be used
to define the hourly control of outdoor ventilation air in an HVAC system or the use of hot water in a
service water heating (SHW) system.
Page 3 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
Profiles Tab / Schedule Form
17.0 Entering Schedules ›› 17.1 Inputs ››
The Fractional option should be selected when defining a schedule for overhead lighting, task lighting,
electric equipment, occupant heat gains, miscellaneous sensible or latent loads, when using the special
"scheduled" control option for outdoor ventilation air, and when defining hot water usage schedules.
b. Fan/Thermostat schedules define the hours in each HVAC equipment operating period. Hours of a day
are designated as "occupied" or "unoccupied." During occupied hours, the occupied thermostat setpoints
are used and systems generally operate to ventilate and condition the building. During unoccupied hours,
the unoccupied thermostat setpoints are used and systems general operate in an on-demand mode to
condition the building.
The Fan/Thermostat option should be selected when defining the "thermostat schedule" for an air
system.
c. Utility Rate schedules define on-peak and off-peak pricing periods for electricity. This option should be
used when scheduling time-of-day periods for an electric rate structure.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Profiles Tab / Schedule Form
About Profiles. A schedule consists of up to 8 profiles. Each profile contains data for one 24-hour period.
Separate profiles represent behavior on different days or at different times of year. On the Assignments tab ,
profiles will be linked to specific days and months of the year.
Page 4 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
The Profiles Tab provides features for defining all the profiles associated with the current schedule. The tab
consists of two panels:
1. The Left-Hand Panel is the working area. It contains the profile name and the profile currently being edited.
In the figure above, data for profile 1 is being edited. This profile has been named "Design Day". It is part of
a fractional schedule indicated by the fact that profile values are defined as percentages.
2. The Right-Hand Panel is a display area which contains graphical images for all eight profiles which are part
of this schedule. This display is useful for seeing at a glance the contents of all profiles in the schedule.
A four step procedure is used to define each profile in the schedule:
a. Open the profile you wish to edit.
b. Specify the profile name.
c. Define the hourly values for the profile.
d. Close the profile.
The Profiles Tab provides multiple ways to carry out each step in the process. A more detailed discussion of
each step in this process is provided below.
1. Open the Profile. A profile must be opened to make it active and place it in the left-hand panel of the tab for
editing. There are three ways to open a profile:
a. Click on the restore button in the upper right-hand corner of the desired profile. This expands the profile
and places it in the left-hand panel of the tab.
b. After clicking on the restore button to activate a profile, you can click on the maximize button in the upper
right-hand corner of the profile to enlarge it further. Some users find it easier to work with the profile
when it has been maximized.
c. Choose the desired profile from the drop-down list at the top of the left-hand panel. This drop-down list
contains the names of all eight profiles in your schedule.
2. Specify the Profile Name. Click on the text in the profile name box at the top of the left hand panel and
then define your name. The profile name should describe the nature or use of the profile.
3. Define Profile Values. HAP provides a variety of ways to change hourly profile values using the mouse, the
arrow keys and manual data entry. All of these procedures involve two basic steps: first you highlight the
hours in the profile you want to change, then you change the values for these hours. There are five ways to
choose the hours to be changed.
a. To choose a single hour, use the mouse to right click on the desired bar in the profile graph.
b. To choose multiple hours, hold the Shift key down and right click on the first and last bars in the desired
group of hours.
c. To choose multiple hours, hold the Shift key down, right click on the first bar in the group, and then use
the right or left arrow key to highlight successive hours.
d. To choose a single hour, enter the hour number in the left-hand text box above the profile graph. The bar
for this hour will be highlighted.
e. To choose multiple hours, enter the range of hours in the left-hand text box above the profile graph. For
example "8-12" will select hours 0800 through 1200.
Once the desired hours in the profile are highlighted, the value for the hours can be changed in three
different ways. Note that when you are changing values for a group of hours, you must continue to hold the
Shift key down while adjusting the height of the bars.
f. Press and hold the left-hand mouse button and use the mouse to drag the profiles bars up or down. As
you drag the bars, the bar value will be displayed above the profile graph in the right-hand text box.
When finished adjusting the bar height, release the mouse button.
g. Use the up or down arrow keys to move the profile bars up or down. As you move the bars, the bar value
will be displayed above the profile graph in the left-hand text box. For fractional schedules, the profile
value changes in 5% increments each time you press the arrow key. For Fan/Thermostat and Utility Rate
schedules, the value changes from one profile level to the next each time you press an arrow key.
Page 5 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
Assignments Tab / Schedule Form
17.0 Entering Schedules ›› 17.1 Inputs ››
h. Specify the desired profile value in the right-hand text box that appears above the profile graph. Note that
when you are manually defining schedule data using the two text boxes that appear above the profile
graph, you can move back and forth between the hour box and the value box by using the right and left
arrow keys.
4. Close the Profile. When finished entering data for a profile, press the minimize button in the upper right-
hand corner of the profile to shrink the profile and return it to the right-hand panel of the Profiles tab. Once
you have closed the profile, you’re ready to edit another profile.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Assignments Tab / Schedule Form
About Assignments. Individual profiles in a schedule can be assigned to different months of the year or days
of the week. This permits different patterns of internal loads, for example, to be modeled at the different times
of year or on different days of the week. The Assignments Tab on the Schedule form is used for this purpose.
The Assignments Tab is divided into two sections:
1. The Left-Hand Panel contains the assignments table. In this table, each row contains assignments for a
different day type. Each column contains assignments for a different month. To make assignments, click on
the desired cells in the table and either enter the profile number or click on the desired profile in the right-
hand panel. In the figure above, for example, profile #1 ("School\_In\_Session") has been assigned to
Monday thru Friday for all 12 months.
Assignments for the Design Day row of the table will be used in cooling design calculations. Assignments
for the other eight rows in the table are used for energy simulation calculations.
When operating in System Design mode, only the Design Day row in the table is enabled as shown below.
Page 6 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
17.2 Common Tasks
17.0 Entering Schedules ››
Creating a New Schedule
17.0 Entering Schedules ›› 17.2 Common Tasks ››
2. The Right-Hand Panel is a display area which contains graphical images for all eight profiles which
comprise the schedule. This is useful reference information when assigning schedule numbers to different
days or months in the assignment table.
Helpful Hints: The Assignments tab provides features to make assigning profiles fast and easy:
a. You can select multiple cells in the table by clicking on the first cell, holding the shift key down and clicking
on the last cell in a group. In this way multiple cells in a row, a column or a block of cells can be highlighted.
b. Profiles can be designated by pressing the number key for the profile number, or by clicking on the profile
image in the right-hand panel. All cells currently highlighted will be assigned to the profile you select.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with schedule input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Schedule
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm
Editing an Existing Schedule
17.0 Entering Schedules ›› 17.2 Common Tasks ››
Printing Schedule Inputs
17.0 Entering Schedules ›› 17.2 Common Tasks ››
Deleting Schedules
17.0 Entering Schedules ›› 17.2 Common Tasks ››
Copying Schedules
17.0 Entering Schedules ›› 17.2 Common Tasks ››
Duplicating a Schedule
17.0 Entering Schedules ›› 17.2 Common Tasks ››
Editing an Existing Schedule
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Schedule Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Schedules
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying Schedules
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Schedule
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 8
17.0 Entering Schedules
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhD1DD.htm