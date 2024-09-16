![header-lesson-05](assets/header-lesson-05.png)

# Measuring the Air Quality Index and Equivalent Carbon Dioxide

## What is the Air Quality Index?

The Air Quality Index (AQI) is a way to measure how clean or polluted the air is in a specific place. It uses numbers and colors to show how safe the air is to breathe. Lower numbers mean the air is cleaner and healthier, while higher numbers mean there are more pollutants in the air that could be harmful, especially for people with breathing problems like asthma. The AQI helps us know when it's okay to be outside or if we should stay indoors to protect our health.

![aqi](assets/aqi.png)

---

## What is Equivalent Carbon Dioxide?

Equivalent carbon dioxide (eCO2), is a measure of the total impact of various greenhouse gases, like methane and nitrous oxide, expressed as an amount of carbon dioxide (CO2) that would have the same effect on global warming. Scientists use eCO2 to help understand how much these gases contribute to climate change and compare their effects more easily. By looking at eCO2 levels, we can better understand and track the overall impact of different activities and industries on the environment.

---

## Measuring Air Quality Index (AQI) with the micro:bit and Kitronik Air Quality and Environmental Board

As in the previous lesson we have to initialize the display. Select the "Display" drawer in the Toolbox. 

![makecode-kitronik-aqb-air-quality-00](assets/makecode-kitronik-aqb-air-quality-00.png)

Select the `turn off/on display` block.

![makecode-kitronik-aqb-air-quality-01](assets/makecode-kitronik-aqb-air-quality-01.png)

Drag the block into the `forever` block

![makecode-kitronik-aqb-air-quality-02](assets/makecode-kitronik-aqb-air-quality-02.png)

 Toggle the `off/on` switch in the block.

![makecode-kitronik-aqb-air-quality-03](assets/makecode-kitronik-aqb-air-quality-03.png)

The display has been initialized and can be used.

![makecode-kitronik-aqb-air-quality-04](assets/makecode-kitronik-aqb-air-quality-04.png)

Move the `forever` block.

![makecode-kitronik-aqb-air-quality-05](assets/makecode-kitronik-aqb-air-quality-05.png)

It is now visible without obstruction.

![makecode-kitronik-aqb-air-quality-06](assets/makecode-kitronik-aqb-air-quality-06.png)

Select the "Sensor" drawer.

![makecode-kitronik-aqb-air-quality-07](assets/makecode-kitronik-aqb-air-quality-07.png)

Here you can find the `establish gas baseline & ambient temperature` and `setup gas sensor` blocks. These blocks help the sensors gather more accurate air quality data.

![makecode-kitronik-aqb-air-quality-08](assets/makecode-kitronik-aqb-air-quality-08.png)

Drag the `setup gas sensor` and `establish gas baseline & ambient temperature` blocks into the `on start` block. This only needs to run once at the beginning of the program.

![makecode-kitronik-aqb-air-quality-09](assets/makecode-kitronik-aqb-air-quality-09.png)

Select the `measure all data readings` block.

![makecode-kitronik-aqb-air-quality-10](assets/makecode-kitronik-aqb-air-quality-10.png)

Place the block into the `forever` block. This will allow the micro:bit to record data in a loop. If this block is placed in the `on start` block, it will only run once. The data will not be updated continuously.

![makecode-kitronik-aqb-air-quality-11](assets/makecode-kitronik-aqb-air-quality-11.png)

Select the "Display" drawer to access the blocks for the OLED display. 

![makecode-kitronik-aqb-air-quality-12](assets/makecode-kitronik-aqb-air-quality-12.png)

Select the block that displays text on the OLED screen.

![makecode-kitronik-aqb-air-quality-13](assets/makecode-kitronik-aqb-air-quality-13.png)

Drag the block into the forever loop below the other block.

![makecode-kitronik-aqb-air-quality-14](assets/makecode-kitronik-aqb-air-quality-14.png)

Select the "Text" drawer in "Advanced" drawer in the Toolbox.

![makecode-kitronik-aqb-air-quality-16](assets/makecode-kitronik-aqb-air-quality-16.png)

Select the `join` block. 

