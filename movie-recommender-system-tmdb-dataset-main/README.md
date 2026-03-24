# 🎬 Movie Recommender System

A simple and interactive **Movie Recommendation Web App** built using **Streamlit**. This app suggests similar movies based on a selected movie and displays their posters using the TMDb API.

---

## 🚀 Features

* Select or type a movie from the dropdown
* Get **Top 5 similar movie recommendations**
* Displays **movie posters**
* Fast and lightweight UI using Streamlit

---

## 🛠️ Tech Stack

* **Python**
* **Streamlit**
* **Pickle**
* **Pandas (assumed for dataset handling)**
* **TMDb API** (for fetching movie posters)

---

## 📁 Project Structure

```
├── app.py
├── model/
│   ├── movie_list.pkl
│   ├── similarity.pkl
```

---

## ⚙️ How It Works

1. The app loads:

   * `movie_list.pkl`: Contains movie data (titles, IDs)
   * `similarity.pkl`: Precomputed similarity matrix

2. When a user selects a movie:

   * The system finds its index
   * Retrieves similarity scores
   * Sorts and selects top 5 similar movies

3. For each recommended movie:

   * Fetches poster using TMDb API
   * Displays name + poster

---

## 🔑 API Used

* **The Movie Database (TMDb) API**
* Used to fetch movie posters dynamically

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone <your-repo-link>
   cd <your-project-folder>
   ```

2. Install dependencies:

   ```bash
   pip install streamlit requests pandas
   ```

3. Run the app:

   ```bash
   streamlit run app.py
   ```

---

## ⚠️ Important Notes

* Ensure the following files exist:

  * `model/movie_list.pkl`
  * `model/similarity.pkl`
* Replace the API key in `app.py` with your own TMDb API key:

  ```python
  api_key = "your_api_key_here"
  ```

---

## 📸 Preview

* Select a movie → Click **Show Recommendation**
* See 5 recommended movies with posters

---

## 💡 Future Improvements

* Add search filtering
* Improve UI design
* Add movie details (rating, overview, genres)
* Deploy on cloud (Streamlit Cloud / Heroku)

---

## 🤝 Contributing

Feel free to fork the project and submit pull requests.

---

## 📜 License

This project is open-source and available under the MIT License.

---

* Add **deployment steps**
* Or write README for your `.ipynb` file too 👍
