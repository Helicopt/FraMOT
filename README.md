# FraMOT
Frame Rate Agnostic Multi-Object Tracking

This project aims to perform Multi-Object Tracking on multiple frame rate inputs, unknown frame rate inputs and dynamic frame rate inputs, leading to a smarter tracking solution called Frame Rate Agnositic Multi-Object Tracking.

Our paper: ![paper](https://arxiv.org/abs/2209.11404)

This repo is still under development and refactorization.


# Inference

## Download trained checkpoint

MOT20 checkpoint: ![MOT20 checkpoint](https://drive.google.com/file/d/1LA6tA78Cakh99j5CFkcgs9S8qdEX_nzC/view?usp=sharing)

put the checkpoint as checkpoints/assoc\_re2/ckpt\_latest.pth

## Data preparation

Comming Soon!

## Run

Taking inference on MOT20 as an example:

```sh
cd EOD
python -u -m eod train --config configs/tracking/base_x_m20_mhvfl_assoc_base_afr_p3.yaml --nm 1 --ng 4 --launch pytorch -e
```
--ng is to set how many GPU could be used, modify as the number of your devices.

# Training

Coming Soon!



# FraMOT dataset and evaluation

The multi-frame-rate dataset generation and evaluation code can be found at https://github.com/Helicopt/FraMOT-eval.


# Acknowledgement

A large part of the code base is borrowed from an older version of project ModelTC/United-Perception (previously called EOD). Thanks for the hardwork of contributors in the UP project!