![makecode-kitronik-aqb-air-quality-17](assets/makecode-kitronik-aqb-air-quality-17.png)

Place the block in the first oval that holds strings.

![makecode-kitronik-aqb-air-quality-18](assets/makecode-kitronik-aqb-air-quality-18.png)

Clear the text in the two ovals to create empty strings.

![makecode-kitronik-aqb-air-quality-19](assets/makecode-kitronik-aqb-air-quality-19.png)

Duplicate the box that displays text once.

![makecode-kitronik-aqb-air-quality-20](assets/makecode-kitronik-aqb-air-quality-20.png)

Select the duplicated block.

![makecode-kitronik-aqb-air-quality-21](assets/makecode-kitronik-aqb-air-quality-21.png)

Place the block in the `forever` block below the other block as displayed below:

![makecode-kitronik-aqb-air-quality-22](assets/makecode-kitronik-aqb-air-quality-22.png)

The data the micro:bit we will be reading is AQI score and the eCO2 level. The eCO2 level is measured in parts per million (ppm). 

The data will need to be represented as two separate strings for the AQI and three separate strings for the eCO2.

| Sting 1          | String 2    | String 3 |
| ---------------- | ----------- | -------- |
| `"AQI Score : "` | `aq1_data`  | NONE     |
| `"eCO2: "`       | `ec02_data` | `" ppm"` |

This will require a third string for the eCO2 only. Add another sting box with the `+` button.

![makecode-kitronik-aqb-air-quality-23](assets/makecode-kitronik-aqb-air-quality-23.png)

The third string is now available.

![makecode-kitronik-aqb-air-quality-24](assets/makecode-kitronik-aqb-air-quality-24.png)

Enter the data as determined above. Make sure to enter the whitespace. These spaces are necessary to have the Data display correctly. 

| String 1         | String 2    | String 3 |
| ---------------- | ----------- | -------- |
| `"AQI Score : "` | `aqi_data`  | NONE     |
| `"eCO2: "`       | `ec02_data` | `"       |

![makecode-kitronik-aqb-air-quality-25](assets/makecode-kitronik-aqb-air-quality-25.png)

Select the "Sensor" drawer.

![makecode-kitronik-aqb-air-quality-26](assets/makecode-kitronik-aqb-air-quality-26.png)

Select the `get IAQ Score`,  and `Read eCO2` blocks 

![makecode-kitronik-aqb-air-quality-27](assets/makecode-kitronik-aqb-air-quality-27.png)

Place them in the corresponding text fields.

![makecode-kitronik-aqb-air-quality-28](assets/makecode-kitronik-aqb-air-quality-28.png)

The code, as it is, will output the text for both measurements on the first line with only one visible

![makecode-kitronik-aqb-air-quality-29](assets/makecode-kitronik-aqb-air-quality-29.png)

Change the line number to `2` .

![makecode-kitronik-aqb-air-quality-30](assets/makecode-kitronik-aqb-air-quality-30.png)

The code is almost complete. The only thing needed now is a `pause` block. This will help give a more accurate reading from the sensors. Select the `Basic` drawer in the Toolbox.

![makecode-kitronik-aqb-air-quality-31](assets/makecode-kitronik-aqb-air-quality-31.png)

Select the `pause` block.

![makecode-kitronik-aqb-air-quality-32](assets/makecode-kitronik-aqb-air-quality-32.png)

Drag the `pause` block to the end of the code blocks in the `forever` block.

![makecode-kitronik-aqb-air-quality-33](assets/makecode-kitronik-aqb-air-quality-33.png)

Click on the triangle drop down button.

![makecode-kitronik-aqb-air-quality-34](assets/makecode-kitronik-aqb-air-quality-34.png)

Select 5 seconds.

![makecode-kitronik-aqb-air-quality-35](assets/makecode-kitronik-aqb-air-quality-35.png)

The `pause` block uses milliseconds (ms) and 5 seconds is 5000 miliseconds.

![makecode-kitronik-aqb-air-quality-36](assets/makecode-kitronik-aqb-air-quality-36.png)

The code is now ready to be flashed on the micro:bit.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:S91222-97206-38819-26043" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>