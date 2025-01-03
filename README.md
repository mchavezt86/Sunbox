<picture>
  <img alt="Shows Sunbox" src="./screenshots/Sunbox.jpg">
</picture>

---

<div align="center">
    <h1>SunBox: Screen-to-Camera Communication with Ambient Light</h1>
</div>

Using [Camera2 API][1] as the starting point, this repository contains the main code for the **Sunbox** Android app.

Description
------------

The code follows the following logic:
1. Select the appropriate resolution, the type of code (QR or DM) and the rate of Reed-Solomon code
2. Once the camera starts, it will try to detect the screen (FLCoS reflecting sunlight).
3. The detection succeeds when a rectangle is drawn surrounding the screen.
4. By pressing the circular button, the camera starts capturing the QR or DM codes transmitted and
based on the information from step 1, the program decodes the message.

Requirements
------------
* The code requires the FLCoS from **Sunbox** specified in the [Sunbox paper](https://dl.acm.org/doi/10.1145/3534602).
* The information displayed by **Sunbox** should be created [this code](https://github.com/mchavezt86/SunboxVideo).
* The hardware parts that are modelled in [this site](https://github.com/mchavezt86/FreeCAD-PhD/tree/master/Sunbox). 

Citation
------------
If you find this repo useful for your academic work, please cite our [original paper](https://dl.acm.org/doi/10.1145/3534602).

[1]: https://developer.android.com/reference/android/hardware/camera2/package-summary.html
