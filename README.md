# book recommendation system

## Overview

The **Book Recommendation System** is an AI-driven application that offers personalized book suggestions by analyzing user ratings through collaborative filtering. It helps users discover new titles based on their interests and popular trends in the community.

## Features

- **Personalized Recommendations**: Users receive tailored book suggestions based on their ratings and the preferences of similar users.
- **Popular Books List**: The system can display a list of the top 50 popular books, allowing users to explore trending titles.

## Installation and Usage 

To set up the Book Recommendation System locally, follow these steps:

1. **Clone the Repository**:
```bash
 git clone https://github.com/Raanjeetsgolu/book-recommendation-system.git
 cd book-recommendation-system
```

2. **Install Dependencies**:
Make sure you have Python installed, then install the required packages:

```bash
pip install -r requirements.txt
```
3. **Run the Flask application**:
```bash
python3 app.py
```

4. Access the App: Open your browser and navigate to `http://127.0.0.1:5000`.

## 🐳 Docker setup


**Option 1: Pull from Docker Hub**

```bash
docker run -td -p 5000:5000 --name book-recommendation-app  raanjeetsgolu/book-recommendation-app:3.0-1
```
Access the application: Open your browser and navigate to `http://127.0.0.1:5000`.

**Option 2: Build Locally**


1.***Build the Docker image***:

```bash
docker build -t book-recommendation-app .
  ```
2.***Run the Docker container***:
   ```bash
docker run -td -p 5000:5000 --name book-recommendation-app  book-recommendation-app
   ```
3.***Access the application***:
 Open your browser and navigate to http://127.0.0.1:5000

## 🛠 Technologies

+ Python 3.10
+ Flask (for the web server)
+ Pandas, Numpy (for data processing)
+ Scikit-Learn (for similarity computation)
+ Docker (for containerization)
+ pickle (for dumping and loading the model)
