# Ex.07 Restaurant Website
## Date:19-05-2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
home.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Parantha</title>
    <style>
      
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #cafa6c;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: rgb(124, 203, 245);
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .banner {
            background-size: cover;
            margin-right: 2%;
            margin-left: 2%;
            margin-top: 1%;
            border-radius: 37px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 30px 20px;
            background: url('banner.jpg') no-repeat center center/cover;
            color: rgb(226, 250, 72);
            height: 300px;
            text-align: center;
        }

        .banner-content {
            max-width: 50%;
        }

        .banner-content h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: rgb(0, 0, 0);
        }

        .banner-content p {
            font-size: 1rem;
            margin-bottom: 15px;
            color: black;
        }

        .banner-content a {
            background: transparent;
            color: rgb(0, 0, 0);
            padding: 8px 15px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            border: solid;
            border-color: #000000;
            transition: background 0.3s ease;
        }

        .banner-content a:hover {
            background: #c4ff2f;
        }

        .features {
            display: flex  ;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px;
            gap: 15px;
            background: #dff64a;
        }

        .feature {
            background: white;
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            flex: 1;
            text-align: center;
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }

        .feature h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #1f1714;
        }

        .feature p {
            font-size: 0.9rem;
            color: #555;
        }

        footer {
            background: rgba(17, 0, 0, 0.804);
            color: rgb(252, 249, 249);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }


        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                height: auto;
                text-align: center;
            }

            .banner-content {
                max-width: 100%;
            }

            .features {
                flex-direction: column;
                gap: 20px;
            }

            .feature {
                flex: none;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Parantha</h1></div>
        </div>
        
            <nav>
                <a href="home .html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <hr width="95%"> 
    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to THE Parantha HOTEL</h1>
            <p>Where the Ocean Meets Your Plate, and Every Meal is an Adventure.</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <footer>
        <p>Designed by : Paranthaman S</p>
    </footer>

</body>
</html>
~~~
menu.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Parantha - Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: rgb(125, 252, 247);
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .menu-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2rem;
            color: #000000;
            margin-bottom: 15px;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-details {
            padding: 10px;
        }

        .menu-details h3 {
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .menu-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1rem;
            color: #ff5722;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 10px;
        }

        footer {
            background: white;
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 100px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Parantha</h1></div>
        </div>
        
            <nav>
                <a href="home .html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="1.jpg" alt="Lobster Bisque">
                <div class="menu-details">
                    <h3>Lobster Bisque</h3>
                    <p class="price">₹1999/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="2.jpg" alt="Grilled Octopus">
                <div class="menu-details">
                    <h3>Grilled Octopus</h3>
                    <p class="price">₹4999/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="3.jpg" alt="Shrimp Scampi">
                <div class="menu-details">
                    <h3>Shrimp Scampi</h3>
                    <p class="price">₹5999/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="4.jpg" alt="Bouillabaisse">
                <div class="menu-details">
                    <h3>Bouillabaisse</h3>
                    <p class="price">₹1790/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="5.jpg" alt=" Sushi & Sashimi">
                <div class="menu-details">
                    <h3> Sushi & Sashimi</h3>
                    <p class="price">₹7999/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="6.jpg" alt="Ceviche">
                <div class="menu-details">
                    <h3>Ceviche</h3>
                    <p class="price">₹1777/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="7.jpg" alt=" Paella de Mariscos">
                <div class="menu-details">
                    <h3> Paella de Mariscos</h3>
                    <p class="price">₹2222/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="8.jpg" alt="Crab Cakes">
                <div class="menu-details">
                    <h3>Crab Cakes</h3>
                    <p class="price">₹3599/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="9.jpg" alt="Fish Tacos">
                <div class="menu-details">
                    <h3>Fish Tacos</h3>
                    <p class="price">₹3999/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="10.jpg" alt="Salmon Teriyaki">
                <div class="menu-details">
                    <h3>Salmon Teriyaki</h3>
                    <p class="price">₹2999/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="11.jpg" alt="Jambalaya">
                <div class="menu-details">
                    <h3>Jambalaya</h3>
                    <p class="price">₹2500/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="12.jpg" alt="Chilli Crab">
                <div class="menu-details">
                    <h3>Chilli Crab</h3>
                    <p class="price">₹5000/-</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>Designed by : Paranthaman s </p>
    </footer>

</body>
</html>
~~~
contact.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>THE Parantha- contact us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: rgb(143, 225, 254);
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }


        .contact-banner h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            color:rgb(245, 10, 10);
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 30px 15px;
            background: rgb(235, 70, 70);
            gap: 20px;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 4px 4px 4px 6px rgba(0, 0, 0, 0.1);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #1f1714;
            text-align: center;
        }

        .contact-details p {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }

        .contact-form textarea {
            height: 100px;
        }

        .contact-form button {
            width: 100%;
            padding: 10px;
            background: #ff5722;
            color: rgb(197, 242, 108);
            font-size: 1.1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #e64a19;
        }

        footer {
            background: rgb(249, 105, 105);
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Parantha</h1></div>
        </div>
        
            <nav>
                <a href="home .html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="contact-banner">
     
    </div>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            
            <p><strong>Phone:</strong> +91 9999999999</p>
            <p><strong>Email:</strong> Parantha@gmail.com</p>
            <p><strong>Hours:</strong> Mon-Sun(10 AM - 10 PM)</p>
        </div>

        <div class="contact-form">
            <h2>Send Us a Message</h2>
            <form action="/submit-contact" method="POST">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>

                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" placeholder="Your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>Designed by :Paranthaman S</p>
    </footer>

</body>
</html>
~~~
admin.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>THE Parantha-Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: rgb(117, 218, 243);
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }


        .admin-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2rem;
            color: #000000;
            margin-bottom: 20px;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-item:hover {
            transform: scale(1.05);
        }

        .admin-details {
            padding: 15px;
        }

        .admin-details h3 {
            text-align: center;
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .admin-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        footer {
            background: white;
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Parantha</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <div class="admin-container">
        <h1>Our Administration Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="IMAGE.jpg" alt="CEO">
                <div class="admin-details">
                    <h3>Paranthaman</h3>
                    <p>CEO - Leading The Baratie with a vision of excellence and innovation in hospitality.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="IMAGE2.webp" alt="Manager">
                <div class="admin-details">
                    <h3>captain vijayakanth</h3>
                    <p>Manager - Ensures smooth operations and a great dining experience for all guests.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="IMAGE3.webp" alt="Master Chef">
                <div class="admin-details">
                    <h3>chef dhammu</h3>
                    <p>Master Chef - Brings authentic Italian flavors to every dish served.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="IMAGE4.webp" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Rashmika Manthana</h3>
                    <p>Assistant Managing Director - Supporting the team with strategy and execution excellence.</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>Designed by : Paranthaman S</p>
    </footer>

</body>
</html>
~~~

## OUTPUT:
![alt text](<Screenshot 2025-05-19 071841.png>)
![alt text](<Screenshot 2025-05-19 071901.png>)
![alt text](<Screenshot 2025-05-19 071921.png>)
![alt text](<Screenshot 2025-05-19 071933.png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
