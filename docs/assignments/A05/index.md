# A5 – Bracket Design & Fits

## Objectives
* Conduct stress analysis to determine appropriate dimensions for structural features.
* Generate free body diagrams (FBDs) to visualize forces and constraints for each feature.
* Identify and document known and unknown variables, assumptions, and algebraic models for stress calculations.
* Perform stiffness analysis to establish minimum required dimensions based on deflection constraints.
* Compare stress and stiffness analyses to ensure structural integrity and compliance with given constraints.
* Create detailed multiview sketches illustrating dimensions derived from both stress and stiffness analyses.
* Reflect on and document key engineering lessons learned throughout the process.

## Description
Detail design a bracket, using the concept design in Appendix B, to hold a horizontal force applied symmetrically by a strap outline in resource #1. The bracket’s dimensions are designed with different fit classes. Each dimension of the T beam is part of the fit:
* “a” intention for use where accuracy is not essential
* “b” is about the closest fits that can be expected to run freely
* “c” is where accurate location and minimum play is desired
Design using a safety factor of 4 and applied load in between 500 lbf < F < 800 lbf. Choose one of three metals, aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4). Furthermore, state assumptions and approximations about the design in order to use fundamental strength of materials analysis. For example, use the proper stress analysis and deflection analysis where appropriate. Assume no failure due to direct shear stress.
<img width="323" height="238" alt="image" src="https://github.com/user-attachments/assets/19dc4a2b-4123-4f32-96d6-7b1cb47ad817" />

___________________________________________________________

# Initial Work
The first thing that I did, after reading the introductory information and viewing the images, was draw out what the T-beam and mark the tolerances on each section, as given in the descriptive image above. I also made note of the given values, namely the safety factor of 4, the strap that would be used having a width of 3/4", and the load being a value between 500 and 800 lbs. Then, I made a rough draft of what the final bracket would look like with a front, right, and top view. At this point, I had already decided to use a symmetrical design, to minimize the workload. After this, I marked on my rough draft what the different sections were, as our appendices had shown. 

Now, having designated the sections, I began drawing the FBD's of each according to the given recommendations, treating section A as a uniformly loaded cantilever beam, B as an axially loaded bar, and C as a simply supported beam with a concentrated center load. Having come this far, I began speculating on what sections D and E could be modeled as. Eventually, I drew them out and saw that D could be modeled as an axially loaded bar, like B, while E could be modeled as a uniformly loaded cantilever beam, like A. Now, having laid out what I would be dealing with, I finally decided on the load value and the material type. Of the three material types, the steel had the best elasticity and had the intermediate tensile strength among the three, which I figured would be a useful combination of properties for the intended purpose. For the load, I decided on 600 lbs. as an even middle-ground value.

<img width="500" height="250" alt="IMG_1094" src="https://github.com/user-attachments/assets/99bc733f-cc86-4ce0-9d92-b8fdb7bc1dd3" />

<img width="500" height="250" alt="IMG_1095" src="https://github.com/user-attachments/assets/aaa1cd0c-0101-454e-bea9-005d37c8eaed" />

# Stress Analysis
Now that all of the initial and material property values had been established, I was able to begin the stress analysis. For each of the sections, I have depicted a rough isometric view and FBD denoting the major dimensions and any acting forces. For the entire stress analysis, we will assume that there will be NO FAILURES due to shear stress.

## Section A
Section A was, as we were given, meant to be treated as a cantilever beam with a uniform load, and so we treated it as such. The load acting on A is double our chosen force value, since the strap is being pulled on both sides with our chosen force value, 600 lbs.
Knowns:
* F = 600 lbf
* W = 2F = 1200 lbf
* S = 58,000 psi
* SF = 4
* Section Modulus (Z)

Unknowns:
* Length (L)
* Radius (r)

