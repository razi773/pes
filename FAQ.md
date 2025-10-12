# FAQ - Energy Utopia Challenge

## Frequently Asked Questions

---

## 📋 General Questions

### Q1: Who can participate in this challenge?
**A:** Only IEEE Student Branch (SB) members can participate. Each Student Branch can send one team of maximum 5 members.

### Q2: Can I participate individually or do I need a team?
**A:** You can participate individually or as part of a team (up to 5 members). However, having a full team with diverse skills (data science, programming, domain knowledge) is recommended.

### Q3: What if my Student Branch wants to send multiple teams?
**A:** Only one team per Student Branch is allowed according to the rules.

### Q4: Do all team members need to be from the same Student Branch?
**A:** Yes, all team members must be from the same IEEE Student Branch.

---

## 🎯 Topic Selection

### Q5: Can I work on multiple topics?
**A:** No, you must choose ONE topic from the four available options and focus your solution on that specific area.

### Q6: How do I choose the best topic for my team?
**A:** Consider:
- **Data availability**: Which topic has data you can easily access?
- **Team expertise**: What skills does your team have?
- **Interest**: Which problem excites your team most?
- **Impact**: Where can you make the biggest difference?

### Q7: Can I combine multiple topics?
**A:** While your main focus should be on one topic, you can mention how your solution could extend to other areas. However, your primary deliverables should address one specific topic.

### Q8: What if I change my mind about the topic after Phase 1?
**A:** It's best to stick with your chosen topic, as changing it would require redoing most of your work. Choose carefully in the beginning.

---

## 📊 Data Requirements

### Q9: Where can I find data for my project?
**A:** Several sources:
- **Public datasets**: Kaggle, UCI Machine Learning Repository, government open data portals
- **APIs**: Weather APIs (OpenWeatherMap), energy APIs
- **Web scraping**: Energy company websites, utility data
- **Simulation**: Generate realistic synthetic data
- **Research papers**: Many include datasets or links

### Q10: Can I use synthetic/simulated data?
**A:** Yes! The rules explicitly state you can generate realistic scenarios. Just make sure to document your simulation methodology clearly.

### Q11: How much data do I need?
**A:** There's no specific requirement, but you need enough data to:
- Train your AI model effectively
- Validate your results
- Demonstrate meaningful insights
Typically, thousands of data points for time-series tasks, or enough examples for classification tasks.

### Q12: Do I need to share my data publicly?
**A:** You should include your data (or a sample) in your GitHub repository, or provide clear instructions on how to obtain it. If using proprietary data, provide sample data or synthetic alternatives.

### Q13: Can I use proprietary/confidential data?
**A:** You can use it for development, but your final submission should be reproducible by others. Consider using anonymized versions or synthetic alternatives for your public repository.

---

## 💻 Technical Questions

### Q14: What programming languages can I use?
**A:** Any programming language is acceptable, but Python is recommended due to its extensive AI/ML libraries and ecosystem.

### Q15: What tools and frameworks should I use?
**A:** Common choices include:
- **Languages**: Python, R, Julia
- **ML Libraries**: scikit-learn, TensorFlow, PyTorch, XGBoost
- **Time Series**: statsmodels, Prophet, LSTM
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn, plotly
- **Deployment**: Flask, Streamlit, FastAPI, Docker

### Q16: Do I need to deploy my solution to the cloud?
**A:** Not required for Phase 1. For Phase 2, you should have a working demo (can be local), but cloud deployment is impressive and may earn extra points.

### Q17: What evaluation metrics should I use?
**A:** Depends on your topic:
- **Forecasting**: MAE, RMSE, MAPE, R²
- **Classification** (anomaly/maintenance): Precision, Recall, F1-score, ROC-AUC
- **Business**: Cost savings, efficiency improvements, energy reduction

### Q18: How complex should my model be?
**A:** Focus on effectiveness, not complexity. A simple model that works well is better than a complex model that doesn't. Document why you chose your approach.

---

## 📝 Deliverables

### Q19: What should be included in the Phase 1 proposal report?
**A:** Your report should include:
1. Topic selection and justification
2. Problem statement
3. Objectives and expected impact
4. Data sources and collection plan
5. Preliminary AI approach
6. Timeline for Phase 2

Length: 5-10 pages is typical, but quality matters more than length.

### Q20: How detailed should my Phase 1 code be?
**A:** Phase 1 should show:
- Data collection/generation code
- Exploratory data analysis
- Data preprocessing
- Initial model experiments
It doesn't need to be perfect, but should demonstrate progress.

### Q21: What format should my reports be in?
**A:** PDF is standard and recommended. Ensure it's well-formatted, readable, and professional.

### Q22: How long should the demo video be?
**A:** Keep it concise - aim for 3-5 minutes. Show your solution working, highlight key features, and demonstrate impact.

