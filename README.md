Sure! Below is the completed README document for your project:

---

# Coders of Delhi: Social Network Analysis

A Python-powered project that simulates a mini social network, offering personalized friend and page recommendations through graph-based analysis and clean data pipelines.

## Project Overview

This project demonstrates a modular approach to social network modeling. It processes raw user-page interaction data and delivers intelligent recommendations by following a structured three-step pipeline:

---

## 1. Data Cleaning & Structuring

**Script**: `clean_and_structure.py`

- Cleans the input dataset by removing invalid users, inactive entries, and duplicate friends/pages.
- Ensures data integrity before recommendation engines are executed.
- Outputs `cleaned_codebook_data.json`, the cleaned dataset used in further analysis.

---

## 2. Graph Modeling

**Script**: `colab_notebook.py`

- Loads and visualizes users, their connections, and liked pages.
- Structures user relationships and interest mapping using graph and set-based representations.
- Helps understand the topology of the network and prepares data for analysis.

---

## 3. Recommendation Engines

### a. People You May Know

**Script**: `people_you_may_know.py`

- Analyzes mutual friends using set operations.
- Suggests potential new connections to increase engagement.
- Mimics how social platforms recommend new friends.

### b. Pages You Might Like

**Script**: `pages_you_might_likes.py`

- Recommends new pages based on shared interests with similar users.
- Uses collaborative filtering logic for suggesting content users are likely to engage with.

---

## File Structure

```
├── colab_notebook.py              # Data loader and visualizer
├── clean_and_structure.py         # Data cleaning pipeline
├── people_you_may_know.py         # Friend recommendation system
├── pages_you_might_likes.py       # Page recommendation system
├── social_data.json             # Raw data
├── cleaned_codebook_data.json     # Structured, clean data
```

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/ANKIT-12GU/Coders-Of-Delhi.git
cd Coders-Of-Delhi
```

2. Run the data cleaning script:

```bash
python clean_and_structure.py
```

3. Generate friend recommendations:

```bash
python people_you_may_know.py
```

4. Generate page recommendations:

```bash
python pages_you_might_likes.py
```

---

## Sample Output

### People You May Know:

```bash
People You May Know for User 1: [4]
```

**Explanation**:
- **User 1** (Amit) is recommended **User 4** (Sara) as a potential new friend based on mutual connections.

### Pages You Might Like:

```bash
Pages You Might Like for User 1: [102, 103, 104]
```

**Explanation**:
- **102**: "Data Science Enthusiasts" — liked by **Priya**, a friend of Amit.
- **103**: "AI & ML Community" — liked by **Rahul**, another user sharing common interests.
- **104**: "Web Dev Hub" — recommended based on indirect overlap of interests from **Sara**.

---

Crafted with precision by [Ankit Kumar](https://github.com/ANKIT-12GU)

---
