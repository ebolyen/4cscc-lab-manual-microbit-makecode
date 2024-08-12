![header-lesson-05](assets/header-lesson-05.png)

# Measuring Temperature Humidity and Atmospheric Pressure

## What is Celcius?

Celsius is a way to measure temperature. It's named after a scientist named Anders Celsius. In Celsius, water freezes at 0 degrees and boils at 100 degrees. So, if it's 20 degrees Celsius outside, it's not too cold or too hot—it's just right for a lot of people. Scientists use Celsius because it's easy to understand and it's based on how water behaves at different temperatures.

![c-f-examples](assets/c-f-examples.png)

## What is Humidity?

Humidity is a measure of how much moisture or water vapor is in the air around us. It's what makes the air feel sticky or dry. When humidity is high, like on a humid day, it means there's a lot of moisture in the air. When humidity is low, the air feels drier. Humidity is important for weather and how comfortable we feel. It can affect things like how quickly sweat evaporates from our skin, which helps cool us down.

## What is Atmospheric Pressure?

Atmospheric pressure is the weight of the air pushing down on us and everything around us. It's like the pressure you feel when you dive deep underwater. This pressure comes from the huge blanket of air, called the atmosphere, that surrounds the Earth. Atmospheric pressure changes with the weather and altitude. It's important for predicting weather patterns because high pressure usually means clear skies, while low pressure often brings clouds and rain.

![pressure-diagram](assets/pressure-diagram.png)

## Measuring Temperature Humidity and Atmospheric Pressure with the micro:bit and the Kitronik Air Quality and Environmental Board

As in the previous lesson we have to initialize the display. Select the "Display" drawer in the Toolbox.

![makecode-kitronik-aqb-temperature-00](assets/makecode-kitronik-aqb-temperature-00.png)

Select the `turn off/on display` block.

![makecode-kitronik-aqb-temperature-01](assets/makecode-kitronik-aqb-temperature-01.png)

Drag the block into the `forever` block.

![makecode-kitronik-aqb-temperature-02](assets/makecode-kitronik-aqb-temperature-02.png)

 Toggle the `off/on` switch in the block.

![makecode-kitronik-aqb-temperature-03](assets/makecode-kitronik-aqb-temperature-03.png)

The display has been initialized and can be used.

![makecode-kitronik-aqb-temperature-04](assets/makecode-kitronik-aqb-temperature-04.png)

Move the `forever` block.

![makecode-kitronik-aqb-temperature-05](assets/makecode-kitronik-aqb-temperature-05.png)

It is now visible without obstruction.

![makecode-kitronik-aqb-temperature-06](assets/makecode-kitronik-aqb-temperature-06.png)

Select the "Sensor" drawer.

![makecode-kitronik-aqb-temperature-07](assets/makecode-kitronik-aqb-temperature-07.png)

Here you can find the `establish gas baseline & ambient temperature block`. This block helps the sensors gather more accurate air quality data.

![makecode-kitronik-aqb-temperature-08](assets/makecode-kitronik-aqb-temperature-08.png)

Drag the block into the `on start` block. This only needs to run once at the beginning of the program.

![makecode-kitronik-aqb-temperature-09](assets/makecode-kitronik-aqb-temperature-09.png)

Select the `measure all data readings` block.

![makecode-kitronik-aqb-temperature-10](assets/makecode-kitronik-aqb-temperature-10.png)

Place the block into the `forever` block. This will allow the micro:bit to record data in a loop. If this block is placed in the `on start` block, it will only run once. The data will not be updated continuously.

![makecode-kitronik-aqb-temperature-11](assets/makecode-kitronik-aqb-temperature-11.png)

Select the "Display" drawer to access the blocks for the OLED display. 

![makecode-kitronik-aqb-temperature-12](assets/makecode-kitronik-aqb-temperature-12.png)

Select the block that displays text on the OLED screen.

![makecode-kitronik-aqb-temperature-13](assets/makecode-kitronik-aqb-temperature-13.png)

Drag the block into the forever loop below the other block.

![makecode-kitronik-aqb-temperature-14](assets/makecode-kitronik-aqb-temperature-14.png)

Select the "Text" drawer in "Advanced" drawer in the Toolbox.

![makecode-kitronik-aqb-temperature-15](assets/makecode-kitronik-aqb-temperature-15.png)

Select the `join` block. This block combines two strings. This block is necessary only if you combine two different strings from distinct sources, such as a sensor value or a variable.

![makecode-kitronik-aqb-temperature-16](assets/makecode-kitronik-aqb-temperature-16.png)

Place the block in the first oval that holds strings.

![makecode-kitronik-aqb-temperature-17](assets/makecode-kitronik-aqb-temperature-17.png)

