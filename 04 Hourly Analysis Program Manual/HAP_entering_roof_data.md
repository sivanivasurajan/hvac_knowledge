19.0 Entering Roof Data
Overview for Roofs and the Roof Form
19.0 Entering Roof Data ››
This chapter explains input data for roof assemblies.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Overview for Roofs and the Roof Form
About Roofs. HAP uses the term "roof" to refer to opaque horizontal or sloped surfaces of the building
separating ambient air from indoor air. A roof is defined by the sequence of material layers used to construct it
and the physical properties of each layer. These properties include density, specific heat, thickness and
R-value. When a ceiling return air plenum is used, the roof assembly should include the plenum air space and
the ceiling tiles. Together, layer information is used to calculate transfer function coefficients which describe
the dynamic thermal performance of the roof. Ultimately, transfer function coefficients are used to compute
roof transmission loads. One roof type should be defined for each different roof construction used in the
building.
Each project you create can contain many different roof constructions. This allows each different roof
assembly in your building to be modeled. Roof data can be defined by selecting one of a number of pre-
defined roof types offered by HAP, or by building your own roof, layer by layer. Roofs are first entered and
stored in the project using the Roof form. They are then linked to specific roof exposures while entering space
data.
Page 1 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
Common Roof Assembly Applications
19.0 Entering Roof Data ››
The Roof Form, shown above, is used to define data for one roof assembly. The Roof Form contains three
key components:
1. The Title Bar appears across the top of the form. It lists the name of the roof whose data is displayed in the
form. At the right end of the title bar is a button for closing the form.
2. The Working Area is in the center of the form and contains information describing the roof’s construction. In
the working area, inputs are divided into three groups:
a. Roof Assembly Name is used to select a pre-defined roof construction, or to directly enter your own
reference name for the roof. The drop-down list of pre-defined roofs contains three general roof types
(light, medium, heavy). The drop-down list also contains a large number of common roof constructions.
When you are directly defining your roof rather than using HAP’s pre-defined roof types, directly specify
your roof name rather than selecting from the drop-down list.
b. Outside Surface Color and Absorptivity define the solar radiation absorptance characteristics for the
outside surface of the roof. Users may choose from one of three standard surface colors (light, medium,
dark) and the absorptivity will be defaulted. Or, users may directly specify the absorptivity value.
c. Roof Layers Table describes the material layers which comprise the roof, and the thermophysical
properties of each layer. This table provides features for inserting and removing layers, for selecting
layers from a predefined list and modifying or directly defining layer properties.
Data at the bottom of this table lists the total thickness and weight for the roof assembly as well as the
overall R-value and U-value.
3. Command Buttons appear along the bottom of the form. Three buttons are provided:
a. Press OK to save the roof data and return to the main program window. Before saving the roof, the
program automatically generates transfer function coefficients for the roof. These coefficients describe
the dynamic thermal performance of the roof and are used when calculating roof transmission loads.
b. Press Cancel to return to the main program window without saving changes to the roof. If you press
cancel when creating a new roof, no data is saved and a new roof is not added to your project.
c. Press Help to display this overview topic.
Roof Features. HAP provides useful features for:
Creating a new roof.
Editing an existing roof.
Printing roofs.
Deleting roofs.
Copying roofs.
Duplicating a roof.
Application Information. Click here for further information about Common Roof Assembly Applications .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Common Roof Assembly Applications
There are three common situations for defining a roof assembly: defining a custom roof, defining a pre-defined
roof and defining a simple roof. The Roof Form is used in all three cases, but its features are used in slightly
different ways. The procedures for these applications are described below.
1. Defining a Custom Roof. Use this procedure when you have complete specifications for the roof assembly
and therefore want to directly specify the roof characteristics rather than choosing default roof
characteristics.
Page 2 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
19.1 Inputs
19.0 Entering Roof Data ››
Roof Assembly Name
19.0 Entering Roof Data ›› 19.1 Inputs ››
a. Enter a reference name for the roof rather than selecting a pre-defined roof from the drop-down list.
b. Specify the outside surface color or absorptivity .
c. In the Roof Layer Table specify roof layers from inside to outside using your construction specifications. If
necessary, use the features for inserting or removing layers in the table. Properties of each layer can be
defined directly, or you can choose layers from the layer drop-down list.
d. Press the OK button to save the data and return to the main program window.
2. Defining a Pre-Defined Roof. Use this procedure when you are approximating the roof construction with
one of HAP’s pre-defined roof types. This procedure can also be used when you have complete roof
specifications but you know one of HAP’s pre-defined roof types matches or is similar to your specification.
In the latter case, you can save time by choosing a pre-defined roof type and then adjusting its properties.
a. Use the Roof Assembly Name drop-down list to choose from the list of HAP’s pre-defined roof types.
Several dozen common types of built-up, asphalt shingle, wood shingle, and slate roof constructions are
offered in this list. When you choose a roof type, its name and data will be loaded into the form. After the
data is loaded, you can modify the roof name to make it more descriptive if you wish.
b. Modify the outside surface color or absorptivity if necessary.
c. If you are modeling a roof that is similar to one of HAP’s predefined roof types, modify the properties of
the roof layers as necessary. This may involve adjusting the properties of individual layers, or adding
layers such as insulation, plenum air spaces or ceiling tiles.
3. Defining a Simple Roof. Use this procedure when the exact roof construction is not known and you only
need to approximate the general thermal performance of a roof. This is typically only done for preliminary
block load estimates where the accuracy of roof transmission calculations is not critical.
a. Use the Roof Assembly Name drop-down list to choose one of the three "simple" roof types found at the
top of the drop-down list: Light Weight Roof, Medium Weight Roof and Heavy Weight Roof. When you
choose a roof type, its data will be displayed in the form.
b. Modify the outside surface color or absorptivity , if necessary.
c. Adjust data in the roof layer table , if necessary.
d. Press the OK button to save the data and return to the main program window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains input data found in the Roof Assembly Properties window.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Roof Assembly Name
The Roof Assembly Name item can be used as drop-down list or as a text box depending on how you wish to
enter roof data:
Page 3 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
Roof Outside Surface Color & Absorptivity
19.0 Entering Roof Data ›› 19.1 Inputs ››
Roof Layer Table
19.0 Entering Roof Data ›› 19.1 Inputs ››
1. Drop Down List. When choosing one of HAP’s pre-defined or simple roof constructions, use this input as a
drop-down list. The list contains three simple roof types and several dozen common types of built-up,
asphalt shingle, wood shingle, and slate roof constructions. When a roof type is selected from this list,
default data for the roof will be displayed in the form. You can then save this default data, or customize it
before saving the roof.
2. Text Box. When directly defining the roof construction, use this input as a text box to enter the reference
name for your roof. This is typically done when you have complete specifications for the roof and are
building your own roof layer by layer rather than using one of HAP’s simple or pre-defined roofs.
Whether the roof assembly name is defined directly or by choosing from the drop-down list, it is an important
reference value for the roof. The name will appear on selection lists when linking the roof to a exposures in a
space, in the main program window, and on roof and space reports. Therefore, it is important that the roof
name be descriptive so you can easily recognize it when it appears on selection lists or in reports.
The Common Roof Assembly Applications help topic provides further information about choosing roof types
and directly defining roof data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Roof Outside Surface Color & Absorptivity
Information about the absorptivity of the exterior surface of the roof is required to calculate solar heat absorbed
by the roof. Absorptivity information can be defined in two ways:
1. Outside Surface Color can be selected from a drop down list. When a color type is selected, an
absorptivity value is assumed and is displayed on the form. The surface color options and the
corresponding assumptions for absorptivity (α) are as follows: Dark: α=0.9, Medium: α=0.675, Light: α=0.45.
2. Absorptivity can also be directly defined if you have specific information about the absorptance properties
of the roof. Note that when you define an absorptivity value of 0.9, 0.675 or 0.45, HAP will display the
appropriate outside surface color label (dark, medium, light). If you specify a different absorptivity value, the
outside surface color item will be blank.
Application Information. ASHRAE recommends using the Dark designation (α=0.9) for exterior roof surfaces
unless you are confident the roof surface will retain a lower absorptivity during its life. Often air pollution or
weathering darkens surfaces which are originally medium or light colored, so the average absorptivity of the
roof surface over the lifetime of the building is closer to that of a dark surface rather than a medium or light
surface. This recommendation mainly applies to buildings in urban areas where air pollution is more prevalent
or to roof surfaces which are expected to darken through weathering.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Roof Layer Table
Page 4 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
The Roof Layer Table defines the sequence of material layers in the roof and the thermophysical properties of
these layers. Each row in the table contains data for a separate layer in the roof. The top rows list the inside
surface resistance and the innermost material layer. Layers then work outward to the outermost material layer
and the outside surface resistance. Columns in the table contain different properties for each layer. Finally,
totals at the bottom of the table list the total thickness and weight for the assembly and the overall R-value and
U-value for the roof.
The Roof Layer Table provides a variety of features for inserting and removing layers, and for defining layers
and layer properties:
1. To Navigate in the table, use your mouse to click on desired cells in the table, or use the [Tab] and [Shift]
[Tab] key combinations to move forward and backward through cells in the table.
2. To Insert a Layer into the table, first position the mouse cursor in the column of buttons to the left of the
layer name. An arrow will appear. Right click on the button for the layer above which you wish to insert a
new layer. On the pop-up menu that appears, select the Insert option. A layer will be inserted above the
layer you designated. Note that roof assemblies are limited to ten layers: inside and outside surface
resistances plus eight material layers.
Example: In the figure above, you can insert a layer between ‘Inside Surface Resistance’ and ’22 gage steel
deck’ by right-clicking on the button next to the ’22 gage steel deck’ layer, and then selecting the Insert
option.
3. To Remove a Layer from the table, first position the mouse cursor in the column of buttons to the left of the
layer name. An arrow will appear. Right-click on the button for the layer you wish to remove. On the pop-up
menu that appears, select the Remove option. The layer will be deleted. Note that roof assemblies must
contain at least three layers (inside and outside surface resistances, plus one material layer), so HAP will
not permit you to remove the final material layer from a roof.
Example: In the figure above, the insulation layer can be removed by right-clicking on the button to the left
of the ‘R-14 Board Insulation’ layer name and then choosing the Remove option in the pop-up menu.
4. To Directly Input Layer Data type in the name of the layer and then enter its physical properties: thickness,
density, specific heat and R-value. Weight will be calculated automatically from density and thickness. The
direct input approach is typically used when you have complete specifications for the roof and its material
properties.
5. To Choose Default Layer Data use the layer name item as a drop-down list. The list contains data for a
variety of common construction materials. When you choose an item from the list, its name and properties
will be displayed in the table. You can use this data as is, or you can modify the name and adjust the
material properties if necessary.
Each material layer is described with five properties. The first four properties are user-defined; the fifth is
calculated from the user-defined properties. Each property is briefly discussed below:
1. Thickness defines the inside-to-outside dimension of the layer. It influences the mass of the layer (density x
thickness) and the thermal resistance of the layer (thickness / conductivity).
Page 5 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
19.2 Common Tasks
19.0 Entering Roof Data ››
Creating a New Roof
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Editing an Existing Roof
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Printing Roof Inputs
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Deleting Roofs
2. Density defines the mass per unit volume for the material layer. For layers which are not homogeneous a
gross overall density value should be entered rather than the density of one of the layer components.
Density influences the mass of the layer (thickness x density).
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
This section describes how to perform common tasks with roof assembly input data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Creating a New Roof
Please see Creating a New Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Editing an Existing Roof
Please see Editing an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Printing Roof Inputs
Please see Generating Input Data Reports .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Copying Roofs
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Duplicating a Roof
19.0 Entering Roof Data ›› 19.2 Common Tasks ››
Deleting Roofs
Please see Deleting Items .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Copying Roofs
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Duplicating a Roof
Please see Duplicating an Existing Item .
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 7
19.0 Entering Roof Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhF3D7.htm