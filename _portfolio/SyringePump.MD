---
title: "Syringe Pump"
excerpt: "A fully functional syringe pump assembley including both 3D printed and manufactured off-the-shelf parts that is capable of flow rates from 1 uL/min to 10 mL/min."
header:
  image: /assets/img/image.png
  teaser: /assets/img/Team Rendezvous Render.PNG
gallery:
  - image_path: assets/img/image.png
  - image_path: assets/img/Team Rendezvous Render.PNG
  - image_path: assets/img/Slide-4.png
   
---

# Purpose

Syringe pumps are biomedical devices designed to administer medication and small amounts of fluid to a patient via an intravenous line. The benefit of using a syringe pump is its ability to introduce a precise dosage of medicine into a patient’s body at a defined flow rate, which is necessary for certain conditions. Standard syringe pumps used in hospitals and other medical settings range in cost from $1500 up to $7000. Many patients, including NICU babies and chemotherapy patients, require this type of technology for treatments, however its cost makes it financially inaccessible for many. Several measures have been taken to utilize additive manufacturing and 3D printing to develop syringe pumps, infusion pumps, and other technology that can function the same way a standard pump would. This method is also more cost effective, as 3D printing is inexpensive, along with the other components required to operate the pump, such as an Arduino, motor, buttons, a potentiometer, and a switch. The use of these alternative solutions for a syringe pump in hospitals and other medical settings would assist in eliminating the financial barrier for many patients without compromising quality of care.

# Features

The syringe pump designed for this project was required to meet many parameters and constraints. These parameters and constraints included (a) the pump be driven by a stepper motor coupled to a lead screw; (b) the flow rate of the pump be set in the Arduino program & work with integer and decimal flow rate; (c) the pump be compatible with syringes of different diameters; (d) an LED light to turn green when running, yellow when paused, and red when out of liquid; (e) a latching button to start and pause the motion of the pump; (f) a switch that is triggered when the plunger has reached its limit; (g) short and clean electrical writing with proper terminations; (h) protection of electrical components from user and exposure to liquids; (i) unique branding on our enclosure to distinguish our design from other teams; (j) assembled as a single unit; (k) two monetary buttons that move the motor clockwise and counterclockwise; and (l) potentiometer to control the flowrate of the pump.

* **Massive Print Area: 1140 x 1200 x 1100 mm.** With a build envelop just shy of 4 feet in all dimensions, the LF3DP is capable of printing furniture and other large objects.
* **High Volumetric Output Extruder: 1 kg/hr - 450 C.** This printer come standard with a MDPH2 extruder by Massive Dimension, which can extrude at a rate of 1 kg/hr. Unlike typical filament extruders, the MDPH2 uses a screw to convey and liquify plastic pellets before the molten material is pushed out of a large nozzle (1 to 5 mm extrusion diameter). Please note: This printer can also be configured for other high flow rate extruders, such as the Typhoon and Pulsar by Dyze Design.
* **Affordable Pellet Feedstock** Pellets are the cheapest form of feedstock for any plastic-based manufacturing process. Save 50-75% of material costs by using pellets instead of spools of filament. Concentrated colorant can be added to the virgin material to achieve any color in the rainbow without requiring large amounts of storage. Recyled material can also be used for sustainable material printing.

# Off-The-Shelf Required Parts


# 3D-Printed Parts


# Operating Instructions

In order to operate the syringe pump properly, these instructions must be followed. Assuming that the proper code has been uploaded to the Arduino, the user can plug the power supply into an outlet. Once connected to the power supply, the user can load the syringe into the  syringe pump. Once the syringe is properly loaded, the user can then push the latching button to activate the motor. The latching button is used to start or pause the motion of the pump, therefore only when the button is pushed can the motor spin. After the latching button is pressed to activate the motor, the user can also push either of the two monetary buttons to change the direction of the motor, clockwise or counterclockwise. This will either push or pull the plunger. The user can also use the potentiometer dial to adjust the flowrate of the pump. Additionally, when the motor is running, the LED will display a green light. When the latching button is pressed to pause the motor, the LED will change from green to yellow. When the latching button is pressed to reactivate the motor, and the pump releases all of the liquid that it was previously holding, the LED will change from green to red. Once the LED is red, the user will know that the syringe pump has finished its task, and the user can reset the pump back into its original position.

# Arduino Code
The arduino code used to program the syringe pump can be found here in my Github repository.

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e66b6ac86d6a05dc1?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Large Format 3D Printer Gallery" %}
