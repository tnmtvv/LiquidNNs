# LiquidNNs
 
This is the official repository for LiquidNNs project for Skoltech ML 2025 course. Team 3 members: Anuar Daurenov, Dmitry Gribanov, Tatyana Matveeva, Maksim Makarov, Tatiana Kobernik

This repository allows you to train Liquid Neural Networks on different datasets:
- Gestures
- Occupancy
- Traffic volume prediction
- Ozone level forecasting
- Power consumption

## Datasets
All datasets are available in the ```notebooks/data``` folder. 


## Training and evaluating the models 

For reproducing the experiments from the original articles, please use the ```notebooks/old_repo_reproduction``` folder where correspoding file for conda environment is located.

```
conda env create -f environment.yml
```

All notebooks are located in the ```notebooks```
For training Neural Circuit Policies, you can go to ```notebooks/new_repo_reproduction```

Each notebook trains the specified model for the given number of epochs and evaluates the validation performance after every 50 epochs creating corresponding ```log``` file.
All results are stored in the ```notebooks/new_repo_reproduction``` ```notebooks/old_repo_reproduction``` as csv files.

The corresponding plots can be found in the ```results```

## Results overview

Here are the validation metrics vs epochs with new implementation's LTC and CfC models applied on the old datasets with the same preprocessing.


<p align="center">
    <img src="notebooks\new_repo_reproduction\gesture\Gesture_accuracy.jpg" width="300">
    <img src="notebooks\new_repo_reproduction\ozone\Ozone_f1.jpg" width="300">
    <br>
    <img src="notebooks\new_repo_reproduction\power\Power_MSE_log.jpg" width="300">
    <img src="notebooks\new_repo_reproduction\traffic\Traffic_MSE.jpg" width="300">
</p>


## Reproducibility

Original article experiments can be reproduced locally. Experiments for Gesture, Occupancy, and Ozone were executed in Google Colab, while Traffic and Power were run on an A40 remote server.

## Papers
| Models | References |
| ----- | ----- |
| Liquid time-constant Networks | https://arxiv.org/abs/2006.04439 |
| Neural ODEs | https://papers.nips.cc/paper/7892-neural-ordinary-differential-equations.pdf |
| Continuous-time RNNs | https://www.sciencedirect.com/science/article/abs/pii/S089360800580125X |
Continuous-time Gated Recurrent Units (GRU) | https://arxiv.org/abs/1710.04110 |
| Closed forms Continious time models | https://arxiv.org/abs/2106.13898 |
| Neural Circuit Policies | https://www.nature.com/articles/s42256-020-00237-3?error=cookies_not_supported&code=495468f3-76f3-414b-bf0f-ba9f0d6b20f1
## References

Github repository for ncps library: https://github.com/mlech26l/ncps

Github repository for LTC project: https://github.com/raminmh/liquid_time_constant_networks
