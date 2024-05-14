# EXP.NO:06
# DATE  :22/04/2024

# SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

**AIM:**

To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

**APPARATUS REQUIRED:**
 
⦁	Laptop with MobaXterm

⦁	Cadence tool

**PROCEDURE:**

**SCHEMATIC ENTRY:**

**Creating a new library:**

⦁	In the library manager, execute File - New library. The new library form appears.
⦁	In the new library form, type ‘my design lib’ in the name section.
⦁	In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
⦁	In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
⦁	In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
⦁	After creating a new library you can verify it from the library manager.
⦁	If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

**Creating a schematic cell view:**

⦁	In the CIW or library manager, execute file – new – cell viw.
⦁	Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
⦁	Click ok when done the above setting. A black schematic window for the inverter design appears.

**Adding components to schematic:**

⦁	In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
⦁	Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
⦁	After you complete the add instance form move your cursor to the schematic window and click left to place a component.
⦁	This is a table of components for building the inverter schematic.
⦁	After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.


![329846808-f5f632bf-813c-49b8-9560-e003735a039b](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/1064f72f-493b-4ab5-ab91-b7a20645361a)

**Adding pins to schematic:**

⦁	Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
⦁	Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.
⦁	Select cancel and then the schematic window enter window file or press the f bind key.

**Adding wires to schematic:**

⦁	Click the wire (narrow) icon in the schematic window.
⦁	In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
⦁	Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
⦁	Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

**Saving the design:**

	Click the check and save icon in the schematic editor window observe CIW output for any errors.

**BUILDING THE INVERTER TEST DESIGN:**

**Creating the inverter test cell view:**

⦁	In the CIW or library manager, execute file – new – cell view.
⦁	Setup the newfile as shown below.
⦁	Click ok when done. A blank schematic window for the inverter test design appears.
⦁	Using the components list and properties/ comments in this table build the inverter test schematic.
⦁	Add the above components using create – instance or by pressing I.
⦁	Click the wire (narrow) icon and wire your schematic.
⦁	Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
⦁	Click on the check and save icon to save the design.

![329847018-4d10ff4d-985f-4bb3-9b23-df5c6bd43d00](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/65b9b65a-ccb4-4b6d-8374-d04fd4f43377)


**ANALOG SIMULATION WITH SPECTRA:**

**Starting the simulation environment:**

⦁	In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears.
Choosing a simulator:
⦁	In the simulation window (ADE) execute setup – simulator / directory / host.
⦁	In the choosing simulator form, set the simulator field to specra and click ok.
⦁	In the simulation window (ADE) execute the setup model libraries.
To complete, move the cursor and click ok.

**Choosing Analysis:**

⦁	Click the choose- Analysis icon in the simulation window (ADE).
⦁	The choosing analysis form appears.
⦁	To Setup the transient analysis.
⦁	In the analysis section select tron.
⦁	Set the stop time as 100ns
⦁	Click at the moderate or enabled button and the bottom and then click apply.
⦁	To set for DC analysis
⦁	In the analysis section select DC.
⦁	Turn on save DC operating point.
⦁	Turn on the component parameters.
⦁	Double click the select Vpulse source or Type V0 (capital V zero).
⦁	Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8.
⦁	Select the enable button and click apply and then click ok.

**Selecting output for plotting:**

⦁	Execute the o/p’s to be plotted  -select on sschematic in the simulation window.
⦁	Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

**Running the simulation:**

⦁	Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
⦁	When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.


![329847153-bec78f49-0b22-4012-8267-e61dcb2c1918](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/d90dd416-8069-4d01-8deb-686031c47eba)


![329847193-f5382e05-7e36-445a-b4a9-607642df73db](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/573d80a1-c721-493a-9acd-56d8066248eb)

**CMOS NAND GATE**

**NAND SCHEMATIC**

![329847300-7eccb786-06d1-4edc-8b0f-727d1f1ae022](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/3dd202e7-b5f6-49c6-ae6e-d2edfcc5a4b0)

**NAND TEST CELL VIEW**

![329847432-96c32b28-0060-40bf-9bce-e215442026a6](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/5ff945f7-42e8-477a-9b35-5b99f6fc6a98)

**NAND SIMULATION WITH SPECTRA**

![329847456-ef51f28a-43e9-4b3c-9aa5-f02153a93954](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/e13a4c6f-fd77-40ed-a5b8-7bfabf88dc43)

**CMOS NOR GATE NOR SCHEMATIC**

![329847489-090388f6-e981-4d94-957e-137b13aa0789](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/9f396f05-cdf1-453b-8aae-b3b93a2fdf0e)

**NOR TEST CELL VIEW**

![329847537-03dafb60-7956-4601-be8e-c539280bdcc8](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/5cf4eced-68ce-4225-8fba-218b59d505e3)

**NOR SIMULATION WITH SPECTRA**

![329847572-23cc1bd8-8598-4aa1-ba7d-a3d86c0315f2](https://github.com/KarthikeyanManickam/VLSI-LAB-EXP-6/assets/164841362/c64df7ed-5c76-4633-acad-68ec0865eef9)

**RESULT:**

Thus the design and simulation the CMOS inverter and observe the DC and transient responses using cadence tool is verified successfully.






