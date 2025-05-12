# Smart Movie Recommender System

This is a **real-time movie recommender system** based on **collaborative filtering** using only **Pandas**. It also includes a **search engine functionality** built using **TF-IDF** and **cosine similarity** to help users find the movie they want recommendations for. The backend is implemented using **FastAPI**, and the frontend is a static HTML/CSS/JavaScript interface.

<p align="center">
  <img src="./documentation/move%20recommender%201.png" alt="UI Screenshot" width="600"/>
</p>

---

## Features

* Collaborative Filtering using only `pandas`
* Real-time recommendations
* Search functionality using TF-IDF and cosine similarity
* FastAPI backend
* Lightweight frontend using HTML, CSS, and JS
* Optimized for quick querying

---

## Installation Guide

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd <your-repo-name>
```

### 2. Install dependencies

Make sure you have Python 3.7+

```bash
pip install -r requirements.txt
```

### 3. Download the dataset

This step is required only for the first time to set up the environment.

```bash
python dataset_loader.py
```

This will download and prepare a \~600MB movies and ratings dataset needed by the system.

---

## Running the Application

### 1. Start the FastAPI backend

```bash
python main.py
```

The FastAPI server will start and be accessible at `http://localhost:5000`

### 2. Open the frontend

Open the following file in your browser:

```
client/app.html
```

This will open a simple user interface where you can:

* Search for your favorite movie
* Get real-time recommendations instantly

---

## Screenshot

![UI Screenshot](./documentation/move%20recommender%202.png)

---

## Folder Structure

```
├── client/
│   └── app.html           # Frontend UI
├── dataset_loader.py      # Script to download and setup the dataset
├── main.py                # FastAPI backend server
├── requirements.txt       # Python dependencies
└── README.md              # This guide
```

---

## Notes

* Real-time recommendations are computed on the fly when the user searches for a movie.
* Make sure to run `dataset_loader.py` before starting the server.
* FastAPI must be running for the HTML frontend to communicate with the backend.

---

Happy recommending! 🍿
