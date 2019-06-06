## Results

Before tuning:

|     Tracker Name      | Accuracy | Robustness | Lost Number |  EAO  |
| :-------------------: | :------: | :--------: | :---------: | :---: |
| Custom_checkpoint_e11 |  0.585   |   0.370    |    79.0     | 0.314 |
| Custom_checkpoint_e12 |  0.585   |   0.393    |    84.0     | 0.310 |
| Custom_checkpoint_e7  |  0.566   |   0.398    |    85.0     | 0.310 |
| Custom_checkpoint_e13 |  0.582   |   0.384    |    82.0     | 0.307 |
| Custom_checkpoint_e9  |  0.573   |   0.337    |    72.0     | 0.304 |
| Custom_checkpoint_e10 |  0.571   |   0.365    |    78.0     | 0.300 |
| Custom_checkpoint_e8  |  0.564   |   0.342    |    73.0     | 0.299 |
| Custom_checkpoint_e20 |  0.567   |   0.431    |    92.0     | 0.291 |
| Custom_checkpoint_e5  |  0.521   |   0.403    |    86.0     | 0.281 |
| Custom_checkpoint_e17 |  0.559   |   0.407    |    87.0     | 0.281 |
| Custom_checkpoint_e15 |  0.567   |   0.421    |    90.0     | 0.281 |
| Custom_checkpoint_e16 |  0.584   |   0.421    |    90.0     | 0.279 |
| Custom_checkpoint_e14 |  0.573   |   0.421    |    90.0     | 0.273 |
| Custom_checkpoint_e19 |  0.561   |   0.445    |    95.0     | 0.271 |
| Custom_checkpoint_e6  |  0.562   |   0.454    |    97.0     | 0.268 |
| Custom_checkpoint_e18 |  0.552   |   0.445    |    95.0     | 0.267 |
| Custom_checkpoint_e4  |  0.515   |   0.445    |    95.0     | 0.261 |
| Custom_checkpoint_e3  |  0.477   |   0.478    |    102.0    | 0.225 |
| Custom_checkpoint_e2  |  0.442   |   0.459    |    98.0     | 0.211 |
| Custom_checkpoint_e1  |  0.396   |   0.567    |    121.0    | 0.172 |


After tuning:

|                                Tracker Name                                | Accuracy | Robustness | Lost Number |  EAO  |
| :------------------------------------------------------------------------: | :------: | :--------: | :---------: | :---: |
| Custom_checkpoint_e11_r255_penalty_k_0_000_window_influence_0_480_lr_0_300 |  0.586   |   0.318    |    68.0     | 0.351 |
| Custom_checkpoint_e11_r255_penalty_k_0_020_window_influence_0_500_lr_0_500 |  0.586   |   0.314    |    67.0     | 0.349 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_500_lr_0_350 |  0.586   |   0.332    |    71.0     | 0.347 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_460_lr_0_350 |  0.586   |   0.290    |    62.0     | 0.347 |
| Custom_checkpoint_e11_r255_penalty_k_0_080_window_influence_0_440_lr_0_450 |  0.587   |   0.309    |    66.0     | 0.347 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_480_lr_0_250 |  0.590   |   0.332    |    71.0     | 0.346 |
| Custom_checkpoint_e11_r255_penalty_k_0_160_window_influence_0_440_lr_0_300 |  0.583   |   0.309    |    66.0     | 0.345 |
| Custom_checkpoint_e11_r255_penalty_k_0_020_window_influence_0_480_lr_0_450 |  0.588   |   0.314    |    67.0     | 0.344 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_480_lr_0_450 |  0.587   |   0.300    |    64.0     | 0.344 |
| Custom_checkpoint_e11_r255_penalty_k_0_040_window_influence_0_500_lr_0_350 |  0.590   |   0.323    |    69.0     | 0.344 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_460_lr_0_250 |  0.586   |   0.342    |    73.0     | 0.342 |
| Custom_checkpoint_e11_r255_penalty_k_0_040_window_influence_0_480_lr_0_250 |  0.585   |   0.300    |    64.0     | 0.342 |
| Custom_checkpoint_e11_r255_penalty_k_0_100_window_influence_0_480_lr_0_300 |  0.584   |   0.295    |    63.0     | 0.341 |
| Custom_checkpoint_e11_r255_penalty_k_0_020_window_influence_0_500_lr_0_350 |  0.588   |   0.318    |    68.0     | 0.341 |
| Custom_checkpoint_e11_r255_penalty_k_0_000_window_influence_0_440_lr_0_300 |  0.581   |   0.295    |    63.0     | 0.341 |
| Custom_checkpoint_e11_r255_penalty_k_0_060_window_influence_0_440_lr_0_500 |  0.586   |   0.328    |    70.0     | 0.341 |
| Custom_checkpoint_e11_r255_penalty_k_0_200_window_influence_0_400_lr_0_550 |  0.587   |   0.332    |    71.0     | 0.341 |
| Custom_checkpoint_e11_r255_penalty_k_0_180_window_influence_0_460_lr_0_550 |  0.589   |   0.318    |    68.0     | 0.340 |
| Custom_checkpoint_e11_r255_penalty_k_0_020_window_influence_0_460_lr_0_500 |  0.582   |   0.318    |    68.0     | 0.340 |
| Custom_checkpoint_e11_r255_penalty_k_0_040_window_influence_0_460_lr_0_350 |  0.588   |   0.332    |    71.0     | 0.340 |


## Errors
--- 
```bash
THCudaCheck FAIL file=/pytorch/aten/src/THC/THCGeneral.cpp line=663 error=11 : invalid argument
```
Possible reason: Version mismatch between CUDA and PyTorch. I am using RTX2080 seris GPU and my system cuda version is 10.0. However, PyTorch 0.4.1 is compiled with CUDA9 and I installed PyTorch by running `conda install pytorch=0.4.1 cuda92 -c pytorch`.
Solution: 
* Remove `torch.backends.cudnn.benchmark = True` in the tool scripts.
* Downgrade system CUDA to 9.2

---
```bash
ValueError: could not convert string to float: 'Occ'
```
Possible reason: some processes exited unexpectedly when running `tune.sh`.

Solution:
```bash
find ./result/VOT2018/ -type f -exec awk -v x=10 'NR==x{exit 1}' {} \; -exec echo rm -f {} \; | sh
```
