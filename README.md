# HK Election Data / 香港選舉數據

This repository contains data related to Hong Kong elections, converted from PDF files (sourced from the Registration and Electoral Office) into machine-readable formats (CSV/Excel).

本儲存庫包含與香港選舉相關的數據，這些數據由 PDF 文件（源自選舉事務處）轉換為機器可讀格式（CSV/Excel）。

## Directory Structure / 目錄結構

The data is organized into the following structure:
數據按以下結構組織：

```
data/
├── raw/                                  # Original raw data (PDFs) / 原始數據 (PDF)
│   ├── 2017_voter_registration/
│   └── 2018_legislative_council_by_election/
└── processed/                            # Cleaned data (CSV/Excel) / 已清理數據 (CSV/Excel)
    ├── polling_stations/                 # Polling station addresses and coordinates / 票站地址及座標
    ├── voter_registration/               # Voter registration statistics / 選民登記統計
    │   ├── total/                        # Total registered voters / 登記選民總數
    │   └── new/                          # New voter registrations / 新增選民登記
    └── voter_turnout/                    # Voter turnout statistics / 投票率統計
        ├── hourly/                       # Hourly turnout by polling station / 各票站每小時投票率
        └── demographics/                 # Turnout by age group and gender / 按年齡組別及性別劃分的投票率
```

## Data Descriptions / 數據說明

### Voter Turnout (`data/processed/voter_turnout/`) / 投票率
- **Hourly**: Hourly voter turnout statistics for each polling station across various years.
  **每小時**: 各年份各票站每小時的投票數據。
- **Demographics**: Voter turnout demographics broken down by age group and gender for each polling station.
  **人口統計**: 各票站按年齡組別及性別劃分的投票人數。

### Polling Stations (`data/processed/polling_stations/`) / 票站資料
Details for polling stations from recent elections, including addresses, geographical coordinates, and the number of assigned voters.
最近選舉各票站的詳細資料，包括地址、經緯度及獲分配的選民人數。

### Voter Registration (`data/processed/voter_registration/`) / 選民登記
- **Total**: Voter registration figures by constituency and age group (2011-2017).
  **總數**: 2011年至2017年各選區按年齡組別劃分的選民登記人數。
- **New**: Statistics on *newly* registered voters by constituency and age group (2011-2017).
  **新增**: 2011年至2017年各選區按年齡組別劃分的新增選民登記人數。

*Note: Constituency boundaries may differ between 2011-2014 and 2015-2017.*
*注意：2011-2014年與2015-2017年的選區分界可能有所不同。*

## Disclaimer / 免責聲明
This data is being processed by a learner. Please report any errors or issues.
此數據由學習者處理。如有任何錯誤或問題，請回報。
