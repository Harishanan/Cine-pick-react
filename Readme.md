# 🎬 Movie Explorer

A stylish, fast, and user-friendly movie discovery app built with React and the TMDb API. Whether you're looking for the latest blockbuster or a hidden gem, Movie Explorer helps you find it in seconds.

---

## 📸 App Preview

Click the image below to preview the app in action:

[![Watch Demo](Images/cine-pick-webpage.mp4)](images/demo.mp4)

---

## ✨ Features

- 🔍 **Live Movie Search**: Search thousands of movies with real-time suggestions and clean results.
- 📈 **Trending Now Section**: Displays the top 5 most searched movies by users across the app.
- 🎞️ **Detailed Movie Cards**: Each result shows poster, rating, language, and release year.
- ⏳ **Debounced Search Input**: Reduces API calls and improves performance.
- ⚙️ **Appwrite Integration**: Stores search data securely and retrieves trending results dynamically.

---

## 🔥 How the "Trending Now" Section Works

The "Trending Now" section is not based on TMDb’s default trending API — instead, it’s **custom-built using Appwrite** for a smarter, app-specific view of what's hot.

### Here's how it works:
1. **Search Tracking**: Whenever a user searches for a movie and it returns results, the app sends the first match to Appwrite's backend along with the search term.
2. **Data Storage**: Appwrite keeps track of how many times each movie has been searched.
3. **Trending Fetch**: On app load, the top 5 most searched movies are retrieved from Appwrite and displayed under "Trending Now".
4. **Dynamic Updates**: As more users search, this list evolves based on real-time user behavior.

This approach makes your app feel more interactive and personalized to actual user interest.

---

## 🛠️ Tech Stack

- [React](https://reactjs.org/)
- [TMDb API](https://developers.themoviedb.org/3/)
- [Appwrite](https://appwrite.io/)
- [react-use](https://github.com/streamich/react-use) for debounce
- CSS (custom styles)

---

## ⚙️ Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/movie-explorer.git
cd movie-explorer
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Setup Environment Variables

Create a .env file in the root directory:

```bash
VITE_TMDB_API_KEY=your_tmdb_api_key
```
Get your API key from TMDb.


### 4. Start the Development Server

```bash
npm run dev
```
---

## 🙌 Acknowledgements
The Movie Database (TMDb)

Appwrite

Icons by Flaticon


