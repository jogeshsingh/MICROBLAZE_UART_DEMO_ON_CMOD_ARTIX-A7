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

6. drag the clock wizard from board section --to block interface

  ![clock_6](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/6ca0dd16-c3e5-4a18-a9d4-30711ffee793)


7. click on " + " sign in board interface , then write microblaze , select the microblaze by
   double-click .

   ![microblaze7](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/93f11589-6d8a-42a8-a3a2-44c2a3ab8056)

 8. Now  , you'd be able to see the microblaze soft core IP in block interface ,
     "run block automation"

     ![block_automation_8](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/e869e4b8-a2d9-445d-b0d2-143e8c2d3059)

9.   set the following parameters as default.

   ![9](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/76ad967b-cc21-4856-8611-4461ca3af6bb)

 10. Now drag USB UART and cell RAM .

   ![10_uart_cell_ram](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/a6fbd575-51f6-45ca-9c43-140f213ac459)

11.  "Run connection automation"

  ![11_run_connection_automation](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/e792664d-7849-42f8-b996-43f541e0b551)

12. here's the final diagram created in block interface .

     ![12_final](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/5fba99d6-a11c-4bb6-952d-a86fcbfe019d)

 13. Now save the block diagram    
     file -> save_block_design

     ![13_save_bd](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/a74cfef5-06de-4354-83dd-7b4c4fc16ea6)

 14. Now Export Hardware--including bitstream
          
      ![export_hardware](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/9287ee0d-dbb6-4603-bd69-11b48a274b23)

      ![include_bitstream](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/f7a19716-4cea-49ac-b1cf-da72f262fa5a)

15. Remember to save this XSA FILE --in location--you'd be able to remember later

      ![XSA_FILE_LOCATION](https://github.com/jogeshsingh/MICROBLAZE_UART_DEMO_ON_CMOD_ARTIX-A7/assets/98607828/b77375a9-a049-4076-aadb-73c8cd373ec9)

 # Now Let's move to VITIS
 
    

   
   


