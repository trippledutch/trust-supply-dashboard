# Trust.Supply Economic Dashboard v5.7 - User Guide

**Your Complete Validator Economics Planning Tool**

---

## 🎯 What Does This Dashboard Do?

The Trust.Supply Economic Dashboard helps you plan and optimize your validator strategy by calculating:
- **Daily & yearly validations** your nodes will earn
- **Token yield** (MNW earned vs staked)
- **Annual profit** in USD
- **ROI** (return on investment)
- **Optimal node configurations** for maximum returns

**Key Feature:** Dynamic highlighting automatically shows you the BEST configurations based on YOUR settings.

---

## 📊 Common Use Cases

### 1. Planning Your First Validator
**Scenario:** "I want to become a validator. How many nodes should I run?"

**How to use:**
1. Keep default settings for daily validations and current price
2. Look at the **Multi-Node VPS Strategy** table
3. Find the **GREEN rows** ⭐ - these show optimal configurations
4. Default shows: **90 nodes = 9.80% ROI** (highest)
5. Check the profit: ~$2,650/year at current price

**Decision:** Target 80-90 nodes for best returns before EVLS penalty kicks in at 100.

---

### 2. Optimizing Existing Validators
**Scenario:** "I have 100 nodes. Should I add more or reduce?"

**How to use:**
1. Enter **100** in "My Nodes Calculator"
2. See your current economics:
   - Daily Validations: ~446
   - ROI: ~8.80%
   - EVLS Penalty: 10.26%
3. Compare to the green optimal rows in the table
4. See that 90 nodes shows higher ROI (9.80%)

**Decision:** Consider reducing to 90 nodes to avoid EVLS penalty and boost ROI by 1%.

---

### 3. Modeling Suite.Supply Launch
**Scenario:** "Suite.Supply has launched on January 9th, 2026. How will network growth affect my earnings?"

**How to use:**
1. Set your current nodes (e.g., 100)
2. Adjust **"Active Nodes"** slider:
   - Current: 4,339 nodes
   - After Suite.Supply: 8,000-10,000 nodes (estimate)
3. Watch your metrics update in real-time:
   - Daily Validations: 446 → ~223 (drops)
   - Annual Profit: $2,645 → ~$1,320 (drops)
   - ROI: 8.80% → ~4.40% (drops)

**Key Insight:** More network nodes = more competition = lower earnings per node (unless Daily Validations also increases!)

**Decision:** Set realistic expectations. Your per-node earnings will likely decrease as the network grows.

---

### 4. Price Projections
**Scenario:** "What if MNW price goes to $0.30? How does that change my returns?"

**How to use:**
1. Change **"Current Price"** from current → $0.30
2. Watch profit metrics update:
   - Annual Profit: $2,645 → ~$4,750 (increases)
   - ROI: 8.80% → ~15.80% (increases)
3. Check which configs are still optimal (green rows)
4. Note: Same config wins, just higher returns

**Decision:** Higher price = proportionally higher profits. The optimal node count usually stays the same.

---

### 5. Bear Market Planning
**Scenario:** "What if MNW price drops to $0.08? Is it still profitable?"

**How to use:**
1. Change **"Current Price"** to $0.08
2. Check 90-node configuration:
   - Annual Profit: $2,652 → ~$1,270
   - ROI: 9.80% → ~4.70%
   - Still profitable? Yes ✅
3. Find break-even point by lowering price further

**Decision:** At $0.08, still profitable but lower returns. VPS cost of $72/year is covered as long as price stays above ~$0.04.

---

### 6. Comparing Node Counts
**Scenario:** "Should I run 75, 80, or 90 nodes? What's the difference?"

**How to use:**
1. Look at **Multi-Node VPS Strategy** table
2. Compare side-by-side:

| Nodes | Daily Val | Annual Profit | ROI | EVLS |
|-------|-----------|---------------|-----|------|
| 75 | 373 | $2,198 | 9.75% | 0% |
| 80 | 397 | $2,350 | 9.77% | 0% |
| 90 | 447 | $2,652 | 9.80% | 0% |

**Key Insight:** All three have 0% EVLS, but 90 nodes gives:
- +$454/year more profit than 75 nodes
- +$302/year more profit than 80 nodes
- Highest ROI at 9.80%

**Decision:** Go with up to 90 nodes if you can - maximum returns without EVLS penalty.

---

### 7. Network Size Scenarios
**Scenario:** "What if the network shrinks to 2,000 nodes?"

**How to use:**
1. Enter your node count (e.g., 100)
2. Adjust **"Active Nodes"** to 2,000
3. Watch earnings INCREASE:
   - Daily Validations: 446 → ~895
   - Annual Profit: $2,645 → ~$5,310
   - ROI: 8.80% → ~17.70%

**Key Insight:** Smaller network = less competition = higher per-node earnings!

**Decision:** Bear markets might hurt price, but fewer validators means more validations for you.

---

### 8. EVLS Penalty Analysis
**Scenario:** "I want to run 150 nodes. What's the EVLS impact?"

**How to use:**
1. Find the 150-node row in Multi-Node table
2. Check EVLS columns:
   - EVLS Penalty: 24.21%
   - EVLS Loss: $794/year (compared to no penalty)
3. Compare to 90 nodes:
   - 90 nodes profit: $2,652/year
   - 150 nodes profit: $3,155/year
   - Difference: +$503/year but 24% less efficient

**Decision:** 150 nodes makes more total profit but lower ROI (7.01% vs 9.80%). Better to run two separate 75-node validators on different wallets!

---

