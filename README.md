# Book-Recommender
# 📚 Personalized Book Recommendation System using Generative AI

This project is an AI-powered Book Recommendation System that offers personalized book suggestions based on user input. It combines **machine learning techniques** with a **Streamlit interface**, **generative search suggestions**, and **SHAP-based model explanations** to enhance user experience and interpretability.

---

## 🔍 Features

✅ **Personalized Recommendations**:  
Suggests similar books based on title and author using TF-IDF and KNN.

✅ **Author Display**:  
Displays the author's name along with each recommendation.

✅ **Search Suggestions**:  
Dynamically filters book titles to help users easily find the book they're looking for.

✅ **Explanation Module (SHAP)**:  
Visualizes the reasons behind the similarity of selected books.

✅ **Interactive UI (Streamlit)**:  
Fast and clean web interface for users to interact with the system.

---

## 🗂️ Project Structure

book-recommender/
│
├── app.py # Main Streamlit application
├── recommend.py # Backend recommendation logic
├── explain.py # SHAP explanation module
├── books.csv # Dataset of book metadata
├── ratings.csv # Dataset of user ratings
├── requirements.txt # Python dependencies
└── .gitignore # Git ignore rules

yaml
Copy
Edit

---

## 🧠 Tech Stack

- **Frontend**: Streamlit (Python)
- **Backend**: scikit-learn (TF-IDF + KNN), pandas, numpy
- **Explainability**: SHAP
- **Language**: Python 3.9+

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/book-recommender.git
cd book-recommender

### 2. Set up a Virtual Environment (optional but recommended)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate      # Linux/macOS
venv\Scripts\activate         # Windows

###3. Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt

🚀 Usage
Run the App
bash
Copy
Edit
streamlit run app.py
Select a book from the dropdown.

Get up to 5 personalized recommendations.

View the author of each book.

Optionally, enter an index in explain.py to visualize similarity using SHAP.

📊 Datasets Used
books.csv: Contains details like ISBN, title, author, and publisher.

ratings.csv: Contains user ratings (User-ID, ISBN, Book-Rating).

Make sure both files are in the root directory before running the app.

📎 Example
<p align="center"> <img src="https://your-screenshot-link.com/preview.png" alt="Streamlit UI Preview" width="600"/> </p>
🧪 Future Improvements
Add content-based filtering with book descriptions

Enable genre-based filtering

Store user sessions for long-term personalization

Deploy with Docker or on a cloud platform (e.g., Streamlit Cloud, Heroku)
