# Flight Fare Prediction

Built this from scratch because I was tired of seeing random flight prices and thought, why not make a machine try to understand this chaos?

---

## What’s this about?

Flight ticket prices are all over the place. Ever wondered why the same flight costs ₹3,000 today and ₹9,000 tomorrow? I did. So I took a raw dataset from Kaggle and decided to build a machine learning model that could predict flight fares based on features like airline, journey date, duration, number of stops, and more.

This project wasn’t about getting a perfect model — it was about learning everything in the process: from cleaning messy data to making sense of it and finally using it to make predictions that actually kinda work.

---

## How I built it 

### Step 1: Understanding the data

Started with a CSV file full of weird formats and half-cleaned text. Things like:

- "2h 45m" in the duration column
- "1 stop" as text instead of a number
- Dates mixed in with times, not even in the right format

So the first few hours? Just cleaning that mess.

### Step 2: Cleaning + Feature Engineering

- Split `Date_of_Journey` into day and month
- Converted `Dep_Time` and `Arrival_Time` into hour and minute
- Transformed `Duration` into total minutes
- Used label encoding and one-hot encoding depending on the column type
- Dropped garbage columns like "Additional_Info" that weren’t doing anything

This was the part where I realized data cleaning isn’t sexy, but it’s 70% of the work.

### Step 3: EDA (Exploratory Data Analysis)

- Compared prices across different airlines
- Checked how number of stops impacts price (spoiler: more stops = cheaper)
- Visualized relationships using boxplots, violin plots, and bar graphs

Honestly, this step helped me figure out which features actually mattered.

### Step 4: Model Building

Tried a bunch of regression models:
- Linear Regression (meh)
- Decision Tree (better)
- Random Forest Regressor (worked best)

### Step 5: Evaluation

| Model                 | R² Score | MAE      | RMSE     |
|----------------------|----------|----------|----------|
| Linear Regression     | 0.63     | ₹2,100   | ₹3,200   |
| Decision Tree         | 0.75     | ₹1,650   | ₹2,700   |
| Random Forest         | 0.82     | ₹1,300   | ₹2,100   |

The Random Forest model gave me the best results — solid R² score, low error, and consistent predictions.

---

## Tools Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## What’s next?

- Thinking of deploying this using Streamlit so it’s interactive
- Might try XGBoost or CatBoost just to compare
- Would love to connect it to real-time flight data one day using APIs

---

## Stuff I learned

- Feature engineering is everything. The better your features, the better your model.
- Datetime columns are always tricky. Always.
- Never underestimate how long data cleaning takes.
- Visualizing stuff helps. A lot.
- If you don't understand the data, your model definitely won’t.

---

## About me

Hi, I’m Tushar Suredia — a Data Analyst who loves building things that actually do something.  
This was one of my first serious attempts at applying ML to a real-world-style dataset, and honestly, I had a lot of fun figuring it out.

- GitHub: [https://github.com/twoChar]
- LinkedIn: [https://www.linkedin.com/in/twochar/]
- Gmail: [connectwith.twochar@gmail.com]

---

This project wasn’t perfect — but it was real.  
And that’s what matters.

If you read this far — thanks. And if you’re working on your own project, keep going. It’s worth it.
