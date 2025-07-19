Movie Recommendation System (CSC 575)

Welcome to the final project for CSC 575 – Intelligent Information Retrieval

This system offers an interactive movie recommendation engine that combines **search**, **ranking**, **content filtering**, **collaborative filtering (BPR)**, and a smart **hybrid strategy**. It uses **The Movies Dataset** and provides a Gradio-based UI for easy interaction.

---
Dataset= "https://drive.google.com/file/d/1PZ35s9QAAybuqplytOArOLfiSTiD0F4J/view?usp=sharing"
---

## Project Structure

| File                                | Description                                    |
| ----------------------------------- | ---------------------------------------------- |
| `movie_recommendation_system.ipynb` | Main notebook with all models and hybrid logic |
| `README.md`                         | You’re reading it!                             |
| `self_evaluation.pdf`               | Reflection on project and contributions        |

---

## How to Run

You can run the system directly in **Google Colab** or **Jupyter Notebook**.

### Option 1: Run in Google Colab (Recommended)

1. Open `movie_recommendation_system.ipynb` in Google Colab
2. Upload the dataset file: `cleanedmovies.csv`
3. Run each cell in order
4. The Gradio UI will launch directly, or you can use the external link shown below the cell for a fullscreen version

---

## Features Implemented

- **Search** by title, genre, overview (TF-IDF)
- **Popularity-Based Recommendations** (rating + vote count)
- **Content-Based Filtering** using TF-IDF vectorization
- **BPR Model** via LightFM for collaborative filtering
- **Hybrid Recommendation Logic**: switch between popularity and BPR
- **Faceted Filtering** with genre, language, release year
- **Interactive UI** built using Gradio

---

## Dataset

We use [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset).
Please download and extract `cleanedmovies.csv` manually and upload it when prompted in the notebook.

---

## Evaluation Metrics

- `Precision@k`
- `Recall@k`
- (Planned) `nDCG`
- User-based qualitative evaluation
