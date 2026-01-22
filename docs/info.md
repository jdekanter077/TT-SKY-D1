<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This is a redo of a very minimal UART reviever which I made as Matura-Project in Gymnasium. [Hackaday Link](https://hackaday.io/project/189419-analogdiscrete-uart-reciever). It can switch between a internal and external clock signal, and will automaticly detect when there is a UART message coming into the input. Then it activates the shift register to sample the input and will stop sampling when the start bit has travelled through the shift register. A Parity Check will be done, and the result outputted.

UART INPUT: rx_i
CLK INPUT: clk_i

output: all the recieved bits and the parity match signal.

## How to test

Send a UART message to the input and watch if the data bits match what you sended

## External hardware

UART Input, (optional) CLK Input, LED Output
