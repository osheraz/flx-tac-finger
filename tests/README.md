##  Procedure
All design files can be found in `cad` repo.\
<img src="pics/proc.jpeg" width=50% height=50% align="center">

1. **Print parts**: Print `FingerBody.stl` and `SensorSocket.stl` in PLA using 3D printer. 
2. **Mix silicone** : Mix your silicone according to the manufacturer requirements, we used Smooth-On's silicone, which are easy to use without any vacuum degassing requirement. Mix enough Mold Star silicone ( equal amount A:B) to fill the shell of the `FingerBody`.
3. **Pour silicone**: slowly pour the silicone into the shell of the `FingerBody`. Let the silicone rest for approximtly 3 hours.
4.  **Wall removal**: Carefully remove the thin-walled molds of the  `FingerBody` using a small utility knife.
5. **Glue FSR**: Position& glue the FSR 400 short into the  `SensorSocket`.
6. **Attach insert**: Attach M2 heat insert at the bottom of the  `FingerBody` .
7.  **Wire**: Wire the FSR sensor to an analog pin of the Arduino Nano through a voltage divider of 4.7k$\Omega$ resistor.

# Test
<img src="pics/MotoForce.png" width=30% height=30% align="center">

We test the characteristic force distribution of the FlX finger, we have designed an experiment using a six degrees-of-freedom robotic arm equipped with a Force/Torque sensor and a rigid pole at its tip. During the experiment, the pole was pushed against the finger with predefined forces between $0-10~N$ and at 50 equal length locations along the contact pad. Results for FlX finger with initial voltage of 200 (mV) are seen in `test` repo. 
To acquire somewhat repeatability of measurements, leveling screws on the back side of the finger body are used to vary the height of the sensor socket and, thus, tune the initial voltage on the FSR. By standard, we tune the initial voltage $V_o$ with a weight of 100 grams directly placed on the contact pad when in an horizontal posture.


## Reference

[1] Ma, R., & Dollar, A. (2017). Yale OpenHand Project: Optimizing Open-Source Hand Designs for Ease of Fabrication and Adoption. _IEEE Robotics & Automation Magazine, 24_, 32-40.







