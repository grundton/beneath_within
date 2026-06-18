[![DOI](https://zenodo.org/badge/1258335814.svg)](https://doi.org/10.5281/zenodo.20745386)
# beneath_within

This repository contains the Pure Data patch for the piece "Beneath, Within", which was premiered in KUL in 2025.

## Idea
Two ML models are trained on tenor saxophone and gong recordings. In a performance two performers play these, and audio signals from both instruments are used as input for two nn_tilde objects in Pure Data. The models can feedback into themselves, into each other and can merge their latent space signals based on MIDI CC messages from a third performer.

## File structure
It uses the 4 Pure Data subprocesses, which can be found in the folder "sub".
It also uses 2 models to be used within the RAVE/nn_tilde framework in Pure Data, which are expected to be in the folder "m".
The models are:
- Beneath_Within_AlexTenorEtu_v0_best1M_fid_0.999_streaming.ts (4 latent dimensions)
- Beneath_Within_CedrikGong_v0_bes500k_fid_0.999_streaming_z8.ts (8 latent dimensions)

They can be downloaded from [https://doi.org/10.5281/zenodo.20744762](https://doi.org/10.5281/zenodo.20744762).

## Interface
The patch is expected to be operated with a KORG nanoKONTROL2 and contains mappings for this controller.
