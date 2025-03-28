# legged-robots-manipulation
## Introduction
piper on isaacgym. based on https://github.com/aCodeDog/legged-robots-manipulation

## Installation

### install isaac_gym,rsl_rl,legged_gym

1. You are supposed to install the cuda11.8, isaac_gym,rsl_rl and legged_gym.Please install the above dependencies ([Isaac Gym Preview 4](https://developer.nvidia.com/isaac-gym), [rsl_rl](https://github.com/leggedrobotics/rsl_rl), [legged_gym](https://github.com/leggedrobotics/legged_gym/tree/master)) as described in [legged_gym](https://github.com/leggedrobotics/legged_gym/tree/master).




### install legged-robots-manipulation


```
wget https://download.pytorch.org/whl/cu118/torch-2.1.1%2Bcu118-cp38-cp38-linux_x86_64.whl
wget https://download.pytorch.org/whl/cu118/torchvision-0.16.1%2Bcu118-cp38-cp38-linux_x86_64.whl
pip install torch-2.1.1+cu118-cp38-cp38-linux_x86_64.whl torchvision-0.16.1+cu118-cp38-cp38-linux_x86_64.whl
cd rsl_rl
pip install -e .
cd ..
pip install -e .
```


## Train
```
cd loco_manipulation_gym/scripts

python train.py --task=go2_piper --rl_device=cuda:0

# or

python train.py --task=airbot_piper  --rl_device=cuda:0 
```

## Play
```
cd loco_manipulation_gym/scripts

python play.py --task=go2_piper --rl_device=cuda:0

# or

python play.py --task=airbot_piper  --rl_device=cuda:0 
```