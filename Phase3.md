# Air Brakes - Phase 3 Report

Team: Katherine Heaslet, Jamison Cabral, Alex Wang, Benjamin Given, Isaac Rosas, Johnathan Villeneuve

---

## 1. Fabrication Details

### 1.1 Printer Used
To fabricate the model and assembly components, a Bambu P2S was used with a 0.4 mm nozzle and a textured PEI plate. This allowed access to a build plate large enough to print nearly all components in two plates, and allowed for easy rapid iteration and prototyping of individual components. 

### 1.2 Filament Type
For this model, basic Ash Grey PLA was used to print all components besides hardware. PLA offers material properties that sufficed for the functionality of the prototype. That mainly includes structural stiffness, low friction across certain build plate patterns, and ease of printability.

### 1.3 Print Settings
When printing all components, consistent print settings were used. This includes the following:

**Strength Settings:**  
15% infill was used with a grid pattern. 5 top shells each with 1 mm thickness using rectilinear patterns for the inner solid surfaces and monotonic line patterns for exposed solid layers. 2 wall loops.

**Quality Settings:**  
Layer heights of 0.2 mm each. 0.012 mm resolution. Arc fitting enabled. Aligned seam positions.

**Support Settings:**  
Grid support patterns were used to increase print quality consistency, regardless of the increased usage of filament. A threshold angle of 30 degrees was used. Initial layer density of 90%. Top and bottom z distance of 0.2 mm.

### 1.4 Number of Prints and Reprints
In total, over 15 individual prints were done, including printing plates containing multiple components were completed. Most of these prints included iterated components with adjusted tolerances. A list of components and print counts:

| Component   | # Prints |
|------------|---------|
| Linkage     | 5       |
| Spindle     | 4       |
| Lower Base  | 1       |
| Upper Base  | 4       |
| Small Pin   | 6       |
| Dowel       | 5       |
| T-Rail      | 7       |
| Air Flaps   | 9       |

### 1.5 Problems Encountered During Printing
The largest error encountered during printing was PEI bed adhesion. After lots of usage the printer bed can get oils tracked on from hands. This prevents filament from sticking to the bed during printing and can lead to prints completely failing. The solution to this was cleaning with hot water and dish soap, ensuring adhesion by watching the behavior of the water on the build plate after washing.

---

## 2. Assembly Procedure and Challenges

### 2.1 Step-by-Step Assembly Process
Assembly is begun by pressing the upper base into the lower base after aligning the cross pattern of the lower base with the upper base. After, the t-rails get screwed into the upper base of the air brake frame, ensuring straight alignment of the flap path. After, the flaps are slid onto the t-rails, and pins are inserted into the flaps. Next, the spindle is attached to the center, with pins being inserted into the spindle as well. Lastly, the linkages are attached to connect the spindle to the flaps.

### 2.2 Tools and Methods Used
A hammer was used to press dowels into the linkages, and an electric screwdriver was used to attach the t-rails to the air-brake frame.

### 2.3 Challenges During Assembly
Main challenges during assembly involved pins breaking, flap rail guides breaking, and tolerance editing. Pins would get stuck in the linkage, spindle or airflap after breaking, and involve reprinting. Another challenging aspect was trying to get the screws to sit flush with the surface of the t-rails to prevent friction in the sliding of the flaps on the t-rails.

### 2.4 Adjustments
Main tolerance issues stemmed from t-rail adapter guides on the flaps, and pins connecting linkages to spindles and flaps. Pins were created to allow for slight movement to ensure smooth functionality. The pins were made larger than original to ensure the absence of shear stress failure. Holes and tolerances with each connecting component were adjusted to account for the new pin sizes. The wall width of the t-rail adapters on the flaps were lessened to reduce friction with the air brake frame.

---

## 3. Test Procedures, Results, and Interpretation

### 3.1 Description of Test Setup
The final assembly of the airbrake mechanism was tested without the use of a servo motor. Instead, manual input was applied by rotating the central spindle by hand. This allowed for direct observation of the mechanism’s motion and interaction between components. The fully assembled system included the spindle, linkages, pins, guide rails, and airbrake flaps.

### 3.2 Testing Methods
The testing focused primarily on evaluating the kinematic behavior of the mechanism. The following methods were used:

**Motion Test:**  
The central spindle was manually rotated to observe deployment and retraction of the airbrake flaps.

**Functionality Test:**  
The mechanism was checked to ensure that all linkages, pins, and flaps moved together as intended.

**Repeatability Test:**  
The spindle was rotated multiple times to verify consistent motion during repeated deployment and retraction cycles.

**Cantilever Behavior Check:**  
The airbrake flaps were observed during motion to ensure they behaved as cantilevered members, remaining properly constrained at their connections while extending outward without unintended rotation or excessive deformation.

