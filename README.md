# Unsupervised & Reinforcement Learning Practical

A two-part AI/ML practical exploring **Unsupervised Learning (K-Means Clustering)** and **Reinforcement Learning fundamentals**, each grounded in a simple business scenario. Built as a Google Colab notebook for coursework, this project introduces customer segmentation and the agent-action-reward framework without requiring students to memorize the underlying math.

## Learning Objectives

- Understand customer segmentation using K-Means Clustering.
- Observe how similar customers are grouped together based on behavior.
- Interpret clusters from a business point of view.
- Understand the basic idea of Reinforcement Learning.
- Identify Agent, Action, and Reward using a simple example.
- Distinguish between Exploration and Exploitation.

## Part A: Customer Segmentation Using K-Means

**Business Problem:** An online retailer wants to understand different types of customers based on two behavioral signals — Monthly Spending and App Visits — and group them into meaningful segments.

**What the notebook does:**
1. Builds a small sample customer dataset (8 customers, `Monthly_Spending`, `App_Visits`).
2. Selects the relevant numeric features for clustering.
3. Applies **K-Means Clustering** with `K = 3` to group customers.
4. Visualizes the resulting clusters on a scatter plot.
5. Walks through a **business interpretation activity** — naming each cluster (e.g., "Premium Customers", "Medium-Value Customers", "Low-Engagement Customers") and proposing a business action (loyalty rewards, personalized recommendations, re-engagement campaigns).

## Part B: Introduction to Reinforcement Learning

**Business Scenario:** A delivery company must choose between two routes (Route A and Route B) to consistently achieve faster deliveries.

**What the notebook does:**
1. Defines example reward sequences for each route.
2. Calculates the **average reward** per route to simulate a learning signal.
3. Introduces the core RL vocabulary in context:
   - **Agent:** Delivery decision system
   - **Environment:** Roads and traffic
   - **Action:** Choose Route A or Route B
   - **Reward:** Feedback based on delivery performance
4. Demonstrates **Exploration** (randomly trying a route) vs. **Exploitation** (choosing the route with the best known average reward) with runnable code examples.
5. Closes with a comparison table contrasting Supervised, Unsupervised, and Reinforcement Learning, plus a written reflection section.

## Tech Stack

- Python 3
- pandas
- matplotlib
- scikit-learn (`KMeans`)
- Google Colab (recommended environment)

## Getting Started

1. Open `Unsupervised_and_Reinforcement_Learning.ipynb` in Google Colab or Jupyter.
2. Run the cells sequentially — Part A (clustering) first, then Part B (reinforcement learning).
3. Complete the in-notebook business interpretation activity and reflection questions.
4. Save a screenshot of the customer-segmentation graph for submission.

## Repository Structure

```
├── Unsupervised_and_Reinforcement_Learning.ipynb   # Main practical notebook
├── README.md                                       # Project documentation
└── part-a/unsupervised-learning/                   # (suggested folder for submission assets, e.g. screenshots)
```

## Key Takeaways

- Unsupervised learning finds hidden patterns in data without labeled outcomes — useful for segmentation.
- K-Means groups similar data points into `K` clusters based on feature similarity; cluster numbers are arbitrary labels, not rankings.
- Reinforcement Learning learns through interaction: an agent takes actions in an environment and receives rewards.
- Balancing exploration (trying new options) and exploitation (using known-good options) is central to RL decision-making.
- Supervised, unsupervised, and reinforcement learning each suit different business problems — churn prediction, segmentation, and route/process optimization, respectively.

## License

This project is intended for educational purposes as part of an AI/ML coursework practical.
