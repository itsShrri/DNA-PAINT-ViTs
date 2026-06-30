This repository contains the PyTorch implementation of a machine learning pipeline designed to classify molecular binding events in Single-Molecule Localization Microscopy (SMLM). It chronicles the transition from analyzing static peak-intensity frames to deploying a spatiotemporal model that verifies physical hybridization kinetics.

# The DNA-PAINT Dataset
DNA-PAINT is a super-resolution microscopy technique that relies on the transient binding and unbinding ("blinking") of fluorescent DNA strands. The dataset consists of highly noisy, diffraction-limited optical data. The primary challenge is distinguishing true molecular binding events from transient background noise and irregular optical artifacts that temporarily mimic target molecules.

# Peak Frame Classification (ViT & CvT)
My initial approach treated classification as a static image recognition task.
- Extracted only the peak brightness frame from each detected event.
- Applied a standard Vision Transformer (ViT) and a Convolutional Vision Transformer (CvT) to classify the local spatial geometry (e.g., spot symmetry and edge gradients).

# Event-Level Decision (Temporal-ViT & Temporal-CvT)

# Comparison with State-Of-The-Art (Yin et al.)
