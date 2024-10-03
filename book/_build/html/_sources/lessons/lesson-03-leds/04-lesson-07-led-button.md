![header-lesson-03](assets/header-lesson-03.png)

# Using a Button and an LED 

Open [MakeCode](https://makecode.microbit.org/) and create a new project.

![makecode-blink-one-led-00](assets/makecode-blink-one-led-00.png)

First, we need to add a button. Select the Input drawer on in the Toolbox.

![makecode-button-led-00](assets/makecode-button-led-00.png)

Drag the `on button` block onto the workspace.

![makecode-button-led-01](assets/makecode-button-led-01.png)

This is a special block that does not need to be placed into the `on start` or `forever` blocks. In fact, the shape of the block will not allow you to place it in these blocks.

![makecode-button-led-02](assets/makecode-button-led-02.png)

Select Advanced.

![makecode-button-led-03](assets/makecode-button-led-03.png)

Then select Pins.

![makecode-button-led-04](assets/makecode-button-led-04.png)

Select the `digital write` block.

![makecode-button-led-05](assets/makecode-button-led-05.png)

Place the `digital write` block in the `on button` block.

![makecode-button-led-06](assets/makecode-button-led-06.png)

Duplicate the `on button` block. Make sure that you are duplicating the `on button` block and not the `digital write` block.

![makecode-button-led-07](assets/makecode-button-led-07.png)

The duplicated block is over the duplicated block.

![makecode-button-led-08](assets/makecode-button-led-08.png)

Move the new block to the side. Notice how the block is a different color than the other block. This is because the code is the same, and MakeCode will ignore duplicated blocks.

![makecode-button-led-09](assets/makecode-button-led-09.png)

Toggle the `A` on the `on button` block and select `B`. This will change the code to react to button `B` instead of button `A`.

![makecode-button-led-10](assets/makecode-button-led-10.png)

The block is now the same colors as the other `on button` block,

![makecode-button-led-11](assets/makecode-button-led-11.png)

This code will not turn the LED on and off, because both of the values in the blocks are `0`. This code will only keep an LED off or at `0`. The value in the `on button b` block must be changed.

![makecode-button-led-12](assets/makecode-button-led-12.png)

Change the digital signal from `0` to `1`.

![makecode-button-led-13](assets/makecode-button-led-13.png)

The program is now complete, and button `A` should turn the LED off and button `B` will turn the LED on. 

Try switching the values so button `A` turns the LED on and button `B` turns the LED off.

The micro:bit is now ready to be flashed with code. Press the download button to transfer the code to the micro:bit.
