# Thompson-Sampling-Algorithm-Implementation-Python-

# Thompson Sampling for Online Ads Optimization

This project demonstrates the use of **Thompson Sampling**, a reinforcement learning algorithm, to solve the *Multi-Armed Bandit Problem* for online advertisement selection.  

The algorithm dynamically chooses ads to maximize the click-through rate (CTR) by balancing **exploration** (trying different ads) and **exploitation** (focusing on the best-performing ads).

---

## 📌 Project Overview
- **Dataset**: `Ads_CTR_Optimisation.csv`  
  Contains simulated click-through data for 10 different ads.  
- **Algorithm Used**: Thompson Sampling (Bayesian Approach).  
- **Goal**: Identify the ad with the highest probability of user clicks while minimizing wasted impressions.  

---

## ⚙️ How It Works
1. At each round, the algorithm:
   - Samples from a Beta distribution for each ad.
   - Selects the ad with the highest sampled value.
   - Updates success/failure counts based on whether the ad was clicked.
2. Over time, it converges to selecting the best-performing ad most frequently.  

---

## 📊 Visualization
The code plots a histogram showing how many times each ad was selected during the simulation:

📈 Results

The histogram shows which ad is most effective.

The algorithm learns to select the best ad more often as rounds increase.

Total reward indicates the number of successful ad clicks.

🔮 Future Improvements

Compare with Upper Confidence Bound (UCB) algorithm.

Apply to real-world ad click datasets.

Extend to large-scale bandit problems with many ads.
