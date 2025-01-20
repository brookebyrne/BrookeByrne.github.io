---
title: "Syringe Pump"
excerpt: "A fully functional syringe pump assembley including both 3D printed and manufactured off-the-shelf parts that is capable of flow rates from 1 uL/min to 10 mL/min."
header:
  image: /assets/img/image.png
  teaser: /assets/img/Team Rendezvous Render.PNG
gallery:
  - image_path: assets/img/image.png
  - image_path: assets/img/Team Rendezvous Render.PNG
  - image_path: assets/img/wiring.png
  - image_path: assets/img/middlesupport.png
  - image_path: assets/img/endsupport.png
  - image_path: assets/img/insert.png
  - image_path: assets/img/middleinsert.png
  - image_path: assets/img/rodsupport.png
  - image_path: assets/img/motormountingplate.png
  - image_path: assets/img/carraige.png
---

## Purpose

Syringe pumps are biomedical devices designed to administer medication and small amounts of fluid to a patient via an intravenous line. The benefit of using a syringe pump is its ability to introduce a precise dosage of medicine into a patient’s body at a defined flow rate, which is necessary for certain conditions. Standard syringe pumps used in hospitals and other medical settings range in cost from $1500 up to $7000. Many patients, including NICU babies and chemotherapy patients, require this type of technology for treatments, however its cost makes it financially inaccessible for many. Several measures have been taken to utilize additive manufacturing and 3D printing to develop syringe pumps, infusion pumps, and other technology that can function the same way a standard pump would. This method is also more cost effective, as 3D printing is inexpensive, along with the other components required to operate the pump, such as an Arduino, motor, buttons, a potentiometer, and a switch. The use of these alternative solutions for a syringe pump in hospitals and other medical settings would assist in eliminating the financial barrier for many patients without compromising quality of care.

## Features

* **Compatible with Multiple Syringe Diameters** The 3D printed parts have been intentionally designed to include an insert that would allow for use with multiple different standard sizes of syringes.
* **LED Indicator Light** This pump includes an LED light to turn green when running, yellow when paused, and red when out of liquid.
* **Supports a Wide Range of Flow Rates** The syringe pump has been programmed to function from flow rates 1 uL/min to 10 mL/min. The flow rate can be controlled using a potentiometer on the side of the box.
* **Easy Reset** The pump can move both backwards and forwards using the buttons on the side of the box to easily reset the syringe pump after use.

## Off-The-Shelf Required Parts
| Part Name | 
|-----------|

## 3D-Printed Parts

| Part Name |
|----------------------|
| Middle Support |
| End Support |
| Rod Support |
| Motor Mounting Plate |
| Carriage |
| Middle Insert |
| Syringe Insert |

## Operating Instructions

In order to operate the syringe pump properly, these instructions must be followed. Assuming that the proper code has been uploaded to the Arduino, the user can plug the power supply into an outlet. Once connected to the power supply, the user can load the syringe into the  syringe pump. Once the syringe is properly loaded, the user can then push the latching button to activate the motor. The latching button is used to start or pause the motion of the pump, therefore only when the button is pushed can the motor spin. After the latching button is pressed to activate the motor, the user can also push either of the two monetary buttons to change the direction of the motor, clockwise or counterclockwise. This will either push or pull the plunger. The user can also use the potentiometer dial to adjust the flowrate of the pump. Additionally, when the motor is running, the LED will display a green light. When the latching button is pressed to pause the motor, the LED will change from green to yellow. When the latching button is pressed to reactivate the motor, and the pump releases all of the liquid that it was previously holding, the LED will change from green to red. Once the LED is red, the user will know that the syringe pump has finished its task, and the user can reset the pump back into its original position.

## Arduino Code
The arduino code used to program the syringe pump can be found [here](https://github.com/brookebyrne/SyringPumpArduino/blob/main/code) in my Github repository.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e66b6ac86d6a05dc1?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Syringe Pump Photo Gallery" %}
