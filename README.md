# legged-robots-manipulation
## Introduction
piper on isaacgym. based on https://github.com/aCodeDog/legged-robots-manipulation

## Installation

### install isaac_gym,rsl_rl,legged_gym

1. You are supposed to install the isaac_gym,rsl_rl and legged_gym.Please install the above dependencies ([Isaac Gym Preview 4](https://developer.nvidia.com/isaac-gym), [rsl_rl](https://github.com/leggedrobotics/rsl_rl), [legged_gym](https://github.com/leggedrobotics/legged_gym/tree/master)) as described in [legged_gym](https://github.com/leggedrobotics/legged_gym/tree/master).




### install legged-robots-manipulation


```
cd legged-robots-manipulation
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