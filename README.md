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

Dataset/
├── 對局 (Matches)/
│   ├── 大師對局 (Master Matches)/
│   │   ├── 以棋手分類 (By Player)/  # e.g., 許銀川 (Xu Yinchuan), 胡榮華 (Hu Ronghua), 呂欽 (Lu Qin), etc.
│   │   ├── 以賽事分類 (By Tournament)/ # e.g., 象甲聯賽 (Xiangqi League), 五羊杯 (Five Rams Cup), etc.
│   │   └── 以開局分類 (By Opening)/    # e.g., 中炮局 (Central Cannon), 屏風馬 (Screen Horse), etc.
│   └── 電腦對局 (Computer Matches)/
│       ├── 人機賽 (Man-Machine Matches)/
│       └── 電腦對局競賽 (Computer vs. Computer)/
├── 中局 (Midgame)/
├── 殘局 (Endgame)/
├── 殺局_殺法_練習題 (Checkmate Tactics & Puzzles)/
├── 全盤戰術 (Full-Game Tactics)/
└── 開局 (Opening Variations)/
