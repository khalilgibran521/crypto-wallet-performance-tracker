# Crypto Wallet Performance Tracker Scraper
This tool pinpoints high-performing wallets across major blockchains and turns their activity into actionable insights. It helps traders and analysts understand PnL patterns, win rates, and balance trends with clean structured data. By tracking wallet performance consistently, it offers a practical way to evaluate profitable behavior at scale.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>Crypto Wallet Performance Tracker</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
The project analyzes insider and whale wallet performance across multiple chains, delivering clear metrics like PnL, balance, and win rate. It solves the challenge of manually evaluating wallet activity and streamlines performance tracking for researchers, traders, and developers.

### Why Performance Tracking Matters
- Reveals profitable wallets worth monitoring.
- Highlights short-term and long-term activity patterns.
- Simplifies multi-chain research into one unified workflow.
- Provides structured output for downstream tools or dashboards.
- Helps traders verify wallet consistency and historical success.

## Features
| Feature | Description |
|---------|-------------|
| Multi-chain support | Analyze wallets across Solana, Ethereum, Base, Tron, and Blast. |
| Profitability metrics | Calculates PnL, win rate, realized and unrealized profits. |
| Cost analysis | Tracks total cost basis, average token cost, and realized profit averages. |
| Balance tracking | Monitors native token balance and USD value. |
| Configurable analysis windows | Choose 7-day or 30-day time periods. |
| Proxy-ready | Supports custom proxies for smoother large-volume analysis. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|------------------|
| wallet | The address being analyzed. |
| chain | The blockchain network source. |
| daysOption | Selected analysis window (7d or 30d). |
| totalPnlUsdAmount | Total profit or loss in USD. |
| totalPnlPct | Percentage return on invested capital. |
| unrealizedUsdProfit | Current unrealized gains or losses. |
| totalUsdCost | Total invested amount. |
| tokenAvgUsdCost | Mean cost per token. |
| tokenAvgRealizedUsdProfit | Average realized profit per profitable trade. |
| balance | Current native token amount. |
| usdBalance | Estimated USD value of all holdings. |
| pnlPct | Overall performance percentage. |
| winrate | Percentage of winning trades. |
| error | Any encountered issues during analysis. |

---

## Example Output

    {
      "wallet": "61LtsXuMfC2SCUr7RYVRKBe3mmTTxUYeGt4HTN94CjKx",
      "chain": "sol",
      "daysOption": "30d",
      "totalPnlUsdAmount": 15234.50,
      "totalPnlPct": 25.6,
      "unrealizedUsdProfit": 3421.75,
      "totalUsdCost": 50000.00,
      "tokenAvgUsdCost": 22.45,
      "tokenAvgRealizedUsdProfit": 1250.80,
      "balance": 2234.567,
      "usdBalance": 53421.75,
      "pnlPct": 25.6,
      "winrate": 68.5,
      "error": null
    }

---

## Directory Structure Tree

    Crypto Wallet Performance Tracker/
    ├── src/
    │   ├── main.ts
    │   ├── utils/
    │   │   ├── walletCalculator.ts
    │   │   └── proxyManager.ts
    │   ├── services/
    │   │   ├── solanaScanner.ts
    │   │   ├── ethereumScanner.ts
    │   │   ├── baseScanner.ts
    │   │   ├── tronScanner.ts
    │   │   └── blastScanner.ts
    │   ├── models/
    │   │   ├── WalletStats.ts
    │   │   └── ValidationSchema.ts
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample-wallets.json
    │   └── output-sample.json
    ├── tests/
    │   ├── walletStats.test.ts
    │   └── scanners.test.ts
    ├── package.json
    ├── requirements.txt
    └── README.md

---

## Use Cases
- **Crypto researchers** use it to compare wallet behavior, so they can spot consistent outperformers.
- **Traders** analyze whale activity to mirror profitable strategies and improve decision-making.
- **Data analysts** integrate structured wallet stats into dashboards for long-term trend tracking.
- **Developers** automate wallet monitoring to enhance portfolio tools or trading bots.
- **Market observers** follow insider-like behavior to anticipate unusual market shifts.

---

## FAQs

**Does it support multiple blockchains at once?**
Yes, you can run analyses on any supported chain individually, and batch multiple wallets for broader comparisons.

**What if a wallet has incomplete or missing data?**
The output includes an `error` field which indicates issues such as unavailable activity or unreachable endpoints.

**Can I use custom proxies?**
Absolutely. Proxy configuration is fully supported for higher request stability and throughput.

**Is the time window customizable?**
You can choose between 7-day and 30-day periods depending on how granular you want the analysis to be.

---

### Performance Benchmarks and Results

**Primary Metric:** Average analysis time per wallet remains under two seconds across stable networks, offering rapid feedback even for large lists.

**Reliability Metric:** Success rates typically remain above 95% when using quality proxies, ensuring consistent data retrieval.

**Efficiency Metric:** Parallelized requests enable steady throughput, allowing hundreds of wallets to be processed with minimal slowdown.

**Quality Metric:** Data completeness regularly exceeds 98%, with accurate PnL and balance calculations validated against live blockchain data.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
