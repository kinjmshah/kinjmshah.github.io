---
title: "Automated Point-of-Care Pancreatic Cancer Diagnostic"
permalink: /portfolio/UPennSeniorDesign
---

Detected pancreatic cancer cell derived exosomes from human serum at concentrations modeling precancerous stages by developing an automated, microfluidics based point-of-care diagnostic device. Created automated, cost-effective, on-chip serum processing and diagnosis protocol involving 3D printed encasingdesigned using SolidWorks, Arduino based microcontroller, and image processing using MATLAB.          

### Bioengineering Senior Design Award
### 1st Honorable Mention - School of Engineering and Applied Science Senior Design Competition
<!-- [Senior Design Competition Presentation Video](https://www.youtube.com/watch?v=NbAuyVjuLLE&t=1s) -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/NbAuyVjuLLE?start=233" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Motivation
Point of care diagnostics still require significant manual pre-processing with expensive, non-portable equipment. To make point of care diagnostics a reality, complete sample processing needs to take place on-chip at the patient bedside. 
<div align="center">
  <img src='/images/seniorDesign/goals.png'>
</div>

## Workflow
The device brings diagnosis to the point of care: a physician injects a patient blood sample into our PDMS chip (which uses a size-based filter as a centrifuge substitute), and the sample is automatically processed to generate a diagnosis. The iPhone app videos and analyzes the fluorescence of tagged molecules to provide a diagnosis.
<div align="center">
  <img src='/images/seniorDesign/workflow.png'>
</div>

## Sample Processing
The automation involves arduino-programming to control a servo motor to rotate a series of syringes to dispense reagents on a timed basis, a solenoid to push a needle to puncture parafilm used to hold the reagents in the syringes via negative pressure for reagent dispensing, and a pump to remove fluids after each incubation period. This processes enables GPC1 positive exosomes to be tagged with fluorescent antibodies, enabling them to be imaged by the iPhone. 
<div align="center">
  <img src='/images/seniorDesign/process.png'>
</div>

## Device Design
The CAD model was designed in SolidWorks and 3D printed. The syringes were sealed with parafilm to create a vaccum in the tube to hold the liquid until the film is punctured by the needle attached to the solenoid. The syringes are held in a rotating disk which positions the appropriate reagent at the necessary time, as controlled by the microcontroller. 
<div align="center">
  <img src='/images/seniorDesign/cadModel.png'>   <img src='/images/seniorDesign/inside.png'>
</div>
