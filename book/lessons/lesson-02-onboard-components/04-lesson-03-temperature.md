![header-lesson-02](assets/header-lesson-02.png)

# Using the Temperature Sensor
This section focuses on the onboard temperature sensor. As mentioned previously, this sensor is not a dedicated temperature sensor; it is attached to the processor. It is also not as accurate as the temperature sensors used in later sections of this manual.

![microbit-processor](assets/microbit-processor.png)

To display the temperature, we first need to add a string representing the value returned by the sensor. To do so, click on the "Basic" drawer in the Toolbox.

![makecode-temperature-01](assets/makecode-temperature-01.png)

Select the `show string` block.

![makecode-temperature-02](assets/makecode-temperature-02.png)

Place the `show string` block in the `forever` block.

![makecode-temperature-03](assets/makecode-temperature-03.png)

Next, we need to get the block that reads the temperature. To do so, click on the "Input" drawer of the Toolbox.

![makecode-temperature-04](assets/makecode-temperature-04.png)

Select the `temperature (°C)` block.

![makecode-temperature-05](assets/makecode-temperature-05.png)

Place the `temperature (°C)` block in the `show string` block. 

![makecode-temperature-06](assets/makecode-temperature-06.png)

The micro:bit is now ready to be flashed with code. Press the download button to transfer the code to the micro:bit.
