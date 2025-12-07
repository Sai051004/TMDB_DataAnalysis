# 🎬 Cinemania – Movie Recommendation System

Cinemania is a movie recommendation web application built using **Streamlit** and **machine learning algorithms**.  
It suggests similar movies based on user selection and displays details such as cast, genres, keywords, and posters using the **TMDb API**.

---

## 🚀 Features

- 🎥 Get top 10 personalized movie recommendations  
- 🌟 Fetch detailed movie information including:
  - Movie posters
  - Cast
  - Genres
  - Keywords
- 🍿 Sidebar shows trending and popular movies
- 💡 Interactive UI built using **Streamlit**

---

## 🧠 How It Works

1. **Data Preparation:**  
   - Movie data and feature vectors are preprocessed and stored in `movie_list.pkl` and `similarity.pkl`.
   - The dataset used to create these files is available here:  
     👉 **[Download Dataset (Google Drive)](https://drive.google.com/drive/folders/1kVnwYAi66RP-vx0QgOD9A8aM-XS-O_zc?usp=sharing)**

2. **Recommendation Logic:**  
   - When a user selects a movie, a similarity matrix compares features (like genres, cast, etc.) to find the top 10 similar movies.

3. **API Integration:**  
   - The app fetches additional details (cast, keywords, poster, release date, and genres) using the **TMDb API**.

4. **Machine Learning Model:**  
   - The model is trained and evaluated in `machineLearningAlgo.ipynb`, which includes feature extraction and similarity computation.

**How To Run:-** 
![How To Run](https://github.com/Sai051004/TMDB_DataAnalysis/blob/main/Screenshot%202025-12-07%20150825.png)
**Image:** 
![Image](https://github.com/Sai051004/TMDB_DataAnalysis/blob/main/Screenshot%202025-12-07%20150611.png)
**Example1:** 
![Example1](https://github.com/Sai051004/TMDB_DataAnalysis/blob/main/Screenshot%202025-12-07%20145525.png)
**Example2:** 
![Example2](https://github.com/Sai051004/TMDB_DataAnalysis/blob/main/Screenshot%202025-12-07%20151239.png)
**Example3:** 
![Example3](https://github.com/Sai051004/TMDB_DataAnalysis/blob/main/Screenshot%202025-12-07%20151218.png)



---

## 🧰 Technologies Used

- **Python 3.x**
- **Streamlit** – Web framework for building interactive apps
- **Pickle** – To store preprocessed data
- **Requests** – To call the TMDb API
- **Pandas & NumPy** – Data manipulation
- **Scikit-learn** – For machine learning similarity computations
- **TMDb API** – Movie details and posters

---

## ⚙️ Setup Instructions

1. **Clone this repository**
   ```bash
   git clone https://github.com/yourusername/Cinemania.git
   cd Cinemania
   ```

2. **Install the dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Add your TMDb API key**  
   Replace the API key in `app.py`:
   ```python
   api_key = "YOUR_TMDB_API_KEY"
   ```

4. **Run the Streamlit app**
   ```bash
   streamlit run app.py
   ```

5. **Access the application**  
   Open your browser and navigate to:
   ```
   http://localhost:8501
   ```

---

## 🧩 Files Overview

| File | Description |
|------|--------------|
| `app.py` | Main Streamlit web app that handles UI and API integration |
| `machineLearningAlgo.ipynb` | Notebook for feature extraction, preprocessing, and similarity matrix generation |
| `movie_list.pkl` | Serialized dataset of movies |
| `similarity.pkl` | Precomputed similarity matrix for recommendations |

---

## 🎯 Future Enhancements

- 🎬 Add filtering by genre, rating, or language  
- 📱 Make UI responsive for mobile devices  
- 🧮 Integrate deep learning models for better similarity scoring  
- 💾 Allow users to save favorite movies or recommendation lists  

---

## ❤️ Acknowledgments

- [The Movie Database (TMDb)](https://www.themoviedb.org/) for the API and data  
- Streamlit for an easy and interactive UI framework
