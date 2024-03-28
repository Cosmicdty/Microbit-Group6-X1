
> Open this page at https://makecode.microbit.org/#editor

## You can view or edit this project


To edit this repository in Microbit MakeCode.😇


* open https://makecode.microbit.org/#editor
* Instructions on how to use this code：💭
1. We can see the far left side of the code, configuring the initial settings for Neopixel and OLED in the start module.👇

    ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/de360803-fae2-4e06-b50f-7cca846fe6eb)

2. The below code module is the text that turns on the OLED by pressing button A, displays the N-shaped logo and starts by pressing the button.👉

   ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/9f6a9239-21e9-477e-bd64-05ee3231afc1)
   ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/4b8618e4-f1a0-4a71-9d2d-04b4978de1ef)

3. Then next to the right, cycle through the Forever module to read the data on pin 2 (pin 2 is connected to the pulse sensor for heart rate measurement). 👇
 
  ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/d4187a18-f540-44ab-bd0f-df9da93f5552)
 
4. This is followed by pressing button B to clear the screen before displaying icons and heart rate on the OLED, as well as step-by-step text for the inhale, hold, and exhale phases. Finally, the display is switched off 10s after the end of the process.👉

  ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/c6832b8f-0819-4139-951d-7f18cfc844fd)
  ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/49d055d7-6d0e-4b1e-8de9-6c7068f2a950)
  ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/5d31d151-f779-4ceb-8987-10c3c160c151)

5. Then next to it on the right side from top to bottom, the code module serves to synchronise the illumination of the Neopixel Ring LEDs by pressing key B. In order, the red light is on for 4s, the yellow light stays on for 7s and the blue light goes off one by one for a total of 8s.👇

   ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/0a50db8d-bc2b-4931-b85e-4446a3046868)
   ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/372ff5bd-6d2d-4920-9193-6472ba6f5d54)

6. Then the following code module is to switch off the display after 5 minutes (to avoid automatic switching off if the user has made a mistake or if the display has not been used for a long time).👇
   
    ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/7c817be4-c8ac-4f64-bb3c-a295edb17175)

7. Then the following code module is to draw 3 rectangles for landscaping the screen. It is displayed every 500ms. (New idea: phases of steps can be represented in a certain chronological order)👉

    ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/eb9c015f-6ecd-4a95-83cb-348c8da83806)

8. Then the code in the forever module on the right uses a pulse sensor to measure and calculate how many beats per minute the heart rate is. As well as displaying a heart icon the first time finger data is detected.👇

    ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/60d15df8-69eb-4af2-89a4-03c267470d26)
    ![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/1e9b4713-4c97-425d-8ec5-63f150f0ef2c)


(The principle is to set the counter to 1 when a level signal greater than 870 is detected and the counter is 0. When a level signal less than 430 is detected and the counter is 1, the counter is set to 0. Determine the time taken for the level signal to reach 870 again according to the time when the counter changes, and thus calculate the time for a complete wave. Originally only 60000ms/T was needed to calculate the heart rate. However, the equation (60000 - 60000 % T) / T was used to present the result as an integer. It should also be possible to use the rounding function in the Math code module.)

9. The final code module is used to display the heart rate value every 500ms, allowing the heart rate value to change on the OLED.💛

![image](https://github.com/Cosmicdty/Microbit-Group6-X1/assets/145985380/2ce3fd43-ddb7-4fd4-ac11-c47352aa0610)

(one problem encountered was that when the heart rate value appeared to be a three-digit number, the OLED display would stay at a three-digit display. I'm guessing this is because the numbers show up residually on the OLEDs. In order not to have incorrectly large values, I limited the value to 99. The final value could then be displayed in the normal range)

💚💛🧡




