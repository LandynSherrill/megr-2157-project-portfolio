# A6 – Bracket Drawing (Drawings 1)

## Objective
The goal of this assignment is to generate a comprehensive solid model and multi-view engineering drawing that accurately represents the designed bracket, incorporating all of the features to ensure that both the strength and stiffness requirements are met.

## Initial work
First and foremost, we have to turn to the data gathered from A5, particularly the dimensioning of the bracket sections under both the stress and stiffness analyses. Observing these values, we can note that for every dimensional value, the stress analysis returned a larger number. Considering this, this would mean that the governing value for all dimensions will be the stress values. Now that we know this, we can safely adopt the stress values for our part's dimensions.
Having decided on the dimensions, we can now input these into our CAD software and create a model of the bracket.

<img width="800" height="600" alt="IMG_1117" src="https://github.com/user-attachments/assets/867da5ea-cf41-4b9e-8685-e19aa1b247bf" />

With our newly 3d modeled bracket, we can now create a drawing of the same bracket, using many of the same dimension lines used in the model. This is also done in the standard 3rd-angle projection, and we make sure that the gap tolerances are observed and match our fit tolerances. 

[A6 Part Drawing.pdf](https://github.com/user-attachments/files/32911813/A6.Part.Drawing.pdf)

[A6 Part edraw.html](https://github.com/user-attachments/files/32911885/A6.Part.edraw.html)

## Lessons learned
On the top of the bracket, the dimensioning was by far the strictest at 0.5 thousandths, while the underside of it, section C, had the loosest constraints, at 2 thousandths. The top is meant to be where the bracket slides onto and stays on the rails, while section C hangs beneath, being necessary for weight and such but not vital in the same way. This gives good reason for the top-side to be far more strict with it's measurements, while the underside doesn't need as much. If we were to universally apply that strictest dimensioning constraint as used on the top, this would force the tooling for the part to be far, far more precise in all aspects so as to achieve the "necessary" dimensioning. Naturally, this skyrockets the cost, and, especially for non-critical parts, does so needlessly, since they could have completed the same tasks with no further risk at far less precise levels of tooling. 

## Linkage Work
Now, what we did for the main bracket we shall do for the linkage we also designed in A5. Since we have recorded the major values of this as well, we can be just as, if not quicker, making this than the bracket. We, when completing the last assignment, were only able to determine the total cross sectional area, and left exact dimensions alone, however at this point I decided to make it a square cross sectional area, which got us to our particular depth of the link, and was very important in determining the final width as well. 

[A6 Link Drawing.pdf](https://github.com/user-attachments/files/32911799/A6.Link.Drawing.pdf)

[A6 Link edraw.html](https://github.com/user-attachments/files/32911848/A6.Link.edraw.html)

When dealing with the holes in the link, it is important to remember that each is meant to have a certain fit, and therefore a certain tolerance for the holes. For the hole meant for the bracket's section A, we had an AC6, whose holes have a tolerance of 0.002", while the hole for the new weight had a FN1 fit, whose tolerance sits at half a thousandth of an inch. These are both, therefore, accounted in the drawing according to their designation, as well as their matching tolerance being listed.

