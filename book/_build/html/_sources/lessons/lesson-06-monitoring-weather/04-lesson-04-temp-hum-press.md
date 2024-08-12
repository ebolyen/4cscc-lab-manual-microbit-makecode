![header-lesson-06](assets/header-lesson-06.png)

# Measuring Temperature Humidity and Atmospheric Pressure

![sparkfun-weatherbit-bme280](assets/sparkfun-weatherbit-bme280.png)

Click on the "OLED" drawer in the Toolbox.

![makecode-weatherbit-temp-hum-press-01](assets/makecode-weatherbit-temp-hum-press-01.png)

Select the `initialize OLED` block. 

![makecode-weatherbit-temp-hum-press-02](assets/makecode-weatherbit-temp-hum-press-02.png)

Place the `initialize OLED` block in the `on start` block. This only needs to run once. **Do not change the dimensions.**

![makecode-weatherbit-temp-hum-press-03](assets/makecode-weatherbit-temp-hum-press-03.png)

Click on the "Weatherbit" drawer in the Toolbox.

![makecode-weatherbit-temp-hum-press-04](assets/makecode-weatherbit-temp-hum-press-04.png)

Select the `start weather monitoring` block.

![makecode-weatherbit-temp-hum-press-05](assets/makecode-weatherbit-temp-hum-press-05.png)

Place the `start weather monitoring` block in the `on start` block. This code only needs to run once.

![makecode-weatherbit-temp-hum-press-06](assets/makecode-weatherbit-temp-hum-press-06.png)

The `forever` block can be moved.

![makecode-weatherbit-temp-hum-press-07](assets/makecode-weatherbit-temp-hum-press-07.png)

It is now unobstructed.

![makecode-weatherbit-temp-hum-press-08](assets/makecode-weatherbit-temp-hum-press-08.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-09](assets/makecode-weatherbit-temp-hum-press-09.png)

Select the `show string` block.

![makecode-weatherbit-temp-hum-press-10](assets/makecode-weatherbit-temp-hum-press-10.png)

Place the `show string` block in the `forever` block.

![makecode-weatherbit-temp-hum-press-11](assets/makecode-weatherbit-temp-hum-press-11.png)

We now need to format the strings as in the previous lesson. Click on the "Advanced" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-12](assets/makecode-weatherbit-temp-hum-press-12.png)

Click on the "Text" drawer.

![makecode-weatherbit-temp-hum-press-13](assets/makecode-weatherbit-temp-hum-press-13.png)

Select the `join` block.

![makecode-weatherbit-temp-hum-press-14](assets/makecode-weatherbit-temp-hum-press-14.png)

Place the `join` block in the `show string` block.

![makecode-weatherbit-temp-hum-press-15](assets/makecode-weatherbit-temp-hum-press-15.png)

The data the micro:bit we will be reading is temperature data in celsius, relative humidity and atmospheric pressure. Temperature data is often displayed with the C at the end to indicate that the reading is in celsius. Relative humidity is a percentage and is often followed by a `%`. Atmospheric pressure is often measured in Kilopascals (kPa). 

The data will need to be represented as three separate strings.

| Sting 1           | String 2     | String 3 |
| ----------------- | ------------ | -------- |
| `"Temperature: "` | `temp_data`  | `" C"`   |
| `"Humidity: "`    | `hum_data`   | `"%"`    |
| `"Pressure: "`    | `press data` | `" kPa"` |

This will require a third string. Add another sting box with the `+` button.

![makecode-weatherbit-temp-hum-press-16](assets/makecode-weatherbit-temp-hum-press-16.png)

Clear the text in all three ovals to create empty strings.

![makecode-weatherbit-temp-hum-press-19](assets/makecode-weatherbit-temp-hum-press-19.png)

Duplicate the box that displays text twice.

![makecode-weatherbit-temp-hum-press-20](assets/makecode-weatherbit-temp-hum-press-20.png)

Select the two duplicated blocks.

![makecode-weatherbit-temp-hum-press-21](assets/makecode-weatherbit-temp-hum-press-21.png)

Place the blocks in the `forever` block below the other block as displayed below:

![makecode-weatherbit-temp-hum-press-22](assets/makecode-weatherbit-temp-hum-press-22.png)

Enter the data as determined above. Notice that there are spaces called **whitespace**. These spaces are necessary to have the Data display correctly. 

