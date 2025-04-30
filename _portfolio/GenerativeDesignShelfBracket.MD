---
title: "Generative Design Shelf Bracket"
excerpt: "Shelf bracekets designed using Fusion360's generative design feature sustaining over 20lbs"
header:
  image: /assets/img/gd7.jpg
  teaser: /assets/img/gd7.jpg
gallery:
  - image_path: /assets/img/gd2.jpg
  - image_path: /assets/img/gd3.jpg
  - image_path: /assets/img/gd4.jpg
  - image_path: /assets/img/gd5.jpg
  - image_path: /assets/img/gd6.jpg
  - image_path: /assets/img/gd7.jpg
---

## Overview of the Part and Application
The part I designed for this project is a wall-mounted shelf bracket developed using generative design and produced through additive manufacturing, specifically Selective Laser Sintering (SLS). The final design had to conform to strict dimensional constraints imposed byrequirement of the project, which limited the maximum build size for any part to 120 mm × 120 mm × 120 mm. My design fell within a reduced envelope of 120 mm × 120 mm × 50 mm, a choice driven by the need to ensure reliable printability while leaving room for other student projects in the shared print queue.

The primary function of the bracket is to support a horizontal shelf capable of holding up to 20 pounds (approximately 9 kg) of distributed weight. This weight could include decorative items, books, small electronics, or other household objects like keys or a wallet. The design includes key structural and functional features such as wall-mounting holes, a flat surface where the shelf can rest, and an optimized geometry that reduces unnecessary material while maintaining mechanical integrity under realistic load conditions.

The bracket was made out of Nylon 12. Nylon 12 is well-known for its high tensile strength, excellent fatigue resistance, and moderate flexibility, making it particularly effective for parts that must bear loads without being brittle. 

A key objective of this project was to minimize the mass of the bracket while maintaining part strength. In additive manufacturing, this is critical because material consumption directly impacts the cost of production and the print time. Unlike traditional manufacturing processes that start with a block of material and remove waste, additive manufacturing only deposits material where it’s needed. This makes mass reduction both a practical and economical priority, especially for production-scale applications or designs using more expensive engineered materials.

## Real-World Relevance and Function
In a typical use case, this bracket would be printed in pairs and mounted to a vertical surface such as drywall, concrete, or wood using some fasteners. A shelf board—likely made of wood, acrylic, or composite material—would then be placed across the top surfaces of the two brackets to form a complete shelving unit. In this project I used two pieces of plywood, cut out by using a laser cutter, and glued on top of eachother. 

This part is relevant to me as I prepare to graduate and move into a new apartment, I will be responsible for furnishing my own living space for the first time. This shelf bracket not only serves a practical function in my future home but also acts as a tangible reminder of the skills I’ve developed through my digital fabrication coursework and minor. 

## Functional Value
While the market is already saturated with mass-produced shelf brackets made from metal or plastic, this project allowed me to create a bracket specifically tailored to my wants. The generative design approach produced a form that is lightweight and structurally efficient, with a geometry that would be difficult to manufacture using traditional techniques like injection molding or CNC machining.

Even though the final bracket may not be significantly cheaper than a commercially available one (particularly when considering the cost of SLS printing), the knowledge gained from the design process far outweighs any cost inefficiencies. Moreover, for contexts where space constraints, aesthetic preferences, or mounting conditions are unique, a custom-designed part becomes not just valuable-but necessary.

Additionally, this project helped me develop a greater appreciation for how generative design fits into the larger ecosystem of modern engineering. The bracket may be simple in application, but the experience of optimizing its geometry, analyzing its performance under real-world loads, and translating it into a physical part provided deep insights into the future of design. This bracket, therefore, represents more than a shelf support—it represents an educational tool, a portfolio piece, and a potential springboard into more complex, custom design challenges in my future career.

## Preserve and Obstacle Geometry
In my model, critical preserve regions included the mounting holes — one set that attaches the bracket to the wall and another that supports the shelf plank. These features needed to remain untouched by the generative solver to ensure that the part could be installed using standard fasteners and tools.
Obstacle geometries were defined around these preserved holes to ensure proper clearance for a screwdriver or drill during installation. Additionally, the area that contacts the wall had to remain flat and unobstructed for a flush mount. I also reserved a flat region at the top of the bracket where the shelf would rest securely.

