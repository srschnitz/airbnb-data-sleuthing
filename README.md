# airbnb-data-sleuthing
An exploratory dive into Airbnb data; flagging anomalies, clustering property types, and uncovering booking behaviors with Power BI and Python. This project reflects my commitment to continuous learning, collaborative growth, and building transparent, asset-driven analytics for real-world impact.
From Castles to Caves: Airbnb Data Diagnostics
Welcome to my exploratory dive into Airbnb data. This project flags pricing anomalies, clusters property types, and uncovers booking behaviors using Power BI and Python. It’s part of my journey to deepen my analytics skills, share insights, and connect with others in the data community.

Adding updated notebook - Airbnb Dynamic Pricing Model (Python · XGBoost · Optuna)

**R² 0.783 | RMSE 0.354** on hold-out test set — **100% leakage-free validation**

### Key Features Engineered
- Train-only target encoding of `neighbourhood_cleansed`
- Per-person ratios (bedrooms, bathrooms, amenities per guest)
- Superhost × review score interaction
- Strict train/test separation (no data leakage)

### Results
| Model                     | R²     | RMSE   | Notes                     |
|---------------------------|--------|--------|---------------------------|
| Linear baseline           | 0.55   | 0.53   |                           |
| XGBoost (leaked encoding) | ~0.91  | —      | Invalid — used test data  |
| XGBoost (this repo)       | **0.783** | **0.354** | Production-ready       |

