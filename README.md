# AAVE v3 Rates Analysis

This project provides a curated dataset and framework for analyzing the **hourly supply and borrowing rates** on the AAVE v3 lending protocol across **Ethereum**, **Arbitrum**, and **Base** networks over the past two years.

## Dataset Overview

The dataset includes the following fields:

| Field             | Description |
|------------------|-------------|
| `Timestamp`       | Hourly UTC timestamp of each data point |
| `Network`         | Blockchain network (Ethereum, Arbitrum, Base) |
| `Token`           | Supported asset (e.g., USDC, DAI, ETH) |
| `Supply Rate (%)` | Annualized supply rate for lenders |
| `Borrowing Rate (%)` | Annualized borrowing rate for users |
| `Utilization Rate (%)` | Percentage of supplied funds being borrowed |

## Files Included

- `aave_v3_rates_sample.csv` — Tabular CSV format for Excel/BI tools
- `aave_v3_rates_sample.json` — JSON structured data for developers

## Data Collection Method

Data was collected via:

- **AAVE v3 Subgraphs** for Ethereum, Arbitrum, and Base
- Historical data pulled using GraphQL queries
- Cleaned and normalized for consistency
- Processed via Python and exported to CSV and JSON formats

## Use Cases

- Rate trend analysis across networks and time
- Comparing lending profitability on different chains
- Risk modeling via utilization rate
- Building DeFi strategies based on interest dynamics

## Limitations

- Some missing hourly snapshots due to subgraph downtime
- Stable/variable rate distinction omitted in this version
- Historical token lists may vary by network and time

## Setup for Developers

Clone the repository and install any future dependencies (TBD):

```bash
git clone https://github.com/destinedai/aave-v3-rates-analysis.git
cd aave-v3-rates-analysis
