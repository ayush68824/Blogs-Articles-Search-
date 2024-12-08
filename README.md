# Blogs-Articles-Search-
This project is a responsive search webpage designed for users to search and filter blogs and articles while offering a light and dark theme toggle for an improved user experience.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dynamic Search Portal</title>
  <link rel="stylesheet" href="style.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
  <div class="container">
    <div class="header">
      <h1>Explore Popular Blogs & Articles</h1>
      <button id="theme-toggle" onclick="toggleTheme()">
        <i id="theme-icon" class="fas fa-moon"></i>
      </button>
    </div>
    <div class="search-box">
      <input type="text" id="search-input" placeholder="Search for blogs, articles..." oninput="performSearch()">
      <button id="search-btn" onclick="performSearch()">🔍</button>
    </div>
    <div class="filters">
      <label for="filter">Filter:</label>
      <select id="filter" onchange="performSearch()">
        <option value="all">All</option>
        <option value="blog">Blogs</option>
        <option value="article">Articles</option>
      </select>
    </div>
    <div id="results" class="results">
      <!-- Search results will be displayed here -->
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html>
