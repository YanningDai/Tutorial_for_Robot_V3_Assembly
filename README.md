# Robot V3 Assembly Guide

## Step 1 - Preparing the PCB

1. Cut four wires on PCB's surface with a knife, like this: 

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/bd36a766-ff9f-4779-8949-294a7c9edfff" width="600">

&emsp;&emsp;Check with Mohanned or Joel to confirm which wires to cut.

&emsp;&emsp;(Hereafter, this board will be referred to as the PCB.)

2. Solder the Voltage Transformation Module to the PCB:

  - First, check the voltage ouput. Apply a 12V input voltage and adjust the screw to set the output to 5V (acceptable range is 4.9-5.1V).
  
  - Next, solder the power module to the PCB in the position shown below:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/dec340f3-c9d3-4464-ae50-058d3950cae0" width="600">

&emsp;&emsp;(The power module is located at the bottom left corner, with four pins.) 

  - Solder Power Wires to the PCB:

&emsp;&emsp;Use one red and one black wire, each approximately 29cm long. Solder these wires to the power input terminals on the PCB:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/8fd229ac-c97e-4493-a5b1-480f7cadda20" width="600">

&emsp;&emsp;Ensure that you use protective tubes on all solder joints, as demonstrated with the black wires.
  
## Step2 - Assembling the Mechanical Structure of the Robot Arm

For each robot arm, you will need:

  1) 3D-printed components: Two of each type shown below
​	
&emsp;&emsp;<img src="https://github.com/user-attachments/assets/3d6047cd-43ff-402f-b261-6be4426f60aa" width="600">
​	
  3) 8 motors and 8 cameras

  4) 8 3D-printed threaded heads

  5) 4 spring tubes, each 30 cm long (refer to Video 1 for cutting instructions).

Assembly Steps:

1. Assemble arm segment:
   
&emsp;&emsp;Each robot arm consists of two segments, and each segment requires the assembly of two 3D-printed components. Secure these components with 4×8 screws. 
   
&emsp;&emsp;<img src="https://github.com/user-attachments/assets/2782f0c6-4df4-4301-8ea7-d70f728215cb" width="600">

2. Assemble mtors: 
  
&emsp;&emsp;Secure 4 motors on each arm segment. Each motor needs 2 small screws. 
  
&emsp;&emsp;Choose longer screws for stability:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/15c037f0-e7ae-437b-84f9-1b74ec1933ee" width="600">

&emsp;&emsp;Arrangement of the motors:
  
&emsp;&emsp;<img src="https://github.com/user-attachments/assets/f9d9e91c-113f-4140-90f0-c63296bcef9d" width="600">

3. Assemble tubes and the remaining 2 components: 

&emsp;&emsp;Position them as shown below. Then, tighten each of the two outer components with four screws at each corner.

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/f8b6c5bd-439c-48f6-8b01-db760e4ede18" width="600">

4. Assemble cameras (4 cameras and 8 screws for each segment)

5. Insert the 3D-printed threaded heads (4 for each segment)

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/41d7d0e5-a643-4ea1-9787-adc60d8096a6" width="600">

6. Attach the End Connector to the Square Plate (with 2 srews)

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/9f750724-c11a-488f-930a-64fd96f491d9" width="600">

## Step3 - Assembling the Circuitry for the Robot Arm

For each robot arm, you will need:

  1) 2 PCBs and 8 ESPs

  2) Pin converters for the PCBs: 4 red and 4 blue converters
     
  4) Connecting Wires: 2 types, 4 wires for each type (see the images below)

  5) Wires and boards for limit switch (he installation for this module is not included here; please consult Mohannad for details)

Assembly Steps:

1. Attach pin converters to PCBs:

&emsp;&emsp;4 converters for each side, alternating in color (blue, red, blue, red).

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/843e6b28-e932-464d-a36d-c6da7e5151bd" width="600">

2. Connect Cameras and Motors from arm segments to the PCBs: 

&emsp;&emsp;Follow the connection scheme below:

