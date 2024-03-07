# 3D Printing Procedures
## Getting Started
1. Install PrusaSlicer from https://www.prusa3d.com/page/prusaslicer_424/
2. Configure the following
    1. Prusa FFF:
        1. Prusa i3 Mk3s w/ 0.4 mm nozzle
    2. Filaments:
        1. Prusament PLA
        2. Prusament PETG
        3. AmazonBasics PLA
3. Always return to defaults
4. Discuss model layout (auto-arrange)
    1. Instances
    2. Spacing
    3. .3mf vs .stl
3. Discuss layer heights and speeds
4. Discuss supports
5. Discuss infill percentages
6. Discuss brims
7. Discuss heterogenous configurations
8. Discuss gcode warnings and how to resolve
9. https://e4e-octopi.dynamic.ucsd.edu discussion
10. Slice and print https://www.3dbenchy.com/ or other pending (draft) job

## Slicing Procedure
1. Obtain a .3mf or .stl file to print
2. Load into PrusaSlicer
3. Configure the appropriate parameters
    1. Instances
    2. Spacing/Orientation
    3. Layer heights/quality
    4. Supports
    5. Infill
    6. Brims
4. Save project to \\e4e-nas.ucsd.edu\hardware-dev\print_archive as `%Y-%m-%d {project} {print name}.3mf`
5. Slice the project
6. Review g-code messages
7. Export g-code to \\e4e-nas.ucsd.edu\hardware-dev\print_archive as the default name

## Printing Procedure
1. Open https://e4e-octopi.dynamic.ucsd.edu
2. Log in
3. Upload the g-code
4. In the `Control` tab, verify that the bed is clear
5. In the `Files` section, locate the g-code file that you just uploaded
6. Load and print the file
7. Monitor status in [#3d-printing](https://ucsde4e.slack.com/archives/CKKA4LPS8)

## Print Completion Procedure
1. Open https://e4e-octopi.dynamic.ucsd.edu
2. Log in
3. Enter the filament usage data
4. Click `Save`
5. Gently remove the prints from the print plate
6. Replace and clean the print plate

## Filament Change Procedure
### For users
On filament runout:
1. Discard previous spool
2. Open new spool
3. Take a picture of the spool information (Brand, material, diameter, color, weight, lot number) and put it in the [#3d-printing](https://ucsde4e.slack.com/archives/CKKA4LPS8) channel in Slack
4. Open OcotoPrint and copy the current filament usage into the 3d-printing channel in Slack
5. Follow the instructions on the Prusa i3 mk3 to unload the old filament and load new filament
