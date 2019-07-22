#README

This Directory Serves To Store directions and specifications about electrical components of the microscope setup.

IMPORTANT Point about Schematics and EagleCAD:

	Schematics were created in EagleCAD free version.  These schematics make use of 3rd party libraries provided
        by sites like Element14 and handdrawn library parts based off of datasheets when not found.

	Opening a Schematic In EagleCAD:

		Since the free version of EagleCAD seems to limit all projects to the specific eagle/ folder designated
		 by the program on Install, it is recommended to move the schematic to this directory if intending to do 
		 work on the underlying schematic or pre-Gerber pcb board layout.

		In order to have access to the libraries, from the Eagle Control Panel: 
				Right click Libraries -> Library Manager
				Upper left Tab -> Available
				Browse -> Search for each library in EagleLibraries
				If the library is new it will be added in the Available dialog
				Click on the desired library and click Use button
				You should now see the library in the In Use Tab

Directory Layout:
	|
	|
	| ------- EagleLibraries/
	|		|	:Since Schematics were created in EagleCAD (freeware edition), additional libraries are housed here
	|		|
	|		|
	|		| ------- 3rdParty/ 
	|		|		: Part libraries that were imported from 3rd Party distributors.  See About.txt if wanting to look up revisions.
	|		|
	|		|
	|		| ------- HandCreated/
	|				: Parts that were created from Manufacturer DataSheets by individuals.  
	|				   Add the file name to Confirmed.txt when a pcb footprint has been used and verified.
	|
	|
	| ------- USB_TO_ILDA_Adapter/ 
	|		|	: Electronics for using ILDA device as a laser illumination source
	|		|
	|		|
	|		| ------- (Version) /
	|				|	:See About.txt for Version Different highlights
	|				|
	|				|
	|				| ------- Schematics/
	|				|		: Electrical Connection Schematics
	|				|
	|				|
	|				| ------- Gerber/
	|				|		: Gerber Files for PCBs that have been proven 
	|				|
	|				|
	|				| ------ DataSheets/
	|						: DataSheets Related to important components (ICs at the very least)
	|				
	|
	| ------ USB_TO_RS485_Connection/
	|		|	:Electronic connector and connections for RS-485 Comm with OrientalMotors CRPK
	|		|
	|		|
	|		| ------ Schematics/
	|		|		: Electrical Connections (Since this is a non-standard connection)
	|		|
	|		|
	|		| ------ DataSheets/
	|		|		: DataSheets related to important Components (motor controller and USB adapter)
	|		|
	|		|
	|		| ------ Figures/
	|				: Explanations for adapting the non-standard connection
	|		
	|
	| ------ Power_Supply/
			|	:Electrical connections for using Wall Power to provide stable voltage to OrientalMotors CRPK
			|
			|
			| ------ Schematics/
			|		: Electrical Connections (For pins to terminals etc.)
			|
			|
			| ------ DataSheets/ 
			|		: DataSheets related to important components
			|
			|
			| ------ Figures/
					:Explanation for making connections if there is a difficulty
