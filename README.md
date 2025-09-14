# 🎬 Movie Recommendation System with Mood Analysis and IMDb Integration  

## 📌 Overview  
This project is a **Mood-Based Movie Recommendation System** that combines **Collaborative Filtering (SVD-based)** with **Mood Analysis** to deliver personalized movie suggestions.  

Most recommendation systems only rely on ratings or user-item history. This project goes one step further by allowing users to provide their **current mood** (e.g., happy, sad, romantic, excited, calm), and then tailoring recommendations accordingly.  

Additionally, it integrates with the **OMDb API** to fetch **IMDb details and posters**, providing not only personalized recommendations but also a visually engaging and informative user experience.  

---

## 🎯 Motivation  
In today’s digital world, users have endless entertainment choices. While traditional recommendation systems are useful, they often fail to consider **human emotions**.  
This project was designed to:  
- Enhance personalization by factoring in **user mood**.  
- Combine **collaborative filtering** with **contextual filtering (mood)**.  
- Provide recommendations that are **accurate, meaningful, and user-friendly**.  
- Bridge the gap between **AI-driven predictions** and **user experience** by integrating IMDb posters and links.  

---

## 🚀 Features  
- 🔹 **Mood-Aware Recommendations** – Suggests movies that align with the user’s current mood.  
- 🔹 **Collaborative Filtering (SVD)** – Predicts ratings for unseen movies using historical user-movie interactions.  
- 🔹 **IMDb Integration** – Fetches movie posters, IMDb ratings, and details from OMDb API.  
- 🔹 **Real-Time Predictions** – Takes **User ID + Mood input** and returns a ranked list of movie suggestions.  
- 🔹 **Interactive Visualization** – Displays movie posters in popup windows for a better visual experience.  
- 🔹 **User-Friendly Output** – Provides predicted ratings, star ratings, and IMDb links alongside recommendations.  

---

## 🛠️ Tech Stack  
- **Programming Language:** Python  
- **Libraries & Tools:**  
  - Data Handling: Pandas, NumPy  
  - Machine Learning: Scikit-learn (Collaborative Filtering with SVD)  
  - Visualization: Matplotlib  
  - API & Image Processing: Requests, Pillow  
- **Model:** Collaborative Filtering (Mean Imputation + SVD-based predictions)  
- **API:** OMDb API (for IMDb movie details & posters)  
- **Dataset:** Custom Movie Ratings Dataset (`movies dataset 480.csv`)  

---
## Work Flow
## 🔄 Workflow Diagram (Conceptual)
    A[User Input: User ID + Mood] --> B[Load Dataset]
    B --> C[Preprocessing: Encoding & Cleaning]
    C --> D[Train-Test Split + User-Item Matrix]
    D --> E[Collaborative Filtering (SVD Predictions)]
    E --> F[Mood Filtering: Match mood & remove watched]
    F --> G[Recommendation List]
    G --> H[Fetch IMDb Posters + Links via OMDb API]
    H --> I[Final Output: Ranked Movies + Posters]

## Output (Example)
## 📝 Example Output  

💡 Available moods: happy, sad, romantic, excited, calm  

Enter your User ID: 5  
Enter your current mood: romantic  

🎬 Recommended Movies for Mood 'romantic' (User 5):  

The Notebook  
Rating: 4.20 ⭐⭐⭐⭐  
IMDb: https://www.imdb.com/title/tt0332280/  
------------------------------------------------------------  

Titanic  
Rating: 4.05 ⭐⭐⭐⭐  
IMDb: https://www.imdb.com/title/tt0120338/  
------------------------------------------------------------  

Pride and Prejudice  
Rating: 3.90 ⭐⭐⭐⭐  
IMDb: https://www.imdb.com/title/tt0414387/  
------------------------------------------------------------  

