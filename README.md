# 🎬 Movie Discovery App

A modern, responsive movie discovery application built with React and powered by TMDB API. Find your next favorite movie with ease, featuring trending movies, search functionality, and a beautiful user interface.

## 🌟 Features

- **🔍 Smart Search**: Search through thousands of movies with debounced input for better performance
- **📈 Trending Movies**: View top 5 trending movies based on user search activity
- **🎯 Movie Discovery**: Browse popular movies when not searching
- **📱 Responsive Design**: Beautiful UI that works on all devices
- **⚡ Fast Performance**: Optimized with debounced search and efficient data fetching
- **🎨 Modern UI**: Clean, intuitive interface with smooth animations

## 🚀 Live Demo

Visit the live application: **[Movie App](https://movie-app-six-ruddy.vercel.app/)**

## 🛠️ Tech Stack

- **Frontend**: React 18, Vite
- **Styling**: CSS3 with modern design patterns
- **API**: The Movie Database (TMDB) API
- **Database**: Appwrite (for trending movies tracking)
- **Deployment**: Vercel
- **State Management**: React Hooks (useState, useEffect)
- **Performance**: react-use (debounced search)

## 📦 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- TMDB API key
- Appwrite project setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/movie-app.git
cd movie-app
```

### 2. Install dependencies
```bash
npm install
# or
yarn install
```

### 3. Environment Setup
Create a `.env` file in the root directory:

```env
VITE_TMDB_API_KEY=your_tmdb_api_key_here
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
```

### 4. Get API Keys

#### TMDB API Key:
1. Visit [TMDB](https://www.themoviedb.org/)
2. Create an account and go to Settings > API
3. Generate your API key

#### Appwrite Setup:
1. Create project at [Appwrite Cloud](https://cloud.appwrite.io/)
2. Create a database
3. Create a collection with these attributes:
   - `searchTerm` (string)
   - `count` (integer)
   - `movie_id` (integer)
   - `poster_url` (string)

### 5. Run the development server
```bash
npm run dev
# or
yarn dev
```

Visit `http://localhost:5173` to see the application.

## 🏗️ Project Structure

```
movie-app/
├── public/
│   └── hero.png
├── src/
│   ├── components/
│   │   ├── MovieCard.jsx
│   │   ├── Search.jsx
│   │   └── Spinner.jsx
│   ├── appwrite.js
│   ├── App.jsx
│   ├── App.css
│   └── main.jsx
├── .env
├── package.json
└── README.md
```

## 🔧 Key Components

### App.jsx
Main application component handling:
- State management for movies and search
- API calls to TMDB
- Trending movies from Appwrite
- Debounced search functionality

### appwrite.js
Backend integration for:
- Tracking search counts
- Managing trending movies
- Database operations

### Components
- **MovieCard**: Displays individual movie information
- **Search**: Search input with real-time functionality
- **Spinner**: Loading indicator

## 🌐 API Integration

### TMDB API Endpoints Used:
- `/search/movie` - Search for movies
- `/discover/movie` - Get popular movies

### Appwrite Operations:
- Store and update search counts
- Retrieve trending movies
- Track popular searches

## 📊 Features in Detail

### Smart Search
- Debounced search input (500ms delay)
- Real-time movie suggestions
- Search term tracking for trending analysis

### Trending Movies
- Top 5 movies based on search frequency
- Displays search count ranking
- Updates automatically based on user activity

### Responsive Design
- Mobile-first approach
- Flexible grid layouts
- Smooth hover effects and animations

## 🚀 Deployment

The app is deployed on Vercel with automatic deployments from the main branch.

### Deploy your own:
1. Fork this repository
2. Connect to Vercel
3. Add environment variables
4. Deploy!

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for the comprehensive movie API
- [Appwrite](https://appwrite.io/) for the backend services
- [Vercel](https://vercel.com/) for hosting and deployment
- React community for excellent documentation and tools

## 📞 Contact

Your Name - [@yourusername](https://twitter.com/yourusername) - your.email@example.com

Project Link: [https://github.com/yourusername/movie-app](https://github.com/yourusername/movie-app)

---

⭐ If you found this project helpful, please give it a star!
