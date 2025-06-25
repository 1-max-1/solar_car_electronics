# Solar car power electronics
![20241006_190208 (1)](https://github.com/user-attachments/assets/8429375f-b38d-4101-b26a-fb593ffa0a16)
![Image](https://github.com/user-attachments/assets/69b67532-8be0-4f2a-a504-522f4f5f946e)
![Image](https://github.com/user-attachments/assets/62ba5613-8f0d-467a-b030-b451a482d1b3)

*The PCB files are not public currently as this is a course assignment.*

This project is an efficient power electronics system designed to run a small solar-powered car. The main circuit elements are as follows:
- A buck converter designed to transfer power from the solar panels to the motors.
- PWM control IC to produce the signal that switches the buck converter.
- Push-pull system to drive the mosfet gate and reduce switching losses.
- PI feedback loop to ensure the system is always operating at the solar panel's maximum power point. This ensures the highest amount of energy transferred to the motors, allowing the car to go further and faster.
The feedback loop is implemented with an RC network and an opamp, no software is used.
- The maximum power point depends on solar panel characteristics and can be adjusted depending on how sunny the weather is.

The inductor `L1` is not shown in the 3d model, but it was an inductor with a ferrite core that we designed and constructed ourselves using winding machines.
We had a maximum limit on the total capacitance in the circuit, so we put most of the capacitance on the input side. This minimized losses from the solar panel.
The output capacitance does not matter as much in this case because the motors were not largely affected by the voltage fluctuations.
And finally we chose the switching frequency to be as low as possible to reduce switching losses. The lower limit was decided by the maximum size of the capacitor.

The system was constructed on a stripboard and added to a supplied solar car. We then raced against several other teams.
Our car easily won the first round, however the remainder of the race was cancelled due to weather changes, so we did not get a chance to test it further.

A full PCB was also designed and ordered, but did not arrive in time for the race so the components were never transferred to the PCB.
