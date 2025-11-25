# Ex02 Commercial Website
## Date:25-11-2025

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
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sweet Crumbs Bakery</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
</head>
<body>
  <header>
    <div class="logo">Sweet Crumbs</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#products">Our Products</a>
      <a href="#about">About</a>
      <a href="#contact" class="btn">Contact</a>
    </nav>
  </header>

  <section class="hero" id="home">
    <div class="hero-text">
      <h1>Freshly Baked Happiness</h1>
      <p>Delicious breads, pastries, and cakes made with love every day.</p>
      <a href="#products" class="btn">Shop Now</a>
    </div>
    <div class="hero-image">
      <img src="cake.avif" alt="Bakery items">
    </div>
  </section>

  <section class="products" id="products">
    <h2>Our Best Sellers</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="ButteryCroissant.jpg" alt="Croissant">
        <h3>Buttery Croissant</h3>
        <p>Flaky, golden, and irresistibly buttery.</p>
      </div>
      <div class="product-card">
        <img src="choco.webp" alt="Chocolate Cake">
        <h3>Chocolate Dream Cake</h3>
        <p>Rich chocolate layers with creamy ganache.</p>
      </div>
      <div class="product-card">
        <img src="baguette.jpg" alt="Baguette">
        <h3>Classic Baguette</h3>
        <p>Crunchy outside, soft inside, perfect for any meal.</p>
      </div>
    </div>
  </section>

 <section class="about" id="about">
  <div class="about-container">
    <div class="about-image">
      <img src="macroon2.jpg" alt="Baking in process">
    </div>
    <div class="about-text">
      <h2>About Sweet Crumbs</h2>
      <p>
        At <strong>Sweet Crumbs Bakery</strong>, baking isn’t just a craft — it’s our love language.  
        Every loaf, pastry, and cake is made from scratch with locally sourced ingredients,  
        time-honored recipes, and a pinch of joy in every bite.
      </p>
      <p>
        From the aroma of freshly baked bread in the morning to the last slice of cake in the evening,  
        our mission is to make every day a little sweeter.
      </p>
      <a href="#contact" class="btn">Visit Us Today</a>
    </div>
  </div>
</section>
 <section class="contact" id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>© 2025 Sweet Crumbs Bakery. All rights reserved.</p>
  </footer>
</body>
</html>

style.css

:root {
  --primary: #d2691e;
  --secondary: #fff4e6;
  --accent: #f4a261;
  --text-dark: #5a3e2b;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  color: var(--text-dark);
  background-color: var(--secondary);
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 50px;
  background-color: rgb(245, 245, 245);
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}

.logo {
  font-family: 'Pacifico', cursive;
  font-size: 28px;
  color: var(--primary);
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: var(--text-dark);
  font-weight: 500;
}

nav a.btn {
  background: var(--primary);
  color: white;
  padding: 8px 15px;
  border-radius: 6px;
}

.hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding: 50px;
  align-items: center;
  gap: 20px;
}

.hero-text h1 {
  font-size: 48px;
  color: var(--primary);
}

.hero-text p {
  margin: 20px 0;
}

.hero-text .btn {
  background: var(--accent);
  color: white;
  padding: 10px 18px;
  border-radius: 6px;
  text-decoration: none;
}

.hero-image img {
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.1);
}

.products {
  text-align: center;
  padding: 50px 20px;
}

.products h2 {
  margin-bottom: 30px;
  font-size: 32px;
}

.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
  gap: 20px;
}

.product-card {
  background: white;
  border-radius: 12px;
  padding: 15px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.05);
}

.product-card img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 15px;
}




.about {
  padding: 60px 20px;
  background-color: var(--secondary);
}

.about-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  gap: 40px;
  max-width: 1100px;
  margin: auto;
}

.about-image img {
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.1);
}

.about-text h2 {
  font-size: 36px;
  margin-bottom: 20px;
  color: var(--primary);
}

.about-text p {
  margin-bottom: 15px;
  line-height: 1.6;
}

.about-text .btn {
  background: var(--accent);
  color: white;
  padding: 10px 20px;
  border-radius: 6px;
  text-decoration: none;
  font-weight: 600;
  display: inline-block;
  transition: background 0.3s ease;
}

.about-text .btn:hover {
  background: #e07a4e;
}
.contact {
  padding: 50px 20px;
  text-align: center;
}

.contact form {
  max-width: 400px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.contact input,
.contact textarea {
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 6px;
}

.contact button {
  background: var(--primary);
  color: white;
  padding: 10px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

footer {
  text-align: center;
  padding: 20px;
  background: white;
  box-shadow: 0 -2px 10px rgba(0,0,0,0.05);
  margin-top: 30px;
}

.contact {
  padding: 50px 20px;
  text-align: center;
}

.contact form {
  max-width: 400px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.contact input,
.contact textarea {
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 6px;
}

.contact button {
  background: var(--primary);
  color: white;
  padding: 10px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

footer {
  text-align: center;
  padding: 20px;
  background: white;
  box-shadow: 0 -2px 10px rgba(0,0,0,0.05);
  margin-top: 30px;
}

@media (max-width: 768px) {
  .hero {
    grid-template-columns: 1fr;
  }
}
```

## OUTPUT
<img width="1914" height="1091" alt="Screenshot 2025-08-11 190922" src="https://github.com/user-attachments/assets/9e9cd584-3748-4ae7-b8d9-70cfebc57b05" />
<img width="1919" height="1087" alt="Screenshot 2025-08-11 190939" src="https://github.com/user-attachments/assets/5fa05a9a-b389-458e-a46f-ecf6d3ae2a98" />

<img width="1907" height="1091" alt="Screenshot 2025-08-11 191002" src="https://github.com/user-attachments/assets/7e3be2e7-41a0-4b55-baeb-7c5894ba36f8" />
<img width="1919" height="1088" alt="Screenshot 2025-08-11 191017" src="https://github.com/user-attachments/assets/1d782b3f-4f43-46b2-9b73-12ff382f6a45" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
