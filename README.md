# crystal-equivalent-circuit
This is a crystal equivalent circuit in LTSpice.

## Circuit in LTSpice

![kép](https://github.com/user-attachments/assets/d34090c7-9ad2-4987-abaf-4126414080c5)

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
