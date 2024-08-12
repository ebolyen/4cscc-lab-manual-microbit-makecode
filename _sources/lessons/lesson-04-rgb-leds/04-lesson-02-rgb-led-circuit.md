![header-lesson-04](assets/header-lesson-04.png)

# Building an RGB LED Circuit

In this section, you will build a circuit that blinks red, green, and blue on the RGB LED. The wire colors match the color of the LED in this circuit to help visually. If the wire colors are not available, the circuit will still work.

Attach the micro:bit to the Kitronik prototyping plate in the edge connector. Be sure that the micro:bit is inserted with the LED display facing up all the way in the edge connector, and not at an angle.

![kitronik-rgb-led-00](assets/kitronik-rgb-led-00.png)

Insert the RGB LED in the breadboard. The LED in the kit is a common cathode RGB LED as in the diagram displayed below:

![common-cathode-rgb-led-diagram](assets/common-cathode-rgb-led-diagram.png)

Take note of where the longer lead is, as this is the ground. Place the RGB LED in the breadboard.

![kitronik-rgb-led-01](assets/kitronik-rgb-led-01.png)

Take a 47Ω resistor and place one lead in the same row as the red lead on the RGB LED and the other lead a few rows away from it.

![kitronik-rgb-led-02](assets/kitronik-rgb-led-02.png)

Take another 47Ω resistor. Place one lead in the same row as the green lead, and the other lead a few rows away from it as the row with green lead on the RGB LED.

![kitronik-rgb-led-03](assets/kitronik-rgb-led-03.png)

Take another 47Ω resistor. Place one lead in the same row as the blue lead, and the other lead a few rows away from it as the row with blue lead on the RGB LED. Make sure that the green and blue leads and respective resistors are on different rows.

![kitronik-rgb-led-04](assets/kitronik-rgb-led-04.png)

Take a male-to-female jumper wire and place the female end on pin `0` on the Kitronik prototyping plate breakout board. Place the male lead in the row, linking the red lead with a resistor.

![kitronik-rgb-led-05](assets/kitronik-rgb-led-05.png)

Take another male-to-female jumper wire and place the female end on pin `1` on the Kitronik prototyping plate breakout board. Place the male lead in the row, linking the green lead with a resistor.

![kitronik-rgb-led-06](assets/kitronik-rgb-led-06.png)

Take another male-to-female jumper wire and place the female end on pin `2` on the Kitronik prototyping plate breakout board. Place the male lead in the row, linking the blue lead with a resistor.

![kitronik-rgb-led-07](assets/kitronik-rgb-led-07.png)

Take one more male-to-female jumper wire and place the female end on `0V`. Place the male end of the jumper wire in the same row as the common cathode on the RGB LED.

![kitronik-rgb-led-08](assets/kitronik-rgb-led-08.png)

This circuit should be similar to the circuit displayed below:

![kitronik-rgb-led-09](assets/kitronik-rgb-led-09.png)



