# Machine Learning-Simulated Lamb Waves and PINN/CNN to Predict Young Modulus 


**Simulated Lamb-Wave Young’s Modulus Identification Using CNNs and PINNs**

## Group Info

- Mashal Shami
  - Email: [mmshami@email.sc.edu](mailto:YOUR_EMAIL@email.sc.ed)
- Jannatul Ferdausi
  - Email: [FERDAUSI@email.sc.edu](mailto:JANATUL_EMAIL@email.sc.edu)

## Project Summary/Abstract

This project uses simulated Lamb-wave signals to predict Young’s modulus, which measures how stiff a material is. We generate pristine plate wave data in MATLAB at different Young’s modulus values, then use machine-learning models to predict the modulus of an unknown signal. We will compare a regular Convolutional Neural Network (CNN) with a Physics-Informed Neural Network (PINN). The project will show whether adding physics constraints improves material-property prediction.

## Problem Description

- **Problem description:** Engineers need ways to estimate material properties without breaking or cutting the material. Our goal is to predict Young’s modulus from simulated Lamb-wave signals measured from a pristine 1 mm plate.

- **Motivation**
  - Lamb waves can be used for non-destructive material testing.
  - Young’s modulus is an important property for understanding material stiffness.
  - Comparing a CNN and PINN helps us study whether physics improves machine-learning predictions.

- **Challenges**
  - Waveform signals are noisy and can look similar for different modulus values.
  - The PINN must balance data loss with PDE and boundary-condition losses.
  - Models may predict poorly for values near the edges of the training range.

## Contribution

### [`Replication of existing work`], [`Extension of existing work`]

We use the ideas from Mehtaj and Banerjee [2] to explore physics-informed machine learning for guided-wave propagation. We also use the general PINN method described by Raissi et al. [1].

Our project extends this work by:

- Creating a MATLAB-generated dataset of pristine Lamb-wave signals with different Young’s modulus values.
- Comparing a data-driven CNN baseline with a PINN on the same modulus-prediction problem.
- Testing both models on held-out unknown modulus values and reporting prediction error, CNN RMSE, and PINN PDE loss.

## References

See [`references.bib`](references.bib) for BibTeX entries.
