# The Limits and Potentials of Deep Learning for Robotics
## Niko Sunderhauf, Oliver Brock, Walter Scheirer, Raia Hadsell, Dieter Fox, Jurgen Leitner, Ben Upcroft, Pieter Abbeel, Wolfram Burgard, Michael Milford, Peter Corke
* Review paper for challenges in robotics from RSS workshop 
* Robotic Vision:
  - vs Computer vision - robotic vision results in actions, not just information.
  - Learning Challenges:
    1. Uncertainty estimation
    2. Identifying unknowns - closed (all data/classes represented in training) vs open set (new data seen at test). 
    3. lifelong/incremental learning 
    4. class incremental learning
    5. (II.A.5) **active learning (unsupervised incremental learning)** [21,24,29]
  - Embodiment challenges
    1. temporal (use video data as video, not Frames). CORe50 Dataset (rotating household objects)
    2. spatial (use different viewpoints, deal with occlusions)
    3. **active vision/sensing** [5,14,25,73,130]
  - Reasoning challenges
    1. object/scene semantics (contect, expect fork in kitchen not bathroom
    2. object/scene geometry (depth, 3d structure)
    3. reasoning about semantics/geometry together
* Benchmarking 
  - robotics is an "open set" problem - lots of novelty at deployment time.
    * problem often lies not with feature recognition but "readout" layer of NN, in establishing decision boundaries for an unknown number of classes 
  - *Visual Psychophysics* - psychophysics is probing of inner mechanisms of visual processing. 
    * should develop perturbed images in order to classify accuracy of model very finely.
* Pixel - to - action (end to end)
  - reality gap/domain transfer is a problem, can use progressive nets maybe? domain randomization? 
* DL for Physics-absed models
  - sys-ID is pretty brittle for normal things
  - humans use "intuitive" instead of exact models
  - DL models are data-inefficient, can have larger basins of convergence 
* Some rambling about whether we should "program" things or "fit things" with data 
* Are all programs decomposable? maybbe - suboptimal decompositions yield suboptimal results. Maybe we should just automate all of computer science 
* Data Efficiency - needed eventually
  
  
## Future investigation:
* What is "epistemic uncertainty" in the context of adversarial examples?
* [70] Confusion loss to ignore data variation in different domains, [121, 122, 123] for "aligning data" for reality gap
* [96] - progressive nets *transfer learning* compositionality of networks 
