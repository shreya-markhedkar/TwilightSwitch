# Twilight switch with flashing light using transistor and light detecting resistor

![Screenshot 2023-02-11 142159](https://user-images.githubusercontent.com/81920073/218249444-0e5805c7-9fe7-4754-97c0-f08d6ee15b09.png)

## What is this?
The project is automatic flashing light with a twilight switch where LDR is used as a
sensor.
The components used are: light dependent resistors (LDR), transistors, LEDs, fixed
resistors, variable resistors, capacitors and wires. The variable resistor is used to adjust
the sensitivity of LDR.
In the presence of light, LDR offers low resistance and in dark it offers high resistance.

When light falls on LDR, it has a low resistance value, so there is sufficient base current
through transistor Q1 for the transistor to conduct. Its collector voltage is then small, so
that the transistors Q2 and Q3, n-p-n darlington, is off, and the LED is off.
When the surrounding light reduces, the resistance of the LDR increases until the base
current in Q1 becomes insufficient and the transistor switches off. Its collector voltage
then rises, Q2 conducts, and LED glows.
This process takes place quite quickly, because when the collector voltage of Q2 suddenly
becomes nearly 0 V, this potential is immediately applied to the base of Q1 via capacitor
C₁, which really cuts off Q1.
Then the capacitor charges. The LDR is now being illuminated by the lighted LED.
Owing to the optical feedback, the resistance value of the LDR diminishes, the voltage
across R2 increases, and T1 conducts again. The darlington pair switches off, and the
LED stops glowing.
Due to this feedback, this circuit works as an oscillator that works as a flasher light. 
