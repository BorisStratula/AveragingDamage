APDL script to perform numerical fatigue estimates based on a fatigue damage theory.

## General information
A fatigue damage theory from [1, 2] is implemented for Ansys using the APDL script. To obtain consistent results independent of the mesh size, an averaging algorithm from [3] is implemented over the equivalent stress field.

## Usage
The code is intended to be used in Ansys Workbench environment.
The following steps are recommended to use the code:

1. Copy all script files to your local machine

2. Set the path to the script files, line 4 in Main.mac

3. Set the desired number of load steps, line 29 in Main.mac

4. Set material properties such as Young's modulus and fatigue limit, lines 47 and 63-65 in Main.mac

5. Create a static structure project in Ansys Workbench

6. Add geometry and apply boundary conditions

7. In the static structure, right next to the boundary conditions, insert 'commands' script and import Main.mac

8. Execute the solution using the GUI

9. After completion, check the results in project_folder/project_folder_files/dp0/SYS/MECH/, all text data will be saved in solve.out under the title 'debug info'.

## References
[1] https://link.springer.com/chapter/10.1007/978-981-33-4826-4_12
[2] https://www.researchgate.net/publication/350059424_Multi-mode_Model_and_Calculation_Method_for_Fatigue_Damage_Development
[3] https://www.sciencedirect.com/science/article/abs/pii/S0749641921001339?via%3Dihub
