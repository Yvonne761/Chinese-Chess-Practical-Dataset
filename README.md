# Chinese-Chess-Practical-Dataset
A large-scale, practical-oriented Chinese Chess (Xiangqi) dataset featuring 58k+ instances derived from master-level match records. Designed for sequential modeling, opening recognition, and AI training with zero synthetic bias.

# Chinese Chess Practical Dataset (CCPD)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## 📌 Overview
**Chinese Chess Practical Dataset (CCPD)** is a large-scale, high-quality collection of Chinese Chess (Xiangqi) records designed for artificial intelligence research, sequential modeling, and opening recognition. 

The core philosophy of this dataset is its **practical-oriented** collection standard. Every instance—ranging from complete game matches to tactical puzzles—is derived exclusively from **actual match records** or **professional master reviews**, rather than synthetic or man-made "composed problems" (排局).

## 📊 Dataset Statistics
The dataset comprises a total of **58,528** instances, providing a solid foundation for deep learning and sequence analysis.

### Composition
- **Full Game Matches:** 53,953 games (Ideal for sequential modeling)
- **Midgame Puzzles:** 2,807 instances
- **Opening Variations:** 961 instances
- **Tactical Exercises:** 433 instances
- **Endgame Scenarios:** 244 instances

![Dataset Structure](./Fig1_Structure.png)
*Fig 1: Overview of Dataset Composition*

## 🌟 Key Features
- **Authenticity:** All data reflects real-world competitive play, capturing the inherent complexity and move probability distributions of human masters.
- **Diversity:** Covers decades of professional match history, including a wide range of opening systems (e.g., Central Cannon vs. Screen Horse).
- **Zero Synthetic Bias:** By avoiding artificial scenarios, the dataset mitigates potential training biases and enhances the model's ability to generalize to genuine human decision-making.

### Historical Trend
The dataset captures the evolution of Xiangqi strategies over time, with records spanning from the 1950 to 2013.
![Yearly Distribution](./Fig7_Year_Dist.png)
*Fig 7: Game Distribution by Year*

## 🚀 Applications
This dataset is suitable for various AI tasks, including:
1. **Opening Classification:** Training models (like LSTM/CNN) to recognize opening systems.
2. **Move Prediction:** Learning sequence dependencies in master-level play.
3. **Tactical Analysis:** Solving real-world midgame and endgame problems.

## 📂 File Structure
```text
├── csv_data/
│   ├── games_parsed.csv     # Raw game sequences and metadata
│   ├── opening_stats.csv    # Frequency analysis of opening systems
│   ├── player_stats.csv     # Statistics for professional players
│   └── struct_data.csv      # Category-wise distribution
└── figures/                 # Statistical visualizations
