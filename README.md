# Programming and control system optimization for In-House Hydroelectric Power Plant Setup  
The idea here is to program controls for a very CRUDE hydroelectric power plant. We start with a base program that simulates a changing environment and manages our analog input signals accordingly. Our job is to write a program that incorporates these signals and controls various analog and digital devices in order to run the system with a safe and stable process. We also want to create an HMI that will allow the Operator to interact easily and effectively with our system.  

- The entire plant control code is programmed in both ladder logic and functional block diagram, which gives the operator liberty to alter code however he sees fit.
- Hand-Off-Auto [HOA]: Give the Operator control over all devices to include manual setpoints for analog devices.
    

I have been using the PLC IEC-61131-3 language such as:  
- FBD - Function Block Diagram
- LD - Ladder Diagram
  
  
CPU : Siemens S7-1511 F-1 PN __[Fail safe CPU]  
HMI : WinCC RT advanced

Inputs:-
1. Baffle
2. Oil Pump VFD
3. Rotor Speed
4. Power Station Interlock
5. Generator Brake

Alarm Conditions:-
1. Overcurrent
2. High Oil Temp
3. Rotor Overspeed
4. Oil Low Flow
5. Oil High Flow
6. E-Stop
7. Brake Failure

- Main [OB]

  ![Screenshot (60)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/ad0d21a2-af47-45d0-a96c-ee9cd4684481)

  ![Screenshot (61)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/a8849cc3-7686-44c1-9438-1ab6f3695c25)
  
  ![Screenshot (62)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/513de3cb-e2f0-457f-b49e-bba6b1530377)

- Ladder Diagram:-
    
  -  Digital Output:
      
      ![Screenshot (63)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/39bd29cd-3bb7-4218-acb2-06fb956071bb)
     
  - Analog Output:

      ![Screenshot (64)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/23b47d69-08db-4033-9b8d-119d340c3945)

  - Analog Input:
      
     ![Screenshot (65)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/862d72ea-c5d8-4c90-8e1b-d9317f8453a1)

  - Hand-Off-Auto:

    ![Screenshot (66)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/affdc855-2384-4c13-840d-22d7bdb58726)

    ![Screenshot (67)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/617993c0-2766-4bf0-8d30-2229e5070b6f)

  - Alarms:

    ![Screenshot (69)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/002990cc-0065-44bf-bfc2-7cc0ed03a66a)

    ![Screenshot (70)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/1ed09395-43a7-4a72-ace6-f2bb60906312)

- Functional Block Diagram :-
    
    - Inputs and Outputs:

      ![Screenshot (71)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/61c68e22-ca9d-413c-b3dc-514639a2dcb2)

    - Hand-Off-Auto:

      ![Screenshot (72)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/fc5a4cd4-630e-48d5-8e93-78d185b7a65f)

    - Alarms:

      ![Screenshot (73)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/aa73277d-6387-47ef-aaba-eddcbd19a941)

      ![Screenshot (74)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/7fde03fa-6be9-4984-94ac-18dcf32f1a2c)

- HMI:

    ![Screenshot (77)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/09e70ac9-47bc-4a80-95f0-023b9b9f5c2d)

    ![Screenshot (78)](https://github.com/riitesh07/Programming-and-control-system-optimization-for-In-House-Hydroelectric-Power-Plant/assets/68095076/4153d779-681a-4c0d-8094-e3f062285b33)







    





