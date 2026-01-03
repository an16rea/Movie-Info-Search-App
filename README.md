# Movie-Info-Search-App

🎬 Movie Search App
A sleek, modern web application for searching and discovering movies with real-time data from TheMovieDB API. Features a beautiful UI with color-coded ratings, smooth transitions, and an intuitive user experience.
<img width="1849" height="925" alt="image" src="https://github.com/user-attachments/assets/1076b18d-2b69-4815-82af-db4cfd69a417" />
<img width="1858" height="927" alt="image" src="https://github.com/user-attachments/assets/55525c12-94ac-43f2-bc83-63d49e8b209d" />
<img width="1868" height="928" alt="image" src="https://github.com/user-attachments/assets/722146a9-4f68-46f7-ba86-a7af8b264433" />
<img width="1871" height="920" alt="image" src="https://github.com/user-attachments/assets/af98a741-342e-43a9-b545-2d1a58b6a6ec" />
<img width="240" height="773" alt="image" src="https://github.com/user-attachments/assets/0323bcf0-ecd3-442a-98da-be0546f8d814" />

✨ Features

Real-time Movie Search - Search thousands of movies instantly using TheMovieDB API
Color-Coded Ratings - Visual rating system with green (7+), orange (5-7), and red (<5) indicators
Smart UI Transition - Landing page transforms into a compact header after first search
Sticky Header - Search bar stays accessible at the top while browsing results
Responsive Cards - Beautiful movie cards displaying:

Movie poster
Title
Release date
Rating (out of 10) with vote count
Plot overview


Error Handling - Graceful handling of empty searches, no results, and API errors

🚀 Demo

Landing Page: Clean, centered interface with prominent search
Search Results: Compact header with scrollable movie grid
Movie Cards: Rich information display with ratings and posters

🛠️ Technologies Used

HTML5 - Semantic structure
CSS3 - Flexbox layout, transitions, and modern styling
JavaScript (ES6) - Async API calls and DOM manipulation
jQuery - AJAX requests and simplified DOM operations
TheMovieDB API - Movie data and ratings

📦 Installation

Clone the repository:

bashgit clone https://github.com/yourusername/movie-search-app.git

Navigate to the project directory:

bashcd movie-search-app

Open index.html in your browser or use a local server:

bash# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

Visit http://localhost:8000 in your browser

🔑 API Setup
This project uses TheMovieDB API. The API key is included in the code for demo purposes, but you should get your own:

Sign up at TheMovieDB
Go to Settings → API → Request an API Key
Replace the API key in the code:

javascriptapi_key=YOUR_API_KEY_HERE
💻 Usage

Search: Type a movie name in the search box
Results: View color-coded ratings and movie details
Navigate: Scroll through results while search bar stays at top
New Search: Use the top search bar for additional searches

🎨 Color Rating System

🟢 Green (7.0-10.0): Highly rated movies
🟠 Orange (5.0-6.9): Average movies
🔴 Red (0-4.9): Low-rated movies

📂 Project Structure
movie-search-app/
│
├── index.html          # Main HTML file with embedded CSS and JS
├── README.md           # This file
└── screenshots/        # (Optional) App screenshots
🔧 How It Works
API Call
javascript$.ajax({
  url: `https://api.themoviedb.org/3/search/movie?api_key=...&query=${searchTerm}`,
  method: 'GET',
  success: function(data) {
    // Process and display results
  }
});
UI Transition

Before search: Centered landing page with large title
After search: Compact sticky header with search bar
Uses display: none/block and CSS classes to toggle views

Rating Logic
javascriptlet ratingClass = 'low';
if (rating >= 7) ratingClass = 'high';
else if (rating >= 5) ratingClass = 'medium';
🤝 Contributing
Contributions are welcome! Here are some ideas:

Fork the project
Create your feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request

📝 License
This project is open source and available under the MIT License.
👤 Author
Andrea Dass

GitHub: @an16rea
LinkedIn: Andrea Dass
www.linkedin.com/in/andrea-dass-8b327421a

🙏 Acknowledgments
Was originally made during my computer science class in high school, then I implemented it and created a more advanced and user friendly interface to advance my learning

TheMovieDB for the amazing API
Icons and inspiration from the web development community

📧 Contact
Have questions or suggestions? Feel free to reach out or open an issue!