The data the micro:bit we will be reading is temperature data in celsius, relative humidity and atmospheric pressure. Temperature data is often displayed with the C at the end to indicate that the reading is in celsius. Relative humidity is a percentage and is often followed by a `%`. Atmospheric pressure is often measured in Kilopascals (kPa). 

The data will need to be represented as three separate strings.

| Sting 1           | String 2     | String 3 |
| ----------------- | ------------ | -------- |
| `"Temperature: "` | `temp_data`  | `" C"`   |
| `"Humidity: "`    | `hum_data`   | `"%"`    |
| `"Pressure: "`    | `press data` | `" kPa"` |

This will require a third string. Add another sting box with the `+` button.

![makecode-kitronik-aqb-display-20](assets/makecode-kitronik-aqb-display-20.png)

Clear the text in all three ovals to create empty strings.

![makecode-kitronik-aqb-temperature-18](assets/makecode-kitronik-aqb-temperature-18.png)

Duplicate the box that displays text twice.

![makecode-kitronik-aqb-temperature-19](assets/makecode-kitronik-aqb-temperature-19.png)

Select the two duplicated blocks.

![makecode-kitronik-aqb-temperature-20](assets/makecode-kitronik-aqb-temperature-20.png)

Place the blocks in the `forever` block below the other block as displayed below:

![makecode-kitronik-aqb-temperature-21](assets/makecode-kitronik-aqb-temperature-21.png)

Enter the data as determined above. Notice that there are spaces called **whitespace**. These spaces are necessary to have the Data display correctly. 

| Sting 1           | String 2     | String 3 |
| ----------------- | ------------ | -------- |
| `"Temperature: "` | `temp_data`  | `" C"`   |
| `"Humidity: "`    | `hum_data`   | `"%"`    |
| `"Pressure: "`    | `press data` | `" hPa"` |

![makecode-kitronik-aqb-temperature-22](assets/makecode-kitronik-aqb-temperature-22.png)

The board reads atmospheric pressure in pascals. The preferred scale is kilopascals. There are 1000 pascals in one kilopascal. The out put must be divided by 1000 to convert it to kilopascals. This requires a l little math in the code. Select the `Math` drawer.

![makecode-kitronik-aqb-temperature-23](assets/makecode-kitronik-aqb-temperature-23.png)

Look for the division block.

![makecode-kitronik-aqb-temperature-24](assets/makecode-kitronik-aqb-temperature-24.png)

Drag the division block into the text area of the block that displays text on the OLED.

![makecode-kitronik-aqb-temperature-25](assets/makecode-kitronik-aqb-temperature-25.png)

Type `1000` as the divisor of the division block.

![makecode-kitronik-aqb-temperature-26](assets/makecode-kitronik-aqb-temperature-26.png)

Select the "Sensor" drawer.

![makecode-kitronik-aqb-temperature-27](assets/makecode-kitronik-aqb-temperature-27.png)

Select the `Read Temperature in`, `Read Pressure in`, and `Read Humidity` blocks 

![makecode-kitronik-aqb-temperature-28](assets/makecode-kitronik-aqb-temperature-28.png)

Place them in the corresponding text fields. Make sure that the `Read Pressure in` block is the dividend of the division block.

![makecode-kitronik-aqb-temperature-29](assets/makecode-kitronik-aqb-temperature-29.png)

The code as it is will output the text for all three measurments on the first line with only one visible.

![makecode-kitronik-aqb-temperature-30](assets/makecode-kitronik-aqb-temperature-30.png)

Change the line numbers to `2` and `3`.

![makecode-kitronik-aqb-temperature-31](assets/makecode-kitronik-aqb-temperature-31.png)

The code is almost complete. The only thing needed now is a `pause` block. This will help give a more accurate reading from the sensors. Select the `Basic` drawer in the Toolbox.

![makecode-kitronik-aqb-temperature-32](assets/makecode-kitronik-aqb-temperature-32.png)

Select the `pause` block.

![makecode-kitronik-aqb-temperature-33](assets/makecode-kitronik-aqb-temperature-33.png)

Drag the `pause` block to the end of the code blocks in the `forever` block.

![makecode-kitronik-aqb-temperature-34](assets/makecode-kitronik-aqb-temperature-34.png)

Click on the triangle drop down button.

![makecode-kitronik-aqb-temperature-35](assets/makecode-kitronik-aqb-temperature-35.png)

Select 5 seconds.

![makecode-kitronik-aqb-temperature-36](assets/makecode-kitronik-aqb-temperature-36.png)

The `pause` block uses milliseconds (ms) and 5 seconds is 5000 miliseconds.

![makecode-kitronik-aqb-temperature-37](assets/makecode-kitronik-aqb-temperature-37.png)

The code is now ready to be flashed on the micro:bit.

TODO:NOTE AND IMAGE ABOUT THE PROCESS LENGTHY PROCESS.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:S41590-25281-54010-62696" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>
