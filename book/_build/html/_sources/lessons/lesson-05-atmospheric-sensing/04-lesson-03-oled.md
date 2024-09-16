# Using the OLED Display

## What is an OLED Display?

An OLED display is a type of screen used in many devices, such as phones and TVs. What makes OLED special is that each pixel on the screen can emit its own light, unlike older screens, where a separate backlight is needed. This makes OLED displays bright and colorful, with deep blacks and vibrant colors. They also use less power, which helps devices last longer between charges. Overall, OLED displays give us clearer and more colorful images on our devices.

![kitronik-aqb-oled-coordinates](assets/kitronik-aqb-oled-coordinates.png)

The picture above shows the dimensions of the OLED screen. The coordinates start on the upper left corner of the OLED screen. The screen is 128 pixels in width on the x-axis and 64 pixels in height on the y-axis.

---

## Using the OLED Display on the Kitronik Air Quality and Environmental Board


![makecode-kitronik-aqb-display-00](assets/makecode-kitronik-aqb-display-00.png)

For the display to function, the display must be turned on using the `turn off/on display` block.

![makecode-kitronik-aqb-display-01](assets/makecode-kitronik-aqb-display-01.png)

Drag the `turn off/on display` into the `on start` block. This code needs to only run once at the beginning of the program.

![makecode-kitronik-aqb-display-02](assets/makecode-kitronik-aqb-display-02.png)

 Toggle the `off/on` switch in the block,

![makecode-kitronik-aqb-display-03](assets/makecode-kitronik-aqb-display-03.png)

The display has been initialized, and it can be used.

![makecode-kitronik-aqb-display-04](assets/makecode-kitronik-aqb-display-04.png)

Notice that the `forever` block is behind the block inside of the `on start` block

![makecode-kitronik-aqb-display-05](assets/makecode-kitronik-aqb-display-05.png)

Move the forever block to make it visible. You may rearrange blocks at any time. The blocks do not run in the order that they are displayed. 

![makecode-kitronik-aqb-display-06](assets/makecode-kitronik-aqb-display-06.png)

Select the `show < > on line <1> with alignment` block. This is the block that displays text on the OLED screen. The blank oval will be the number or string that will be displayed. The second oval with a default `1` is the line number. The OLED can display up to eight lines on the OLED screen.

![makecode-kitronik-aqb-display-07](assets/makecode-kitronik-aqb-display-07.png)

Drag this block into the `forever` block. As mentioned before, this block will run the code in a loop, which is what you need to display sensor data in real-time. Next select the `Advanced` drawer in the Toolbox.

![makecode-kitronik-aqb-display-08](assets/makecode-kitronik-aqb-display-08.png)

Select `Text`. This section is where the blocks for strings are.

![makecode-kitronik-aqb-display-09](assets/makecode-kitronik-aqb-display-09.png)

Select the empty string block.

![makecode-kitronik-aqb-display-10](assets/makecode-kitronik-aqb-display-10.png)

Drag the empty string block into the first oval.

![makecode-kitronik-aqb-display-11](assets/makecode-kitronik-aqb-display-11.png)

Type "Four Corners Science and Computing Club" in the empty string block. Run the code on the micro:bit.

![makecode-kitronik-aqb-display-12](assets/makecode-kitronik-aqb-display-12.png)

Notice how the text runs to the next line. 

TODO: ADD PHOTO OF THE OUTPUT

The micro:bit does not understand word boundaries. This means a word could be split between two lines, with part of it at the end of one line and the rest at the start of the next. To avoid this, it’s best to break up longer strings into multiple lines. You can duplicate the existing block to do this, as it's usually quicker than finding the block again in the Toolbox. 

There is no set character limit for the lines on the OLED, as some characters are wider than others. It is best to test your code for readability and modify it to be displayed as you intend it to be displayed.

![makecode-kitronik-aqb-display-13](assets/makecode-kitronik-aqb-display-13.png)

Drag the duplicate directly below the other block.

![makecode-kitronik-aqb-display-14](assets/makecode-kitronik-aqb-display-14.png)

Now that the block is below the next block, you can now have two lines of text.

![makecode-kitronik-aqb-display-15](assets/makecode-kitronik-aqb-display-15.png)

The text is the same, and must be changed.

![makecode-kitronik-aqb-display-16](assets/makecode-kitronik-aqb-display-16.png)

Modify the text so "Four Corners Science and Computing Club" is displayed on two lines.

![makecode-kitronik-aqb-display-17](assets/makecode-kitronik-aqb-display-17.png)

Notice that the line number is still `1`. This must be changed or only one line of text will be displayed.

![makecode-kitronik-aqb-display-18](assets/makecode-kitronik-aqb-display-18.png)

Change the line `1` to line `2`. 

![makecode-kitronik-aqb-display-19](assets/makecode-kitronik-aqb-display-19.png)

The text is now displayed on two lines.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:S42841-02102-50736-79156" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

TODO: ADD PHOTO OF THE NEW OUTPUT

