18.0 Entering Wall Data
Overview for Walls and the Wall Form
18.0 Entering Wall Data ››
This chapter explains input data for wall assemblies.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Walls and the Wall Form
About Walls. HAP uses the term "wall" to refer to opaque vertical surfaces of the building separating ambient
air from indoor air. A wall is defined by the sequence of material layers used to construct it and the physical
properties of each layer. These properties include density, specific heat, thickness and R-value. Together, this
information is used to calculate transfer function coefficients which describe the dynamic thermal performance
of the wall. Ultimately, transfer function coefficients are used to compute wall transmission loads. One wall
type should be defined for each different wall construction used in the building.
Each project you create can contain many different wall constructions. This allows each different wall
assembly in your building to be modeled. Wall data can be defined by selecting one of a number of pre-
defined wall types offered by HAP, or by building your own wall, layer by layer. Walls are first entered and
stored in the project using the Wall form. They are then linked to specific exposures while entering space data.
The Wall Form, shown above, is used to define data for one wall assembly. The Wall Form contains three key
components:
Page 1 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
Common Wall Assembly Applications
18.0 Entering Wall Data ››
1. The Title Bar appears across the top of the form. It lists the name of the wall whose data is displayed in the
form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains information describing the wall’s construction. In
the working area, inputs are divided into three groups:
a. Wall Assembly Name is used to select a pre-defined wall construction, or to directly enter your own
reference name for the wall. The drop-down list of pre-defined walls contains four general wall types
(very light, light, medium, heavy). The drop-down list also contains a large number of common wall
constructions. When you are directly defining your wall rather than using HAP’s pre-defined wall types,
directly specify your wall name rather than selecting from the drop-down list.
b. Outside Surface Color and Absorptivity define the solar radiation absorptance characteristics for the
outside surface of the wall. Users may choose from one of three standard surface colors (light, medium,
dark) and the absorptivity will be defaulted. Or, users may directly specify the absorptivity value.
c. Wall Layers Table describes the material layers which comprise the wall, and the thermophysical
properties of each layer. This table provides features for inserting and removing layers, for selecting
layers from a predefined list and modifying or directly defining layer properties.
Data at the bottom of this table lists the total thickness and weight for the wall assembly as well as the
overall R-value and U-value.3.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the wall data and return to the main program window. Before saving the wall, the
program automatically generates transfer function coefficients for the wall. These coefficients describe
the dynamic thermal performance of the wall and are used when calculating wall transmission loads.
b. Press Cancel to return to the main program window without saving changes to the wall. If you press
cancel when creating a new wall, no data is saved and a new wall is not added to your project.
c. Press Help to display this overview topic.
Wall Features. HAP provides useful features for:
Creating a new wall.
Editing an existing wall.
Printing walls.
Deleting walls.
Copying walls.
Duplicating a wall.
Application Information. Click here for further information about Common Wall Assembly Applications .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Wall Assembly Applications
There are three common situations for defining a wall assembly: defining a custom wall, defining a pre-defined
wall and defining a simple wall. The Wall Form is used in all three cases, but its features are used in slightly
different ways. The procedures for these applications are described below.
1. Defining a Custom Wall. Use this procedure when you have complete specifications for the wall assembly
and therefore want to directly specify the wall characteristics rather than choosing default wall
characteristics.
a. Enter a reference name for the wall rather than selecting a pre-defined wall from the drop-down list.
Page 2 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
18.1 Inputs
18.0 Entering Wall Data ››
Wall Assembly Name
18.0 Entering Wall Data ›› 18.1 Inputs ››
b. Specify the outside surface color or absorptivity .
c. In the Wall Layer Table specify wall layers from inside to outside using your construction specifications. If
necessary, use the features for adding or deleting layers in the table. Properties of each layer can be
defined directly, or you can choose layers from the layer drop-down list.
d. Press the OK button to save the data and return to the main program window.
2. Defining a Pre-Defined Wall. Use this procedure when you are approximating the wall construction with
one of HAP’s pre-defined wall types. This procedure can also be used when you have complete wall
specifications but you know one of HAP’s pre-defined wall types matches or is similar to your specification.
In the latter case, you can save time by choosing a pre-defined wall type and then adjusting its properties.
a. Use the Wall Assembly Name drop-down list to choose from the list of HAP’s pre-defined wall types.
Several dozen common types of brick, concrete block, concrete and wood frame wall constructions are
offered in this list. When you choose a wall type, its name and data will be loaded into the form. After the
data is loaded, you can modify the wall name to make it more descriptive if you wish.
b. Modify the outside surface color or absorptivity if necessary.
c. If you are modeling a wall that is similar to one of HAP’s predefined wall types, modify the properties of
the wall layers as necessary. This may involve adjusting the properties of individual layers, or adding or
rearranging layers such as insulation.
d. Press the OK button to save the data and return to the main program window.
3. Defining a Simple Wall. Use this procedure when the exact wall construction is not known and you only
need to approximate the general thermal performance of a wall. This is typically only done for preliminary
block load estimates where the accuracy of wall transmission calculations is not critical.
a. Use the Wall Assembly Name drop-down list to choose one of the four "simple" wall types found at the
top of the drop-down list: Very Light Weight Wall, Light Weight Wall, Medium Weight Wall and Heavy
Weight Wall. When you choose a wall type, its data will be displayed in the form.
b. Modify the outside surface color or absorptivity , if necessary.
c. Adjust data in the wall layer table , if necessary.
d. Press the OK button to save the data and return to the main program window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data found in the Wall Assembly Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Wall Assembly Name
The Wall Assembly Name item can be used as drop-down list or as a text box depending on how you wish to
enter wall data:
Page 3 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
Wall Outside Surface Color & Absorptivity
18.0 Entering Wall Data ›› 18.1 Inputs ››
Wall Layer Table
18.0 Entering Wall Data ›› 18.1 Inputs ››
1. Drop Down List. When choosing one of HAP’s pre-defined or simple wall constructions, use this input as a
drop-down list. The list contains four simple wall types and several dozen common types of brick, concrete
block, concrete and wood frame wall constructions. When a wall type is selected from this list, default data
for the wall will be displayed in the form. You can then save this default data, or customize it before saving
the wall.
2. Text Box. When directly defining the wall construction, use this input as a text box to enter the reference
name for your wall. This is typically done when you have complete specifications for the wall and are
building your own wall layer by layer rather than using one of HAP’s simple or pre-defined walls.
Whether the wall assembly name is defined directly or by choosing from the drop-down list, it is an important
reference value for the wall. The name will appear on selection lists when linking the wall to a exposures in a
space, in the main program window, and on wall and space reports. Therefore, it is important that the wall
name be descriptive so you can easily recognize it when it appears on selection lists or in reports.
The Common Wall Assembly Applications help topic provides further information about choosing wall types
and directly defining wall data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Wall Outside Surface Color & Absorptivity
Information about the absorptivity of the exterior surface of the wall is required to calculate solar heat absorbed
by the wall. Absorptivity information can be defined in two ways:
1. Outside Surface Color can be selected from a drop down list. When a color type is selected, an
absorptivity value is assumed and is displayed on the form. The surface color options and the
corresponding assumptions for absorptivity (α) are as follows: Dark: α=0.9, Medium: α=0.675, Light: α=0.45.
2. Absorptivity can also be directly defined if you have specific information about the absorptance properties
of the wall. Note that when you define an absorptivity value of 0.9, 0.675 or 0.45, HAP will display the
appropriate outside surface color label (dark, medium, light). If you specify a different absorptivity value, the
outside surface color item will be blank.
Application Information. ASHRAE recommends using the Dark designation (α=0.9) for exterior wall surfaces
unless you are confident the wall surface will retain a lower absorptivity during its life. Often air pollution or
weathering darkens surfaces which are originally medium or light colored, so the average absorptivity of the
wall surface over the lifetime of the building is closer to that of a dark surface rather than a medium or light
surface. This recommendation mainly applies to buildings in urban areas where air pollution is more prevalent
or to wall surfaces which are expected to darken through weathering.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Wall Layer Table
Page 4 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
The Wall Layer Table defines the sequence of material layers in the wall and the thermophysical properties of
these layers. Each row in the table contains data for a separate layer in the wall. The top rows list the inside
surface resistance and the innermost material layer. Layers then work outward to the outermost material layer
and the outside surface resistance. Columns in the table contain different properties for each layer. Finally,
totals at the bottom of the table list the total thickness and weight for the assembly and the overall R-value and
U-value for the wall.
The Wall Layer Table provides a variety of features for inserting and removing layers, and for defining layers
and layer properties:
1. To Navigate in the table, use your mouse to click on desired cells in the table, or use the [Tab] and [Shift]
[Tab] key combinations to move forward and backward through cells in the table.
2. To Insert a Layer into the table, first position the mouse cursor in the column of buttons to the left of the
layer name. An arrow will appear. Right click on the button for the layer above which you wish to insert a
new layer. On the pop-up menu that appears, select the Insert option. A layer will be inserted above the
layer you designated. Note that wall assemblies are limited to ten layers: inside and outside surface
resistances plus eight material layers.
Example: In the figure above, you can insert a layer between ‘Inside Surface Resistance’ and ‘5/8" Gypsum
Board’ by right-clicking on the button next to the ‘5/8" Gypsum Board’ layer, and then selecting the Insert
option.
3. To Remove a Layer from the table, first position the mouse cursor in the column of buttons to the left of the
layer name. An arrow will appear. Right-click on the button for the layer you wish to remove. On the pop-up
menu that appears, select the Remove option. The layer will be deleted. Note that wall assemblies must
contain at least three layers (inside and outside surface resistances, plus one material layer), so HAP will
not permit you to remove the final material layer from a wall.
Example: In the figure above, the Air Space layer can be removed by right-clicking on the button to the left
of the ‘Air Space’ layer name and then choosing the Remove option in the pop-up menu.
4. To Directly Input Layer Data type in the name of the layer and then enter its physical properties: thickness,
density, specific heat and R-value. Weight will be calculated automatically from density and thickness. The
direct input approach is typically used when you have complete specifications for the wall and its material
properties.
5. To Choose Default Layer Data use the layer name item as a drop-down list. The list contains data for a
variety of common construction materials. When you choose an item from the list, its name and properties
will be displayed in the table. You can use this data as is, or you can modify the name and adjust the
material properties if necessary.
Each material layer is described with five properties. The first four properties are user-defined; the fifth is
calculated from the user-defined properties. Each property is briefly discussed below:
Page 5 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
18.2 Common Tasks
18.0 Entering Wall Data ››
Creating a New Wall
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
Editing an Existing Wall
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
Printing Wall Inputs
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
1. Thickness defines the inside-to-outside dimension of the layer. It influences the mass of the layer (density x
thickness) and the thermal resistance of the layer (thickness / conductivity).
2. Density defines the mass per unit volume for the material layer. For layers which are not homogeneous,
such as hollow concrete blocks, a gross overall density value should be entered rather than the density of
one of the layer components. Density influences the mass of the layer (thickness x density).
3. Specific Heat defines the heat capacity of the material. For layers which are not homogeneous, the gross
overall specific heat should be defined rather than the specific heat of one of the layer components. Specific
heat influences the thermal capacitance of the layer (specific heat x mass).
4. R-Value defines the thermal resistance of the material layer. For the "inside surface resistance" layer the
R-value is the convection coefficient between the innermost layer and indoor air. For the "outside surface
resistance" the R-value is the convection coefficient between the outermost layer and outdoor air.
5. Weight defines the mass per unit surface area of the material layer. This is not an input item. Rather, it is
calculated using the density and thickness values for the layer (density x thickness). It is displayed for
reference purposes only.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section describes how to perform common tasks with wall assembly input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Wall
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Wall
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Wall Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm
Deleting Walls
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
Copying Walls
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
Duplicating a Wall
18.0 Entering Wall Data ›› 18.2 Common Tasks ››
Deleting Walls
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying Walls
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Wall
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 7
18.0 Entering Wall Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hh6727.htm