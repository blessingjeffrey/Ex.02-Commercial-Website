# Ex02 Commercial Website
## Date: 10/09/2025
## Name: Blessing Jeffrey YL
## Reg.no: 212223220014

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Virat Kohli Official Store - Home</title>
    <link rel="stylesheet" href="web.css">
</head>

<body>

    <nav class="navbar">
        <div class="logo">Virat Kohli Store</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="merchandise.html">Merchandise</a></li>
            <li><a href="biography.html">Biography</a></li>
            
        </ul>
    </nav>

    <section class="hero">
        <h1>Welcome to Virat Kohli Official Merchandise</h1>
        <p>Wear your passion for cricket with official products endorsed by Virat Kohli!</p>
        <a href="merchandise.html" class="btn">Shop Now</a>
    </section>

    <section class="products">
        <h2>Featured Products</h2>
        <div class="product-list">
            <div class="product-card">
                <img src="signed tshirt.jpg" alt="VK T-Shirt">
                <h3>Virat Kohli Signature T-Shirt</h3>
                <p>Official licensed T-shirt for fans.</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="vk cap.jpg" alt="VK Cap">
                <h3>Virat Kohli Cap</h3>
                <p>Limited edition cap endorsed by Virat Kohli.</p>
                <button>Buy Now</button>
            </div>
        </div>
    </section>

    <footer class="footer">
        <p>&copy; 2025 Virat Kohli Official Store. All rights reserved.</p>
    </footer>

</body>

</html>
```
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Merchandise - Virat Kohli Store</title>
    <link rel="stylesheet" href="web.css">
</head>

<body>

    <nav class="navbar">
        <div class="logo">Virat Kohli Store</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="merchandise.html">Merchandise</a></li>
            <li><a href="biography.html">Biography</a></li>
        </ul>
    </nav>

    <section class="products">
        <h2>All Merchandise</h2>
        <div class="product-list">

            <div class="product-card">
                <img src="vk jersey.png" alt="VK Jersey">
                <h3>Virat Kohli Match Jersey</h3>
                <p>High-quality jersey worn by Virat Kohli.</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="vk mug.webp" alt="VK Mug">
                <h3>Virat Kohli Mug</h3>
                <p>Official Virat Kohli coffee mug for cricket fans.</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="vk poster.webp" alt="VK Poster">
                <h3>Autographed Virat Kohli Poster</h3>
                <p>Limited edition autographed poster for collectors.</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <footer class="footer">
        <p>&copy; 2025 Virat Kohli Official Store. All rights reserved.</p>
    </footer>

</body>

</html>
```
```

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biography - Virat Kohli</title>
    <link rel="stylesheet" href="web.css">
</head>

<body>

    <nav class="navbar">
        <div class="logo">Virat Kohli Store</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="merchandise.html">Merchandise</a></li>
            <li><a href="biography.html">Biography</a></li>
        </ul>
    </nav>

    <section class="biography">
        <h2>About Virat Kohli</h2>
        <img src="VIRAT-KOHLI-IPL-2025.jpg" alt="Virat Kohli">
        <p>
            Virat Kohli is one of the greatest cricketers of his generation. Born on November 5, 1988, he has led
            India to numerous victories as captain and is known for his aggressive play, impeccable technique, and
            unmatched passion for cricket. Off the field, he is a global icon with millions of fans worldwide.
        </p>
    </section>

    <footer class="footer">
        <p>&copy; 2025 Virat Kohli Official Store. All rights reserved.</p>
    </footer>

</body>

</html>

```

CSS

```

/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #000; /* Black background */
    color: #FFD700; /* Gold text color */
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #D50032; /* RCB Red */
    padding: 1rem 2rem;
    color: white;
}

.navbar .logo {
    font-size: 1.8rem;
    font-weight: bold;
}

.navbar .nav-links {
    list-style: none;
    display: flex;
    gap: 1.5rem;
}

.navbar .nav-links a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    transition: color 0.3s;
}

.navbar .nav-links a:hover {
    color: #FFD700; /* Gold on hover */
}

/* Hero Section */
.hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 5rem 1rem;
    background: #D50032; /* RCB Red background */
    color: #FFD700;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.hero .btn {
    text-decoration: none;
    background-color: #FFD700; /* Gold Button */
    color: #000;
    padding: 0.8rem 1.5rem;
    border-radius: 5px;
    font-weight: bold;
    transition: background-color 0.3s;
}

.hero .btn:hover {
    background-color: #FFC300;
}

/* Products Section */
.products {
    padding: 3rem 2rem;
    text-align: center;
}

.products h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
    color: #FFD700;
}

.product-list {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
}

.product-card {
    background-color: #1C1C1C; /* Dark background for contrast */
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(255, 215, 0, 0.2);
    max-width: 250px;
    text-align: center;
    transition: transform 0.3s;
}

.product-card:hover {
    transform: translateY(-10px);
}

.product-card img {
    max-width: 100%;
    border-radius: 8px;
    margin-bottom: 1rem;
}

.product-card h3 {
    margin-bottom: 1rem;
    color: #FFD700;
}

.product-card p {
    font-size: 0.95rem;
    margin-bottom: 1rem;
    color: #FFD700;
}

.product-card button {
    padding: 0.5rem 1rem;
    background-color: #D50032; /* Red button */
    border: none;
    color: white;
    border-radius: 5px;
    font-weight: bold;
    cursor: pointer;
}

.product-card button:hover {
    background-color: #B71C1C;
}

/* Biography Section */
.biography {
    padding: 3rem 2rem;
    text-align: center;
}

.biography img {
    max-width: 300px;
    border-radius: 10px;
    margin: 1rem 0;
    border: 4px solid #FFD700;
}

.biography p {
    font-size: 1.1rem;
    line-height: 1.6;
    max-width: 800px;
    margin: 0 auto;
    color: #FFD700;
}

/* Footer */
.footer {
    background-color: #D50032;
    color: white;
    text-align: center;
    padding: 1.5rem;
    margin-top: 3rem;
}

```
## OUTPUT
<img width="1917" height="965" alt="image" src="https://github.com/user-attachments/assets/91c1af4b-dbea-4a44-af7d-11f7fc01e3b1" />

<img width="1918" height="963" alt="image" src="https://github.com/user-attachments/assets/e311f7e3-f733-4b06-84e5-82632ab7a84e" />

<img width="1918" height="861" alt="image" src="https://github.com/user-attachments/assets/05c8ccab-aac2-439c-b1c3-de8ae2c2be31" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
