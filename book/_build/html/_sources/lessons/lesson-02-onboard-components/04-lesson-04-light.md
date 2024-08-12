![header-lesson-02](assets/header-lesson-02.png)

# Using the Light Sensor

This section will focus on the micro: bit's light-sensing capabilities. The micro:bit has no dedicated light sensor, but the LED display can act like a primitive light sensor.

![microbit-display](assets/microbit-display.png)

To display the light level, we first need to add a string representing the value returned by the sensor. To do so, click on the "Basic" drawer in the Toolbox.

![makecode-light-01](assets/makecode-light-01.png)

Select the `show string` block.

![makecode-light-02](assets/makecode-light-02.png)

Place the `show string` block in the `forever block.`

![makecode-light-03](assets/makecode-light-03.png)

Next you need to get the block that reads the light level. Click on the "Input" drawer of the Toolbox.

![makecode-light-04](assets/makecode-light-04.png)

Select the `light level` block.

![makecode-light-05](assets/makecode-light-05.png)

Place the `light level` block in the `show string` block.

![makecode-light-06](assets/makecode-light-06.png)

The code is now ready to be flashed on the micro:bit.
