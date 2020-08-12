# PolicyGradients

Pytorch single thread implementation of REINFORCE, Trust Region Policy Optimization (TRPO) & Proximal Policy Optimization (PPO).

## LunarLander-v2
<p align="center">
  <img src="GIFs/LunarLander-v2_TRPO_10.gif" alt="LunarLander gif" height=300 style="float:left"/>
  <img src="GIFs/LunarLander-v2.png" alt="comparison LunarLander" height=350/>
</p>

## Acrobot-v1
<p align="center">
  <img src="GIFs/Acrobot-v1_TRPO_10.gif" alt="Acrobot-v1" height=300 style="float:left"/>
  <img src="GIFs/Acrobot-v1.png" alt="comparison Acrobot" height=350/>
</p>

## CartPole-v0
<p align="center">
  <img src="GIFs/CartPole-v0_TRPO_10.gif" alt="CartPole-v0" height=300 style="float:left"/>
  <img src="GIFs/CartPole-v0.png" alt="comparison CartPole" height=350/>
</p>

## Train
```shell
python train.py \
  --algo TRPO \
  --seeds 10 20 30 \
  --env_name LunarLander-v2 \
```


## Test
```shell
python test.py \
  --algo PPO \
  --env_name Acrobot-v1 \
  --seed 10
```

## Plot
```shell
python plot.py \
  --algos REINFORCE PPO TRPO \
  --env_name LunarLander-v2
```

## References
<ul>
  <li> <a href="https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf"> REINFORCE </a> </li>
  <li> <a href="https://arxiv.org/pdf/1707.06347.pdf"> Proximal Policy Optimization </a> </li>
  <li> <a href="https://arxiv.org/pdf/1502.05477.pdf"> Trust Region Policy Optimization </a> </li>
</ul>
