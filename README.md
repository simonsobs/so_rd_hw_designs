# so_rd_hw_designs
For storing design and fabrication files for circuit boards and other hardware within the readout and detector working group in a version controlled way.

## 300K LNA hardware
Ultimately, the printed circuit board (PCB) and power supply box designs should live here.

### 300K LNA PCB
The directories under`300k_amp_ps_box/pcb` contain all the files necessary for editing, fabricating, and viewing the 300K LNA circuit boards.
`300k_amp_ps_box/pcb/Bottom_board` contains a picture of the electronics schematic for the bottom board, a .step file which is a 3D model of the bottom board, and the gerber files necessary to manufacture the bottom circuit board (under `Project_Outputs_for_Bottom_Board`).
This same exact structure exists under`300k_amp_ps_box/pcb/Top_board` but instead describes the Top board of the 300K LNA PCB. In addition, [here are the assembly documents for both Top and Bottom boards](https://docs.google.com/presentation/d/1A_KDBGtZD-UfWHo1MMT_YvrvhtoMr0XffyKuqTHIMP8/edit?usp=sharing) 

#### Editing and Viewing the 300K LNA PCB with Altium
The user should copy the contents of the "altium_files" directory and place them into the directory in which their copy of Altium lives. Specifically, the user should:
  1. Copy all _directories_ under `300k_amp_ps_box/pcb/altium_files/Projects` into their Altium/Projects directory. 
  2. Place all files in `300k_amp_ps_box/pcb/altium_files/Library/ExportIntLib` into their Altium/Library/ExportIntLib directory OR just copy and place the ExportIntLib directory under User/Path/to/Altium/Library. 
  3. Open Altium and navigate to Open Project
  4. Open `300k_amp_filtered_PS_supply` to see the entire PCB project. The Top and Bottom board projects exist because the 300k_amp_filtered_PS_supply _composed of_ the two smaller projects: `Top_board` and `Bottom_board`.
  5. User should now be able to view and edit the boards. User can reference [The Altium tutorial documents](https://www.altium.com/documentation/altium-designer/tutorial-complete-design-walkthrough) for a quick guide to make edits within Altium. 
