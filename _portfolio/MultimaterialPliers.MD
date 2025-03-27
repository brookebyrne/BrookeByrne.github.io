---
title: "Multimaterial PLA/TPU 95 Pliers"
excerpt: "This project involves the design and fabrication of 3D printed pliers with a flexible spring component that allows for immediate functionality upon removal from the print bed."
header:
  image: /assets/img/plierpic5.jpg
  teaser: /assets/img/plierpic5.jpg
gallery:
  - image_path: /assets/img/plierpic1.jpg
  - image_path: /assets/img/plierpic4.jpg
  - image_path: /assets/img/plierpic5.jpg
---

## Print-in-place Parts

Print-in-place models are functional multi-component designs that work immediately after removal from the print bed, without the need for post-processing or assembly. These models are created through single material extrusion by carefully designing the parts and orienting the print to allow for clearance between printed joints where motion or rotation is required. However, even with optimized print settings, these models can be plagued by crunchy movement due to the irregularities of plastic extrusion. Another method to obtain useful motion is to include a flexible element in the model, whether that is a thin piece of a rigid plastic or a second elastomeric material.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a492af1e1da68b0a7e?mode=embed" width="1024" height="768" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Other Applications

Print-in-place models have been used in various applications beyond functional multi-component designs. According to a study by Sells et al. (2010), print-in-place techniques have been employed to create deployable structures, such as origami-inspired folding mechanisms, which can be printed as a single piece and then unfolded after printing (1). Additionally, research by Ou et al. (2016) has explored the use of print-in-place methods to fabricate adaptive, transformable structures that can change shape and functionality, such as morphing robotic grippers (2).

In terms of material combinations that work well for print-in-place, a combination of rigid and flexible materials has proven effective. Rigid materials, such as PLA or ABS, can provide structural support, while flexible materials, such as TPU or flexible PLA, can enable the desired motion or deformation (3). For example, a study by Fontana et al. (2019) investigated the use of a rigid PLA frame with TPU hinges to create print-in-place mechanisms with improved mobility and reduced crunchy movement (4).

## Iterative Design Process

The spring component was created by making one sketch with a repeating square infill pattern and notches on all 4 sides that would interlock with gaps on the handles. The dimensions of the flexible spring component were derived into sketches of both the handles and the jaws. The shapes of the spring were offset to allow for tolerance if needed, and the handles and jaws were built around these shapes. The jaws interface were flat, and the handles were built to be ergonomical. There needed to be space between the handles and the jaw to allow for the pliers to open and close. The sketches were each extruded upwards to the desired thickness, and the patterns and dimensions of the sketches allowed the design to easily be changed if needed. The parts were then assembled in a Fusion 360 assembly, and the project utilized Voron printers, TPU 95, and PLA.

## Relevant Specifications

- The jaw length is 68 mm.
- The pliers have a 5 mm gap between the jaws, allowing for a jaw capacity of up to 100 mm in length.
- The handles of the pliers are 100 mm in length.
- The pliers are not designed to handle a large amount of weight due to the use of 3D printed materials.

## Print Settings

Standard DF Lab 3D print settings were used for the TPU 95 and PLA materials. This included 2 top and bottom layers, 3 perimeter layers, and a modification to a honeycomb infill pattern. The infill density was set to 25% for the TPU and 15% for the PLA. No support material was necessary for this design.

## GIF

![gif](/assets/img/pliergif1.GIF)

![gif](/assets/img/pliergif2.GIF)

## References:

Sells, E., Bailard, S., Smith, Z., Bowyer, A., & Olliver, V. (2010). RepRap: the replicating rapid prototyper-maximizing customizability by breeding the means of production. Handbook of Research in Mass Customization and Personalization, 1, 568-580.

Ou, J., Dublon, G., Cheng, C. Y., Heibeck, F., Willis, K. D., & Ishii, H. (2016, May). Cilllia: 3D printed micro-pillar structures for surface texture, actuation and sensing. In Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems (pp. 5753-5764).

Engel, A., Bayer, D., & Oberloier, S. (2020). The use of flexible materials for fused filament fabrication of print-in-place mechanisms. Additive Manufacturing, 31, 100996.

Fontana, M., Zingali, A., & Rovetta, S. (2019, July). Design and characterization of 3D printed revolute joints for print-in-place mechanisms. In 2019 2nd IEEE International Conference on Industrial Cyber-Physical Systems (ICPS) (pp. 287-292). IEEE.