&emsp;&emsp;The joint closest to the end of the robot arm is the first segment, and the one closest to the base is the second segment.

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/a976d87f-0d27-4549-8414-231fd14633f6" width="600">

&emsp;&emsp;The PCB connected to the second segment is called the bottom PCB (later fixed to the top of the square box), while the PCB connected to the first segment is the top PCB. Each joint has four cameras/motors, numbered as follows:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/7eacdb7c-7ab9-4a35-acaa-a91f53dfb1d2" width="600">

&emsp;&emsp;(The limit switch is connected to camera/motor 2; the others are numbered counterclockwise.)

&emsp;&emsp;The final wiring configuration should look like this:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/824c603f-5931-4c36-8208-0142b44bad7b" width="600">

&emsp;&emsp;(Note: The PCB connected to the first segment needs to be flipped over when fixed to the box, rotated 180 degrees.)

3 Secure the PCBs to the Box: 

&emsp;&emsp;Use screws to secure the two PCBs to the top and bottom of a 3D-printed square box, using three screws per PCB.

## Step4 - Assembling the Power and FPGA Components

For each robot arm:

1. Assemble the Power Module:

&emsp;&emsp;Secure the Ethernet cable and the power adapter with screws.
    
&emsp;&emsp;<img src="https://github.com/user-attachments/assets/6f41c4ef-eb74-4502-a169-aacc185ddd71" width="600">

&emsp;&emsp;Take one black and one red power wire, process both ends as shown, and insert them into the power adapter.

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/4d9990b4-8044-4bdd-8ce4-d8b50536835a" width="600">

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/d060f6da-0162-47e3-9aaf-f7d383c11bd5" width="600">

&emsp;&emsp;Cut both ends with wire cutters, attach protectors at the end, and crimp them (ps. these are 12 V wires for powering the motor).

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/5c86cfc0-981c-4d49-8e84-bbf3d3a82d8a" width="600">

2. Attach the Beam to Power Module box:

&emsp;&emsp;Melt and embed two threaded inserts into the beam (see Video 2).
   
&emsp;&emsp;Use screws to secure the beam to the power module box in the position shown:

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/c46cbcc9-697a-4f33-8560-ff3afe52a364" width="600">

&emsp;&emsp;Assemble the power board onto the beam with screws; placing the FPGA underneath it, between the bottom PCB and the power board.

&emsp;&emsp;(Temporary note: I'm not sure about the name of this board, and it’s currently referred to as the power board.)

3. Solder 5V power wires:

&emsp;&emsp;For each PCB, we need two wires:

&emsp;&emsp;- Short Wire: Solder together two wires, one 10 cm and one 5 cm.
    
&emsp;&emsp;- Long Wire: Solder together two wires, one 15 cm and one 5 cm. Note: Reverse the black and red wires because the board has an inverted wiring sequence.

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/566015bf-98cb-4a45-99ea-bc54ed4f1c7c" width="600">

&emsp;&emsp;Make sure to slide small protective tubes onto the wires before soldering, and then shrink the tubes with hot air.

&emsp;&emsp;Then, connet the power wires to boards. Each wire have different connections at two ends:

&emsp;&emsp;- The short wire (without flipping): connects its larger end to the PCB and the smaller end to the power board on the beam.

&emsp;&emsp;- The long wire (flipped): connects its larger end to the PCB and the smaller end to the FPGA.
    

4. Connect the Remaining Wires:

&emsp;&emsp;On the FPGA, there is a 2*2 set of female headers; connect only the two sets shown below. The outer header connects to the top PCB, and the inner header connects to the bottom PCB.

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/debffb37-44ad-4a1c-9072-65ebd33684ee" width="600">

&emsp;&emsp;Connect a short wire from the FPGA to the power board on the beam.
    
&emsp;&emsp;The limit switch wires connect to the power board.
    
&emsp;&emsp;Connect the FPGA to the Power Module box using an Ethernet cable.

5 Assemble all the Boxes and Finish!

&emsp;&emsp;<img src="https://github.com/user-attachments/assets/45910e75-31c0-40db-b924-5ee6647f510e" width="600">