Assumptions:
* The feature resembles a uniformly loaded cantilever beam, which we will use for analysis
* The shape of the section is cylindrical, and will hold the strap w/o slippage
* The section's length must be greater than the strap's width (3/4"), so assume L = 1"
* Neglect torque

With these knowns and having made choice assumptions, we may now solve for r, the only remaining unknown value
<img width="600" height="300" alt="IMG_1080" src="https://github.com/user-attachments/assets/e5435a53-1e32-4fd2-b518-3252f271aa6a" />

Section A Dimensions: r = 0.375", L = 1"

## Section B
Section B was possibly the easiest section, with the form already being given to us and not having to appeal to beam stress equations, since it was a direct tension equation. We do, however have to assume a height value, as there is no possibility of deducing it from our known information.
Knowns:
* W = 1200 lbf
* S = 58,000 psi
* SF = 4

Unknowns:
* Length (L)
* Width (d)
* Height (h)
* Area (A)

Assumptions:
* The feature resembles an axially tensioned rod, which we will use for analysis
* The length of the part = The diameter of section A
* The height of the section must be greater than the diameter of A, with clearance for fitting the strap; assume h = 1"
* Neglect torque

Given these knowns and assumptions, we may now solve for the width of the section, d.
<img width="600" height="300" alt="IMG_1081" src="https://github.com/user-attachments/assets/0ad62e13-9e8a-4671-89b2-37656f873696" />

Section B Dimensions: h = 1", d = 0.1104", L = 0.750"

## Section C
Section C is easily the biggest part available, having to fit to the underside of the T beam.

Knowns:
* W = 1200 lbf
* SF = 4
* S = 58,000 psi
* F = 600 lbf
* Section Modulus (Z)

Unknowns:
* Length (L)
* Width (d)
* Height (h)

Assumptions:
* The feature resembles a beam supported on both sides with a center load, which we will use for analysis
* The width of the part (d) = The length of section A; d = 1"
* The length of the part (L) = The T-beam's length; L = 2.496"
* Neglect Torque

Given these knowns and assumptions, we can now solve for the height of the section, h.
<img width="600" height="300" alt="IMG_1082" src="https://github.com/user-attachments/assets/a13b895b-e679-4817-9f5e-182a2ab6009d" />

Section C Dimensions: L = 2.496", d = 1", h = 0.5566"

## Section D
Section D is very similar, though seemingly larger or at least thicker than section B. It is also the first section where the load is actually our chosen load value, 600 lbf, since that is split across both sides as shown in the section C FBD.

Knowns:
* F = 600 lbf
* S = 58,000 psi
* SF = 4

Unknowns:
* Length (L)
* Width (d)
* Height (h)
* Area (A)

Assumptions:
* The feature resembles an axially tensioned rod, which we will use for analysis
* The height of the section (h) = The T-beam's "c" side; h = 1.499"
* The width of the section (d) = The width of section C; d = 1"
* A = L*d
* Neglect torque

With this, we may now calculate the length of the section.

<img width="600" height="300" alt="IMG_1083" src="https://github.com/user-attachments/assets/a11889df-d538-4b71-8a4e-45de383cf44e" />

Section D Dimensions: L = 0.0414", d = 1", h = 1.499"

## Section E
Section E was possibly the most confusing sections to model at first, but very straightforward once I had realized it's essentially just an upside-down version of a uniformly loaded cantilever beam.

Knowns:
* F = 600 lbf
* S = 58,000 psi
* SF = 4
* Section Modulus (Z)

Unknowns:
* Length (L)
* Width (d)
* Height (h)

Assumptions:
* The feature resembles a uniformly loaded cantilever beam, which we will use for analysis
* The width of the section (d) = The width of section D; d = 1"
* The length of the section (L) = The length of the T-beam top; L = 0.9992"
* Neglect torque

We can now, with these values and assumptions, find the height of the section.
<img width="600" height="300" alt="IMG_1084" src="https://github.com/user-attachments/assets/f16ea88b-fdb4-4776-92cd-549748c420c9" />

Section E Dimensions: L = 0.9992", d = 1", h = 0.3522"

# Stiffness Analysis
Most of the models outlined in the stress analysis can be ported over to our stiffness analysis, however we will be using the elastic modulus of our material instead of the tensile strength. We will, across the analysis, operate under the assumption that the shear deflection is negligible, that there will be no failures due to shear, and that the maximum deflection in each section is 0.005".

## Section A
Knowns:
* F = 600 lbf 
* W = 1200 lbf
* E = 2.9*10^7 psi
* SF = 4
* e_max = 0.005"
* Moment of Inertia

Unknowns:
* Length (L)
* Width (d)

Assumptions:
* The feature resembles a uniformly loaded cantilever beam, which we will use for analysis
* The shape of the section is cylindrical, and will hold the strap w/o slippage
* The section's length must be greater than the strap's width (3/4"), so assume L = 1"

<img width="600" height="300" alt="IMG_1085" src="https://github.com/user-attachments/assets/0e050b8c-ac8a-41a8-84cc-9fc3a9e1d9b6" />

Section A Dimensions: L = 1", dia = 0.5388"

## Section B
For this section, I had a slight hang-up surrounding the height of the section. I had confused myself and began treating section B as if though it only  met with section A halfway, so I had initially set the height to 0.5", though upon closer inspection and thought I realized that this was not the case and set it to a more properly useful 0.8" height.

Knowns:
* F = 600 lbf
* W = 1200 lbf
* E = 2.9*10^7 psi
* SF = 4
* e_max = 0.005"

Unknowns:
* Length (L)
* Width (d)
* Height (h)
* Area (A)

Assumptions:
* The feature resembles an axially tensioned rod, which we will use for analysis
* The length of the section (L) = The diameter of section A; L = 0.5388"
* The height of the section must be greater than the diameter of A, with clearance for fitting the strap; assume h = 0.8"
* A = L*d

Now we can calculate the width of the section.

<img width="600" height="300" alt="IMG_1088" src="https://github.com/user-attachments/assets/b139eb8d-732d-4024-9a92-0ee9f252b64e" />

Section B Dimensions: L = 0.5388", h = 0.8", d = 0.0492"

## Section C
Knowns:
* F = 600 lbf
* W = 1200 lbf
* E = 2.9*10^7 psi
* SF = 4
* Moment of Inertia (I)
* e_max = 0.005"

Unknowns:
* Length (L)
* Width (d)
* Height (h)

Assumptions:
* The feature resembles a beam supported on both sides with a center load , which we will use for analysis
* The width of the section (d) = The length of section A; d = 1"
* The length of the section (L) = The T-beam's length; L = 2.496"

Now we may calculate the height of the section.

<img width="600" height="300" alt="IMG_1089" src="https://github.com/user-attachments/assets/c5d03299-411d-4cf7-b5f1-b0e44c38f7a5" />

Section C Dimensions: L = 2.496", d = 1", h = 0.1288"

## Section D
Knowns:
* F = 600 lbf
* E = 2.9*10^7 psi
* SF = 4
* e_max = 0.005"

Unknowns:
* Length (L)
* Width (d)
* Height (h)
* Area (A)

Assumptions:
* The feature resembles an axially tensioned rod, which we will use for analysis
* The width of the section (d) = The length of section A; d = 1"
* The height of the section (h) = The T-beam's length; h = 1.499"
* A = L*d

Now the length of the section can be calculated.

<img width="600" height="300" alt="IMG_1090" src="https://github.com/user-attachments/assets/a9961bb2-0626-4e70-868b-51677efd4085" />

Section D Dimensions: L = 0.0248", h = 1.499", d = 1"

## Section E
Knowns:
* F = 600 lbf
* E = 2.9*10^7 psi
* SF = 4
* Moment of Inertia (I)
* e_max = 0.005"

Unknowns:
* Length (L)
* Width (d)
* Height (h)

Assumptions:
* The feature resembles a uniformly loaded cantilever beam , which we will use for analysis
* The width of the section (d) = The length of section A; d = 1"
* The length of the section (L) = The T-beam's length; L = 0.9992"

Now we may find the value for the section's height.

<img width="600" height="300" alt="IMG_1091" src="https://github.com/user-attachments/assets/4e5ce0f1-eae9-4626-be18-a94125885617" />

Section E dimensions: L = 0.9992", d = 1", h = 0.2915"

## Multiview Sketches
Before we could draw the Multiview sketches, I decided to compile the dimensions for each section within both analyses, which I did on this table. 

<img width="500" height="225" alt="IMG_1096" src="https://github.com/user-attachments/assets/6cc27437-22a8-42fe-bbc4-4f61e8e166c3" />

Then, I drew each of the sketches. They are not drawn entirely to scale, but the feature differences are, I think, quite readily apparent regardless.

<img width="350" height="350" alt="IMG_1097" src="https://github.com/user-attachments/assets/5bba99a6-7d81-4a40-9511-19e999f49285" />

<img width="500" height="350" alt="IMG_1098" src="https://github.com/user-attachments/assets/6b164c89-56f0-44e6-a115-6cf9e19ffcd3" />

# Lessons Learned
## Governing Failure mode
Looking at the features, the most prominent is the cylindrical mount attached to the bracket. When we look at it, we can see that the governing force was the stress, since it ended up having a diameter of 0.75" in that model as compared to the far lesser 0.5388" diameter of the stiffness model. This difference is quite significant, the stress causing the feature to be nearly a time and a half larger, ~0.2112".
## Error Propogation
For section B, the diameter of section A is used to determine the length (according to my drawing system) of the section. Fortunately, I had no issues with the transferring, having no early errors or late catches that needed to be made to keep the values accurate. The thing that could have caught any issues with this would be thoroughly checking over the equation used to determine A's diameter, which if done wrong would throw off the section B value when ported over.
## Assumption sensitivity
In completing this assignment, I had to make an assumption about the material used, with me having chosen steel while tungsten and aluminum were available. If I were to have chosen steel while either one of these other materials had been used, nearly all of the work done would be rendered inaccurate. Since nearly all of the math relied on the tensile strength or elastic modulus, both of which are material properties, if we changed the material, the elastic modulus would decrease since the steel had the highest value, and the tensile strength would either increase or decrease. 


# Fits
Design a link (Appendix E) that connects feature A to another cylindrical feature, such that the connection can hold using the same amount of force. The link is to be made from one of the three specified metals.
* The hole in the link that connects to feature A must be designed as a running/sliding fit.
* The hole in the link that connects to the 1-inch diameter shaft must be designed with light assembly pressure.
Tasks:
Design the dimensions of the link.
* Use stress/strength equations to determine the required cross-sectional area of the linkage, focusing on the smallest cross-sectional area at the holes.
* Apply the axial deflection equation to verify both the cross-sectional area and the length of the linkage, again considering the smallest cross-sectional area at the holes.
Select the proper fit for feature A.
* Discuss the design process used, and cite resources (include page numbers) in your documentation.
* Select the proper manufacturing technique. Show the process included tables used.
Select the proper fit for the 1-inch shaft.
* Discuss the process used, and cite resources (include page numbers) in your documentation.
* Select the proper manufacturing technique. Show the process included tables used.

## Work
We have already been informed of the fit needed for the link's A portion, a running/sliding fit, as well as having been given a hint for the fit of the 1-inch diameter portion of the link, which I shall call Z. If we turn to Machinery's handbook, on p. 652, we can see the same wording used to describe the Z fit being used to also describe an FN1 light drive fit. We will also be operating with the assumption of A's diameter being 0.75", as determined in the stress analysis. 
After having deduced this, we find that the cross-sectional area centered at Z will be the smallest, so we will work there. We know that the load is the same on A as before, meaning 1200 lbf, and we will continue to use the steel as the chosen material.
We then find the area is 0.0828 in^2 and are thus able to use it in the axial deflection equation to determine the length between the two centers of the holes. This ends up being 2.5".

## A's Proper Fit
As stated before, we have been given the fit type for A, the running/sliding fit. Since this will not be in a machine and instead hang static, extreme dimensional precision is largely unnecessary. As a result, I have opted to use the AC6 fit, which greatly reduces the costs and technique needed to make while not sacrificing the fit and still being capable of handling strong pressures, as stated on p. 651. If we then turn to p. 655, in Table 8b, we can find the AC6 values that match our 0.75" diameter, which gives us an H9 hole and an e8 shaft. These two grades can both be operated on with boring, as shown on p. 650 in Table 7. This gives us a far more reasonable price point than the other processes do without compromising our precision.

## Z's Proper Fit
Now, we look at Z. We have already established that Z uses an FN1 fit, and have been given that Z's diameter is 1". Turning to p. 659 and Table 11, we can find the appropriate grades of an H6 hole and a (speculative) grade 7 shaft. I say speculative because, for some reason, the values we've gotten do not explicitly list the shaft grade. However, if we return back to p. 650, we can find the tolerance values on the grade 7 column, so we will assume this is accurate. With this being the case, we can utilize reaming, according to p. 650's Table 7, which is a higher cost than the boring used on A, but it necessary for the greater precision of the fit.

<img width="500" height="200" alt="IMG_1093" src="https://github.com/user-attachments/assets/3084b49c-3673-4da5-9797-f7e9b534a574" />

The time spent on this project totalled to roughly 16 hours.
