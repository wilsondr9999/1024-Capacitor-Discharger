# Capacitor Discharger

This project is a passive (unpowered) capacitor discharger that can safely discharge capacitors up to 450V and 1000 uF.  It assists the operator in quickly discharging the capacitor and providing visual feedback of the discharging process and its completion.


## Overview

![](img/Case-PCB-3D-Ortho.jpg)

The capacitor discharger is a handheld unit with 2 LEDs for indication, and two standard shrouded test lead ports on one end.  It's purpose is to allow safe discharge of a capacitor that is in-circuit prior to working on that circuit.  Capacitors can hold a charge, sometimes for a long period of time, and in some circuits the amount of energy they can hold is dangerous, even potentially lethal.

This unit allows the operator to touch two test leads to the capacitor terminals, and the unit will allow the capacitor to discharge at a constant rate of 125 mA.  This is sufficient current to discharge the largest capacitor that is recommended to be discharged with this unit (a capacitor rated up to 450V, and up to 1000 uF of capacitance) within about 15 seconds.

## Principle of Operation

The unit is a passive device, i.e. it is not powered and no batteries or power source is needed.  The energy in the capacitor is used to light the indicator LEDs during the discharge.

An IGBT transistor is used in a specific configuration to allow the capacitor to discharge at a constant current of 125 mA.  The capacitor's energy is dumped into 11 resistors rated at 5W each.

One LED (yellow) lights as the capacitor is discharging.  This LED will remain lit until the capacitor has no more energy (usually when it's voltage is less than 2V).

The other LED (red) lights if the capacitor voltage is above 30V.  This LED will extinguish when the capacitor has discharged to less than 30V, indicating that the capacitor would be safe to touch.

## Instructions for Use

Attach two test leads to the 4mm jacks on the end of the unit.  The unit does not have a polarity restriction, and can discharge capacitors in both orientations.  It is recommended that your test leads are of a type that are rated for at least the working voltage of the capacitor you intend to discharge.  If the voltage is greater than 50V, it is recommended to use high voltage test leads with a category rating of at least CAT I / 600V.

For voltages greater than 50V, use appropriate personal protective equipment (PPE), including electrical safety gloves and safety glasses.

With appropriate personal safety equipment in place, touch the test leads to the capacitor leads in either orientation.  The unit will begin discharging the capacitor, and you will see the yellow discharging LED light up.  The red >30V LED will also light if the capacitor voltage is currently greater than 30V.

Keep the test leads connected to the capacitor until the >30V LED light extinguished.  Once the >30V LED light is extinguished, the capacitor is safe to work with.  If the work requires as close to zero charge in the capacitor as possible, continue holding the test leads connected to the capacitor until the discharge LED light is extinguished.


