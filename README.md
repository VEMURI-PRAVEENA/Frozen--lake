

```markdown
# Comparative Analysis of Q-Learning and Policy Gradient Methods in Stochastic FrozenLake Environment

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![OpenAI Gym](https://img.shields.io/badge/OpenAI%20Gym-0.26.0-red)
![PyTorch](https://img.shields.io/badge/PyTorch-1.13.0-orange)

This repository contains the implementation and experimental results for our research paper comparing Q-Learning and Policy Gradient methods in the stochastic FrozenLake environment from OpenAI Gym.

## 📝 Abstract
We present a comprehensive comparison between Q-Learning and Policy Gradient algorithms in the stochastic FrozenLake domain. Our analysis focuses on convergence speed, accumulated rewards, and learning stability, utilizing a custom reward function that significantly improves learning efficiency. Experimental results demonstrate that while Q-Learning shows quicker initial improvements, Policy Gradient methods achieve higher success rates (62% vs 42%) and better handle environmental stochasticity.

## 🏆 Key Findings
- Policy Gradient methods outperform Q-Learning in stochastic environments
- Success rates: 62% (Policy Gradient) vs 42% (Q-Learning)
- Policy Gradient shows better long-term performance despite slower initial learning
- Custom reward function improves learning efficiency by 15%

## 🚀 Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/frozenlake-comparison.git
cd frozenlake-comparison
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## 🧪 Experiments
The repository contains implementations of:
- Q-Learning with ε-greedy exploration
- Policy Gradient with neural network policy
- Custom reward function implementation
- Training and evaluation scripts

### File Structure
```
├── data/                   # Saved models and training logs
├── figs/                   # Result figures and plots
├── src/
│   ├── q_learning/         # Q-Learning implementation
│   ├── policy_gradient/    # Policy Gradient implementation
│   ├── env_wrappers.py     # Custom environment wrappers
│   ├── utils.py            # Utility functions
│   └── config.py           # Experiment configurations
├── requirements.txt        # Python dependencies
└── README.md               # This file
```

## 🏃‍♂️ How to Run
### Training Q-Learning
```bash
python src/q_learning/train.py --env FrozenLake-v1 --is_slippery True --episodes 500
```

### Training Policy Gradient
```bash
python src/policy_gradient/train.py --env FrozenLake-v1 --is_slippery True --episodes 500
```

### Evaluation
```bash
python src/evaluate.py --model q_learning --env FrozenLake-v1 --is_slippery True
python src/evaluate.py --model policy_gradient --env FrozenLake-v1 --is_slippery True
```

## 📊 Results
Our experiments show the following performance metrics:

| Metric               | Q-Learning | Policy Gradient |
|----------------------|------------|-----------------|
| Average Reward       | -156.3     | -89.5           |
| Success Rate         | 42%        | 62%             |
| Convergence Episode  | ~300       | ~400            |
| Training Stability   | High       | Moderate        |

![Training Curves](figs/training_curves.png)

## 📚 References
1. Sutton & Barto (2018). Reinforcement Learning: An Introduction
2. Watkins & Dayan (1992). Q-learning
3. Williams (1992). Policy Gradient methods
4. Mnih et al. (2015). Human-level control through deep RL
5. Schulman et al. (2015). Trust Region Policy Optimization

## ✉️ Contact
For questions or collaborations, please contact:
- Vemuri Praveena: vemuripraveena2622@vitap.ac.in
- Dr. D. John Pradeep: john.darsy@vitap.ac.in

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```


