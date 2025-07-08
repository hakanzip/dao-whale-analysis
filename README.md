# DAO Whale Distribution Analysis

This project investigates the distribution of governance tokens in a DAO ecosystem, focusing on how much of the total supply is controlled by whale wallets.

---

## 📦 Dataset

- **Source**: Internally compiled DAO token distribution data
- **Format**: CSV
- **Fields**:
  - `wallet_address`: Public address of the holder
  - `token_amount`: Number of DAO tokens held
  - `percentage_of_total`: Share of total supply
  - `group`: Categorized as Whale / Dolphin / Shrimp

---

## 🎯 Objective

To analyze the level of decentralization in DAO governance by examining token concentration and identifying the dominance of whale wallets.

---

## 📁 Directory Structure

```text
dao_whale/
├── data/                         # Raw CSV file with DAO token data
├── images/                       # Visual outputs
│   ├── non_whale_balance.png
│   ├── top5_dao_whale_count.png
│   ├── unique_users_per_dao.png
│   └── whale_ratio_distribution.png
├── notebook/
│   └── dao_whalep.ipynb          # Main analysis notebook
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

---

## 🔍 Methodology

- Loaded and validated DAO token holding dataset
- Calculated percentage ownership per wallet
- Grouped holders into categories:
  - Whale: >5%
  - Dolphin: 1–5%
  - Shrimp: <1%
- Visualized distribution across DAOs:
  - Whale dominance
  - Address count
  - Non-whale balances
  - Whale ratio density

---

## 📊 Key Insights

- DAO token ownership is highly concentrated in whales
- Some DAOs have >90% of their tokens held by <5 wallets
- Non-whale balances often remain insignificant in governance control
- Very few DAOs have truly decentralized token distribution

---

## 🖼️ Visual Outputs (Saved in `/images/`)

- `non_whale_balance.png` → Total token share of non-whale addresses
- `top5_dao_whale_count.png` → Number of whale wallets in top 5 DAOs
- `unique_users_per_dao.png` → Active token holders per DAO
- `whale_ratio_distribution.png` → Whale ratio distribution histogram (DAO-wise)

---

## 🧰 Tools Used

- Python 3.9
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run `notebook/dao_whalep.ipynb` in Jupyter

---

## 👤 Author

**Hakan Ataş**  
Data Scientist | Crypto Analyst | Blockchain Researcher

This project aims to measure and visualize governance centralization risks in DAO ecosystems through whale distribution analysis.
