# Hands-on Reinforcement Learning

A compact collection of deep reinforcement learning algorithms implemented in Jupyter notebooks for learning, experimentation, and review.

Each notebook combines the core mathematical ideas with a minimal PyTorch implementation. The focus is on making the connection between equations and code easy to follow—not on providing a production-ready reinforcement learning framework.

## Algorithms

| Notebook | Algorithm | Setting | Main concepts |
| --- | --- | --- | --- |
| [REINFORCE](./REINFORCE.ipynb) | Monte Carlo policy gradient | Discrete actions, on-policy | Policy gradient, trajectory return, categorical policy |
| [Actor-Critic](./Actor-Critic.ipynb) | One-step Actor-Critic | Discrete actions, on-policy | TD error, value baseline, separate actor and critic |
| [PPO](./PPO.ipynb) | Proximal Policy Optimization (PPO-Clip) | Discrete actions, on-policy | GAE, probability ratio, clipped surrogate objective |
| [GRPO](./GRPO.ipynb) | Group Relative Policy Optimization | Discrete actions, on-policy | Group-relative advantage, clipped surrogate objective, reference-policy KL |
| [DQN](./DQN.ipynb) | Deep Q-Network | Discrete actions, off-policy | Q-learning, experience replay, target network, ε-greedy exploration |
| [SAC](./SAC.ipynb) | Soft Actor-Critic | Continuous actions, off-policy | Maximum entropy, double Q-learning, replay buffer, automatic temperature tuning |

The notebooks form a natural learning sequence:

```text
REINFORCE
    └── Actor-Critic
            └── PPO
                    └── GRPO

Off-policy branch
    ├── DQN
    └── SAC
```
