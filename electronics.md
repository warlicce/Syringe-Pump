# Electronic Set Up of the Syringe Pump

## Schematic of how the arduino, breadboard, motor, and power will connect.

![Electronics Schematic](/Syringe-Pump/sp/es.png)

## Diagram of Wiring from Lecture

![Electronics PPT Schematic](/Syringe-Pump/pptschematic.png)

## Image of my arudino and breadboard wiring

![Electronics Image](/Syringe-Pump/sp/ei.png)

## My running Syringe Pump!

<iframe width="560" height="315" src="https://www.youtube.com/embed/B65MKff-elY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# Food for Thought
By playing with the running syringe pump, we were able to calculate the steps per mL and the max flow rate of the instrument. Thinking about the steps per mL, we saw that microstepping can be controlled on the chip by wiring the MS1,2,3 ports to either 4 volts (low) or 24 volts (high). The resolution is the highest when all three pins are wired to high voltage, rather than low. The highest revolution we could achieve was 16 steps per rotation. By multiplying the microsteps by the known 200 rotations, we get 3200 steps per rotation. Using simple algebra, we can calculate the steps per mL by dividing the pitch by the steps to get a distance moved per step. This value can be divided by distance per mL on the syringe, which gives roughly 90 steps per mL.

The max flow rate of the system is controlled by the motor speed, but in reality the syringe pump could not spin as fast as the motor due to the friction between the nut and the bolt moving the plunger driver forward. Theoretically the max rate would be 700rpm x 1.25mm pitch, but that is not realistic.
