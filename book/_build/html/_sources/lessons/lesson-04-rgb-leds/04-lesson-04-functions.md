![header-lesson-04](assets/header-lesson-04.png)

# Using Functions to Alternate Colors

## What is a Function?

A function in programming is a set of instructions that performs a specific task. You can think of it like a mini-program within your larger program. When you use a function, you give it a name and tell it what to do, so whenever you need to perform that task, you just call the function by its name instead of writing the same code over and over again. This makes your code more organized and easier to read.

## Creating a Function in MakeCode

To create a function, select the "Advanced" drawer in the Toolbox.

![makecode-rgb-led-function-01](assets/makecode-rgb-led-function-01.png)

Select the "Functions" drawer.

![makecode-rgb-led-function-02](assets/makecode-rgb-led-function-02.png)

Click on "Make a Function...".

![makecode-rgb-led-function-03](assets/makecode-rgb-led-function-03.png)

A new window will open to edit the new function.

![makecode-rgb-led-function-04](assets/makecode-rgb-led-function-04.png)

First, change the name of the function.

![makecode-rgb-led-function-05](assets/makecode-rgb-led-function-05.png)

In this example, you will create a function called red that will have all the blocks to turn an RGB LED red. Change the name to "red" and click the "Done" button. 

![makecode-rgb-led-function-06](assets/makecode-rgb-led-function-06.png)

The empty function called "red" will be placed on the workspace.

![makecode-rgb-led-function-07](assets/makecode-rgb-led-function-07.png)

Rearrange the `red` function block to make space for more function blocks.

![makecode-rgb-led-function-08](assets/makecode-rgb-led-function-08.png)

Select the "Pins" drawer in "Advanced". Select an `analog write` block.

![makecode-rgb-led-function-10](assets/makecode-rgb-led-function-10.png)

Place the `analog write` block in the `red` function.

![makecode-rgb-led-function-11](assets/makecode-rgb-led-function-11.png)

Duplicate the `analog write` block twice.

![makecode-rgb-led-function-12](assets/makecode-rgb-led-function-12.png)

Place the two duplicated `analog write` blocks in the `red` function. Change the pins as in the previous lesson. Change the values to illuminate the RGB LED red (255, 0, 0).  

![makecode-rgb-led-function-13](assets/makecode-rgb-led-function-13.png)

Duplicate the function block twice.

![makecode-rgb-led-function-14](assets/makecode-rgb-led-function-14.png)

The `red` function duplicates will stack.

![makecode-rgb-led-function-15](assets/makecode-rgb-led-function-15.png)

Rearrange the duplicated blocks.

![makecode-rgb-led-function-16](assets/makecode-rgb-led-function-16.png)

The names of the `function` blocks and the values now must be changed.

![makecode-rgb-led-function-17](assets/makecode-rgb-led-function-17.png)

Change the names of the one function name to `green` with the green values (0, 255, 0). Change the other function name to `blue` with the blue values (0, 0, 255).

![makecode-rgb-led-function-18](assets/makecode-rgb-led-function-18.png)

Now that the functions have been defined, we need to call the functions. Click on the "Functions" drawer of the Toolbox. The function `call` blocks will appear here. 

![makecode-rgb-led-function-20](assets/makecode-rgb-led-function-20.png)

Drag the function `call` blocks to the `forever` block.

![makecode-rgb-led-function-21](assets/makecode-rgb-led-function-21.png)

As in the previous section, you will add delays to control the duration that the color flashes. Click on the "Basic" drawer.

![makecode-rgb-led-function-22](assets/makecode-rgb-led-function-22.png)

Select the `delay` block.

![makecode-rgb-led-function-23](assets/makecode-rgb-led-function-23.png)

Place the `delay` block after the `call red` block. Change the duration that red will stay on.

![makecode-rgb-led-function-24](assets/makecode-rgb-led-function-24.png)

In this example, we will use `500` again, but feel free to experiment with the delay. 

![makecode-rgb-led-function-25](assets/makecode-rgb-led-function-25.png)

Duplicate the `delay` block twice.

![makecode-rgb-led-function-26](assets/makecode-rgb-led-function-26.png)

Place the duplicated `delay` blocks after the `call` boxed.

![makecode-rgb-led-function-27](assets/makecode-rgb-led-function-27.png)

The program is now complete. The LED should alternate red, green, and blue every half a second using functions.
