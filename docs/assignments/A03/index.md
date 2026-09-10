# A3 – Parametric & FEA

## Part 1
The purpose of this assignment is to design a beam that meets our given criteria, having a tensioning load between 300 and 500 lbs, a displacement of 0.009 in, and an elastic modulus between 8.5*10^6 and 11.5*10^6. This also included it being modeled out of aluminum and having a round cross section. Considering this, I listed my choices of these givens and illustrated the bar as a cylindrical rod. Having all of this information, I could structure the tension elongation equation with the chosen givens, with the exception of the cross-sectional area. For this value, I decided to use a radius of 1, giving an area of 3.14. 

<img width="500" height="250" alt="Image" src="https://github.com/user-attachments/assets/cd041d4d-7c40-4465-bdfe-4eccbe6b0a75" />

Now that I had defined all of the variables in the equation besides the length, I could now plug the values into SolidWorks' variable page, and simultaneously have it solve for length in that same page. Doing this, we found the length to be 801.11 in, and so we now could sketch the full part out in the program parametrically. After creating a circle, smart dimensioning it to match our values, and extruding it to the proper length, we then applied a fixture to one end of the rod, to ensure that the further processes would be successful. Once we had done this, we could now apply the load to the rod as well on the opposite end. It was at this point that I had realized that "pure aluminum" that precisely matched our values was not present in the program, and so I used Aluminum Alloy 1060 instead. This had a slightly higher modulus than the one I had initially chosen, which meant that the length of the part would also be slightly longer than initially found. However, very little was changed over all to accommodate this, and after replacing the modulus we simply re-solved the length equation.

## Part 2
At this point, the part had been modeled, fixed, and load-bearing, so it was time to create a mesh in order to get an FEA deflection map & a von Mises stress map. Once we had done this, our maximum stress was found to be 102.3 psi, much less than aluminum 1060's yield strength of 3999 psi, providing us with a safety factor of 39.1. 

<img width="600" height="300" alt="Image" src="https://github.com/user-attachments/assets/ec45736e-8feb-483b-9869-3421e6fbd7eb" />

<img width="600" height="300" alt="Image" src="https://github.com/user-attachments/assets/9704bc20-520e-416e-89cf-ab9674bdfc4f" />

## Part 3
Now we were to compare the FEA and parametric axial deflections, which after computing are 0.00905 and 0.009, respectively. These are nearly the exact same, which makes sense considering they are using many of the same variables and values when being calculated. With them being so close, it could be chalked up to a rounding discrepancy. Now, if I were to choose between the two methods, I believe I would choose the FEA, simply for the fact that it is much more rigorous calculations used.

<img width="3867" height="2231" alt="Image" src="https://github.com/user-attachments/assets/904ab0d0-c1d3-4f6d-bfaa-eedd6dee37f8" />

## 2157 Bonus
For the 2157 only section, I decided to adjust some of the chosen values, setting F to 500 lbs, the radius to 4 and thus the area to 16pi, and substituting these into the direct tension elongation equation to find the new length. Since the material is kept the same, the modulus maintained, and the displacement had no apparent reason to be changed, either. Now, since, when solving for length, the cross-sectional area is in the numerator, I can safely predict that it will be much longer than our initial piece, since the value of the area is now 16 times that which it was before. The denominator, on the other hand, is the load, which increased from 300 to 500, not even doubling and thus being far outpaced by the 16 times multiplication happening above. This prediction turned out to be the case, giving us a length of 9047.8 in, much greater than our initial length value.