### 9. Budget Planning
**Scenario:** "I have $9,000 to invest. What's my best strategy?"

**How to use:**
1. Check investment needed:
   - At $0.10: 1,800 MNW × $0.10 = $180 per node
   - Budget: $9,000 ÷ $180 = 50 nodes possible
2. Look at 50-node config (leave buffer):
   - Investment: 50 × $180 = $9,000
   - Annual Profit: $614
   - ROI: 9.01%
3. VPS cost: $72/year (minimal)

**Decision:** Run 50 nodes, costs ~$97k, gives 9.01% ROI.

---

### 10. Break-Even Analysis
**Scenario:** "What price do I need for my 100 nodes to break even?"

**How to use:**
1. Enter 100 in "My Nodes Calculator"
2. Lower **"Current Price"** gradually
3. Watch "Annual Profit" field
4. Find price where profit = $0
5. Default shows: Break-even ~$0.044

**Decision:** As long as MNW stays above $0.044, your 100-node validator is profitable (before considering token price appreciation).

---

## 🎛️ Key Controls Explained

### Daily Validations
- **What it is:** Total network validations per day
- **Default:** 17,900 (6-month average from actual data)
- **Use:** Model different network activity levels
- **Effect:** Higher = more validations for everyone

### Current Price
- **What it is:** MNW token price in USD
- **Default:** $0.10 (recent market price)
- **Use:** Model bull/bear scenarios
- **Effect:** Directly scales USD profits and ROI

### Active Nodes (My Nodes Calculator)
- **What it is:** Total nodes in the network
- **Default:** 4,339 (current network size)
- **Use:** Model network growth/decline
- **Effect:** More nodes = less per-node share (inverse)

### My Nodes Input
- **What it is:** How many nodes YOU want to run
- **Use:** Calculate your specific economics
- **Effect:** Shows your daily validations, profit, ROI

---

## 💡 Understanding the Colors

### 🟢 Green Rows (⭐ OPTIMAL)
- **Meaning:** Highest ROI configuration(s)
- **Dynamic:** Changes based on your settings
- **Action:** Consider these configurations for best returns

### 🟡 Yellow Rows
- **Meaning:** EVLS penalty active but manageable (100-150 nodes)
- **Action:** Still profitable but less efficient

### 🟠 Orange Rows
- **Meaning:** Higher EVLS penalties (151-499 nodes)
- **Action:** Significant efficiency loss, consider splitting

### 🔴 Red Rows (🚨)
- **Meaning:** Severe EVLS penalties (500+ nodes)
- **Action:** Avoid unless you have specific reasons

---

## 📈 Pro Tips

### Tip 1: Sweet Spot is Usually 80-99 Nodes
- Zero EVLS penalty
- Same cheap VPS ($72/year)
- Maximum returns before cliff at 100

### Tip 2: Never Go Above 100 on One Wallet
- EVLS penalty kicks in immediately
- ROI drops significantly
- Better to run multiple separate validators

### Tip 3: Model Realistic Network Growth
- Suite.Supply will likely add 3,000-5,000 nodes
- Adjust "Active Nodes" to see impact
- Plan for lower per-node earnings

### Tip 4: Price Matters More Than Validations
- 2× price = 2× profit (same ROI %)
- 2× validations = 2× profit (same ROI %)
- But price is independent, validations are shared

### Tip 5: Use My Nodes Calculator
- Quick way to see YOUR specific economics
- Updates in real-time as you adjust settings
- Compare against Multi-Node table

---

## 🎯 Quick Start Guide

**New to Trust.Supply?**
1. Open dashboard at default settings
2. Look for GREEN rows ⭐
3. See: "90 nodes = 9.80% ROI"
4. Check profit: ~$2,650/year
5. Decide if that works for you

**Already running validators?**
1. Enter your node count in "My Nodes Calculator"
2. See your current economics
3. Compare to green optimal configs
4. Consider optimizing if significantly different

**Planning for future?**
1. Adjust "Active Nodes" for network growth
2. Adjust "Current Price" for price targets
3. See how your economics change
4. Make informed decisions

---

## ❓ Common Questions

### Q: Why is 90 nodes almost always optimal?
**A:** It's the highest node count before EVLS penalty (starts at 100). More nodes = more total profit with same VPS cost = better ROI.

### Q: Should I run 100 nodes or split to 2×50?
**A:** Split! 2×50 nodes = 0% EVLS penalty. 1×100 nodes = 10.26% EVLS penalty. Total earnings are higher when split.

### Q: What if I can't afford 90 nodes?
**A:** Any config <100 nodes is excellent! 50, 60, 70, 75, 80 all have 0% EVLS. ROI difference is small (9.59% to 9.80%).

### Q: How accurate are these calculations?
**A:** Very accurate. Based on real validator data from 20 validators over 6 months. Baseline of 4.9662 val/node/day matches actual performance.

### Q: Should I plan for network growth?
**A:** Yes! Use "Active Nodes" slider. Suite.Supply will likely double network size. Your per-node earnings may drop 30-50% unless Daily Validations also increase.

### Q: Is token yield different from ROI?
**A:** Yes! Token Yield = MNW earned vs MNW staked (independent of price). ROI = USD profit vs USD investment (includes price). Both matter!

---

## 🎉 Ready to Use!

Load the dashboard, adjust settings to match your scenario, and look for the green optimal configurations.

**The dashboard adapts to show you the BEST strategy for YOUR specific situation.**

Good luck with your validator journey! 🚀

---

**Dashboard Version:** 5.7 Dynamic  
**Last Updated:** January 17, 2026  
**Created by:** @trippledutch (community tool)