| Sting 1           | String 2     | String 3 |
| ----------------- | ------------ | -------- |
| `"Temperature: "` | `temp_data`  | `" C"`   |
| `"Humidity: "`    | `hum_data`   | `"%"`    |
| `"Pressure: "`    | `press data` | `" hPa"` |

![makecode-weatherbit-temp-hum-press-23](assets/makecode-weatherbit-temp-hum-press-23.png)

Some calculations must be performed for the data to display correctly. Click on the "Math" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-24](assets/makecode-weatherbit-temp-hum-press-24.png)

Select the `square root` block. 

![makecode-weatherbit-temp-hum-press-25](assets/makecode-weatherbit-temp-hum-press-25.png)

Place the `square root` block on the workspace. This is not the calculation that will be performed. You will select another operation from the dropdown menu. 

![makecode-weatherbit-temp-hum-press-26](assets/makecode-weatherbit-temp-hum-press-26.png)

Click on the `integer \` block. This operation will return a value without rounding and without a decimal value.

![makecode-weatherbit-temp-hum-press-27](assets/makecode-weatherbit-temp-hum-press-27.png)

This block will change. Notice that there are now two places for values.

![makecode-weatherbit-temp-hum-press-28](assets/makecode-weatherbit-temp-hum-press-28.png)

Duplicate  block twice.

![makecode-weatherbit-temp-hum-press-29](assets/makecode-weatherbit-temp-hum-press-29.png)

Select the blocks one at a time.

![makecode-weatherbit-temp-hum-press-30](assets/makecode-weatherbit-temp-hum-press-30.png)

Place the blocks in the part where the data sill be in the `join` block.

![makecode-weatherbit-temp-hum-press-31](assets/makecode-weatherbit-temp-hum-press-31.png)

Now you will add the blocks to collect the data. Click on the "Weatherbit" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-32](assets/makecode-weatherbit-temp-hum-press-32.png)

Select the `temperature`, `humidity`, and  `pressure` blocks. 

![makecode-weatherbit-temp-hum-press-34](assets/makecode-weatherbit-temp-hum-press-34.png)

Place them in the corresponding text fields. Make sure that the `Read Pressure in` block is the dividend of the division block.

![makecode-weatherbit-temp-hum-press-35](assets/makecode-weatherbit-temp-hum-press-35.png)

To calculate the temperature correctly, change the `0` to `100`.

![makecode-weatherbit-temp-hum-press-36](assets/makecode-weatherbit-temp-hum-press-36.png)

This will now display the temperature correctly in celsius.

![makecode-weatherbit-temp-hum-press-37](assets/makecode-weatherbit-temp-hum-press-37.png)

To calculate the temperature correctly, change the `0` to `1024`.

![makecode-weatherbit-temp-hum-press-38](assets/makecode-weatherbit-temp-hum-press-38.png)

This will now display the humidity correctly.

![makecode-weatherbit-temp-hum-press-39](assets/makecode-weatherbit-temp-hum-press-39.png)

To calculate the pressure correctly, change the `0` to `25600`.

![makecode-weatherbit-temp-hum-press-40](assets/makecode-weatherbit-temp-hum-press-40.png)

This will now display the pressure correctly.

![makecode-weatherbit-temp-hum-press-41](assets/makecode-weatherbit-temp-hum-press-41.png)

As in the previous section. You need to stop the OLED from repeating the data. Click on the "Basic" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-42](assets/makecode-weatherbit-temp-hum-press-42.png)

Select the `pause` block.

![makecode-weatherbit-temp-hum-press-43](assets/makecode-weatherbit-temp-hum-press-43.png)

Place the pause block below the `show string` blocks in the `forever` block. 

![makecode-weatherbit-temp-hum-press-44](assets/makecode-weatherbit-temp-hum-press-44.png)

Change the pause to 5 seconds in the dropdown menu.

![makecode-weatherbit-temp-hum-press-47](assets/makecode-weatherbit-temp-hum-press-47.png)

Click on the "OLED" drawer of the Toolbox.

![makecode-weatherbit-temp-hum-press-48](assets/makecode-weatherbit-temp-hum-press-48.png)

Select the `clear OLED display` block.

![makecode-weatherbit-temp-hum-press-49](assets/makecode-weatherbit-temp-hum-press-49.png)

Place the `clear OLED display` below the `pause` block in the `forever` block.

![makecode-weatherbit-temp-hum-press-50](assets/makecode-weatherbit-temp-hum-press-50.png)
