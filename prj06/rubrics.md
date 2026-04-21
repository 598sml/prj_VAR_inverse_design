## Statement of Problem (SP):

Problem: Inverse design of metamaterials using the btarget stress stress curve. This is a generative design problem where we use ML models such as diffusion and visual autoregressive models to generate the foundation materials for our specific application. Goals can be summarized to first generating designs from our input curve, and maybe more importantly, two, compare two state of the art models on generative design.

## Implementation Details (ID):

How diffusion model and VAR are trained (the notions of diffusing the noise through multiple steps vs next resolution token prediction) are the main details that should be briefly mentioned in the slides/presentation. Loss for the VQVAE model (first step) is the most important one which is not common in the literature among all other problems. The other two losses (MSE and Cross Entropy) might not be much new for the audience, so it won't be scrutinized during the presentation. Regarding the sufficient amount of information, it will be mentioned as the time allows to do so. It goes without saying that all details may not be possible to mention and will be referenced for audience that might be intereseted.

## Results: (R):

The most important results in this work is whether we can reach an acceptable l2 error after generating the metamaterials, using any of those two models. Also, comparing the two models, which is achieved.

## Reflections (C):

The main learning for me in this project was definitely the two main generative model classes and using autoregressive and diffusion models in the backward path of neural operators.
