🌿 Medicinal Plant Recommendation System (Using Binary Feature Matrix)
📘 Overview

This project is a Medicinal Plant Recommendation System that recommends suitable Ayurvedic or herbal plants based on the user’s symptoms. The system uses a Binary Feature Matrix as the core dataset representation to map symptoms to medicinal plants. The model is designed to help users discover natural remedies efficiently, making it useful for educational, healthcare, and Ayurvedic research purposes.

🧠 Working Principle

Binary Feature Matrix Creation

A dataset is prepared where rows represent medicinal plants and columns represent symptoms.

Each cell in the matrix has a binary value:

1 → The plant is known to treat that symptom.

0 → No known association between the plant and that symptom.

Example:

Plant Name	Fever	Cough	Headache	Nausea
Tulsi	1	1	0	0
Neem	1	0	1	1
Ginger	1	1	1	1

User Input

The user selects or enters a list of symptoms (e.g., “fever”, “cough”).

The system converts these symptoms into a binary vector based on the same feature matrix.

Similarity Matching

The system calculates similarity between the user’s symptom vector and each plant’s symptom profile using distance metrics such as Cosine Similarity or KNN (k-Nearest Neighbors).

Plants with the highest similarity scores are recommended as potential remedies.

Result Display

The recommended medicinal plants are displayed with short descriptions, medicinal properties, or additional information from the dataset.

⚙️ Tech Stack

Programming Language: Python

Libraries Used: NumPy, Pandas, Scikit-learn

Model Used: KNN (for similarity-based recommendation)

UI: Kivy / Tkinter (user-friendly interface for input and display)

Database: MySQL (for structured plant and symptom data storage)

🧩 Key Features

Lightweight and interpretable model

Scalable for large symptom sets (140+ symptoms supported)

Integrates structured Ayurvedic knowledge into data-driven recommendation

Easy to update or extend with new plants and symptoms

Supports user-friendly graphical interface
