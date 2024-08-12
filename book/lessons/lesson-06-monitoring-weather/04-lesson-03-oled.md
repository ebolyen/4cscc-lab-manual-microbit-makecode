![header-lesson-06](assets/header-lesson-06.png)

# Working with OLED

Click on the "OLED" drawer in the Toolbox.

![makecode-elecfreaks-oled-01](assets/makecode-elecfreaks-oled-01.png)

Select the `initialize OLED` block. 

![makecode-elecfreaks-oled-02](assets/makecode-elecfreaks-oled-02.png)

Place the `initialize OLED` block in the `on start` block. This only needs to run once. **Do not change the dimensions.**

![makecode-elecfreaks-oled-03](assets/makecode-elecfreaks-oled-03.png)

The `forever` block can be moved.

![makecode-elecfreaks-oled-04](assets/makecode-elecfreaks-oled-04.png)

It is now unobstructed.

![makecode-elecfreaks-oled-05](assets/makecode-elecfreaks-oled-05.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-elecfreaks-oled-06](assets/makecode-elecfreaks-oled-06.png)

Select the `show string` block.

![makecode-elecfreaks-oled-07](assets/makecode-elecfreaks-oled-07.png)

Place the `show string` block in the `forever` block.

![makecode-elecfreaks-oled-08](assets/makecode-elecfreaks-oled-08.png)

Change the string in the `show string` block. Run the code. 

![makecode-elecfreaks-oled-10](assets/makecode-elecfreaks-oled-10.png)

Notice how the block repeats the string again and again. To prevent this we will first add a delay. Click on the "Basic" drawer of the Toolbox.

![makecode-elecfreaks-oled-11](assets/makecode-elecfreaks-oled-11.png)

Select the `pause` block.

![makecode-elecfreaks-oled-12](assets/makecode-elecfreaks-oled-12.png)

Place the `pause` block below the `show string` block. This will keep the string on the display for the specified value.

![makecode-elecfreaks-oled-13](assets/makecode-elecfreaks-oled-13.png)

Change the value of the `pause` block in the dropdown menu.

![makecode-elecfreaks-oled-14](assets/makecode-elecfreaks-oled-14.png)

We will display the readings every second. This still will not prevent the string from repeating. You will need one more block.

![makecode-elecfreaks-oled-15](assets/makecode-elecfreaks-oled-15.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-elecfreaks-oled-16](assets/makecode-elecfreaks-oled-16.png)

Select the `clear OLED display` block.

![makecode-elecfreaks-oled-17](assets/makecode-elecfreaks-oled-17.png)

Place the `clear OLED display` block below the pause block. This will reset the display after it displays the string for one second, eliminating the repeated strings.

![makecode-elecfreaks-oled-18](assets/makecode-elecfreaks-oled-18.png)

