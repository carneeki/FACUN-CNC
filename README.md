# FACUN-CNC
It's not FANUC. It's FUCAN!

FUCAN CNC is a collection of circuits designed to enable connection of an Arduino,
probably running Grbl, to the "real world".

Developed by an impoverished university student, it is designed to be budget conscious,
whilst minimising compromises on things that are nice to have. One example is that all
logic components are in DIP form factor so they can be socketed and easily replaced in
the event that the magic smoke escapes a component.

## TRI-LIMIT-INTERFACE
TRI-LIMIT-INTERFACE is a 3 axis limit switch debounce and logical OR board. Because we
often have limit switches at each end of our axis limits, this handles debouncing both
ends, and sending a single clean signal to the Arduino.

Grbl has some debounce routines in it, but having this board enables changing to other
systems that may not have debouncing built in.

# LIMIT-INTERFACE
LIMIT-INTERFACE is a single axis, strip board version of the 3 axis board. Not
everyone can fab a PCB, and not everyone can afford to have the large 3 axis board
professionally fabbed. The strip board version can be easily made (and tripled) while
getting started. Once you are up and running, you should be able to route the TRI
version if you are so inclined.

## PUSHBUTTON-DEBOUNCE
PUSHBUTTON-DEBOUNCE is a board for debouncing pushbutton switches.

## ArduinoMiniPro Breakout
The Arduino Mini Pro is a really neat little board. It takes an Arduino and puts it
into a wide DIP array.
