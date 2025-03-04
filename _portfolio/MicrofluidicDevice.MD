---
title: "Microfluidic Particle Sorting Device"
excerpt: "A microfluidic device functioning to sort particles of 125 – 150 μm diameter from 425 – 500 μm diameter particles from a mixed solution."
header:
  image: /assets/img/Team Rendezvous Render.PNG
  teaser: /assets/img/Team Rendezvous Render.PNG
---

## Introduction

Microfluidic devices function like circuit boards for liquids and use small channels to transport minute volumes of fluids. Some channels can be as small as 60 microns, allowing for precise resolution and manipulation of the liquids. These devices have many applications, including medical diagnostics, DNA sequencing, tissue engineering, and environmental testing. Their functionalities include droplet generation, mixing, and particle separation. A key advantage of microfluidics is that, by the principles of fluid mechanics, gravity and inertia have negligible effects, resulting in purely laminar flow without turbulence.

One method used in specifically microfluidic particle sorting is Pinch Flow Fractionation (PFF). This technique relies on a device with a narrow "pinched" section followed by a wider "broad" section. When a fluid containing particles of varying sizes enters the pinched region along with a high-velocity sheath flow, the particles are pushed toward the upper wall at a distance proportional to their radius. As the particles enter the broad section, they follow distinct trajectories based on their initial displacement in the pinch section, enabling efficient size-based separation. Channels are then placed at distinct heights that depend on the trajectories. The heights of trajectories can be calculated by the equation…


Y0 = (wp-D/2)*wb/wp

Where Y0 is the height, wp is the width of the pinch section, wb is the width of the broad section, and D is the diameter of the particle you are trying to separate.

A key application of pinch flow fractionation is in biological research, particularly for sorting and isolating bacteria. For example, recent work has demonstrated the use of PFF to separate bacterial species based on size variations (de Timary et al., 2023). This capability has significant implications for microbiology, diagnostics, and environmental monitoring.

## Instructions

The fabrication of a microfluidic device begins with designing a CAD model that serves as the negative mold for casting the device. The CAD model must include precise channel extrusions while ensuring structural integrity. That being said, to prevent printing failures, tall and thin components should maintain an aspect ratio of less than 4:1, and inlets and outlets must be spaced at least 11 mm apart to avoid interference with the barbs that will later be inserted. The channel dimensions are critical; the smallest channel should be at least 1.2–1.5 times the diameter of the largest particle to prevent clogging. Since PFF is a two-dimensional separation method, the channel depth should be just large enough to accommodate the largest particle to avoid stacking. Outlet channels should be designed symmetrically to ensure even flow distribution and resistance and prevent recombination of separated particles.

Once the CAD design is finalized, a resin mold is printed and cured. The mold must be perfectly flat to ensure uniform bonding to a glass slide. The support material should be added on the bottom of the mold and the mold must lay perfectly horizontal. You can ignore warnings from the printer about cupping. After printing you must wash the mold in isopropyl alcohol (IPA) for a total of 10 minutes—five minutes on the print bed and five minutes in a fresh IPA bath—before allowing it to dry for 30 minutes. Uncured resin must be completely removed, as residual resin can interfere with polydimethylsiloxane (PDMS) curing, leading to defects in the final device. The mold undergoes a short surface cure (60 seconds) to prevent warping, and support materials are carefully removed to avoid damage.

To further enhance the device's durability, a parylene coating can be applied. Parylene is a biocompatible, moisture-resistant polymer that forms a thin protective layer over the mold or the final device. This coating prevents uncured resin monomers from leaching into the PDMS, which could otherwise disrupt crosslinking, leading to feature loss or incomplete curing.

Next, PDMS is cast into the prepared mold. PDMS is commonly used in microfluidics and is mixed in a 10:1 ratio of base to curing agent, degassed in a vacuum chamber to remove air bubbles, and poured into the mold. The mold is then placed in an oven at 65–80°C for at least an hour to ensure complete curing. After cooling, the cured PDMS is carefully peeled from the mold, and inlet/outlet holes are punched to allow fluid flow.

The final step is plasma bonding the PDMS device to a glass slide, ensuring a strong, leak-proof seal. Plasma bonding involves exposing both the PDMS surface and the glass slide to oxygen plasma, which activates the surfaces by creating reactive groups. When pressed together, these surfaces form a covalent bond, ensuring durability and preventing fluid leakage during the operation of the device. This step is crucial for maintaining laminar flow within the microfluidic channels, optimizing the performance of the PFF process.

## Discussion

1. Why are resin-printed molds coated with parylene prior to casting the PDMS? What are hypothetical applications of your microfluidic mixer or sorter?

Resin-printed molds are coated with parylene because it creates a smooth, protective layer that prevents uncured resin from interfering with PDMS curing. Without this coating, the PDMS might not fully set, leading to defects in the final device. Parylene also makes it easier to remove the PDMS without damaging small features.

A microfluidic sorter like this could be used in medical diagnostics to separate different types of blood cells, in bacteria detection, or even in environmental testing to filter tiny pollutants from water. A microfluidic mixer could be useful for drug development or diagnostics, where small liquid volumes need to be mixed precisely for chemical reactions.

2. Why is your geometry conducive to sorting? Discuss specific dimensions (pinch width, outlet width, location of ports, etc.)
The pinched section of the device is designed to align particles based on size before they enter the broader section, where they separate into different paths. The pinch width is narrow enough to force particles into a single-file line, ensuring they sort correctly. The outlet widths are balanced to avoid one outlet from having more resistance than another, and the holes are spaced far enough apart to prevent interference of the barbs that come out of the holes. The depth of the channels is just slightly larger than the biggest particle to stop stacking, ensuring only a single layer of particles moves through at a time.

3. What steps or design features did you use to ensure that each outlet received the same flow rate, preventing disruptions to the streamlines and maintaining proper separation?

To keep flow rates equal, the outlet channels were made with the same cross sectional area and depth, ensuring no one channel has more resistance than another. If outlets are too different, particles might recombine, ruining the sorting process. 

4. Based on the results of testing, could you implement any future changes to improve sorting?

The pinch width might need adjustment to better separate smaller particles. If there was too much overlap in particle paths, changing the geometry of the channels and the CSA could help keep particles on distinct trajectories. Another improvement could be using a different outlet configuration to ensure particles exit the broad section evenly. If clogging was an issue, increasing the channel size slightly might help prevent blockages.

5. Did you attempt the bonus opportunity? If so, describe your approach and success.

I did not attempt the bonus opportunity.


## References 

de Timary G, Rousseau CJ, Van Melderen L, Scheid B. Shear-enhanced sorting of ovoid and filamentous bacterial cells using pinch flow fractionation. Lab Chip. 2023;23(4):659-670. doi:10.1039/D2LC00969B.

## Mold



## Casted Device



## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e66b6ac86d6a05dc1?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Syringe Pump Photo Gallery" %}
