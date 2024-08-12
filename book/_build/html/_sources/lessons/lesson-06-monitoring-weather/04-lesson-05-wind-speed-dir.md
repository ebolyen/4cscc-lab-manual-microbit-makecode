![header-lesson-06](assets/header-lesson-06.png)

# Measuring Wind Speed and Wind Direction



Click on the "OLED" drawer in the Toolbox.

![makecode-weatherbit-ws-wd-01](assets/makecode-weatherbit-ws-wd-01.png)

Select the `initialize OLED` block. 

![makecode-weatherbit-ws-wd-02](assets/makecode-weatherbit-ws-wd-02.png)

Place the `initialize OLED` block in the `on start` block. This only needs to run once. **Do not change the dimensions.**

![makecode-weatherbit-ws-wd-03](assets/makecode-weatherbit-ws-wd-03.png)

Click on the "Weatherbit" drawer in the Toolbox.

![makecode-weatherbit-ws-wd-04](assets/makecode-weatherbit-ws-wd-04.png)

Select the `start wind monitoring` block.

![makecode-weatherbit-ws-wd-05](assets/makecode-weatherbit-ws-wd-05.png)

Place the `start wind monitoring` block in the `on start` block. This code only needs to run once.

![makecode-weatherbit-ws-wd-06](assets/makecode-weatherbit-ws-wd-06.png)

The `forever` block can be moved.

![makecode-weatherbit-ws-wd-07](assets/makecode-weatherbit-ws-wd-07.png)

It is now unobstructed.

![makecode-weatherbit-ws-wd-08](assets/makecode-weatherbit-ws-wd-08.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-weatherbit-ws-wd-09](assets/makecode-weatherbit-ws-wd-09.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-weatherbit-ws-wd-10](assets/makecode-weatherbit-ws-wd-10.png)

Place the `show string` block in the `forever` block.

![makecode-weatherbit-ws-wd-11](assets/makecode-weatherbit-ws-wd-11.png)

We now need to format the strings as in the previous lesson. Click on the "Advanced" drawer of the Toolbox.

![makecode-weatherbit-ws-wd-12](assets/makecode-weatherbit-ws-wd-12.png)

Click on the "Text" drawer.

![makecode-weatherbit-ws-wd-13](assets/makecode-weatherbit-ws-wd-13.png)

Select the `join` block.

![makecode-weatherbit-ws-wd-14](assets/makecode-weatherbit-ws-wd-14.png)

Place the `join` block in the `show string` block.

![makecode-weatherbit-ws-wd-15](assets/makecode-weatherbit-ws-wd-15.png)

![makecode-weatherbit-ws-wd-16](assets/makecode-weatherbit-ws-wd-16.png)

![makecode-weatherbit-ws-wd-17](assets/makecode-weatherbit-ws-wd-17.png)

![makecode-weatherbit-ws-wd-18](assets/makecode-weatherbit-ws-wd-18.png)

![makecode-weatherbit-ws-wd-19](assets/makecode-weatherbit-ws-wd-19.png)

![makecode-weatherbit-ws-wd-20](assets/makecode-weatherbit-ws-wd-20.png)

![makecode-weatherbit-ws-wd-21](assets/makecode-weatherbit-ws-wd-21.png)

![makecode-weatherbit-ws-wd-22](assets/makecode-weatherbit-ws-wd-22.png)

![makecode-weatherbit-ws-wd-23](assets/makecode-weatherbit-ws-wd-23.png)

![makecode-weatherbit-ws-wd-24](assets/makecode-weatherbit-ws-wd-24.png)

![makecode-weatherbit-ws-wd-25](assets/makecode-weatherbit-ws-wd-25.png)

![makecode-weatherbit-ws-wd-26](assets/makecode-weatherbit-ws-wd-26.png)

![makecode-weatherbit-ws-wd-27](assets/makecode-weatherbit-ws-wd-27.png)

![makecode-weatherbit-ws-wd-28](assets/makecode-weatherbit-ws-wd-28.png)

![makecode-weatherbit-ws-wd-29](assets/makecode-weatherbit-ws-wd-29.png)

![makecode-weatherbit-ws-wd-30](assets/makecode-weatherbit-ws-wd-30.png)

![makecode-weatherbit-ws-wd-31](assets/makecode-weatherbit-ws-wd-31.png)

![makecode-weatherbit-ws-wd-32](assets/makecode-weatherbit-ws-wd-32.png)

![makecode-weatherbit-ws-wd-33](assets/makecode-weatherbit-ws-wd-33.png)

![makecode-weatherbit-ws-wd-34](assets/makecode-weatherbit-ws-wd-34.png)

![makecode-weatherbit-ws-wd-35](assets/makecode-weatherbit-ws-wd-35.png)

![makecode-weatherbit-ws-wd-36](assets/makecode-weatherbit-ws-wd-36.png)

As in the previous sections. You need to stop the OLED from repeating the data. Click on the "Basic" drawer of the Toolbox.

![makecode-weatherbit-ws-wd-37](assets/makecode-weatherbit-ws-wd-37.png)

Select the `pause` block.

![makecode-weatherbit-ws-wd-38](assets/makecode-weatherbit-ws-wd-38.png)

Place the pause block below the `show string` blocks in the `forever` block. 

![makecode-weatherbit-ws-wd-39](assets/makecode-weatherbit-ws-wd-39.png)

Change the pause to 5 seconds in the dropdown menu.

![makecode-weatherbit-ws-wd-42](assets/makecode-weatherbit-ws-wd-42.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-weatherbit-ws-wd-43](assets/makecode-weatherbit-ws-wd-43.png)

Select the `clear OLED display` block.

![makecode-weatherbit-ws-wd-44](assets/makecode-weatherbit-ws-wd-44.png)

Place the `clear OLED display` below the `pause` block in the `forever` block.

![makecode-weatherbit-ws-wd-45](assets/makecode-weatherbit-ws-wd-45.png)