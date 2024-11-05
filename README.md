# rawPCB
A simple Printed Circuit Board that you can make at home safely, anytime!

# Objective
Create a single-layer PCB with an embedded MCU (Arduino or STM32) to simply blink an LED.
Depending on the quality of the printer, you can achieve clearance down to 0.3 mm. For this project, all clearances are around 0.35 mm.  
In addition, I also made a layer of solder mask, although I did not include the steps here. However, there is a photo showing the solder mask part in the `images` folder.

# Steps
1. **Schematic Design**  
   For this project, I used EasyEDA for simplicity.  
   ![Schematic Design](https://github.com/user-attachments/assets/57668c73-78d7-47b1-9df7-f2bc9648e2df)

2. **PCB Layout**  
   I also used EasyEDA for this part, achieving about 0.3 mm of clearance between drill holes, traces, and the copper fill region.  
   ![PCB Layout](https://github.com/user-attachments/assets/bf595feb-4c67-402e-91d8-fa52bad33969)

3. **Laser Printing**  
   I used a laser printer instead of an inkjet because laser printers use toner powder, which does not react with the chemical mixture we use for copper etching in Step 7. We’ll use a layer of letter-sized plain paper as a base, with a piece of glossy paper (magazine or newspaper) in the center.  
   ![Laser Printing](https://github.com/user-attachments/assets/701a5094-3f8f-4a00-8cbd-9fbc787d1fb9)

4. **Heat/Pressure Compressing**  
   After printing, place the copper board and the printed paper face-to-face. Pour enough acetone on the paper until it covers the board. Press the paper with a flat, soft object for about 2 minutes, then remove the excess paper by rubbing it under water.

5. **Copper Etching**  
   **WARNING:** For the following step, please follow WHMIS guidelines.  
   Use a glass container and mix approximately 1/3 muriatic acid with 2/3 hydrogen peroxide (a highly corrosive chemical). Place the board into the mixture until the PCB layout fully appears, then rinse it carefully with water and dry it.  
   ![Copper Etching](https://github.com/user-attachments/assets/91c75ff5-950d-4692-93ed-b401c29c1965)

6. **Soldering**  
   Before soldering, ensure you drill all the through-holes with the correct size drill bit. Be careful not to apply too much solder, as it might create shorts that are difficult to remove since we are not using solder masking.  
   ![Soldering](https://github.com/user-attachments/assets/0b811fb6-ba92-4265-9897-0616097906ac)

7. **Debugging**  
   Debug the board, and it’s ready to go! If you are using Arduino MCUs, note that most of them require a bootloading process.
