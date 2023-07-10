# MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7
This Project includes step-by-step guide for running a uart demo on the Microblaze soft core processor from AMD(Xilinx) on CMOD ARTIX-A7 FPGA .
before getting started , make sure you are having the following the below requirements-:
1. Xilinx VIVADO (could be any version -preferably later than 2019.2)
2. Xilinx VITIS  (remember , this has to be same as the vivado verison)..
   (instead of downloading Xilinx VIVADO , just install Xilinx VITIS tool , in which there you can select Vivado to be pre-installed )...
3. CMOD-ARTIX-A7 FPGA ( you can have any other from ARTIX family , or maybe spartan-7 , but then you have to select the same)
4. USB-cable

  if you are done all of the those , then let's go ahead .... 

1. Launch VIVADO
   give a suitable name to project ..
   
![01](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/325a7fe1-4f17-4051-820b-4de77aa4c2ff)


2. In next step , make sure you have board files installed , you just have to copy the
    files from repository , and paste in --: E:\VITIS_2020.2\Vivado\2022.2\data\boards\board_files


   in some case there would not be board_files folder , so you may create the same for that.
   Now select your FPGA board , in my case -- it's CMOD-ARTIX_A735T
   
![2](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/e898d763-95b6-4ac7-8469-0e35469d7924)

3. Click Finish

   ![3](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/94382b1b-4e58-4938-925b-d064290aa3cd)

4.click on -- " create bock design in IP integrator section"
  give a name to this one as well.
  
  ![4](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/6eb0fe07-8c3c-493a-a199-14119561180a)

5. Now , if you do not see the board file section , then click on window , then click-on-boards
   you'll then be able to see the all board tab .


   
   ![5](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/5184c8eb-0c50-443a-a04a-84daac505da8)

