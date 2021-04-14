# Electronic Set Up of the Syringe Pump

## Schematic of how the arduino, breadboard, motor, and power will connect.

![Electronics Schematic](Syringe-Pump/Electronics-Schematic.png)

## Diagram of Wiring from Lecture

![Electronics Image](Syringe-Pump/pptschematic.png)

## Image of my arudino and breadboard wiring

![Electronics Image](Syring-Pump/Electronics-Image.png)

## My running Syringe Pump!

![Pump Running](Syringe-Pump/Assembly_Pictures/20210408_102127.mp4)


# Food for Thought
By playing with the running syringe pump, we were able to calculate the steps per mL and the max flow rate of the instrument. Thinking about the steps per mL, we saw that microstepping can be controlled on the chip by wiring the MS1,2,3 ports to either 4 volts (low) or 24 volts (high). The resolution is the highest when all three pins are wired to high voltage, rather than low. The highest revolution we could achieve was 16 steps per rotation. Using simple algebra, we can calculate the steps per mL based on the given rotation distance. 

The max flow rate of the system is controlled 
