# ✈️ Flight Fare Prediction — A Journey Through Data & Grit

Hey there! I'm Tushar — and this is a story of how I took a raw, messy dataset about flights and turned it into a machine learning project that can predict flight fares with surprising accuracy. This isn't just about hitting high scores on metrics — it's about learning the real, dirty, hands-on work behind an actual ML pipeline.

---

## 🔍 The Problem

Flight prices are unpredictable, right? One day it’s ₹3,000, next day it’s ₹9,000 — same destination, same airline. I thought: _"There has to be a pattern."_  
So, I built a model to **predict flight ticket prices based on details like airlines, journey time, route, stops, and duration**.

No magic, just data.

---

## 💡 My Approach (The Grit & Grind)

I didn’t just throw data at a model — I cleaned it, broke it apart, questioned every column, and slowly built something worth showing.

### 🧹 Step 1: Data Cleaning
- The dataset came with columns like "Duration" in weird formats like `2h 50m`. I wrote logic to convert that into total minutes.
- Converted date/time into day, month, hour, minute — so models could *actually* learn patterns.
- Dealt with missing values, dropped columns that added noise (bye-bye, "Additional Info").

### 📊 Step 2: EDA (Understanding the Beast)
- Checked which airlines were charging more
- Looked at the impact of number of stops on prices
- Plotted distributions, boxplots, violin plots — found gold in the patterns

### 🧱 Step 3: Feature Engineering
- Extracted duration in total minutes
- One-hot encoded airlines, sources, and destinations
- Label-encoded stops (ordinal by nature)

This was the part where I realized: **what you feed into the model is everything**. Garbage in = garbage out.

### 🤖 Step 4: Model Building
I tested:
- **Linear Regression** — baseline
- **Decision Tree** — better
- **Random Forest Regressor** — 🔥 *chef’s kiss*

### 🧪 Step 5: Model Evaluation
I didn’t stop at "It runs." I looked at:
- R² Score
- Mean Absolute Error
- RMSE

---

## 📈 Final Results (Hard-Earned, Not Copy-Pasted)

| Model                 | R² Score | MAE      | RMSE     |
|----------------------|----------|----------|----------|
| Linear Regression     | 0.63     | ₹2,100   | ₹3,200   |
| Decision Tree         | 0.75     | ₹1,650   | ₹2,700   |
| **Random Forest** ✅  | **0.82** | **₹1,300** | **₹2,100** |

🎯 **Best Model**: Random Forest Regressor  
🔥 **R² Score**: 0.82 — solid predictive power  
💸 **Mean Absolute Error**: ₹1,300 — not bad for fare prediction

---

## 🛠️ Tools I Used

- Python
- Pandas & NumPy for data wrangling
- Matplotlib & Seaborn for EDA
- Scikit-learn for ML models

---

## 🚀 What’s Next?

This project was just the beginning. I’m planning to:
- Scrape live flight data and make this model smarter
- Wrap it up in a **Streamlit web app** to show predictions live
- Try out **XGBoost, CatBoost**, and hyperparameter tuning
- Maybe deploy it with Flask or FastAPI just for fun

---

## 🤯 Things I Learned

- Feature engineering is *the real MVP* of ML
- Dates and durations are annoying — but you can tame them
- Models are dumb until you give them good data
- Debugging a Jupyter notebook at 2 AM builds character 😅

---

## 🙋‍♂️ About Me

**Tushar Suredia**  
_Data Engineer | Learner | Builder of things that (hopefully) work_  
📍 India  
[GitHub](#) | [LinkedIn](#) | [Portfolio](#)

---

> _This wasn’t just a project, it was a hands-on lesson in thinking like a machine and sweating like a human._  
> — Thanks for scrolling. Feedback, stars, and job offers welcome. 😄
