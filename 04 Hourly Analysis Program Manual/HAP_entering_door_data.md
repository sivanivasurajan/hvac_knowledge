21.0 Entering Door Data
Overview for Doors and the Door Form
21.0 Entering Door Data ››
This chapter explains input data for door assemblies.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Doors and the Door Form
About Doors. Door data defines the size and heat transmission characteristics of one door. HAP load
calculations consider conduction heat flow through the wood or metal portion of the door, as well as
conduction heat flow and solar heat gains through the glass portion of the door.
Typically, one door assembly represents a single door. If multiple doors of this type exist on an exposure, such
as a pair of swinging entry doors, a bank of entry doors or a series of overhead doors, the quantity of doors on
the exposure can be specified when entering space data. However, if you wish, data for one door assembly
can also be used to define the total area and heat transmission characteristics for a group of doors.
The Door Form is used to define door size and heat transmission characteristics. This form contains the
following seven input items:
Name
Gross Area
Door U-value
Glass Area
Glass U-value
Page 1 of 5
21.0 Entering Door Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF672.htm
21.1 Inputs
21.0 Entering Door Data ››
Door Name
21.0 Entering Door Data ›› 21.1 Inputs ››
Door Gross Area
21.0 Entering Door Data ›› 21.1 Inputs ››
Glass Shade Coefficient
Glass Shaded All Day
The form also contains three command buttons in the lower right hand corner:
Press OK to save the door inputs and return to the HAP main program window.
Press Cancel to return to the HAP main program window without saving changes to the door. If you press
Cancel while creating a new door, a new door will not be added to your door library.
Press Help to display an overview discussion of doors and the door form.
Door Features. Finally, HAP provides useful features for:
Creating a new door.
Editing an existing door.
Printing door data
Deleting doors.
Copying a door.
Duplicating a door.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data in the Door Assembly Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Name
The Door Name is a reference name for the door assembly. The door name will appear on selection lists when
adding a door to a space. It also appears on reports listing door inputs. The name should be descriptive so
you can easily recognize what the data represents later when the name appears on selection lists.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Gross Area
Gross Area is the total exterior surface area of the door, including both glass and wood or metal sections of
the door. The gross area is used together with the door glass area to calculate the net door area. Heat flow
through the wood or metal portion of the door using the net door area and the door U-value.
When defining door data, if the area is known, enter it directly. If only the height and width are known, use the
on-line calculator to calculate the door area and automatically insert it into HAP.
Page 2 of 5
21.0 Entering Door Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF672.htm
Door U-Value
21.0 Entering Door Data ›› 21.1 Inputs ››
Door Glass Area
21.0 Entering Door Data ›› 21.1 Inputs ››
Door Glass U-Value
21.0 Entering Door Data ›› 21.1 Inputs ››
Door Glass Shade Coefficient
21.0 Entering Door Data ›› 21.1 Inputs ››
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door U-Value
The Door U-value defines the heat transmission characteristics of the wood or metal portion of the door. It is
used in load calculations to determine the conduction heat gain through the wood or metal portion of the door.
The door U-value should include consideration of surface convection coefficients as well as thermal resistance
of each wood, metal or insulation layer in this portion of the door.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Glass Area
Glass Area is the exterior surface area of the glass portion of the door. If the door contains glass, HAP will
calculate both conduction and solar loads for this portion of the door using the glass U-value and glass shade
coefficient you define.
If the door does not contain any glass, specify the area as zero.
If the door is 100% glass, specify a glass area that is equal to the door gross area.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Glass U-Value
The Glass U-value defines the overall U-value for glass used in the door. It is used to calculate the conduction
and convection portion of the load for the door glass. The U-value should include consideration of surface
convection coefficients as well as the thermal resistance of glass layers. If internal shades are used with the
door glass, the U-value should also include the thermal resistance of the shading device.
Note: If the door does not contain any glass area, this item is not used in calculations and its value is therefore
not relevant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Glass Shade Coefficient
The Glass Shade Coefficient defines how solar energy is transmitted through the door glass with respect to
transmission through a single pane of reference glass. This factor accounts for the difference between the
optical properties of the door glass and any interior shades, and the properties of reference glass. Shade
coefficient values are often provided in manufacturer’s literature (such as National Fenestration Rating Council
ratings) and in reference sources such as the ASHRAE Handbook of Fundamentals.
Page 3 of 5
21.0 Entering Door Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF672.htm
Door Glass Shaded All Day
21.0 Entering Door Data ›› 21.1 Inputs ››
21.2 Common Tasks
21.0 Entering Door Data ››
Creating a New Door
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Editing an Existing Door
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Printing Door Inputs
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Note: If the door does not contain any glass area, this item is not used in calculations and its value is therefore
not relevant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Door Glass Shaded All Day
The Glass Shaded All Day input is used to model external shading of the door glass. External shading of the
door glass is analyzed on a simple basis. If the entire door glass surface is externally shaded at all times,
place a check mark in the box opposite this item. The program will then assume only diffuse and ground
reflected solar radiation passes through the door glass. If the door glass is not externally shaded, leave the
box unchecked. In this case the program will analyze the transmission of beam, diffuse and ground reflected
solar energy through the door glass. When the door glass will be shaded at some times, but not others, you
must make a judgement whether it is more accurate to analyze full shading or no shading in the program.
Note: If the door does not contain any glass area, this item is not used in calculations and its value is therefore
not relevant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with door input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Door
Please see Creating a New Item
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Door
Please see Editing an Existing Item
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 4 of 5
21.0 Entering Door Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF672.htm
Deleting Door Inputs
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Copying a Door
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Duplicating a Door
21.0 Entering Door Data ›› 21.2 Common Tasks ››
Printing Door Inputs
Please see Generating Input Data Reports
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Door Inputs
Please see Deleting Items
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying a Door
Please see Duplicating an Existing Item
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Door
Please see Duplicating an Existing Item
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 5 of 5
21.0 Entering Door Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF672.htm