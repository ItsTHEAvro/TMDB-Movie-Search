# TMDB Movie Search

TMDB Movie Search is a React-based movie discovery application that allows users to search and explore movies using The Movie Database (TMDB) API. The application provides movie details, ratings, genres, and more.

## Features

- **Search Movies:** Search for movies using keywords.
- **Popular Movies:** Displays trending movies by default.
- **Movie Details:** Shows essential information like title, rating, release year, genres, and a brief overview.
- **Debounced Search:** Implements a delay to optimize API requests and improve performance.
- **Responsive UI:** Designed for desktop and mobile views.

## Tech Stack

- **Frontend:** React.js
- **State Management:** React Hooks (`useState`, `useEffect`)
- **API Handling:** Fetch API
- **Styling:** Tailwind CSS
- **Debouncing:** `react-use`

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/ItsTHEAvro/tmdb-movie-search.git
   cd tmdb-movie-search
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file in the root directory and add your TMDB API key:

   ```sh
   VITE_TMDB_API_KEY=your_api_key_here
   ```

4. Start the development server:
   ```sh
   npm run dev
   ```

## Project Structure

```
TMDB-Movie-Search/
├───.env
├───.gitignore
├───eslint.config.js
├───index.html
├───package-lock.json
├───package.json
├───README.md
├───vite.config.js
│
├───public
│   ├───hero-bg.png
│   ├───hero.png
│   ├───logo.png
│   ├───no-movie.png
│   ├───search.svg
│   └───star.svg
│
└───src
    ├───App.css
    ├───App.jsx
    ├───index.css
    ├───main.jsx
    ├───assets
    └───components
        ├───MovieCard.jsx
        ├───Search.jsx
        └───Spinner.jsx
```

## API Usage

This application uses the TMDB API for fetching movie data. Requests are made to:

- **Search Movies:** `/search/movie?query=<query>`
- **Popular Movies:** `/discover/movie?sort_by=popularity.desc`

## License

This project is licensed under the MIT License. Feel free to modify and distribute it as needed.

## Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/)
- React.js Community
