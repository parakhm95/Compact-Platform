.. Compact Platform documentation master file, created by
   sphinx-quickstart on Fri Jun 21 15:59:38 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Assembling the Drone
=================================================================

1. Chassis Assembly
--------------------


#. Take the chassis, and the following components : 
	* M3 X 6 X 6 Plastic Standoffs : 4 units.
	* Vibration Washer : 4 units - 1.66 mm thick.
	* M3 X 10 screws : 4 units - Plastic or Metal
	* Sorbothane Vibration Dampeners : 4 units. 

	.. list-table:: Step 1.1
		:widths: 300
		:align: center
		:header-rows: 0
	
		* - .. figure::
				../Images/1.JPG
				:scale: 10 %



#. Sandwich the sorbothane dampeners between the chassis and the vibration washer by screwing from the bottom of the chassis into the M3 Standoff and tighten until it looks like the picture shown below :


	.. list-table:: Step 1.2
	   :widths: 300 300 300
	   :align: center
	   :header-rows: 0
	
	   * - .. figure::
	           ../Images/2_a.JPG
	           :width: 150 px
	           :height: 200 px
	     - .. figure::
	           ../Images/2_b.JPG
	           :width: 150 px
	           :height: 200 px
	     - .. figure::
	           ../Images/2_c.JPG
	           :width: 150 px
	           :height: 210 px



#. Desolder the XT60 plug from the DYS, and solder the XT30 plug with 16 AWG wire.

	.. list-table:: Step 1.3
	   :widths: 300 300 300
	   :align: center
	   :header-rows: 0
	
	   * - .. figure::
	           ../Images/3_a.JPG
	           :width: 150 px
	           :height: 200 px
	     - .. figure::
	           ../Images/3_b.JPG
	           :width: 150 px
	           :height: 200 px
	     - .. figure::
	           ../Images/3_c.JPG
	           :width: 150 px
	           :height: 200 px



#. Mount the DYS on the chassis on top of the M3 standoffs from Step 1. **Orient the DYS such that the arrow on the PCB points to the forward side of the chassis.** Secure it using M3 X 8 X 6 standoffs on all four sides.

	.. list-table:: Step 1.4
		:widths: 300 300
		:align: center
		:header-rows: 0

		* - .. figure::
				../Images/4_a.JPG
				:width: 150 px
				:height: 200 px 
		  - .. figure::
				../Images/4_b.JPG
				:width: 150 px
				:height: 200 px

#. Using a M2 X 8 screw, mount the motors, propeller guards, and the quadrotor feet to the chassis, layered in the following order from top to bottom:
	* Motor
	* Chassis
	* Propeller guard
	* Quadrotor foot
   
   Orient the motor's wires such that they align with the arm of the chassis.

	.. list-table:: Step 1.5
		:widths: 300
		:align: center
		:header-rows: 0
	
		* - .. figure::
				../Images/5_a.JPG
				:scale: 10 %

#. Solder the motor wires to the DYS as shown below. Use any order of the wires for now, we will check for rotation direction later.


	.. list-table:: Step 1.6
		:widths: 300
		:align: center
		:header-rows: 0
	
		* - .. figure::
				../Images/6_a.JPG
				:scale: 10 %

1a. Frame Assembly
^^^^^^^^^^^^^^^^^^^
	
	#. Collect the top frame plate and a set of magnet holders.
	
		.. list-table:: Step 1a.1
			:widths: 300 300
			:align: center
			:header-rows: 0
	
			* - .. figure::
					../Images/1a_1_a.JPG
					:width: 150 px
					:height: 210 px 
			  - .. figure::
					../Images/1a_1_b.JPG
					:width: 150 px
					:height: 210 px

	#. Using M3 X 10 screws and M3 Nuts, screw the magnet holders onto the top frame plate such that the flat side is screwed to the top frame plate and the curved edges are facing away from each other. Insert the nuts in the grooves of the magnet holder. Refer to the picture below:

		.. list-table:: Step 1a.2
			:widths: 300
			:align: center
			:header-rows: 0
	
			* - .. figure::
					../Images/1a_2_a.JPG
	           		:scale: 10 %

	#. Take a Propeller bar and a Tag mount and connect them to each other by pushing the tag into the notches or slots of the propeller bar. **You need to repeat this twice so as to obtain 3 of these subassemblies.**

		.. list-table:: Step 1a.3
			:widths: 300
			:align: center
			:header-rows: 0
	
			* - .. figure::
					../Images/1a_3_a.JPG
					:scale: 10 %

1b. Mating Frame and Chassis.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

	#. Now you have the following subassemblies to mate with each other:
		* Propeller bar and Tag mount subassembly X 3.
		* Frame subassembly.
		* Chassis subassembly.

		.. list-table:: Step 1b.1
		   :widths: 300 300 300
		   :align: center
		   :header-rows: 0
		
		   * - .. figure::
		           ../Images/1a_3_a.JPG
		           :scale: 5 %
		           :align: center
		     - .. figure::
		           ../Images/1a_2_a.JPG
		           :scale: 5 %
		           :align: center
		     - .. figure::
		           ../Images/6_a.JPG
		           :scale: 5 %
		           :align: center

	#. Mate the subassemblies such that the propeller bar is attached at the bottom of the propeller guard while the magnet holders sit on the propeller guard. Use M3 X 10 screws and M3 Nuts to mate the magnet holders with the propeller guard. 

		**Mount the 'propeller bar and tag subassembly' to only three sides of the chassis viz. back, left, and right. The front of the robot is left open for the camera. A propeller bar can be mounted to the front if desired.**

		*One of the tag mounts is missing on the right but should be on your build.*

		Refer to the pictures below:

		.. list-table:: Step 1b.2
			:widths: 300 300
			:align: center
			:header-rows: 0
	
			* - .. figure::
					../Images/1b_2_a.JPG
	           		:scale: 5 %
			  - .. figure::
					../Images/1b_2_b.JPG
	           		:scale: 5 %

	#. Result of the mating :

		.. list-table:: Step 1b.3
			:widths: 300
			:align: center
			:header-rows: 0
	
			* - .. figure::
					../Images/1b_3_a.JPG
					:scale: 10 %

7. Take the Pixfalcon/Pixhawk Mini and mount it on top of the M3 standoffs securing the DYS ESC. Take M3 X 8 X 6 standoffs and lock the Pixfalcon in place. **Remember to align the Pixfalcon such that the arrow faces to the front of the robot.**

	.. list-table:: Step 1.7
		:widths: 300
		:align: center
		:header-rows: 0
	
		* - .. figure::
				../Images/7_a.JPG
				:scale: 10 %


#. Take M3 X 5 X 6 standoffs and screw them into the outermost holes of the Raspberry Pi 3 A+ mount plate using M3 Hex Nuts. Mount the plate on top of the Pixhawk board such that the standoffs face upwards. Use M3 Hex Nuts to secure it. Mount the Raspberry Pi 3 A+ board on top of the plate to finish the stack. Use M3 X 6 screws to secure it in place.

	.. list-table:: Step 1.4
		:widths: 300 300
		:align: center
		:header-rows: 0

		* - .. figure::
				../Images/8_a.JPG
				:scale: 5 % 
		  - .. figure::
				../Images/8_b.JPG
				:scale: 5 %





