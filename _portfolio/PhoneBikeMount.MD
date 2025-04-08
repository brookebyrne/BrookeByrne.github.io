---
title: "3D-Printed Phone Mount for Bike Handlebar"
excerpt: "A multimaterial 3D-Printed phone mount for bicyle handlebars using top-down modeling, fully customizable to user phone."
header:
  image:  /assets/img/pic.jpg
  teaser: /assets/img/pic.jpg 
gallery: 
 - image_path:  /assets/img/rendering.png
 - image_path:  /assets/img/pic.jpg
 - image_path:  /assets/img/gif1.gif
 - image_path:  /assets/img/detent.png
 - image_path:  /assets/img/c1.png
 - image_path:  /assets/img/c2.png
 - image_path:  /assets/img/c3.png
 - image_path:  /assets//img/c4.png
 - image_path:  /assets/img/c5.png
 - image_path:  /assets/img/c6.png
 - image_path:  /assets/img/c7.png
 - image_path:  /assets/img/c8.png
 - image_path:  /assets/img/c9.png
---

## Top Down Modeling
This project involved designing a custom phone mount with a rotatable detent mechanism, optimized for use with both cased and uncased phones. To approach this task, we used top-down modeling, which proved highly effective throughout the development process. Top-down modeling is a CAD strategy where the overall assembly and key features are defined first, and individual components are designed in the context of that assembly. This contrasts with bottom-up modeling, where parts are created separately and assembled later.

One of the main benefits of top-down modeling in this assignment was the ease of adjusting individual components without breaking the model or affecting other parts. For example, when tolerances or dimensions needed to be fine-tuned for 3D printing or assembly, I could edit a component directly in the context of the full model. Because of the shared references and in-context design, these changes propagated smoothly across the entire assembly. This workflow allowed me to maintain proper alignment and clearances, avoiding the common issue of one part becoming incompatible after modifying another. It also gave me the flexibility to prototype and iterate quickly, with confidence that each component would remain cohesive within the broader system.

##  Design Rationale
From the beginning, the design was guided by several core principles:
- Minimize part count: Fewer components meant a simpler assembly process and reduced potential points of failure.
- Sleek and lightweight: The goal was to avoid a bulky or cumbersome design, making the mount practical for everyday use.
- Compatibility with a variety of phones: I wanted the mount to accommodate both phones with and without protective cases, which often vary slightly in size.
- Incorporate a detent mechanism: A rotating detent mechanism was integrated to allow the phone to securely snap into portrait or landscape orientation.
- Ease of use: The user should be able to insert or remove the phone quickly while having the flexibility to rotate it on the go.

## Rotation Mechanism
The rotating mechanism used a detent system, which involves a ball bearing and spring placed in a cavity that clicks into predefined positions. In this design, the detent allowed the phone holder to snap between portrait and landscape orientations.

While the mechanism worked, it didn’t perform as well as I’d hoped. The primary issue was undersizing the detent system. The rotating disk and detent interface were too small relative to the weight and leverage of a modern smartphone, especially when mounted off-center on a bike handlebar. As a result, the detent didn’t provide as firm a lock as intended. In future iterations, I would increase the diameter and depth of the detent features to improve the tactile feedback and hold strength.

![dentent](/assests/img/detent.png)

![gif](/assests/img/gif1.gif)

## Adjustments for 3D Printing
I had to modify several dimensions to accommodate the realities of the 3D printing process. For parts printed using FFF (Fused Filament Fabrication) with TPU, I added a tolerance to prevent tight fits, accounting for slight over-extrusion and flexibility of the material. Additionally, for the rotating mechanism printed using powder SLS (Selective Laser Sintering), I included proper clearances between rotating parts to avoid fusion during sintering and ensure smooth movement after printing.

## Printing Technologies and Materials
A combination of FFF and SLS printing was used to produce the final prototype:
- FFF with TPU: The flexible arms that grip the phone were printed in TPU using FFF. TPU was chosen because of its elastic properties, allowing the arms to stretch around phones of different widths and hold them securely.
- SLS with nylon powder: The main body of the mount was printed using powder SLS, which provides strong, durable parts without the need for support structures. This was especially beneficial for printing complex curves and overhangs cleanly.
- FFF with PLA: Early prototypes were printed in PLA using FFF because it was cost-effective and fast, allowing for quick validation of form and fit.

One component was unfortunately excluded from the final SLS batch (needed to printed using FFF with PLA) because I didn’t complete the edits in time for the professor’s scheduled print job, which highlighted the importance of time management during the design cycle. However this did not hurt the overall functionality of the mount

## Assembly and Usage Instructions
To assemble the phone mount:
- Begin by fitting the main body over the detent mechanism, ensuring the ball bearing and spring are in place.
- Partially tighten the body assembly so that it can still slide over the handlebar.
- Insert the TPU arms between the two backing pieces, securing them with the center locking piece.
- Fold the arms inward and fasten them using nuts and bolts to hold them firmly in place.
- Mount the body onto the handlebar and fully tighten all fasteners.
- Once installed, you can easily slip your phone into the flexible TPU arms and rotate the holder to your desired orientation—portrait or landscape.

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a46baa72797a60dee6?mode=embed" width="1024" height="768" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Gallery
{% include gallery caption="Bike Phone Mount Gallery" %}
