![Screenshot 2024-04-11 7 14 16 PM](https://github.com/linuxfandudeguy/laki/assets/164905463/2340eeb9-e27f-43d4-bd14-3790ea2bdf01)
Laki is a homemade browser powered by Microsoft Bing.

https://lakibrowser.netlify.app

laki is also kind of bad so please don't be mean

[U<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Custom Browser</title>
    <!-- Link tags for favicon and apple-touch-icon -->
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
    <link rel="manifest" href="/site.webmanifest">
    <style>
        /* Style for the header container */
        .header-container {
            text-align: center;
            margin-bottom: 20px;
        }

        /* Style for the logo image */
        .logo {
            max-width: 100%;
            height: auto;
        }

        /* Style for the search container */
        .search-container {
            margin: 20px auto;
            max-width: 400px;
            text-align: center;
        }

        /* Style for the search input */
        .search-input {
            padding: 8px;
            width: 60%;
            margin-right: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        /* Style for the search button */
        .search-button {
            padding: 8px 16px;
            border: none;
            border-radius: 5px;
            background-color: #007bff;
            color: #fff;
            cursor: pointer;
        }

        /* Style for the search button on hover */
        .search-button:hover {
            background-color: #0056b3;
        }

        /* Style for the iframe */
        .search-results {
            margin-top: 20px;
            width: 100%;
            height: 80vh;
            border: none;
        }
    </style>
</head>
<body>

<!-- Header container -->
<div class="header-container">
    <!-- Logo image -->
    <img src="https://i.ibb.co/T0LZ9VX/Screenshot-2024-04-11-6-47-38-PM.png" alt="Logo" class="logo">
</div>

<!-- Search container -->
<div class="search-container">
    <!-- Search input -->
    <input type="text" id="searchInput" class="search-input" placeholder="Enter your search query">
    <!-- Search button -->
    <button class="search-button" onclick="performSearch()">Search</button>
</div>

<!-- Container for search results -->
<div id="searchResultsContainer">
</div>

<script>
    function performSearch() {
        // Get the search query from the input field
        var query = document.getElementById('searchInput').value;
        
        // Create an iframe with the search results page loaded
        var iframe = document.createElement('iframe');
        iframe.setAttribute('src', 'https://www.bing.com/search?q=' + encodeURIComponent(query));
        iframe.setAttribute('class', 'search-results');
        
        // Add the iframe to the container
        var container = document.getElementById('searchResultsContainer');
        container.innerHTML = '';
        container.appendChild(iframe);
    }
</script>

</body>
</html>
ploading index (1).html…]()