## Load Case Application and Structural Constraints
To model realistic usage, I applied several types of forces in the generative design setup:
1. Gravity was applied to simulate the constant downward force that the shelf and stored items would exert on the bracket.
2. Bearing loads were applied at the points of wall contact to account for how the bracket would compress against the wall surface.
3. Downward point loads represented the weight of the shelf and any items placed on it, applied to the shelf mounting region.
4. Frictional forces were applied in multiple directions to simulate lateral movement — for instance, someone sliding an object off the shelf. These help ensure the bracket resists side-to-side and forward/backward motion.
5. Moment forces were applied at the edge of the shelf to simulate an unbalanced load, like a heavy object placed near the outer edge. This was important to test against potential rotational failure.

Each force was defined with direction and location based on statics principles and real-world usage. I used my knowledge from engineering coursework and refined assumptions using common-sense load paths — identifying where forces would naturally be applied through the bracket structure.

Fixed structural constraints were placed on all mounting holes, which means those regions were treated as fully anchored and immovable. This constraint simulates the actual conditions where the bracket is fastened tightly to a wall or shelf. These constraints guide the generative solver to build around realistic support points, which generally results in the material being distributed more heavily around these fixed areas to handle stress concentrations.

## Physical Testing for Refinement
To refine this design, I could prototype the bracket using Fused Filament Fabrication (FFF) with cheaper filament and perform physical testing. For instance, incrementally loading the shelf with known weights until deformation or failure occurs would allow me to validate or adjust my assumptions in the digital model. While the current shelf size is relatively small and would likely be used for lightweight items, the same process could scale to larger or more load-intensive applications with refined loading assumptions and geometry.

## Critique of Generative Design
Generative design proved to be an intriguing and educational tool, especially for parts where the structural efficiency is paramount. For a relatively simple part like a shelf bracket, it might be somewhat overengineered, but the design process taught me how forces and constraints interact in a highly visual and iterative way. I can see enormous value in applying generative design to complex assemblies where weight, performance, and irregular loading must be carefully balanced — such as in aerospace, automotive, and structural components.

For example, in Formula 1 racing, generative design could be used to create custom steering wheel components, engine brackets, or aerodynamic structural frames that are extremely lightweight but strong enough to handle the immense stresses of racing. Similarly, in medical device manufacturing, patient-specific implants could be optimized to reduce weight and improve bone integration using generative geometries tailored to individual anatomies.

However, it might fall short in aesthetic design fields where the primary goal is visual impact, not mechanical performance. A second example would be consumer packaging design, where function is usually overshadowed by brand, appearance, and tactile experience — factors that generative design isn’t nescarilly built for. 

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4af93a716a51fa792?mode=embed" width="1024" height="768" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Summary of Forces Applied

| **Name of Force** | **Magnitude** | **Location of Application** | **Rationale** |
|-------------------|----------------|------------------------------|----------------|
| Gravity | 9.807 m / s^2 | Entire part (global) | Represents constant weight from shelf and items |
| Bearing Load | 25 lbs | Wall-mounted mounting holes | Simulates compression against wall under weight |
| Downward Load | 25 lbs | Shelf-mounted holes (top) | Models the downward force of shelf + objects |
| Friction Forces | 15 lbs | Shelf surface and wall face | Accounts for lateral movement of shelf/items |
| Moment Load | 25 lbs | Outer edge of shelf | Simulates off-center loading or tipping forces |

## Shelf in Use
![shelf](/assets/img/gd7.jpg)

## Converged Outcome
![converged outcome](/assets/img/ss1.jpg)

## Chosen Model
I chose to go back in outcome interations because of the desired look of the bracket I wanted. I thought the converged outcomes were all a little boring. Plus I figured that this bracket would be able to support more weight anyway.

![chosen outcome](/assets/img/ss2.jpg)

{% include gallery caption="Shelf Photo Gallery" %}
