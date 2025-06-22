# 📚 Book Recommendation System

A machine learning-powered web application that recommends books to users based on their reading preferences using popularity-based filtering and collaborative filtering (item-item) techniques.

---

## 🔍 Project Description

**Situation**
With the massive growth of online platforms like Amazon, Goodreads, and Netflix, recommendation systems have become essential for personalizing user experiences. In the context of books, millions of titles make it difficult for users to discover relevant content. A system was needed to help readers find books they'll enjoy based on past data and similar user interests.

**Task**
The objective was to build a web-based Book Recommendation System that can suggest relevant books to users using both popularity metrics and collaborative filtering. The system should handle cold-start scenarios (new users or items), offer personalized suggestions, and scale efficiently with large datasets.

**Action**

* Used the **Book-Crossing dataset** containing 1.1M+ ratings from 90K+ users across 270K books.
* Performed **extensive EDA**, handled missing values, outliers, and cleaned text features like book titles and authors.
* Built a **popularity-based recommender** using weighted average ratings to solve the cold-start problem.
* Implemented **item-item collaborative filtering** using **cosine similarity** and **K-Nearest Neighbors (KNN)** to identify similar books based on user ratings.
* Developed the web interface using **Python (Flask)** and deployed the model for real-time recommendation.
* Ensured scalability by converting large sparse matrices into efficient formats using **SciPy**.

**Result**

* Achieved a functional, intuitive recommendation system that provides both **general** (popular) and **personalized** suggestions.
* Web app displays top 50 trending books and allows users to input a book title to get similar recommendations.
* Delivered reliable results for various user categories including new users (cold-start) and returning users with prior activity.

---

## Key Features

* **Hybrid Recommendation Strategy**: Combines popularity and collaborative filtering for more effective suggestions.
* **Cold Start Solution**: Popularity model suggests top books for new users with no interaction history.
* **Interactive Web App**: Built with Flask and Bootstrap for seamless user experience.
* **Real-Time Predictions**: Enter any popular book and get similar titles instantly.
* **Extensive Data Handling**: Cleaned missing values, handled skewed age distributions, and normalized data.
* **Model Deployment**: Stored models using Pickle for efficient loading during app runtime.

---

## 📁 Dataset Used

**Book-Crossing Dataset**

* [📥 Download Link](https://www.kaggle.com/datasets/somnambwl/bookcrossing-dataset)
* Contains:

  * `Books.csv` – Book metadata (title, author, year, publisher, image URLs)
  * `Users.csv` – User demographic information
  * `Ratings.csv` – Explicit and implicit book ratings (scale of 1–10)

---

## 🛠️ Technologies & Libraries

* **Languages**: Python 3.10
* **Frameworks**: Flask, Jinja2
* **Libraries**: Pandas, NumPy, SciPy, scikit-learn, Matplotlib, Seaborn, Pickle
* **Tools**: PyCharm, Jupyter Notebook, Bootstrap (for UI)

---

## 🌐 How to Run the Project

1. Clone the repository
2. Install dependencies using `pip install -r requirements.txt`
3. Run `app.py` to start the Flask server
4. Access the app at `http://localhost:5000/`

---

## 📈 Future Scope

* Integrate **content-based filtering** using genres, summaries, and keywords.
* Add **user login and preferences storage** for more personalized results.
* Deploy the app using **Heroku**, **Streamlit**, or **Docker** for easier access.
* Implement **hybrid models** combining content, collaborative, and sentiment-based approaches.

