33.0 Converting Previous Version Data
33.1 Converting HAP v3.2 Data
33.0 Converting Previous Version Data ››
About Translation of HAP v3.2 Data
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
This chapter explains how data is converted from a previous version of HAP for use in the current version of
HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
This section explains conversion of data from HAP 3.2 (the last MS-DOS version) for use in the current version
of HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
About Translation of HAP v3.2 Data
Converting HAP v3.2 to HAP v5.1. This topic explains the conversion of data from v3.2 to v5.1 format. HAP
v3.2 was the last DOS version of HAP released between 1995 and 2000 and requires a different conversion
process than required when converting a project from one of the HAP v4 or v5 versions. When converting
data from v3.2 to v5.1 format:
1. Input data for the following categories of data is preserved: Design Weather, Spaces, Air Systems,
Schedules, Walls, Roofs, Windows, Doors, and External Shades.
2. Input data for the following categories of data cannot be converted because of major changes in content
and organization of the data between v3.2 and v5.1: Simulation Weather, Calendar, Electric Rates, Fuel
Rates, Plants, and Buildings.
3. Design and energy simulation calculation results are not converted and must be regenerated in v5.1.
4. Modifications to input data are made only to space, system, wall and roof data as described in the
"modification" sections below.
For information on steps required in the program to convert v3.2 data, please click here: Converting HAP v3.2
Data.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review data after
the conversion is complete and before using data in calculations:
1. Review space data to check the Space Usage and OA Requirement 1 input values. Note that the Replace
option on the Edit Menu can be used to change input values for multiple spaces all at one time, if desired.
2. Review system data to check and adjust the value for the new Ventilation Sizing Method input item.
3. Review system data to check cooling sizing criteria. inputs.
4. Review system data to check cooling coil control inputs.
5. Review system data to check heating coil control inputs.
6. Review wall data for changes to "Simple" and "Pre-Defined" wall types.
7. Review roof data for changes to "Simple" and "Pre-Defined" roof types..
Page 1 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Modification of Wall U-Value for Simple and Pre-Defined Walls
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
Modifications to Space Input Data. Between v3.2 and v5.1 features for sizing outdoor ventilation air were
changed. Related to this, inputs for ventilation air were moved from the air system level to the space level.
Therefore, when converting HAP v3.2 data, ventilation inputs are added to the converted space data as
follows:
1. For each space the Space Usage input is set to "User-Defined".
2. The OA Requirement 1 value is set according to ventilation specifications for the air system the space is
linked to. For example, if a space is linked to an air system which specified ventilation air as 20
CFM/person, the space will inherit that ventilation specification. This simple inheritance rule applies if the
system a space is linked to uses CFM/person, CFM/sqft or % of supply air as the units of measure for
ventilation. In SI Metric the inheritance rule is used for L/s/person, L/s/sqm and % of supply air units of
measure. When the air system defines ventilation air as CFM or L/s, the program calculates a CFM/sqft or
L/s/sqm value by dividing total ventilation air by space floor area served by the system. This CFM/sqft or
L/s/sqm is then applied to the space.
Note that when a space is linked to two or more air systems in a project, the space inherits ventilation
settings from the air system with the lowest index number. Because it is nearly impossible for a user to
determine system index numbers, it is best to review the assigned space ventilation rates after data has
been converted to verify desired values are used.
Modifications to Air System Input Data. Due to changes in air system data made in HAP v4.1 and v4.2 the
following modifications are made to system data when it is converted from v3.2 to v5.1 format.
1. The input for design ventilation airflow rate is deleted since it has been moved to the space level.
2. The input "Ventilation Sizing Method" is inserted and is defaulted to "Sum of OA Airflows". After the
conversion is complete this default can be changed, if necessary.
3. Modification of Cooling Sizing Criteria for an Air System.
4. Modification of Cooling Coil Control for an Air System.
5. Modification of Heating Coil Control for an Air System.
6. Convective Cooling/Heating Systems Cannot be Translated.
Modifications to Wall and Roof Data.
1. Modification of Wall U-Value for "Simple" and "Pre-Defined" wall.
2. Modification of Roof U-Value for "Simple" and "Pre-Defined" roofs.
Troubleshooting. In some cases the conversion of HAP v3.2 data will fail and an error message will appear
explaining the reason for the failure. Error conditions fall into three categories. For further information on each
and recommended workaround procedures, click on one of the following:
1. [source] Data Folder does not Contain a Complete Set of Data Files.
2. [destination] Data Folder Does Not Contain a Complete Set of Data Files.
3. Fatal Errors
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modification of Wall U-Value for Simple and Pre-Defined Walls
If your HAP v3.2 or System Design Load v1.2 project contained "simple" or "predefined" types of walls, the
overall U-value may have been adjusted for the reason described below:
For simple and pre-defined walls, HAP v3.2 and System Design Load v1.2 made assumptions about the
material layers comprising the wall and these assumptions determined the overall U-value for the wall.
However, users were allowed to modify the overall U-value. If a modified U-value was defined the program
Page 2 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Modification of Roof U-Value for Simple and Pre-Defined Roofs
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
Modification of Cooling Sizing Criteria for Air Systems
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
Modification of Cooling Coil Control for Air Systems
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
would approximate the wall thermal performance by adjusting the conduction transfer function coefficients. As
long as the modified and original U-values were similar, the approximation was reasonably accurate.
In the current version of HAP, all walls are defined by their constituent material layers. The overall U-value for
a wall must correspond to its material layers. When translating wall data, information about the material layers
in the wall and the U-value corresponding to these layers is translated, but any user-modified U-value cannot
be translated.
Therefore, if your HAP v3.2 or System Design Load v1.2 project contained "simple" or "pre-defined" walls, this
wall data should be inspected after the data conversion is complete.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modification of Roof U-Value for Simple and Pre-Defined Roofs
If your HAP v3.2 or System Design Load v1.2 project contained "simple" or "predefined" types of roofs, the
overall U-value may have been adjusted for the reason described below:
For simple and pre-defined roofs, HAP v3.2 and System Design Load v1.2 made assumptions about the
material layers comprising the roof and these assumptions determined the overall U-value for the roof.
However, users were allowed to modify the overall U-value. If a modified U-value was defined the program
would approximate the roof thermal performance by adjusting the conduction transfer function coefficients. As
long as the modified and original U-values were similar, the approximation was reasonably accurate.
In the current version of HAP, all roofs are defined by their constituent material layers. The overall U-value for
a roof must correspond to its material layers. When translating roof data, information about the material layers
in the roof and the U-value corresponding to these layers is translated, but any user-modified U-value cannot
be translated.
Therefore, if your HAP v3.2 or System Design Load v1.2 project contained "simple" or "pre-defined" roofs, this
roof data should be inspected after the conversion is complete.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modification of Cooling Sizing Criteria for Air Systems
If your HAP v3.2 or System Design Load v1.2 project contained PTAC, WSHP, 2-Pipe Fan Coil or 4-Pipe Fan
Coil air systems in which the cooling sizing criteria was specified in terms of CFM (L/s) or CFM/sqft (L/s/sqm),
this cooling sizing criteria was modified.
In the current version of HAP the cooling sizing criteria for all Terminal Unit systems must be supply air
temperature. Therefore, the original cooling sizing criteria has been replaced with a supply air temperature of
55 F (12.8 C) in the translated data.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modification of Cooling Coil Control for Air Systems
Page 3 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Modification of Heating Coil Control for Air Systems
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
In two situations, the translation process will modify cooling coil control specifications for an air system. Each
situation is described below:
1. Cooling coil control is modified for a Single Zone CAV air system if the following inputs are used:
a. Type of Reset = Not Used.
b. The supply fan is not cycled.
With this type of control, the system will provide a constant volume of constant temperature cold air to the
zone. The system has no way to modulate cooling as zone loads rise and fall. While this input was
permitted in HAP v3.2 and System Design Load v1.2, it usually resulted in unstable operation of the system.
In the current version of HAP, this type of control is not permitted for Single Zone CAV systems. Therefore,
the data translator will change the cooling control to "Cycled or Staged Coil, Fan On". This control models
the operation of DX cooling equipment in which the supply fan runs continuously during occupied hours,
and the DX coil is cycled or staged to modulate cooling provided to the zone. In a hydronic system, this
option represents a control in which water flow through the coil, or supply water temperature to the coil is
varied to modulate cooling output.
2. Cooling coil control is modified for Single Zone CAV, PTAC, WSHP, 2-Pipe Fan Coil and 4-Pipe Fan coil air
systems if the following inputs are used:
a. Both cooling and heating are provided.
b. Fan cycling is used for heating.
c. Fan cycling is not used for cooling.
In HAP v3.2 and System Design Load v1.2, the program assumed that fan cycling was either used for both
cooling and heating, or was used for neither. Because the program inputs permitted fan cycling to be
specified separately for cooling and heating, it created the misleading impression that fan cycling could be
used for heating but not cooling or vice versa. In the current version of HAP, this situation has been
corrected so the program explicitly forces cooling and heating controls to match: either both use fan cycling,
or neither uses fan cycling. When translating data from HAP v3.2 and System Design Load v1.2, any data
in which cooling and heating fan cycling do not match are corrected. For the inputs above, the data
translator will change the cooling control to use fan cycling.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Modification of Heating Coil Control for Air Systems
In two situations, the translation process will modify heating coil control specifications for an air system. Each
situation is described below:
1. Heating coil control is modified for a Single Zone CAV air system if the following inputs are used:
a. Type of Reset = Not Used.
b. The supply fan is not cycled.
With this type of control, the system will provide a constant volume of constant temperature hot air to the
zone. The system has no way to modulate heating as zone loads rise and fall. While this input was
permitted in HAP v3.2 and System Design Load v1.2, it usually resulted in unstable operation of the system.
In the current version of HAP, this type of control is not permitted for Single Zone CAV systems. Therefore,
the data translator will change the heating control to "Cycled or Staged Coil, Fan On". This control models
the operation of electric, combustion or heat pump heating equipment in which the supply fan runs
continuously during occupied hours, and the heat pump, heating element or burners are cycled or staged to
modulate heating provided to the zone. In hydronic systems, this option models control in which water flow
through the coil, or supply water temperature to the coil is varied to modulate heating output.
Page 4 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Convective Cooling/Heating Systems Cannot be Translated
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
[destination] Data Folder Does~Not~Contain~a~Complete~Set~of~Files
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
[source] Data Folder Does Not Contain a Complete Set of Data Files
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
2. Heating coil control is modified for Single Zone CAV, PTAC, WSHP, 2-Pipe Fan Coil and 4-Pipe Fan coil air
systems if the following inputs are used:
a. Both cooling and heating are provided.
b. Fan cycling is used for cooling.
c. Fan cycling is not used for heating.
In HAP v3.2 and System Design Load v1.2, the program assumed that fan cycling was either used for both
cooling and heating, or was used for neither. Because the program inputs permitted fan cycling to be
specified separately for cooling and heating, it created the misleading impression that fan cycling could be
used for heating but not cooling or vice versa. In the current version of HAP, this situation has been
corrected so that the program explicitly forces cooling and heating controls to match: either both use fan
cycling, or neither uses fan cycling. When translating data from HAP v3.2 and System Design Load v1.2,
any data in which cooling and heating fan cycling do not match are corrected. For the inputs above, the
data translator will change the heating control to use fan cycling.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Convective Cooling/Heating Systems Cannot be Translated
If your HAP v3.2 or System Design Load v1.2 project contained any "Convective Cooling/Heating" air systems,
these systems could not be translated. This system type is not offered versions of HAP after v3.2.
Convective Heating Systems can be modeled in the current version of HAP using a Single Zone CAV system
with central cooling and heating disabled and space baseboard heating units inserted in the zone. If you model
the convective heating system in this manner in HAP v3.2, the system data can be translated.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
[destination] Data Folder Does Not Contain a Complete Set of Files
Description: The current HAP v4.7 project folder does not contain a full set of data files. A complete set of
empty HAP v4.7 data files is required before data can be translated from HAP v3.2 or System Design Load
v1.2 to HAP v4.7. The translation from HAP v3.2 to v4.7 is a five stage process. First data is translated from
v3.2 to v4.0 format, then successively from v4.0 to v4.1, v4.1 to v4.2, v4.2 to v4.3, v4.3 to v4.4, v4.4 to v4.5,
v4.5 to v4.6, and finally v4.6 to v4.7, format. HAP creates temporary copies of data files for each intermediate
version of HAP to facilitate this process. This error occurs when HAP fails to create a complete set of one of
the intermediate version data files.
Severity: Fatal. No data was translated.
Workaround: This is an extremely rare error. Please contact Carrier Software Systems for assistance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
[source] Data Folder Does Not Contain a Complete Set of Data Files
Page 5 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Fatal Translation Errors
33.0 Converting Previous Version Data ›› 33.1 Converting HAP v3.2 Data ››
Description: The data folder you chose as the source of HAP v3.2 or System Design Load v1.2 data does not
contain a complete set of data files. Each HAP v3.2 or System Design Load v1.2 data folder must contain a full
set of program data files. If one or more of these files are missing, it means one of the data components (such
as wall data or space data) is missing, and as a result the data cannot be translated to the current version of
HAP.
The most common cause for this error is that the source folder was incorrectly selected. When you choose the
"Convert HAP v3.2 Data" option a dialog appears asking you to choose the v3.2 data folder whose data you
want to convert. To properly choose this folder, you must double-click on the folder name so the folder is
highlighted, and its icon has the appearance of an opened folder. The path to the folder you selected is listed
at the bottom of the dialog and this provides a way to double-check your selection. If you only single-click on
the folder, it has not been selected and the program will usually be attempting to convert data from a folder
one level higher than the folder you intended. As a result, HAP v3.2 data files cannot be found.
Other causes for this error include: data files have been damaged, data files have been deleted manually
using Windows Explorer or DOS commands, or the data was retrieved from an archive and the retrieval
process was incomplete.
Severity: Fatal. No data could be translated.
Workaround: First make sure you have correctly selected the HAP v3.2 data folder as described above (i.e.
you must double-click on the folder name).
If selection of the folder is not the problem, then you should first identify which data files are missing from the
source folder. Use Windows Explorer to view data files in the HAP v3.2 or System Design Load v1.2 folder
being used as the source of this data translation. The following core data files are required for HAP v3.2 and
System Design Load v1.2:
HAP v3.2
System Design Load v1.2
Description of File
HAP32WTD.DAT
SDL12WTD.DAT
Design weather data.
HAP32CAL.DAT
SDL12CAL.DAT
Calendar data.
HAP32SCH.DAT
SDL12SCH.DAT
Schedule data.
HAP32MTL.DAT
SDL12MTL.DAT
Construction material data.
HAP32SPC.DAT
SDL12SPC.DAT
Space data.
HAP32INA.DAT
SDL12INA.DAT
Air system index data.
Next, if this data was recently retrieved from an archive, try retrieving the archive data again. Afterwards check
to see if the core set of files exists after this second attempt at retrieving data.
If this second retrieval does not work, or if you believe data files were manually deleted or are damaged in
some way, please contact Carrier Software Systems. Depending on which data files are missing, it may be
possible to repair the data so a portion of it can be translated to the current version of HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Fatal Translation Errors
In unusual situations a fatal error can cause the data translation to halt. If a fatal error occurs, a message will
be displayed describing the error. If this happens, press OK to return to the HAP main window. Then use the
"Convert HAP v3.2 Data" again to rerun the translation. If a fatal error occurs the second time, please write
down the error message and then contact Carrier Software systems for assistance.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 6 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
33.2 Converting HAP v4.x and v5.x Data
33.0 Converting Previous Version Data ››
About Translation of HAP v4.x and v5.x Data
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
This section explains conversion of data from any HAP v4.x or v5.x version for use in the current version of
HAP.
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
About Translation of HAP v4.x and v5.x Data
This topic discusses the conversion of data from previous 4.0 thru 5.0 versions of HAP to the current HAP v5.1
format.
Converting v4.x and v5.x Data. The Convert HAP v4.x or v5.x Data option on the Project Menu reads data
from an earlier version of HAP and converts it to a format compatible with HAP v5.1. Because the content and
format of data in HAP v5.0 is different from that in previous HAP versions this conversion requires "translating"
data from its old format to the new format.
It is important to make a distinction between "translation" of data and "transfer" of data:
1. "Data Transfer refers to the simple copying of data. The result of a data transfer is an exact copy of the
original data. No data is added, deleted or modified.
2. The result of a "Data Translation" is the original data with missing items added, unusable items discarded
and other items reorganized.
Depending on the version of HAP data you are converting, translation considerations will vary. For specific
information about the data translation and data review procedures for each data conversion scenario, click on
one of the following:
Converting from HAP v5.0 Format
Converting from HAP v4.9 Format
Converting from HAP v4.8 Format
Converting from HAP v4.7 Format
Converting from HAP v4.6 Format
Converting from HAP v4.5 Format
Converting from HAP v4.4 Format
Converting from HAP v4.3 Format
Converting from HAP v4.2 Format.
Converting from HAP v4.1 Format.
Converting from HAP v4.0 Format.
For a description of the steps required to convert old program data, please click the following link:
Converting HAP v4.x or 5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 7 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.0 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data From HAP v4.0 Format
Converting HAP v4.0 to HAP v5.1. When converting data from v4.0 to v5.1 format:
a. Input data for all categories of data which existed in HAP v4.0 is preserved.
b. Design calculation results are not converted and must be regenerated in v5.1.
c. Modifications to input data are made to space, air system, and plant data as described in the
"modification" sections below.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review this input
data after the conversion is complete and before using data in calculations:
Modifications to Space Input Data. Between v4.0 and v5.1, one of the major changes involves features for
sizing outdoor ventilation air (this change was made in v4.2). Related to this, inputs for ventilation air were
moved from the air system level to the space level. Therefore, when converting HAP v4.0 data, ventilation
inputs are added to the converted space data as follows:
1. For each space the Space Usage input is set to "User-Defined".
2. The OA Requirement 1 value is set according to ventilation specifications for the air system the space is
linked to. For example, if a space is linked to an air system which specified ventilation air as 20
CFM/person, the space will inherit that ventilation specification. This simple inheritance rule applies if the
system a space is linked to uses CFM/person, CFM/sqft or % of supply air as the units of measure for
ventilation. In SI Metric the inheritance rule is used for L/s/person, L/s/sqm and % of supply air units of
measure. When the air system defines ventilation air as CFM or L/s, the program calculates a CFM/sqft or
L/s/sqm value by dividing total ventilation air by space floor area served by the system. This CFM/sqft or
L/s/sqm is then applied to the space.
Note that when a space is linked to two or more air systems in a project, the space inherits ventilation
settings from the air system with the lowest index number. Because it is nearly impossible for a user to
determine system index numbers, it is best to review the assigned space ventilation rates after data has
been converted to verify desired values are used.
Modifications to Air System Input Data. Between v4.0 and v5.1 several changes were made in air system
data. These changes are described below.
1. The input for design ventilation airflow rate has been deleted since it has been moved to the space level.
2. The input "Ventilation Sizing Method" has been inserted and is defaulted to "Sum of OA Airflows". After the
conversion is complete this default can be changed, if necessary.
3. The "Cooling Source" input for DX systems was adjusted. In HAP v4.0 a cooling source of "DX" was used.
In HAP v4.1, new options were provided for designating "Air-Cooled DX" and "Water-Cooled DX"
equipment. Therefore, when translating data, all Packaged Rooftop Units, Packaged Vertical Units, Split DX
Air Handling Units, and Packaged or Split DX Fan Coils are assigned a cooling source of "Air-Cooled DX".
Water Source Heat Pump systems are assigned a cooling source of "Water Cooled DX".
4. The "Heating Source" input for heat pump equipment was adjusted. In HAP v4.0 a heating source of "DX"
was used. In HAP v4.1, new options were provided for designating "Air Source Heat Pump" and "Water
Source Heat Pump". Therefore when translating data, all Packaged Rooftop Units, Split DX Air Handling
Units and Packaged or Split DX Fan Coils which used "DX" as a heating source are converted to "Air
Source Heat Pump". All Water Source Heat Pump units are converted to "Water Source Heat Pump" as a
heating source.
5. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted starting in v4.6 is "cycled or
staged capacity, fan on". For central heating coil, the only "capacity control" option permitted now is "cycled
or staged capacity, fan on". Any system using a different capacity control will be switched to "cycled or
staged capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops,
Page 8 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.1 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
vertical packaged units and split DX AHUs. No other combinations of system type and equipment type are
affected by this change..
Modifications to Plant Input Data. HAP v4.0 only offered three simple plant options: cooling plant, hot water
heating plant and steam heating plant. In HAP v4.1 specific plant types were added. Therefore, when
translating data from v4.0 to v5.0, the plant types were converted as follows:
1. All plants with plant type "cooling plant" were changed to "Generic Chilled Water".
2. All plants with plant type "hot water heating plant" were changed to "Generic Hot Water".
3. All plants with plant type "steam heating plant" were changed to "Generic Steam".
Troubleshooting Fatal Errors. Problems which cause this data conversion to fail are rare. If a fatal error does
occur, the program will display a "Data Conversion Failed" error message. Please make a note of any error
messages which appear. Also please make a note of the source you were converting from (active project or
archive file) and the destination project you were placing converted data into. Then contact Carrier software
technical support for assistance.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting Data From HAP v4.1 Format
Converting HAP v4.1 to HAP v5.1. When converting data from v4.1 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design and simulation calculation results are not converted and must be regenerated in v5.1.
c. Modifications to input data are made space, system, plant, cooling tower and boiler data as described in
the "modification" sections below.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review space,
system, plant, cooling tower and boiler data after the conversion is complete and before using data in
calculations:
Modifications to Space Input Data. Between v4.1 and v5.1 one of the major changes involved features for
sizing outdoor ventilation air (this change was made in v4.2). Related to this, inputs for ventilation air were
moved from the air system level to the space level. Therefore, when converting HAP v4.1 data, ventilation
inputs are added to the converted space data as follows:
1. For each space the Space Usage input is set to "User-Defined".
2. The OA Requirement 1 value is set according to ventilation specifications for the air system the space is
linked to. For example, if a space is linked to an air system which specified ventilation air as 20
CFM/person, the space will inherit that ventilation specification. This simple inheritance rule applies if the
system a space is linked to uses CFM/person, CFM/sqft or % of supply air as the units of measure for
ventilation. In SI Metric the inheritance rule is used for L/s/person, L/s/sqm and % of supply air units of
measure. When the air system defines ventilation air as CFM or L/s, the program calculates a CFM/sqft or
Page 9 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
L/s/sqm value by dividing total ventilation air by space floor area served by the system. This CFM/sqft or
L/s/sqm is then applied to the space.
Note that when a space is linked to two or more air systems in a project, the space inherits ventilation
settings from the air system with the lowest index number. Because it is nearly impossible for a user to
determine system index numbers, it is best to review the assigned space ventilation rates after data has
been converted to verify desired values are used.
Modifications to Air System Input Data. The following changes are made when converting air system input
data.
1. The input for design ventilation airflow rate has been deleted since it has been moved to the space level.
2. The input Ventilation Sizing Method has been inserted and is defaulted to "Sum of OA Airflows". After the
conversion is complete this default can be changed, if necessary.
3. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted now is "cycled or staged capacity,
fan on". For central heating coil, the only "capacity control" option permitted now is "cycled or staged
capacity, fan on". Any system using a different capacity control will be switched to "cycled or staged
capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops, vertical
packaged units and split DX AHUs. No other combinations of system type and equipment type are affected
by this change.
4. For water-cooled vertical packaged unit, WSHP, GSHP and GWSHP systems, condenser pump
performance data was moved from the cooling tower inputs to the system inputs. During conversion the
software automatically moves condenser pump performance data from the linked cooling tower to the
system. Values are preserved. Only the location of the data changes.
Modifications to Plant Input Data. The following change was made to plant data:
1. Chiller Plants - Condenser pump performance data was moved from the cooling tower inputs to the plant
inputs. During conversion the software automatically moves condenser pump performance data from the
linked cooling towers to the plant. There is only one situation where pump performance data is altered. If
multiple cooling towers are linked to a plant and different units of measure for pump performance (head,
kW, W/gpm, W/L/s) are used among the towers, units for the condenser pump associated with the first
linked tower will be used in the plant. Data for the pumps whose units do not match must be discarded and
is set to zero. Therefore it is important to check chiller plant data after conversion to correct any situations
where condenser pump data had to be discarded.
Modifications to Cooling Towers. One change was made to cooling tower data:
1. Condenser pump performance data was moved from cooling towers to the plant or system the tower was
linked to. No values were changed. Only the location of the data changed.
Modifications to Boilers. The following change was made to boiler data:
1. Boiler modeling features were expanded in v4.6. While no data for boilers from v4.1 was altered during the
conversion, defaults for the new boiler inputs were assigned. These include boiler type (hot water) and
design hot water supply temperature (180 F, 82.2 C).
Troubleshooting Fatal Errors. Problems which cause the data conversion to fail are rare. If a fatal error does
occur, the program will display a "Data Conversion Failed" error message. Please make a note of any error
messages which appear. Also please make a note of the source you were converting from (active project or
archive file) and the destination project you were placing converted data into. Then contact Carrier software
technical support for assistance.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 10 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.2 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data From HAP v4.3 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data From HAP v4.2 Format
Converting HAP v4.2 to HAP v5.1. When converting data from v4.2 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design and simulation calculation results are not converted and must be regenerated in v5.1.
c. Modifications to input data are made only to air system, plant, cooling tower, and boiler data as described
in the "modification" sections below.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review this input
data after the conversion is complete and before using data in calculations.
Modifications to Air System Input Data. Two changes were made in air system data:
1. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted now is "cycled or staged capacity,
fan on". For central heating coil, the only "capacity control" option permitted now is "cycled or staged
capacity, fan on". Any system using a different capacity control will be switched to "cycled or staged
capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops, vertical
packaged units and split DX AHUs. No other combinations of system type and equipment type are affected
by this change..
2. For water-cooled vertical packaged unit, WSHP, GSHP and GWSHP systems, condenser pump
performance data was moved from the cooling tower inputs to the system inputs. During conversion the
software automatically moves condenser pump performance data from the linked cooling tower to the
system. Values are preserved. Only the location of the data changes.
Modifications to Plant Input Data. The following change was made to plant data:
1. Chiller Plants - Condenser pump performance data was moved from the cooling tower inputs to the plant
inputs. During conversion the software automatically moves condenser pump performance data from the
linked cooling tower to the plant. There is only one situation where pump performance data is altered. If
multiple cooling towers are linked to a plant and different units of measure for pump performance (head,
kW, W/gpm, W/L/s) are used among the towers, units for the condenser pump associated with the first
linked tower will be used in the plant. Data for the pumps whose units do not match must be discarded.
Therefore it is important to check chiller plant data after conversion to correct any situations where
condenser pump data had to be discarded.
Modifications to Cooling Towers. One change was made to cooling tower data:
1. Condenser pump performance data was moved from cooling towers to the plant or system the tower was
linked to. No values were changed. Only the location of the data changed.
Modifications to Boilers. The following change was made to boiler data:
1. Boiler modeling features were expanded in v4.6. While no data for boilers from v4.2 was altered during the
conversion, defaults for the new boiler inputs were assigned. These include boiler type (hot water) and
design hot water supply temperature (180 F, 82.2 C).
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 11 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.3 Format
Converting HAP v4.3 to HAP v5.1. When converting data from v4.3 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design and simulation calculation results are not converted and must be regenerated in v5.1.
c. Modifications to input data are made only to air system, plant, cooling tower and boiler data as described
in the "modification" sections below.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review this input
data after the conversion is complete and before using data in calculations.
In addition, it is also worth reviewing Building input data if you intend to use the converted data for a LEED
Energy and Atmosphere Credit 1 analysis. In the Building Properties window go to the Misc. Energy Use tab.
This tab contains a new input that allows you to designate energy use items as "Process". When v4.3 data
was converted all items default to non-Process. This data should be reviewed and if necessary, modified
before generating the LEED NC 2.2 EA Credit 1 Summary Report.
Modifications to Air System Input Data. Two changes were made in air system data:
1. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted now is "cycled or staged capacity,
fan on". For central heating coil, the only "capacity control" option permitted now is "cycled or staged
capacity, fan on". Any system using a different capacity control will be switched to "cycled or staged
capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops, vertical
packaged units and split DX AHUs. No other combinations of system type and equipment type are affected
by this change..
2. For water-cooled vertical packaged unit, WSHP, GSHP and GWSHP systems, condenser pump
performance data was moved from the cooling tower inputs to the system inputs. During conversion the
software automatically moves condenser pump performance data from the linked cooling tower to the
system. Values are preserved. Only the location of the data changes.
Modifications to Plant Input Data. The following change was made to plant data:
1. Chiller Plants - Condenser pump performance data was moved from the cooling tower inputs to the plant
inputs. During conversion the software automatically moves condenser pump performance data from the
linked cooling tower to the plant. There is only one situation where pump performance data is altered. If
multiple cooling towers are linked to a plant and different units of measure for pump performance (head,
kW, W/gpm, W/L/s) are used among the towers, units for the condenser pump associated with the first
linked tower will be used in the plant. Data for the pumps whose units do not match must be discarded.
Therefore it is important to check chiller plant data after conversion to correct any situations where
condenser pump data had to be discarded.
Modifications to Cooling Towers. One change was made to cooling tower data:
1. Condenser pump performance data was moved from cooling towers to the plant or system the tower was
linked to. No values were changed. Only the location of the data changed.
Modifications to Boilers. The following change was made to boiler data:
1. Boiler modeling features were expanded in v4.6. While no data for boilers from v4.3 was altered during the
conversion, defaults for the new boiler inputs were assigned. These include boiler type (hot water) and
design hot water supply temperature (180 F, 82.2 C).
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 12 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.4 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data From HAP v4.4 Format
Converting HAP v4.4 to HAP v5.1. When converting data from v4.4 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design and simulation calculation results are not converted and must be regenerated in v5.1.
c. Modifications to input data are made only to air system, plant, cooling tower and boiler data as described
in the "modification" sections below.
Reviewing Data after Conversion. Because of modifications to input data, it is important to review this input
data after the conversion is complete and before using data in calculations.
Modifications to Air System Input Data. Two changes were made in air system data:
1. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted now is "cycled or staged capacity,
fan on". For central heating coil, the only "capacity control" option permitted now is "cycled or staged
capacity, fan on". Any system using a different capacity control will be switched to "cycled or staged
capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops, vertical
packaged units and split DX AHUs. No other combinations of system type and equipment type are affected
by this change..
2. For water-cooled vertical packaged unit, WSHP, GSHP and GWSHP systems, condenser pump
performance data was moved from the cooling tower inputs to the system inputs. During conversion the
software automatically moves condenser pump performance data from the linked cooling tower to the
system. Values are preserved. Only the location of the data changes.
Modifications to Plant Input Data. The following change was made to plant data:
1. Chiller Plants - Condenser pump performance data was moved from the cooling tower inputs to the plant
inputs. During conversion the software automatically moves condenser pump performance data from the
linked cooling tower to the plant. There is only one situation where pump performance data is altered. If
multiple cooling towers are linked to a plant and different units of measure for pump performance (head,
kW, W/gpm, W/L/s) are used among the towers, units for the condenser pump associated with the first
linked tower will be used in the plant. Data for the pumps whose units do not match must be discarded.
Therefore it is important to check chiller plant data after conversion to correct any situations where
condenser pump data had to be discarded.
Modifications to Cooling Towers. One change was made to cooling tower data:
1. Condenser pump performance data was moved from cooling towers to the plant or system the tower was
linked to. No values were changed. Only the location of the data changed.
Modifications to Boilers. The following change was made to boiler data:
1. Boiler modeling features were expanded in v4.6. While no data for boilers from v4.4 was altered during the
conversion, defaults for the new boiler inputs were assigned. These include boiler type (hot water) and
design hot water supply temperature (180 F, 82.2 C).
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 13 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data From HAP v4.5 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data From HAP v4.5 Format
Converting HAP v4.5 to HAP v5.1. When converting data from v4.5 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design calculation results are not converted and must be regenerated in v5.1.
c. Simulation results are not converted and must be regenerated in v5.1.
d. Modifications to input data are made only to air system, plant, cooling tower and boiler data as described
in the "modification" sections below.
Reviewing Data after Conversion. Because of modifications to system, plant, cooling tower and boiler input
data, it is important to review this input data after the conversion is complete and before using data in
calculations.
Modifications to Air System Input Data. Two changes were made in air system data:
1. For single-zone CAV systems with equipment types "packaged rooftop", "vertical packaged unit" and "split
DX AHU", the only central cooling coil "capacity control" option permitted now is "cycled or staged capacity,
fan on". For central heating coil, the only "capacity control" option permitted now is "cycled or staged
capacity, fan on". Any system using a different capacity control will be switched to "cycled or staged
capacity, fan on" automatically. Note that this only applies to CAV-single-zone systems for rooftops, vertical
packaged units and split DX AHUs. No other combinations of system type and equipment type are affected
by this change..
2. For water-cooled vertical packaged unit, WSHP, GSHP and GWSHP systems, condenser pump
performance data was moved from the cooling tower inputs to the system inputs. During conversion the
software automatically moves condenser pump performance data from the linked cooling tower to the
system. Values are preserved. Only the location of the data changes.
Modifications to Plant Input Data. The following change was made to plant data:
1. Chiller Plants - Condenser pump performance data was moved from the cooling tower inputs to the plant
inputs. During conversion the software automatically moves condenser pump performance data from the
linked cooling tower to the plant. There is only one situation where pump performance data is altered. If
multiple cooling towers are linked to a plant and different units of measure for pump performance (head,
kW, W/gpm, W/L/s) are used among the towers, units for the condenser pump associated with the first
linked tower will be used in the plant. Data for the pumps whose units do not match must be discarded.
Therefore it is important to check chiller plant data after conversion to correct any situations where
condenser pump data had to be discarded.
Modifications to Cooling Towers. One change was made to cooling tower data:
1. Condenser pump performance data was moved from cooling towers to the plant or system the tower was
linked to. No values were changed. Only the location of the data changed.
Modifications to Boilers. The following change was made to boiler data:
1. Boiler modeling features were expanded in v4.6. While no data for boilers from v4.5 was altered during the
conversion, defaults for the new boiler inputs were assigned. These include boiler type (hot water) and
design hot water supply temperature (180 F, 82.2 C).
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 14 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data from HAP v4.6 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data from HAP v4.7 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data from HAP v4.8 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data from HAP v4.6 Format
Converting HAP v4.6 to HAP v5.1. When converting data from v4.6 to v5.1 format:
a. Input data for all categories of data is preserved.
b. Design calculation results are not converted and must be regenerated in v5.1.
c. Simulation results are not converted and must be regenerated in v5.1.
d. Modifications to input data are made only to air system, plant, cooling tower and boiler data as described
in the "modification" sections below.
Modifications.
a. 2-Pipe Fan Coil air systems created in v4.6 will not automatically have changeover control options set
when data is converted. Changeover control will default to "not used". Users should review the inputs
for systems of this type to set changeover controls, if desired.
b. A new input, "average operating loss" was added to the chiller inputs. For chillers defined in v4.6, this
new input will be defaulted to zero when data is converted. Therefore it will have no effect on calculation
results. Users can edit chiller data and specify an operating loss, if desired.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting Data from HAP v4.7 Format
Converting HAP v4.7 to HAP v5.1. When converting data from v4.7 to v5.1 format:
a. Input data for all categories of data is preserved. No modifications to HAP v4.7 input data are made
during conversion.
b. Design calculation results are not converted and must be recalculated in v5.1.
c. Simulation calculation results are not converted and must be recalculated in v5.1.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting Data from HAP v4.8 Format
Converting HAP v4.8 to HAP v5.1. When converting data from v4.8 to v5.1 format:
Page 15 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm
Converting Data from HAP v4.9 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
Converting Data from HAP v5.0 Format
33.0 Converting Previous Version Data ›› 33.2 Converting HAP v4.x and v5.x Data ››
a. Input data for all categories of data is preserved. No modifications to HAP v4.8 input data are made
during conversion.
b. Design calculation results are not converted and must be recalculated in v5.1.
c. Simulation calculation results are not converted and must be recalculated in v5.1.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting Data from HAP v4.9 Format
Converting HAP v4.9 to HAP v5.1. When converting data from v4.90 or v4.91 to v5.1 format:
a. Input data for all categories of data is preserved. No modifications to HAP v4.90 or v4.91 input data are
made during conversion.
b. Design calculation results are not converted and must be recalculated in v5.1.
c. Simulation calculation results are not converted and must be recalculated in v5.1.
Procedure for Converting HAP v4.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Converting Data from HAP v5.0 Format
Converting HAP v5.0 to HAP v5.1. When converting data from v5.0 to v5.1 format:
a. Input data for all categories of data is preserved. No modifications to HAP v5.0 input data are made
during conversion.
b. Design calculation results are not converted and must be recalculated in v5.1.
c. Simulation calculation results are not converted and must be recalculated in v5.1.
Procedure for Converting HAP v5.x Data. For a description of the steps required to convert old program
data, please click the following link:
Converting HAP v4.x or v5.x Data
Copyright © 1999-2018 Carrier Corporation. All Rights Reserved.
Page 16 of 16
33.0 Converting Previous Version Data
3/5/2026
file:///C:/Users/User/AppData/Local/Temp/~hhE67.htm