### Q23: What should I include in my 5-minute presentation?
**A:** Cover:
- Problem overview (30 sec)
- Your approach (1 min)
- Data and model (1.5 min)
- Results and impact (1.5 min)
- Conclusion (30 sec)
Practice to stay within 5 minutes!

---

## 🎨 Anonymity Requirements

### Q24: Why must my submission be anonymous?
**A:** To ensure fair evaluation without bias toward any specific institution or team.

### Q25: What needs to be anonymous?
**A:** Everything:
- GitHub repository (no names, no university names)
- Code comments (no author names)
- Reports (no names, affiliations)
- Demo video (no faces, names, or institutional logos)
- Presentation (refer to yourselves as "the team")

### Q26: Can I use my personal GitHub account?
**A:** Yes, but make sure the repository name and README don't reveal your identity. Consider using a generic name like "energy-utopia-project".

### Q27: How do I handle commits without revealing identity?
**A:** Configure git with anonymous credentials:
```bash
git config user.name "Anonymous Team"
git config user.email "team@anonymous.local"
```

---

## 🏆 Scoring & Evaluation

### Q28: How exactly is the scoring done?
**A:** 
- **Phase 1 (50 pts)**: Requirements adherence (15), Technical approach (19), Quality (8), Innovation (8)
- **Phase 2 (45 pts)**: Technical approach (20), Prototype (10), Presentation (5), Quality (10)
- **Bonus (5 pts)**: PES/YP membership, business analysis

### Q29: What makes a technically strong approach?
**A:** 
- Appropriate methodology for the problem
- Well-justified choices
- Proper validation
- Clear evaluation metrics
- Good documentation

### Q30: What is the "business scope" bonus?
**A:** Document the business case:
- Implementation costs
- Production/deployment costs
- Training costs (for models)
- Maintenance costs
- Expected ROI or savings

### Q31: How important is innovation vs. execution?
**A:** Both matter! Innovation is 8 points in Phase 1, but technical execution is 19 points. A well-executed standard approach can score higher than a poorly-executed innovative one.

---

## 🔧 GitHub & Submission

### Q32: Should my GitHub repository be public or private?
**A:** Public is recommended for visibility, but make sure it's anonymous. Private is acceptable if you prefer.

### Q33: Can I use Kaggle instead of GitHub?
**A:** The rules mention "GitHub repository and/or Kaggle notebook", so either is acceptable, or you can use both.

### Q34: What should my repository structure look like?
**A:** See PROJECT_TEMPLATE.md for a recommended structure. Key folders: data/, notebooks/, src/, models/, results/

### Q35: Where do I submit my deliverables?
**A:** Via the official submission link provided in the challenge (check the PDF or contact organizers for the exact link).

### Q36: Can I update my repository after the deadline?
**A:** The version at the deadline is what will be evaluated. Later updates won't be considered, so submit on time!

---

## ⏰ Deadlines & Timeline

### Q37: What timezone are the deadlines in?
**A:** GMT+1 (Central European Time - Tunisia time zone)

### Q38: Is there a grace period after the deadline?
**A:** This is not specified, so assume NO grace period. Submit early to avoid last-minute technical issues!

### Q39: What if I miss the Phase 1 deadline?
**A:** You likely won't be able to continue to Phase 2, as Phase 1 is the pre-selection phase.

### Q40: Can I submit Phase 1 early?
**A:** Yes! Submit as soon as you're ready. This gives you more time for Phase 2.

---

## 👥 Team & Membership

### Q41: What is the difference between PES and YP members?
**A:** 
- **PES**: Power and Energy Society - focused on energy domain
- **YP**: Young Professionals - for recent graduates and young professionals
You can be a member of one, both, or neither.

