## Ex02 Commercial Website
## Date: 09/08/2025
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
## Home Page
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Naveen Electricals - Home</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header>
    <div class="logo">Naveen Electricals</div>
    <nav>
      <a href="index.html">Home</a>
      <a href="products.html">Products</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Welcome to Naveen Electricals</h1>
    <p>Your one-stop shop for quality electrical products and solutions.</p>
    <a href="products.html" class="btn">Browse Products</a>
  </section>

  <footer>
    <p>&copy; 2025 Naveen Electricals. All rights reserved.</p>
  </footer>

</body>
</html>

```
## Product Page
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Naveen Electricals - Products</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header>
    <div class="logo">Naveen Electricals</div>
    <nav>
      <a href="index.html">Home</a>
      <a href="products.html">Products</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>

  <section class="features">
    <div class="feature">
      <h3>LED Bulbs</h3>
      <img src="p1.jpeg" alt="LED Bulbs" />
      <p>High-efficiency LED bulbs with long life and low energy consumption.</p>
      <p><strong>Price:</strong> ₹120 each</p>
    </div>

    <div class="feature">
      <h3>Ceiling Fans</h3>
      <img src="p2.jpeg" alt="Ceiling Fan" />
      <p>Stylish ceiling fans with powerful airflow and energy-saving design.</p>
      <p><strong>Price:</strong> ₹3,200</p>
    </div>

    <div class="feature">
      <h3>Switchboards</h3>
      <img src="p3.jpeg" alt="Switchboard" />
      <p>Durable and safe switchboards for homes and offices.</p>
      <p><strong>Price:</strong> ₹450</p>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Naveen Electricals. All rights reserved.</p>
  </footer>

</body>
</html>

```
## Contact Page
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Naveen Electricals - Contact</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">Naveen Electricals</div>
        <nav>
            <a href="index.html">Home</a>
            <a href="products.html">Products</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <section class="contact">
        <div class="contact-info">
            <h2>Contact Us</h2>
            <p><strong>Email:</strong> naveenelectricals@gmail.com</p>
            <p><strong>Phone:</strong> +91 90031 47267</p>
            <p><strong>Address:</strong> 07, Padappai Walajabad Road, Chennai, Tamil Nadu</p>
        </div>
        <img src="store.jpeg" alt="Naveen Electricals Shop" class="contact-img">
    </section>

    <footer>
        <p>&copy; 2025 Naveen Electricals. All rights reserved.</p>
    </footer>
</body>
</html>

```
## CSS Code
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f8f8f8;
  color: #333;
}


header {
  background: #007BFF;
  color: white;
  padding: 15px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header .logo {
  font-size: 22px;
  font-weight: bold;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
  transition: color 0.3s;
}

nav a:hover {
  color: yellow;
}


.hero {
  background: url('hero.jpeg') no-repeat center center/cover;
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
}

.hero h1 {
  font-size: 42px;
  margin-bottom: 15px;
}

.hero p {
  font-size: 18px;
  margin-bottom: 20px;
}

.hero .btn {
  background: yellow;
  color: black;
  padding: 10px 20px;
  border-radius: 25px;
  text-decoration: none;
  font-weight: bold;
}

.hero .btn:hover {
  background: orange;
}


.features {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 40px;
  gap: 20px;
}

.feature {
  background: white;
  border-radius: 10px;
  padding: 20px;
  width: 300px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  text-align: center;
  transition: transform 0.2s;
}

.feature:hover {
  transform: translateY(-5px);
}

.feature img {
  max-width: 100%;
  border-radius: 8px;
  margin-bottom: 10px;
}

.feature h3 {
  color: #007BFF;
}



.contact {
  padding: 40px;
  background: #f1f1f1;
  text-align: center;
}

.contact-info {
  margin-bottom: 20px;
}

.contact-img {
  max-width: 600px;
  border-radius: 10px;
}


footer {
  background: #222;
  color: white;
  text-align: center;
  padding: 15px;
  margin-top: 40px;
}

```
## OUTPUT
<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/ce69c990-a570-41d1-abf3-f640245ab300" />
<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/3e8b610d-e5b8-44ab-a525-843e475bfa5b" />
<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/c244d7d8-af7a-4e37-99ba-62a736a92af3" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
