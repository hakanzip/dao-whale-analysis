# Proof of Stake (PoS) Node Trustworthiness EDA

## Dataset
- 📁 Source: [Kaggle - Proof of Stake Blockchain Dataset](https://www.kaggle.com/datasets/a9910rut/proofofstake-blockchain-dataset?utm_source=chatgpt.com&select=Blockchain101.csv)
- 🎯 Target: `Node Label` (0 = Untrustworthy, 1 = Trustworthy)

## Project Structure
project-root/
├── data/ # Raw dataset (CSV)
├── images/ # Exported plots
│ ├── coin_stake_distribution.png
│ ├── coinstake_node_comparison.png
│ ├── txnsize_distribution_analysis.png
│ ├── txnfee_node_distribution.png
│ ├── eda_has_txnfee_distribution.png
│ └── blockscore_node_label.png
├── notebook/ # Jupyter notebook files
├── requirements.txt # Python library dependencies
└── README.md # Project summary (this file)

## Purpose
To explore node behavior in a PoS blockchain and identify trustworthiness patterns based on staking, transaction, and block metrics.

## Process Summary
- Clipped outliers (1%–99%) on numerical features
- Visual EDA on `Coin Stake`, `Txnsize`, `TxnFee`, `Block Score`, etc.
- Labeled and compared trustworthy vs. untrustworthy nodes
- Visualizations stored in `/images/`

## Tools Used
- Python, Pandas, Matplotlib, Seaborn
- Jupyter Notebook

## Key Findings
- High `Coin Stake` and `Block Score` correlate with trustworthy nodes
- Untrustworthy nodes dominate transactions with no fee
- Most small transactions come from lower trust nodes

## How to Run
1. Clone this repo
2. Run: `pip install -r requirements.txt`
3. Open notebook in `/notebook/` and execute cells
