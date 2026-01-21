# Trust.Supply Tools

**Unofficial community-created analytics suite for Trust.Supply validator economics and MNW tokenomics.**

![Version](https://img.shields.io/badge/Landing_Page-v1.0-blue)
![Version](https://img.shields.io/badge/Dashboard-v1.0.1-blue)
![Version](https://img.shields.io/badge/Analytics-v1.0.6-blue)
![Status](https://img.shields.io/badge/status-production-green)

---

## 🚀 Live Tools

**🌐 Landing Page:** Professional tool selection hub with unified design

**💰 Economic Dashboard (v1.0.1):**
- Comprehensive validator economics and tokenomics modeling
- Live MNW price from CoinGecko
- On-chain staked MNW from Alchemy
- Dynamic liquidity tier analysis
- Token velocity scenarios
- Network scaling projections

**📊 Validator Analytics (v1.0.6):**
- Real-time blockchain transaction analysis
- Validation tracking from Polygon
- Daily average calculations
- Historical transaction logs
- Flexible time period analysis (1-30 days)

---

## ✨ Features

### **Economic Dashboard v1.0.1**

**Real-Time Data Integration:**
- 💰 Live MNW price from CoinGecko API
- 🔗 On-chain staked MNW from Alchemy (Polygon)
- 📊 Automatic data updates
- 🔄 Graceful fallback mechanisms

**Economic Modeling:**
- Dynamic supply distribution (Ethereum/Polygon)
- Liquidity tier analysis (T1/T2/T3)
- Market cap calculations
- Token velocity scenarios (0.5x - 10x)
- Price impact projections (3x, 10x, 100x)

**Validator Economics:**
- Node stake configuration (3m, 6m, 12m)
- Weighted average reward calculations
- EVLS penalty modeling (~3% network reduction)
- Team wallet sustainability tracking
- 2026 quarterly cliff projections

**Advanced Analytics:**
- Network scaling projections
- Daily validation requirements
- Validator profitability calculator
- Treasury depletion scenarios
- Required buyback calculations

### **Validator Analytics v1.0.6**

**Blockchain Analysis:**
- 🔍 Live transaction scanning from Polygon
- 📈 Query and validation counting
- 📊 Daily average calculations
- 📅 Flexible time periods (Today, 3/7/30 days)
- 📋 Detailed transaction history logs
- 🕐 UTC calendar window analysis

**Data Visualization:**
- Total queries and batched transactions
- Total validations (Batched TX × 7)
- Period averages per day
- Today's transactions highlighted
- Clean, readable log table

---

## 🎨 Design System

**Unified Purple Gradient Theme:**
- Consistent design across all three pages
- Purple gradient backgrounds (#667eea → #764ba2)
- White content containers
- Professional shadows and hover effects
- Fully responsive (mobile-friendly)

**Navigation:**
- Landing page with tool selection cards
- "Back to Tools" links on all pages
- Seamless navigation flow
- Professional user experience

---

## 🛠️ Technology Stack

**Frontend:**
- Vanilla HTML/CSS/JavaScript
- Plotly.js for charts (Dashboard)
- No external dependencies (except Plotly)

**APIs:**
- CoinGecko (Live MNW price)
- Alchemy (On-chain Polygon data)
- Etherscan (Transaction history)
- GitHub (Base configuration data)

**Hosting:**
- GitHub Pages
- Static site (no backend required)
- Free hosting

---

## 📦 Installation & Deployment

### **Quick Setup**

1. **Clone or Fork Repository**
```bash
git clone https://github.com/trippledutch/trust-supply-dashboard.git
cd trust-supply-dashboard
```

2. **File Structure**
```
trust-supply-dashboard/
├── index.html              # Landing page
├── dashboard.html          # Economic Dashboard v1.0.1
├── analytics.html          # Validator Analytics v1.0.6
├── favicon.ico
├── dashboard-data.json     # Base configuration data
├── README.md
└── docs/
    ├── v1.0.1_release_notes.md
    ├── v1.0.1_api_integration_guide.md
    └── API_SECURITY_GUIDE.md
```

3. **Deploy to GitHub Pages**
   - Push to GitHub repository
   - Go to Settings → Pages
   - Source: Deploy from branch (main)
   - Save
   - Your site will be live at: `https://yourusername.github.io/repository-name/`

### **API Configuration**

**⚠️ Important: Use Free Tier API Keys Only**

The tools use public API keys visible in client-side code. For security:

**1. Alchemy Setup (Dashboard):**
- Create **FREE tier** app at https://dashboard.alchemy.com/
- Network: Polygon Mainnet
- Plan: Growth (Free) ✅
- Add domain restrictions (Settings → Allowed Origins)
- **⚠️ NEVER use unlimited/paid keys in public code**

**2. Etherscan Setup (Analytics):**
- Get free API key at https://etherscan.io/myapikey
- Add domain whitelist for your GitHub Pages URL
- Free tier: 100,000 calls/day (more than enough)

**3. Update Keys in Code:**

In `dashboard.html`:
```javascript
const ALCHEMY_URL = 
    'https://polygon-mainnet.g.alchemy.com/v2/YOUR_FREE_TIER_KEY';
```

In `analytics.html`:
```javascript
const KEY = "YOUR_ETHERSCAN_API_KEY";
```

**See [API_SECURITY_GUIDE.md](docs/API_SECURITY_GUIDE.md) for complete security details.**

---

## 🔒 Security & Privacy

**Data Collection:**
- ❌ No personal data collected
- ❌ No cookies or tracking
- ❌ No analytics
- ✅ Fully client-side (runs in your browser)

**API Keys:**
- Use FREE tier keys only in public code
- Domain restrictions recommended
- Keys are read-only (query public blockchain data)
- Monitor usage regularly
- Regenerate if abused
- **Never expose unlimited/paid API keys**

**Data Sources:**
- All data from public blockchain
- No sensitive information
- No authentication required

---

## 📊 API Usage & Limits

**Expected Usage (Low Traffic):**

| API | Calls/User | Users/Day | Monthly Total | Free Limit | Usage % |
|-----|------------|-----------|---------------|------------|---------|
| CoinGecko | 1-2 | 10 | 600 | ~100,000 | 0.6% |
| Alchemy | 1-2 | 10 | 600 | 300,000 | 0.2% |
| Etherscan | 1-5 | 20 | 3,000 | 100,000/day | 0.1% |

**Conclusion:** Free tiers are more than sufficient! ✅

**Rate Limits:**
- Built-in API delays prevent spam
- Fallback mechanisms ensure functionality
- User feedback for errors
- Dashboard remains usable even if APIs fail

---

## 🎯 Use Cases

### **For Validators**
- Calculate profitability at different node counts
- Model rewards across staking periods
- Understand EVLS impact on earnings
- Plan validator expansion strategies
- Track real-time network activity

### **For Investors**
- Track real-time market cap
- Analyze supply distribution
- Model price scenarios
- Assess token velocity impact
- Monitor on-chain metrics

### **For Analysts**
- Verify on-chain data
- Monitor network growth
- Economic modeling with real data
- Team treasury sustainability analysis
- Transaction pattern analysis

---

## 📖 Documentation

### **User Guides**
- [v1.0.1 Release Notes](docs/v1.0.1_release_notes.md) - Dashboard features
- [API Integration Guide](docs/v1.0.1_api_integration_guide.md) - Technical details
- [API Security Guide](docs/API_SECURITY_GUIDE.md) - Security best practices

### **Setup Guides**
- [FINAL_SETUP_INSTRUCTIONS.md](docs/FINAL_SETUP_INSTRUCTIONS.md) - Deployment
- [Landing Page Structure](docs/landing-page-structure.md) - File organization

### **Development Docs**
- [Complete Documentation](docs/v1.0.0_complete_documentation.md) - Full feature list
- [Analytics Styling](docs/ANALYTICS_STYLING_COMPLETE.md) - Design system

---

## 🐛 Troubleshooting

### **"Update Data" button fails**
**Solution:**
1. Check browser console (F12)
2. Verify internet connection
3. Dashboard uses fallback to JSON data
4. APIs have built-in error handling

### **Price not updating**
**Solution:**
- CoinGecko API may be rate-limited
- Wait 1 minute and try again
- Dashboard automatically falls back to JSON data

### **Node count seems wrong**
**Solution:**
- Verify on [PolygonScan](https://polygonscan.com/address/0xf994b03d2793788a3ed86eabe792963620bae2c6)
- Check console for Alchemy errors
- Dashboard uses JSON fallback if API fails

### **Analytics not loading transactions**
**Solution:**
- Check Etherscan API key is valid
- Verify domain restrictions allow your site
- Try shorter time period (Today instead of 30 days)
- Check browser console for errors

---

## ⚠️ Important Disclaimers

**This is an unofficial, community-created analytical tool.**

- ⚠️ All data derived from publicly available sources
- ⚠️ Economic models for educational purposes only
- ⚠️ **NOT financial, investment, or legal advice**
- ⚠️ Numbers may contain errors or inaccuracies
- ⚠️ Morpheus.Network and Trust.Supply bear no responsibility
- ⚠️ Users assume all risk for decisions based on these tools
- ⚠️ Always conduct your own research (DYOR)
- ⚠️ Consult qualified professionals before investing

---

## 🤝 Contributing

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

**Code Contributions:**
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

---

## 🙏 Acknowledgments

**Created by:** @trippledutch for the Trust.Supply community

**Special Thanks:**
- Trust.Supply community for feedback and testing
- CoinGecko for free public API
- Alchemy for blockchain infrastructure
- Etherscan for transaction data
- Plotly for charting library

**Data Sources:**
- Morpheus.Network on-chain data
- CoinGecko market data
- Community research and analysis

---

## 📜 License

**Community Tool - Unofficial**

This tool is provided "as is" without warranty of any kind. Use at your own risk.

Not affiliated with Morpheus.Network or Trust.Supply.

---

## 🗺️ Roadmap

### **Current Version (v1.0)**
- ✅ Landing page with tool selection
- ✅ Economic Dashboard with live APIs
- ✅ Validator Analytics with blockchain data
- ✅ Unified purple gradient design
- ✅ Responsive mobile design
- ✅ Complete documentation

### **Future Enhancements**
- [ ] Auto-refresh option (configurable intervals)
- [ ] Historical price charts
- [ ] Ethereum staking integration
- [ ] DEX liquidity tracking
- [ ] Export data features
- [ ] Dark mode option
- [ ] Multi-language support

---

## 📊 Version History

**v1.0.6** (January 21, 2026) - Analytics Purple Theme
- Restyled to match Dashboard purple gradient
- Improved status bar (blue badge)
- Better log table visibility (darker text, larger font)
- Added bottom navigation button
- Enhanced hover effects
- Fixed "Total Validations" label

**v1.0.1** (January 20, 2026) - Dashboard Live Data
- Added CoinGecko API for live MNW price
- Added Alchemy API for on-chain staked MNW
- Enhanced "Update Data" button with loading states
- Robust error handling and fallbacks
- Navigation buttons (top & bottom)

**v1.0** (January 20, 2026) - Initial Production Release
- Landing page with tool selection
- Economic Dashboard with comprehensive modeling
- Validator Analytics with blockchain scanning
- Unified design system
- Complete documentation

---

## 📞 Support & Feedback

### **Get Help**
- Issues: GitHub Issues (if repository is public)
- Questions: Trust.Supply community channels
- Feedback: Community forums

### **Resources**
- Trust.Supply: https://trust.supply/
- Morpheus.Network: https://morpheus.network/
- MNW on CoinGecko: https://www.coingecko.com/en/coins/morpheus-network

---

## 🔗 Quick Links

### **On-Chain Verification**
- [MNW Token on PolygonScan](https://polygonscan.com/token/0x3c59798620e5fec0ae6df1a19c6454094572ab92)
- [Staking Wallet](https://polygonscan.com/address/0xf994b03d2793788a3ed86eabe792963620bae2c6)

### **API Providers**
- [CoinGecko](https://www.coingecko.com/)
- [Alchemy](https://www.alchemy.com/)
- [Etherscan](https://etherscan.io/)

---

## 🎯 Key Metrics

**Tools:** 3 (Landing, Dashboard, Analytics)  
**Version:** v1.0.1 (Dashboard), v1.0.6 (Analytics)  
**APIs Integrated:** 3 (CoinGecko, Alchemy, Etherscan)  
**Lines of Code:** ~5,000+  
**Documentation Pages:** 15+  
**Status:** Production Ready ✅

---

## 🔐 API Security Notes

**Current Approach:** Free Tier Public Keys ✅

**Why This Works:**
- Community tools (not commercial)
- Public blockchain data only
- Low traffic (~0.2% of API limits)
- Free tiers are sufficient
- Domain restrictions add security

**Best Practices:**
- ✅ Use FREE tier keys only
- ✅ Add domain restrictions
- ✅ Monitor usage weekly
- ✅ Keep unlimited keys private
- ✅ Regenerate if abused

**When to Upgrade:**
- Only if getting 100+ daily users
- Only if hitting rate limits
- Consider serverless functions then

**See full [API Security Guide](docs/API_SECURITY_GUIDE.md) for details.**

---

**Made with ❤️ by @trippledutch for the Trust.Supply community**

**Last Updated:** January 21, 2026  
**Status:** Active & Production Ready 🚀
