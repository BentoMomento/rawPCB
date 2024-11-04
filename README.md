# rawPCB
A simple Printed Circuit Board that you can make at home safely, ANYTIME!

# Objective
I created an 1 Layer PCB with with embeded MCU (audrino and STM32) to simplely blink an led.

# Steps
1.  Schematic Design

      For this project I used easyEDA for simplicity
    ![image](https://github.com/user-attachments/assets/57668c73-78d7-47b1-9df7-f2bc9648e2df)
3.  PCB Layout

      I also used easyEDA for this part, achving about 0.3 mm of clearnce between drillholes, trace and copper filling region
    ![image](https://github.com/user-attachments/assets/bf595feb-4c67-402e-91d8-fa52bad33969)
5.  Lazer Printing

      I used a Lazer printer other than inkjet printer is because the material lazer printer used is toner powder, which will not react with the chemical mixure we are using for copper etching in step 7. We will be using a layer of letter size plain paper as a base and a piece of glossy paper in the centre of the base. The glossy paper could be magazine or news papers.
6.  Heat/Pressure compressing

      After done printing, place the copper board and the paper face to face, then pour enogh acetone on the paper until it covers the board. Compress the paper with a flat soft object for about 2 mins. then clean off the exccess paper by rubbing it in water.
7.  Copper etching

      WARNING: for the follwing step, please follow WHMIS
    use a glass container and mix about 1/3 of muriatic acid and 2/3 of hydrogen peroxide(this is a highly corrosive chemical). place the board into the mixure untill the PCB layout fully apears. carefully rise it with water can dry it.
9.  Soldering

      Before soldering, make sure to drill all the through holes with the right size of drill head. when soldering, make sure not to put too much solder as it might crate shorts and be hard to remove since we did not do masking.
10.  Debugging

      Debug the board and it will be ready to go! If you are using adurino mcus, most of them requires a boot loading process.
