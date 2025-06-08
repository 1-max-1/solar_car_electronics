# Solar car power electronics
![20241006_190208 (1)](https://github.com/user-attachments/assets/8429375f-b38d-4101-b26a-fb593ffa0a16)
![Image](https://github.com/user-attachments/assets/69b67532-8be0-4f2a-a504-522f4f5f946e)
![Image](https://github.com/user-attachments/assets/62ba5613-8f0d-467a-b030-b451a482d1b3)

*The PCB files are not public currently as this is a course assignment.*

This project is an efficient power electronics system designed to run a small solar-powered car. The main circuit elements are as follows:
- A buck converter designed to transfer power from the solar panels to the motors. The inductor `L1` is not shown in the 3d model, but it was an inductor that we designed and constructed using winding machines.
- PWM control IC to produce the signal that switches the buck converter.
- Push-pull system to drive the mosfet gate and reduce switching losses.
- Capacitor-based PI feedback loop to ensure the system was always operating at the solar panel's maxmimum power point. This ensures the highest amount of energy transferred to the motors, allowing the car to go further and faster.
The maximum power point depends on solar panel characteristics and can be adjusted depending on how sunny the weather is.

The system was constructed on a stripboard and added to a supplied solar car. We then raced against several other teams.
Our car easily won the first round, however the remainder of the race was cancelled due to weather changes so we did not get a chance to test it further.

A full PCB was also designed and ordered, but did not arrive in time for the race so the components were never transferred to the PCB.