### Q42: How do I get bonus points for membership?
**A:** 
- Have at least one PES member: +1 point
- Have at least one YP member: +1 point  
- Have at least one member who is both YP and PES: +1 point
Maximum membership bonus: 3 points (not 5 as they're not all additive)

### Q43: Do I need to prove membership?
**A:** The submission rules don't specify, but be honest as this may be verified.

### Q44: Can members join IEEE PES or YP during the challenge?
**A:** Probably yes, but confirm with organizers. It's best to have memberships before the final submission.

---

## 🎓 Learning & Resources

### Q45: I'm new to AI/ML. Can I still participate?
**A:** Yes! This is a learning opportunity. Use online courses (Coursera, fast.ai), tutorials, and documentation. Partner with teammates who have more experience.

### Q46: What if I don't understand the technical hints in the PDF?
**A:** Research each term:
- **ARIMA, Prophet**: Time series forecasting models
- **LSTM, Transformers**: Deep learning for sequences
- **Isolation Forest, Autoencoders**: Anomaly detection
- **Survival analysis**: Predicting time-to-event
Start with scikit-learn documentation and tutorials.

### Q47: Where can I learn about energy systems?
**A:** Resources:
- IEEE PES publications
- Online courses on renewable energy
- Energy datasets often include documentation
- YouTube tutorials on energy systems

### Q48: Are there any example projects I can reference?
**A:** Search for:
- "Energy consumption prediction Kaggle"
- "Battery health prediction GitHub"
- "Solar forecasting machine learning"
- "Predictive maintenance tutorial"
But make sure your work is original!

---

## 🤝 Collaboration & Ethics

### Q49: Can we collaborate with other teams?
**A:** You can discuss general ideas, but your work must be original. Don't copy code or share datasets exclusively.

### Q50: Can I use code from online tutorials or GitHub?
**A:** Yes, but:
- Cite your sources
- Understand the code you use
- Make significant modifications
- Don't copy entire projects

### Q51: What if I find my exact problem already solved online?
**A:** That's fine! Learn from it, but create your own implementation with improvements, different data, or novel approaches.

### Q52: Can I use pre-trained models?
**A:** Yes, transfer learning is acceptable (e.g., using BERT, ResNet). Document which parts are pre-trained vs. your contribution.

---

## 🏥 Troubleshooting

### Q53: What if I can't find good data?
**A:** Options:
1. Simulate realistic data (document your methodology)
2. Try a different topic with better data availability
3. Combine multiple smaller datasets
4. Reach out to local utilities or companies (though this takes time)

### Q54: My model performance is poor. What should I do?
**A:** 
1. Check your data quality (missing values, outliers)
2. Try simpler models first (baseline)
3. Ensure proper train/test split
4. Consider more features or better feature engineering
5. Check for data leakage
6. Document your experiments - even "failed" attempts show good process

### Q55: I'm running out of time. What should I prioritize?
**A:** Priority order:
1. Get a working end-to-end solution (even if simple)
2. Document your process well
3. Create a clear demo
4. Make deliverables anonymous
5. Submit on time
Quality matters more than sophistication!

---

## 📞 Contact & Support

### Q56: Who do I contact for questions?
**A:** 
- Email: pes@ieee.tn
- Email: yp@ieee.tn
- Attend the info session: September 24, 2025

### Q57: How quickly will my questions be answered?
**A:** Allow a few business days for responses. Ask questions early, not right before deadlines!

### Q58: Can I get feedback on my Phase 1 submission before Phase 2?
**A:** This isn't specified, but you'll likely get your Phase 1 score which indicates areas to improve.

---

## 🎯 Success Tips

### Q59: What are the most common mistakes teams make?
**A:**
1. Choosing a topic without checking data availability
2. Starting too late
3. Forgetting to make submissions anonymous
4. Poor documentation
5. Over-complexity without validation
6. Missing the deadline

### Q60: What makes a winning team?
**A:** 
- **Clear problem focus**: Well-defined scope
- **Solid technical approach**: Appropriate methods, good validation
- **Strong execution**: Working solution with clear results
- **Excellent documentation**: Easy to understand and reproduce
- **Professional presentation**: Clear, concise, impactful
- **Innovation**: Novel approach or unique insights
- **Impact**: Demonstrates real-world value

---

## 🌟 Final Advice

### Q61: Any last tips for success?
**A:**
1. **Start early** - Don't underestimate data collection time
2. **Document everything** - Future you will thank present you
3. **Focus on one thing well** - Better than many things poorly
4. **Test early and often** - Don't wait until the deadline
5. **Ask for help** - Use the info session and email contacts
6. **Stay organized** - Use version control, organize your files
7. **Communicate as a team** - Regular meetings and clear task division
8. **Have fun!** - This is a learning opportunity

### Q62: What if I don't win?
**A:** Participating is valuable! You'll:
- Learn practical AI/ML skills
- Gain experience with real-world problems
- Build your portfolio
- Network with peers
- Potentially publish or present your work elsewhere

The experience and learning are worth it regardless of the outcome!

---

## 📚 Additional Resources

**Documentation in this repository:**
- `README.md` - Complete challenge details (English)
- `README.fr.md` - Documentation complète (Français)
- `QUICK_REFERENCE.md` - Quick checklist and deadlines
- `PROJECT_TEMPLATE.md` - Code structure and templates
- `TIMELINE_WORKFLOW.md` - Visual timeline and workflow
- `PES & YP Challenge.pdf` - Original challenge document

**External resources:**
- [Kaggle Datasets](https://www.kaggle.com/datasets) - Find energy-related data
- [UCI ML Repository](https://archive.ics.uci.edu/ml/index.php) - Classic ML datasets
- [scikit-learn](https://scikit-learn.org/) - ML library documentation
- [TensorFlow](https://www.tensorflow.org/) - Deep learning framework
- [PyTorch](https://pytorch.org/) - Deep learning framework

---

**Good luck with the Energy Utopia Challenge! 🌟⚡🌍**

*This FAQ is maintained as part of the challenge documentation. If you have questions not covered here, please contact the organizers.*
