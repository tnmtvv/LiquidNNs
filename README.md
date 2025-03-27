# LiquidNNs
 
This is the official repository for LiquidNNs project for Skoltech ML 2025 course. Team 3 members: Anuar Daurenov, Dmitry Gribanov, Tatyana Matveeva, Maksim Makarov, Tatiana Kobernik

This repository allows you to train Liquid Neural Networks on different datasets:
- Gestures
- Occupancy
- Traffic volume prediction
- Ozone level forecasting
- Power consumption
## Requisites

All models were implemented and tested in Google Colab.
All the following steps assume that they are executed under these conditions. You can also use `requirements.txt`

```bash
pip install -r requirements.txt
```

## Datasets
All datasets are available in the ```notebooks/data``` folder.

## Training and evaluating the models 
All notebooks are located in the ```notebooks``` folder.

Each notebook trains the specified model for the given number of epochs and evaluates the validation performance after every ``log`` steps.
All results are stored in the ```notebooks/new_repo_reproduction``` and ```notebooks/old_repo_reproduction``` folder by appending the result to CSV and pdf files.

## Reproducibility
All notebooks of the ```notebooks/new_repo_reproduction``` were created in the colab environment to be standalone. In order to reproduce the results you shall run all cells in Colab. 

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
