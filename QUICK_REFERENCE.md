# Quick Reference Guide - Energy Utopia Challenge

## 🎯 What You Need to Know

### Challenge in One Sentence
Develop an AI solution for one of four energy-related problems: consumption optimization, storage management, renewable energy forecasting, or predictive maintenance.

---

## ⏰ Critical Dates

| Date | Event | What to Submit |
|------|-------|----------------|
| **Sep 24, 2025** | Info Session | Attend to ask questions |
| **Oct 20, 2025** | Phase 1 Deadline | Project proposal + GitHub repo with initial code |
| **Dec 19, 2025** | Phase 2 Deadline | Complete solution + demo video + presentation |

---

## ✅ Phase 1 Checklist (Due: Oct 20, 2025)

- [ ] Choose one of the four topics
- [ ] Write project proposal report covering:
  - [ ] Chosen topic and objectives
  - [ ] Expected impact
  - [ ] Data sources identified
  - [ ] AI model approach planned
- [ ] Create GitHub repository with:
  - [ ] Dataset (collected or generated)
  - [ ] Data collection scripts
  - [ ] Preprocessing code
  - [ ] Exploratory analysis notebooks
  - [ ] Initial model experiments
- [ ] Ensure repository is **anonymous** (no names/affiliations)
- [ ] Submit via the official link

**Score: 50 points**

---

## ✅ Phase 2 Checklist (Due: Dec 19, 2025)

- [ ] Complete full project report documenting:
  - [ ] Complete workflow
  - [ ] Data preparation details
  - [ ] Model training and evaluation
  - [ ] Deployment approach
  - [ ] Additional features
- [ ] Update GitHub repository with:
  - [ ] Full solution code
  - [ ] Trained models
  - [ ] Application/deployment files
  - [ ] Clear README with setup instructions
- [ ] Create demo video showing:
  - [ ] Working solution
  - [ ] Key functionalities
  - [ ] Results and impact
- [ ] Prepare 5-minute presentation in English
- [ ] Ensure all deliverables remain **anonymous**
- [ ] Submit via the official link

**Score: 45 points**

---

## 🎨 Four Topic Options (Choose ONE)

### 1. Energy Consumption Optimization 🏢
- Detect anomalies in usage
- Predict future demand
- Recommend load shifting

**Example datasets:** Smart meter data, building energy data

### 2. Energy Storage Management 🔋
- Forecast battery life
- Optimize charge/discharge
- Detect degradation

**Example datasets:** Battery performance data, charge cycles

### 3. Renewable Energy Forecasting ☀️
- Predict solar/wind production
- Detect production gaps
- Plan storage usage

**Example datasets:** Weather data, solar/wind production data

### 4. Predictive Maintenance ⚙️
- Detect sensor anomalies
- Predict equipment failures
- Support technician decisions

**Example datasets:** Equipment sensor data, failure logs

---

## 💡 Technical Approach Tips

### Step 1: Data Collection
- Public datasets (Kaggle, UCI, government portals)
- APIs (weather APIs, energy APIs)
- Web scraping (energy companies, utilities)
- Simulation (generate realistic scenarios)

### Step 2: Data Preparation
- Handle missing values
- Detect and remove anomalies
- Normalize/standardize
- Feature engineering (rolling averages, trends)

### Step 3: Model Selection

**For forecasting:**
- ARIMA, Prophet
- LSTM, GRU
- Transformers (for complex patterns)

**For anomaly detection:**
- Isolation Forest
- Autoencoders
- One-Class SVM

**For maintenance:**
- Random Forest, XGBoost
- Survival analysis
- LLMs for decision support

### Step 4: Evaluation
- Define clear metrics (MAE, RMSE, F1, Precision, Recall)
- Calculate cost savings potential
- Test on unseen data

---

## 📊 Scoring Breakdown

### Phase 1: Pre-selection (50 points)
- Requirements adherence: 15 pts
- Technical approach: 19 pts
- Deliverable quality: 8 pts
- Innovation: 8 pts

### Phase 2: Final (45 points)
- Technical approach: 20 pts
- Prototype functionality: 10 pts
- Presentation: 5 pts
- Deliverable quality: 10 pts

### Bonus (5 points)
- PES member: +1 pt
- YP member: +1 pt
- YP with PES membership: +1 pt
- Business analysis: +2 pts

**Total possible: 100 points**

---

## 🚫 Common Mistakes to Avoid

1. ❌ Not making deliverables anonymous
2. ❌ Choosing multiple topics instead of one
3. ❌ Submitting after deadline
4. ❌ Not including all required deliverables
5. ❌ Poor documentation in GitHub repository
6. ❌ Presentation not in English
7. ❌ Exceeding 5-minute presentation time
8. ❌ Not defining clear evaluation metrics

---

## 📋 Team Requirements

- **Eligibility:** IEEE Student Branch members only
- **Team size:** Max 5 members
- **Teams per SB:** 1 team per Student Branch
- **Language:** Presentations must be in English

---

## 🎯 Success Factors

### Strong proposals include:
- Clear problem definition
- Well-justified topic choice
- Realistic data sources
- Appropriate AI techniques
- Clear evaluation plan
- Innovative approach

### Strong final solutions include:
- Clean, documented code
- Reproducible results
- Working demo
- Impact quantification
- Professional presentation
- Business considerations (bonus)

---

## 📁 Recommended Repository Structure

```
your-project/
├── README.md                    # Project overview
├── requirements.txt             # Dependencies
├── data/
│   ├── raw/                    # Original data
│   ├── processed/              # Cleaned data
│   └── README.md               # Data sources documentation
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_modeling.ipynb
├── src/
│   ├── data/                   # Data processing scripts
│   ├── models/                 # Model definitions
│   ├── training/               # Training scripts
│   └── inference/              # Prediction scripts
├── models/                      # Saved trained models
├── results/                     # Outputs, plots, metrics
├── deployment/                  # Deployment code
│   ├── app.py                  # Application
│   └── Dockerfile              # Containerization
├── reports/
│   ├── proposal.pdf            # Phase 1 report
│   └── final_report.pdf        # Phase 2 report
└── presentation/
    └── slides.pdf              # Final presentation
```

---

## 📞 Get Help

**Questions?** Contact:
- pes@ieee.tn
- yp@ieee.tn

**Resources:**
- Info Session: September 24, 2025
- This README and README.fr.md for detailed information
- Original PDF: PES & YP Challenge.pdf

---

## 🏁 Getting Started NOW

1. **Form your team** (5 members max from your IEEE Student Branch)
2. **Read the full README.md** (or README.fr.md for French)
3. **Attend the info session** (Sep 24, 2025)
4. **Choose your topic** (discuss with team)
5. **Start exploring data sources** (don't wait!)
6. **Set up your GitHub repository** (make it anonymous)
7. **Begin data collection** (this takes time!)
8. **Document everything** (from day one)

**Remember:** Phase 1 is due October 20, 2025 - that's less than a month away after the info session!

Good luck! 🍀⚡🌍
