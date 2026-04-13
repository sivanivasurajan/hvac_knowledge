20.0 Entering Window Data
Overview for Windows and the Window Form
20.0 Entering Window Data ››
This chapter explains input data for window assemblies.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Windows and the Window Form
About Windows. In HAP the term "window" refers to vertical, sloped and horizontal glass surfaces of the
building separating ambient air from indoor air. A window can be defined by its physical characteristics such as
number of glazings, types and optical properties of glass used, frame type, internal shading properties and
window dimensions. Together these properties are used to calculate the overall U-value and shade coefficient
for the window. As an alternative, the overall U-value and shade coefficient can be directly defined using
manufacturer’s ratings. U-value defines how heat is conducted through the window assembly. Shade
coefficient defines how solar heat is transmitted through the window assembly.
Each project you create can contain many different window constructions. This allows each different window
assembly in your building to be modeled. Windows are first entered and stored in the project using the Window
form. They are then linked to specific window exposures while entering space data.
The Window Form, shown above, is used to define data for one window assembly. The Window Form
contains three key components:
Page 1 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
Common Window Applications
20.0 Entering Window Data ››
1. The Title Bar appears across the top of the form. It lists the name of the window whose data is displayed in
the form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains information describing the window’s assembly.
The following inputs are used to describe a window assembly:
Name
Detailed Input
Height and Width
Frame Type
Internal Shading Type
Overall U-Value
Overall Shade Coefficient
Glass Details
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the window data and return to the main program window.
b. Press Cancel to return to the main program window without saving changes to the window. If you press
cancel when creating a new window, no data is saved and a new window is not added to your project.
c. Press Help to display this overview topic.
Window Features. HAP provides useful features for:
Creating a new window.
Editing an existing window.
Printing windows.
Deleting windows.
Copying windows.
Duplicating a window.
Application Information. Click here for further information about Common Window Applications .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Window Applications
There are three common situations for defining a window assembly: defining a simple window, defining a
detailed window and defining a unit window. The Window Form is used in all three cases, but its features are
used in slightly different ways. The procedures for these applications are described below.
1. Defining a Simple Window. Use this procedure when the overall U-value and shade coefficient are known
from manufacturer’s ratings. In this case you will directly define the window performance rather than letting
HAP estimate window performance:
a. Enter a reference name for the window.
b. Make sure the Detailed Input check box is unmarked. When this box is unchecked, all input items on the
form will be disabled except name, height, width, U-value and shade coefficient.
c. Specify the height and width dimensions of the window.
Page 2 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
20.1 Inputs
20.0 Entering Window Data ››
Window Name
20.0 Entering Window Data ›› 20.1 Inputs ››
d. Using manufacturer’s ratings, specify the overall U-value and shade coefficient for the window.
e. Press the OK button to exit from the form and save the window data.
2. Defining a Detailed Window. Use this procedure when you know the general construction characteristics
of the window, but do not have manufacturer’s data concerning U-value and shade coefficient. In this case,
you will "build" the window assembly by specifying its characteristics. HAP will estimate the U-value and
shade coefficient from the window characteristics you supply.
a. Enter a reference name for the window.
b. Make sure the Detailed Input check box is marked. When this box is checked, all items on the form will
be enabled, except Overall U-Value and Overall Shade Coefficient.
c. Specify the window height and width , the frame type , the type of internal shades and the characteristics
of the glazings and the gaps between glazings. Based on this data, HAP will estimate the overall U-value
and overall shade coefficient for the window assembly.
d. Press the OK button to save the data and return to the main program window.
3. Defining a Unit Window. Use this procedure when describing a unit area of glass rather than an actual
window. This approach is sometimes used for preliminary block load estimates in which window dimensions
are not yet known, but rough estimates of total glazing area are known. This approach is also used for
situations in which the building envelope contains a large number of windows having different sizes and a
user has determined the effort to define each window separately is not justified. In both cases, a window
having a unit area (e.g., 1x1= 1 sqft, 2x2 = 4 sqft, etc…) is defined. Later when entering space data, a
window quantity is specified to account for the total surface area on an exposure. It should be noted that the
unit window approach yields less accurate window performance estimates than the detailed and simple
approaches. To define a unit window:
a. Enter a reference name for the window.
b. Make sure the Detailed Input check box is unmarked. Unit windows must not be defined using the
detailed input items because this causes HAP to estimate window performance, and these estimates
account for the performance effects of the window frame. If you are modeling unit areas of glass, it is not
appropriate to account for frame effects for each unit of area.
c. Specify window height and width for the unit area of glass being modeled. Example: a height of 1 ft and a
width of 1 ft.
d. Specify the U-value and shade coefficient for the unit area of glass. Typically center of glass performance
values tabulated in handbooks such as the ASHRAE Handbook of Fundamentals are used.
e. Press the OK button to save the window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data in the Window Assembly Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Name
Page 3 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
Detailed Input
20.0 Entering Window Data ›› 20.1 Inputs ››
Window Height and Width
20.0 Entering Window Data ›› 20.1 Inputs ››
Window Frame Type
20.0 Entering Window Data ›› 20.1 Inputs ››
This is a reference name for the window. It will appear on selection lists when linking a window type to
exposures in a space and will also appear in reports. The name should be descriptive so you can recognize
what the data represents later when it appears on selection lists.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Detailed Input
This item controls how the window assembly is defined.
1. Detailed Input. When this check box is marked, all items on the window form except for U-value and shade
coefficient will be enabled. When defining a window in "detailed" mode, you describe its physical
components such as the frame, internal shades, height and width, and the properties of its glazings and
gaps between glazings. HAP then estimates the overall U-value and shade coefficient from your
specifications. The detailed input approach is typically used when you know the characteristics of the
window, but do not have manufacturer’s ratings for U-value and shade coefficient.
2. Simple Input. When the "Detailed Input" check box is not marked, all items on the window form are
disabled except for height, width, U-value and shade coefficient. This simple input approach is typically
used when you have manufacturer’s ratings for U-value and shade coefficient and can specify them directly
rather than letting HAP estimate these performance values. The simple input approach is also used when
defining a unit area of glass.
For further information on how to use the "Detailed Inputs" item for common applications, please refer to the
Common Window Applications help topic.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Height and Width
Specify the height and width for the full window aperture.
When defining a window using the "detailed input" option, HAP will make assumptions about the portion of the
window aperture occupied by glass and frame material, depending on the frame type selected. These
assumptions influence the overall U-value and shade coefficient that HAP estimates for the window.
When defining a window without using the "detailed input" option, the full dimensions of the window aperture
must still be defined since manufacturer’s ratings for U-value and shade coefficient refer to performance of the
complete window unit, including the frame material.
In all cases, the height and width define the surface area for a single window of this type. Height and width
values are also used in external shading calculations for the window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Frame Type
Page 4 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
Internal Shade Type
20.0 Entering Window Data ›› 20.1 Inputs ››
Window Overall U-Value
20.0 Entering Window Data ›› 20.1 Inputs ››
Window Overall Shade Coefficient
20.0 Entering Window Data ›› 20.1 Inputs ››
Frame type defines the properties of the window frame material. Choose the desired type from the drop-down
list. Four frame types are offered:
a. Aluminum without thermal breaks.
b. Aluminum with thermal breaks.
c. Wood
d. Vinyl
Frame properties influence heat conduction through the window. Ultimately the choice of a frame type affects
the calculation of the overall window U-value, overall shade coefficient, and the transmission and solar loads
for the window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Internal Shade Type
Internal shade type describes the type of drapes, shades or venetian blinds used with the window. Choose the
desired type from the drop-down list. If interior shades are not used with a window, choose "None" as the
shade type.
The presence of interior shades and the characteristics of the shading device affects conduction and
convection heat flow through the window assembly, as well as the transmission of solar radiation into the
building. Shade properties therefore influence the calculation of the overall window U-value, overall shade
coefficient and the transmission and solar loads for the window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Overall U-Value
Overall U-Value defines heat transmission for the entire window assembly, including both glass and framing
portions of the window. U-value is used in window transmission load calculations.
When using the "detailed input" approach to defining a window, HAP will calculate the overall U-value using
ASHRAE and NFRC (National Fenestration Rating Council) estimation procedures. These procedures account
for variation of heat transmission through the center of glass, edge region of the glass and the window frame,
plus the effects of any interior shading devices.
When using the simple approach to defining a window, an overall U-value from manufacturer’s ratings must be
entered by the user.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Window Overall Shade Coefficient
Overall Shade Coefficient describes how solar energy is transmitted through the window assembly. In simple
terms, the shade coefficient is a ratio of solar transmission for the window divided by solar transmission
through a single pane of reference glass. It therefore accounts for the difference between the optical
properties of your specific window design, framing and interior shades versus the properties of reference
Page 5 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
Glass Details Table
20.0 Entering Window Data ›› 20.1 Inputs ››
glass. Note that "overall" refers to the fact the shade coefficient represents the overall performance of the
window assembly including the effects of center of glass, edge of glass, frame and internal shading.
Some window manufacturers report solar performance in terms of Solar Heat Gain Coefficient (SHGC) at
normal incidence. When given this window performance value you can convert it to Solar Heat Gain
Coefficient using the equation:
Shade Coefficient = Solar Heat Gain Coefficient / 0.87
When using the "detailed input" approach to defining a window, HAP will calculate the overall shade coefficient
using ASHRAE and NFRC (National Fenestration Rating Council) estimation procedures. These procedures
consider solar energy transmission through the glass portion of the window, solar heat absorbed and
transmitted through the window frame, the effects of heat absorbed by glazings in the window assembly and
the effects of internal shading devices.
When using the simple approach to defining a window, an overall shade coefficient from manufacturer’s
ratings must be entered by the user.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Glass Details Table
The Glass Details table defines the characteristics of glazings in a window assembly. It is only enabled when
using the "detailed input" approach to defining a window.
In this table, each row contains data for a separate glazing in the window. Each column defines a different
property of the glazing. A separate input item beneath the table is used to describe the gap between glazings.
Input items in this section of the window form are as follows:
1. Glass Type. For each glazing in the window assembly, choose a glass type from the drop-down list. The list
contains many common types of clear, tinted, reflective and low-e glass. When a glass type is selected, its
optical properties will appear to the right of this input.
This input item is also used to indirectly specify the number of glazings in the window assembly. For a
single-glazed window, choose a glass type for the Outer Pane and "none" for remaining glazings. For a
double-glazed window, choose glass types for the Outer Pane and Glazing #2, and "none" for Glazing #3.
For a triple-glazed window , choose glass types for all three glazings.
2. Transmissivity is the fraction of solar energy transmitted through a single glazing of this glass type. This is
a display-only item; it cannot be changed.
3. Reflectivity is the fraction of solar energy reflected away from the building by a single glazing of this glass
type. This is a display-only item; it cannot be changed.
4. Absorptivity is the fraction of solar energy absorbed by a single glazing of this glass type. This is a display-
only item; it cannot be changed.
Page 6 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
20.2 Common Tasks
20.0 Entering Window Data ››
Creating a New Window
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Editing an Existing Window
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Printing Window Inputs
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Deleting Windows
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Copying Windows
5. Gap Type defines the width of the gap between glazings in a multi-glazing window assembly, and also the
gas which is used to fill the gap. Choose the desired gap type from the drop-down list. When defining a
single-glazed window, this input item is not used and is therefore not relevant.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with window input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Window
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Window
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Window Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Deleting Windows
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Duplicating a Window
20.0 Entering Window Data ›› 20.2 Common Tasks ››
Copying Windows
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Window
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 8 of 8
20.0 Entering Window Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6F70.htm