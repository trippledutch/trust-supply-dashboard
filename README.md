# Trust.Supply Economic Dashboard v1.0.1

**Unofficial community-created analytical tool for Trust.Supply validator economics and MNW tokenomics.**

![Version](https://img.shields.io/badge/version-1.0.1-blue)
![Status](https://img.shields.io/badge/status-production-green)
![License](https://img.shields.io/badge/license-community-orange)

---

## 🚀 QUICK START

### **Access the Dashboard**
1. Open `index.html` in any modern browser
2. Click "📊 Update Data" to load latest values
3. Explore tabs: Metrics, Velocity, Scaling, Treasury, etc.
4. Adjust inputs to model different scenarios

### **Live Demo**
🌐 [View Dashboard](https://trippledutch.github.io/trust-supply-dashboard/) *(if hosted)*

---

## ✨ FEATURES

### **📊 Real-Time Data Integration**
- **Live MNW Price** from CoinGecko API
- **On-Chain Staked MNW** from Alchemy/Polygon
- **Automatic Updates** via "Update Data" button
- **Fallback Mechanisms** ensure 100% uptime

### **💰 Economic Modeling**
- Dynamic supply distribution (Ethereum/Polygon)
- Liquidity tier analysis (T1/T2/T3)
- Market cap calculations
- Token velocity scenarios (0.5x - 10x)
- Price impact projections (3x, 10x, 100x)

### **🔧 Validator Economics**
- Node stake configuration (3m, 6m, 12m)
- Weighted average reward calculations
- EVLS penalty modeling (~3% network reduction)
- Team wallet sustainability tracking
- 2026 quarterly cliff projections

### **📈 Advanced Analytics**
- Network scaling projections
- Daily validation requirements
- Validator profitability calculator
- Treasury depletion scenarios
- Required buyback calculations

---

## 📋 WHAT'S NEW IN v1.0.1

### **🆕 Live Data APIs**
- ✅ CoinGecko integration for real-time MNW price
- ✅ Alchemy integration for on-chain staked MNW
- ✅ Enhanced Update Data button with loading states
- ✅ Robust error handling and fallbacks

### **🎨 UI Improvements**
- ✅ Favicon for browser tabs
- ✅ Loading states ("⏳ Loading...")
- ✅ Success/error status messages
- ✅ Better user feedback

**See:** [v1.0.1 Release Notes](v1.0.1_release_notes.md) for full details

---

## 🛠️ TECHNICAL DETAILS

### **Technology Stack**
- **Frontend:** Vanilla HTML/CSS/JavaScript
- **Charts:** Plotly.js
- **APIs:** CoinGecko, Alchemy, GitHub
- **Hosting:** GitHub Pages *(if applicable)*

### **Browser Requirements**
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ❌ Internet Explorer (not supported)

### **API Dependencies**
| API | Purpose | Fallback |
|-----|---------|----------|
| GitHub | Base configuration | None (required) |
| CoinGecko | Live MNW price | JSON data |
| Alchemy | On-chain nodes | JSON data |

---

## 📊 DATA SOURCES

### **1. GitHub JSON (Base Data)**
- **Location:** `dashboard-data.json`
- **Update:** Manual by maintainer
- **Contains:** All input values, rewards, supply distribution
- **Purpose:** Baseline + API fallback

### **2. CoinGecko API (Live Price)**
- **Endpoint:** https://api.coingecko.com/api/v3/simple/price
- **Update:** Real-time (exchange data)
- **Contains:** Current MNW/USD price
- **Purpose:** Accurate market valuations

### **3. Alchemy API (On-Chain Data)**
- **Endpoint:** Polygon Mainnet RPC
- **Update:** Real-time (blockchain state)
- **Contains:** MNW staking wallet balance
- **Purpose:** Actual active node count

---

## 🔧 CONFIGURATION

### **Input Fields**

**Network Metrics:**
- Total Supply: 47,897,218 MNW
- Total Nodes: Dynamic (from Alchemy or manual)
- Active Validators: ~109
- Daily Validations: ~18,900
- MNW Price: Dynamic (from CoinGecko or manual)

**Supply Distribution:**
- Team Wallet: 1,451,053 MNW
- DEX Liquidity: 1,070,000 MNW
- CEX Locked: 3,380,000 MNW
- Ethereum MNW: ~28.7M (dynamic)
- Polygon MNW: ~2.1M (dynamic)
- Lost MNW: 500,000 MNW

**Node Tiers:**
- 3-Month: 441 nodes @ 0.06 MNW/validation
- 6-Month: 357 nodes @ 0.08 MNW/validation
- 12-Month: 3,540 nodes @ 0.10 MNW/validation

---

## 📖 DOCUMENTATION

### **User Guides**
- [v1.0.1 Release Notes](v1.0.1_release_notes.md) - What's new
- [v1.0.1 Changelog](v1.0.1_changelog.md) - Quick summary

### **Technical Guides**
- [API Integration Guide](v1.0.1_api_integration_guide.md) - Developer reference
- [v1.0.0 Complete Documentation](v1.0.0_complete_documentation.md) - Full feature list

---

## 🎯 USE CASES

### **For Validators**
- Calculate profitability at different node counts
- Model rewards across staking periods
- Understand EVLS impact on earnings
- Plan validator expansion strategies

### **For Investors**
- Track real-time market cap
- Analyze supply distribution
- Model price scenarios
- Assess token velocity impact

### **For Analysts**
- Verify on-chain data
- Monitor network growth
- Economic modeling with real data
- Team treasury sustainability analysis

---

## 🐛 TROUBLESHOOTING

### **Issue: "Update Data" button fails**
**Solution:** 
1. Check browser console (F12)
2. Verify internet connection
3. Dashboard will use last loaded values
4. APIs have fallbacks - shouldn't break

### **Issue: Price not updating**
**Solution:**
- CoinGecko API may be rate-limited
- Wait 1 minute and try again
- Dashboard uses JSON fallback automatically

### **Issue: Node count seems wrong**
**Solution:**
- Verify on PolygonScan: [Staking Wallet](https://polygonscan.com/address/0xf994b03d2793788a3ed86eabe792963620bae2c6)
- Check console for Alchemy errors
- Dashboard uses JSON fallback if API fails

### **Issue: Charts not displaying**
**Solution:**
- Ensure Plotly.js CDN is accessible
- Check browser console for errors
- Try refreshing the page

---

## ⚠️ DISCLAIMERS

**This is an unofficial, community-created analytical tool.**

- ⚠️ All data derived from publicly available sources
- ⚠️ Economic models for educational purposes only
- ⚠️ **NOT financial, investment, or legal advice**
- ⚠️ Numbers may contain errors or inaccuracies
- ⚠️ Morpheus.Network and Trust.Supply bear no responsibility
- ⚠️ Users assume all risk for decisions based on this tool
- ⚠️ Always conduct your own research (DYOR)
- ⚠️ Consult qualified professionals before investing

---

## 🔒 PRIVACY & SECURITY

### **Data Collection**
- ❌ No personal data collected
- ❌ No cookies or tracking
- ❌ No analytics
- ✅ Fully client-side (runs in your browser)

### **API Keys**
- Alchemy API key is public (read-only)
- No sensitive operations possible
- Safe to expose in client code

### **Data Transmission**
- HTTPS only (encrypted)
- Public APIs (no authentication)
- No data sent to third parties

---

## 🤝 CONTRIBUTING

### **How to Help**

**Report Issues:**
- Found a bug? Open an issue
- Calculation error? Let us know
- Suggestion? Share your ideas

**Improve Documentation:**
- Fix typos or unclear sections
- Add examples or use cases
- Translate to other languages

**Enhance Features:**
- Add new APIs or data sources
- Improve charts or visualizations
- Optimize performance

---

## 📜 LICENSE

**Community Tool - Unofficial**

Created by @trippledutch for the Trust.Supply community.

This tool is provided "as is" without warranty of any kind. Use at your own risk.

---

## 🙏 ACKNOWLEDGMENTS

**Special Thanks:**
- Trust.Supply community for feedback
- CoinGecko for free public API
- Alchemy for blockchain infrastructure
- Plotly for charting library

**Data Sources:**
- Morpheus.Network on-chain data
- CoinGecko market data
- Community research and analysis

---

## 📞 SUPPORT

### **Get Help**
- Issues: Open on GitHub
- Questions: Community forums
- Feedback: Where dashboard is shared

### **Resources**
- Trust.Supply: https://trust.supply/
- Morpheus.Network: https://morpheus.network/
- CoinGecko: https://www.coingecko.com/en/coins/morpheus-network

---

## 🗺️ ROADMAP

### **Potential Future Features**
- v1.0.2: Auto-refresh, historical charts
- v1.1.0: Ethereum staking integration
- v1.2.0: DEX liquidity tracking
- v2.0.0: Full on-chain data integration

---

## 📊 VERSION HISTORY

- **v1.0.1** (Jan 20, 2026) - Live data APIs + favicon
- **v1.0.0** (Jan 20, 2026) - Initial production release

---

## 🔗 QUICK LINKS

### **Dashboard Sections**
1. 📊 **Network Metrics** - Current state overview
2. 💹 **Token Velocity** - Price impact modeling
3. 📈 **Scaling Projections** - Network growth scenarios
4. 💰 **Team Treasury** - Sustainability analysis
5. 🧮 **My Nodes** - Personal profitability calculator

### **Documentation**
- [Release Notes](v1.0.1_release_notes.md)
- [API Guide](v1.0.1_api_integration_guide.md)
- [Changelog](v1.0.1_changelog.md)

---

**Made with ❤️ by @trippledutch for the Trust.Supply community**

**Last Updated:** January 20, 2026  
**Version:** 1.0.1  
**Status:** Production Ready ✅
