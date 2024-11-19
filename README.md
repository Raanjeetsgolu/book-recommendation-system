# book recommendation system

## Overview

The **Book Recommendation System** is an AI-driven project designed to provide personalized book suggestions to users based on other user's  ratings. This system utilizes collaborative filtering techniques to analyze user behavior and recommend relevant books, helping users discover new titles that match their interests.

## Features

- **Personalized Recommendations**: Users receive tailored book suggestions based on their ratings and the preferences of similar users.
- **Popular Books List**: The system can display a list of the top 50 popular books, allowing users to explore trending titles.
- **User Queries**: Users can query any book, and the system will respond with relevant recommendations.

## Installation and Usage Instructions

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

4. Access the application in your browser at `http://127.0.0.1:5000`.

## Usage

- **Input**: Enter the name of a book you like.
- **Output**: The system returns a list of similar book recommendations based on collaborative filtering.

## 🐳 Run with Docker

***By pulling the Docker image of this app from Docker Hub.***
```bash
docker run -td -p 5000:5000 --name book-recommendation-app  raanjeetsgolu/book-recommendation-app:3.0-1
```
***By creating a Docker image locally***

1.**Build the Docker image**:
```bash
docker build -t book-recommendation-system .
  ```
2.**Run the Docker container**:
   ```bash
   docker run -p 5000:5000 book-recommendation-system
   ```
3.**Access the application**:
 Open your browser and navigate to http://127.0.0.1:5000.

This will start the application inside a Docker container and make it accessible on your local machine at port 5000.

## 🛠 Technologies

+ Python 3.10
+ Flask (for the web server)
+ Pandas, Numpy (for data processing)
+ Scikit-Learn (for similarity computation)
+ Docker (for containerization)
