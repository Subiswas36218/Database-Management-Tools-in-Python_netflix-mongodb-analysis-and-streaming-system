# 🎬 Netflix Database Analysis and Messaging System

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-green?style=for-the-badge&logo=mongodb)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red?style=for-the-badge)
![PyMongo](https://img.shields.io/badge/PyMongo-Database%20Driver-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-Academic-lightgrey?style=for-the-badge)

---

# 📌 Project Overview

This project was developed for the course:

## **Database Management Tools in Python | Spring 2026**

The project contains two major components:

- 📊 **Part 1:** Netflix Dataset Analysis using MongoDB Atlas
- 📡 **Part 2:** Netflix User-Activity Messaging System

The objective was to explore modern database technologies, analytical querying, NoSQL modelling, inheritance, and queue-based streaming systems using Python.

---

# 🗂️ Project Structure

```text
├── updated_part1_mongodb_netflix_analysis.ipynb
├── part2_netflix_messaging_system.ipynb
├── netflix_titles (1).csv
├── requirements.txt
├── Report.md
└── README.md
```

---

# 📊 Part 1 — Netflix Dataset Analysis

## Features

✅ Dataset loading and exploration  
✅ Data cleaning and preprocessing  
✅ MongoDB Atlas integration  
✅ Aggregation pipeline queries  
✅ Indexing discussion  
✅ Analytical visualizations  
✅ Reflection and discussion  

---

# 🧠 Database Technology Comparison

| Database | Advantages | Limitations |
|---|---|---|
| SQLite | Structured SQL queries | Requires normalization |
| MongoDB Atlas | Flexible schema and arrays | Weaker relational joins |
| Neo4j | Powerful graph traversal | Overkill for aggregation tasks |

---

# 🚀 Selected Database — MongoDB Atlas

MongoDB Atlas was selected because:

- Flexible document-oriented schema
- Natural support for arrays
- Simplified handling of genres and countries
- Efficient aggregation pipelines
- Better scalability for streaming platforms

---

# 🗃️ MongoDB Collection Design

Each Netflix title is stored as a single document.

Example:

```json
{
  "title": "Stranger Things",
  "genre_list": ["Drama", "Sci-Fi"],
  "country_list": ["United States"],
  "release_year": 2019
}
```

---

# ⚡ Indexing Strategy

Indexes created:

- `release_year`
- `genre_list`
- `country_list`

Purpose:

- Faster aggregation
- Improved filtering
- Better query performance

---

# 📈 Analytical Queries

The notebook performs the following analyses:

## 1️⃣ Most Common Netflix Genres

- Uses aggregation pipelines
- Unwinds genre arrays
- Generates bar chart visualizations

---

## 2️⃣ Top Content-Producing Countries

- Aggregates country arrays
- Generates top-country rankings
- Produces grouped bar charts

---

## 3️⃣ Netflix Release Trends Over Time

- Groups by release year
- Creates line chart visualizations
- Shows Netflix growth patterns

---

# 📡 Part 2 — Netflix Messaging System

## Features

✅ Object-Oriented Programming  
✅ Inheritance  
✅ Queue/FIFO behavior  
✅ Kafka-like streaming simulation  
✅ Producer-consumer architecture  
✅ Activity polling and retrieval  

---

# 🧱 Implemented Classes

## Base Classes

- `SimpleTopic`
- `SimpleProducer`
- `SimpleConsumer`

## Derived Classes

- `AdvancedTopic`
- `AdvancedProducer`
- `AdvancedConsumer`

---

# 🔄 Queue Behaviour

FIFO (First-In, First-Out) queue behavior was implemented using:

```python
from collections import deque
```

Reason:

- Preserves event order
- Simulates real streaming systems
- Closely resembles Kafka-like ingestion pipelines

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming |
| MongoDB Atlas | Database |
| Pandas | Data analysis |
| Matplotlib | Visualization |
| PyMongo | MongoDB connection |
| Jupyter Notebook | Development environment |

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/your-repository.git
```

---

## 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

---

## 3️⃣ Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
source venv/bin/activate
```

---

## 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ☁️ MongoDB Atlas Setup

1. Create MongoDB Atlas cluster
2. Add database user
3. Whitelist your IP address
4. Copy MongoDB connection string
5. Replace:

```python
MONGO_URI = 'YOUR_MONGODB_ATLAS_CONNECTION_STRING'
```

inside the notebook.

---

# ▶️ Running the Project

## Start Jupyter Notebook

```bash
jupyter notebook
```

Run notebook cells from top to bottom.

---

# 📌 Dependencies

```text
pandas
numpy
matplotlib
pymongo
jupyter
notebook
ipykernel
dnspython
```

---

# 📚 Academic Context

This project was developed as part of:

## **Database Management Tools in Python — Spring 2026**

The project demonstrates:

- NoSQL database modelling
- Aggregation pipelines
- Data visualization
- Queue-based messaging systems
- Inheritance and OOP concepts

---

# 👨‍💻 Author

## Subhankar Biswas

---

# ⭐ Future Improvements

Potential future enhancements:

- Apache Kafka integration
- Real-time streaming pipelines
- Recommendation system analytics
- Dashboard visualizations
- Distributed database scaling

---

# 📄 License

This project is intended for academic and educational purposes only.
