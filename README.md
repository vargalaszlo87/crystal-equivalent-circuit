# crystal-equivalent-circuit
This is a crystal equivalent circuit in LTSpice. "A crystal is nothing more than a tunable impedance."

## Circuit in LTSpice

The frequency of the crystal is ~10.00MHz in this case.

$$R_{S} = 20ohm$$

$$C_{S} = 0.004pF $$

$$L_{S} = 63.325738mH $$

$$C_{P} = 5pF $$

![kép](https://github.com/user-attachments/assets/d34090c7-9ad2-4987-abaf-4126414080c5)

## Simulation results

**Impedance plot**

The series impedance is **10.00MHz**, the paralell is **10.004Mhz**. The delta is 4.007kHz.

![kép](https://github.com/user-attachments/assets/42156623-88d6-40e8-9bae-af090512c1c7)

**Phase plot with type**

![kép](https://github.com/user-attachments/assets/376e1d4f-15b1-42de-86ba-df3d5c25d770)


## Equations

### Series resonant frequency

$$f_{s} = \frac{1}{2 * \pi * \sqrt{L_{s} * C_{s}}}$$

### Parallel resonsnat frequency

$$f_{p} = \frac{1}{2 * \pi * \sqrt{L_{s} * \left(\frac{C_{p} * C_{s}}{C_{p} + C_{s}}\right)}}$$

### Impredances

$$R = R$$

$$X_{LS} = 2 * \pi * f * L_{s}$$

$$X_{CS} = \frac{1}{2 * \pi * f * C_{s}}$$

$$X_{CP} = \frac{1}{2 * \pi * f * C_{p}}$$

**Series**

$$Z_{s} = \sqrt{R_{s}^2 + (X_{LS} - X_{CS})^2 }$$

**Parallel**

$$Z_{p} = \frac{Z_{s} * X_{CP}}{Z_{s} + X_{CP}}$$
