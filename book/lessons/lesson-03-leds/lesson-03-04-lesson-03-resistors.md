![header-lesson-03](assets/header-lesson-03.png)

# Resistors

## What is a resistor?

A **resistor** is a small but essential part of many electronic circuits. Its job is to control the flow of electricity, almost like a valve controls water in a hose. Resisting or slowing down the electrical current helps keep other parts in the circuit, like lights or motors, from getting too much power and burning out. Resistors come in different strengths, which allow engineers and scientists to decide exactly how much they want to slow down the electricity in different parts of a circuit, ensuring everything works smoothly and safely.

Imagine you have two water tanks, each with a spout at the bottom where the water comes out. If one tank has a big spout and the other has a smaller spout, the water will flow out much faster from the tank with the big spout than from the one with the smaller spout. 

![water-analogy-01](assets/water-analogy-01.png)

Resistors work similarly with electricity. They are like the spouts on the tanks: a resistor with a lower resistance (*R*) lets more electric current (*I*) flow through, like a big spout, while a resistor with a higher resistance lets less electric current, similar to a small spout. This helps control how much electricity goes through different parts of a circuit, like controlling how fast water flows out of the tanks.

![water-analogy-02](assets/water-analogy-02.png)

## Ohm's Law

**Ohm's Law** is a simple rule that helps us understand how electricity works in a circuit. It says that the **electric current** (*I*) flowing through a circuit is directly related to the **voltage** (*V*), which is the push that makes the electricity move, and inversely related to the **resistance** (*R*), which slows down the electricity. 

Think of it like this: if you increase the voltage (*V*), more electric current (*I*) will flow, but if you increase the resistance (*R*), less electric current (*I*) will flow. Ohm's Law helps us figure out one of these things (current (*I*), voltage (*V*), resistance (*R*) if we know the other two, making it easier to design and troubleshoot circuits or calculate the correct resistor value needed in a circuit.

Ohm's law has three formulas. These formulas are commonly represented in a triangle as illustrated below: 

![ohms-law](assets/ohms-law.png)

The three main formulas show the relationship between voltage (*V*), current (*I*), and resistance (*R*). The first formula is  $V = IR$ , which means voltage is the product of current and resistance. The second formula is  $I = \frac{V}{R}$ , which tells us that current is equal to voltage divided by resistance. The third formula is  $R = \frac{V}{I}$​ , which shows that resistance is equal to voltage divided by current. By using these formulas, we can figure out any one of the three values if we know the other two.

## Resistor Color Bands

Resistor color bands are a visual code representing a resistor's resistance value and tolerance, helping engineers and hobbyists quickly identify its specifications in electronic circuits.

There are 2 types of resistors. Four-band resistors and five-band resistors.

![four-five-band-resistor](assets/four-five-band-resistor.png)

Four-band resistors are more commonly included in most hobby kits.

## Interpreting Four-Band Resistors

The color bands on a resistor tell you how strong the resistor is or how much it slows down the electric current. Each color represents a different number, and by reading the colors in a specific order, you can figure out the resistor’s value in ohms.

The values of a resister can be interpreted with the chart below:

![resistor-chart](assets/resistor-chart.png)

The four-band resistor chart helps you determine a resistor's value by looking at its colored stripes. The first two bands represent the first two digits of the resistor’s value. The third band is a multiplier. It tells you how many zeros to add to those two digits. The fourth band shows the tolerance, which tells you how accurate the resistor’s value is, meaning how much it can vary from the stated value. 

The chart allows you to decode the resistor's value in ohms (Ω) by matching the colors to their corresponding numbers.

Here is an example of interpreting the value of a four-band resistor using the color chart.

![resistor-chart-example](assets/resistor-chart-example.png)

## Checkpoint: Interpreting Resistor Values  

Use the resistor chart to interpret the resistor codes below:

![resistor-chart](assets/resistor-chart.png)

![resistor-quiz](assets/quiz-resistor.png)



```{admonition} Click here to reveal the solutions.
:class: dropdown
Solutions:
![resistor-quiz-solutions](assets/quiz-resistor-solutions.png)
A: 1, 0, 1kΩ ⟹ 10 × 1kΩ = 10kΩ<br>
B: 2, 7, 100Ω ⟹ 27 × 10Ω = 270Ω<br>
C: 4, 7, 100Ω ⟹ 47 × 100Ω = 4700Ω = 4.7kΩ<br>
D: 1, 0, 10Ω ⟹ 10 × 10Ω = 100Ω
```