### 3.3 Results Obtained
When the central spindle was rotated, the linkages successfully actuated all four flaps, causing them to deploy outward. Reversing the rotation retracted the flaps back into their original position. The motion of the system was generally smooth and followed the intended linear deployment path.

However, some resistance was observed during rotation. This was primarily due to the use of PLA material and the inherent friction between 3D printed surfaces. Minor roughness in motion was noticeable, especially at certain positions in the rotation.

### 3.4 Interpretation of Results
Overall, the mechanism functioned as expected and validated the intended slider-crank motion predicted in Phase 2. The synchronized movement of the flaps confirmed that the linkage system was properly designed and assembled.

The observed resistance and lack of perfectly smooth motion are attributed to material limitations and manufacturing tolerances associated with FDM 3D printing. PLA components introduce higher friction and less precise surface finishes compared to machined parts.

In a final manufactured version using Aluminum 6061 components and low-friction interfaces such as PTFE-lined surfaces, the motion is expected to be significantly smoother and more efficient. Therefore, while the prototype demonstrates correct functionality, improvements in material and manufacturing would enhance overall performance.

---

## 4. Comparison with Phase 2 Predictions

### 4.1 Expected Performance (from Analysis/Simulation)
Phase 2 predicted smooth and synchronized deployment of the airbrake flaps using a slider-crank mechanism. The system was expected to operate without interference, and analysis showed that stresses in the components would remain well below yielding or failure limits.

### 4.2 Actual Performance
The prototype demonstrated the same overall motion behavior, with the spindle successfully actuating the linkages and deploying the flaps as intended. However, due to 3D printing tolerances, the pins had more play than expected, resulting in less constrained motion and slightly higher perceived forces.

Additionally, the system was tested manually without a motor. In a final design, a motor would limit rotation to the required range, preventing over-rotation and improving control.

### 4.3 Key Similarities and Differences
The kinematic motion closely matched Phase 2 predictions, confirming the validity of the design. The main differences were due to manufacturing tolerances and material limitations, which introduced increased pin movement and friction.

Despite this, the stresses on the components are still expected to remain below yielding limits. Overall, the differences highlight real-world manufacturing effects rather than issues with the core design.

---

## 5. Failures, Mistakes, and Surprises

### 5.1 Failures Observed
Several components failed during assembly and testing. The T-rail guides for the airbrake flaps frequently broke, likely due to stress and friction during motion. Pins also broke often, either during insertion or operation, and sometimes became stuck in other components, requiring reprints. Additionally, the frame was missing a properly designed hole to secure the T-rails with screws, which caused instability and alignment issues.

### 5.2 Mistakes in Design or Fabrication
Most issues were caused by improper tolerances. Fits between pins and holes were either too tight, leading to breakage, or too loose, reducing stability. The design also did not fully account for the limitations of PLA, which is weaker than the aluminum assumed in Phase 2. Some features, like the T-rail guides and pin connections, were not strong enough for real-world use.

### 5.3 Unexpected Behaviors and Outcomes
Although the design worked well in simulation, tolerances had a much larger impact in physical testing than expected. Friction between 3D printed parts was higher than anticipated, especially in the sliding components, which affected smooth motion and contributed to failures. Overall, the prototype functioned correctly, but real-world performance highlighted the gap between ideal simulations and physical manufacturing.

---

## 6. Design Changes for Second Iteration

### 6.1 Geometry Improvements
Several geometry changes would be implemented to improve durability and functionality. The T-rail guides for the airbrake flaps would be reinforced to prevent repeated breakage. Pin interfaces would also be redesigned with improved tolerances to reduce both excessive tightness and looseness. Additionally, proper mounting holes would be added to the frame to securely attach the T-rails and improve overall alignment.

### 6.2 Materials and Manufacturing Improvements
The use of PLA would be replaced with a stronger material, such as PETG or ABS, to improve strength and durability. For a final design, Aluminum 6061 components would be used as originally intended. Low-friction materials such as PTFE would also be incorporated at sliding interfaces to reduce friction and improve motion smoothness.

### 6.3 Assembly Improvements
Assembly would be improved by redesigning pins to be stronger and more reliable, potentially incorporating bearings or bushings to reduce wear and friction. Dedicated screw holes would be added to ensure proper fastening of components. These changes would reduce the likelihood of parts breaking during assembly and improve overall system stability.

### 6.4 Performance Improvements
A servo motor would be integrated into the system to control spindle rotation more precisely. This would prevent over-rotation and ensure the flaps only deploy to the intended positions. Additionally, reducing friction in the guide rails and improving alignment would enhance the smoothness and consistency of motion.
