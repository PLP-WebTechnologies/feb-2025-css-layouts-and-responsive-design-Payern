# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨


ANSWER 

 Step 1: Create the HTML File (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Webpage</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header Section -->
    <header>
        <h1>Welcome to My Responsive Webpage</h1>
    </header>

    <!-- Navigation Section -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Content Section -->
    <main>
        <section id="home">
            <h2>Home</h2>
            <p>This is the home section of the webpage. Here you can find the latest updates and news.</p>
        </section>
        <section id="about">
            <h2>About</h2>
            <p>Learn more about our mission and values in the about section.</p>
        </section>
        <section id="services">
            <h2>Services</h2>
            <p>Explore the services we offer to our customers.</p>
        </section>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>Contact us at: contact@example.com</p>
    </footer>
</body>
</html>
```

 Step 2: Create the CSS File (`styles.css`)

```css
/* Basic Styling */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
}

/* Header Styling */
header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}

/* Navigation Styling */
nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    background-color: #333;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    padding: 10px;
}

nav ul li a:hover {
    background-color: #111;
}

/* Main Content Styling */
main {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
}

section {
    margin: 20px 0;
    width: 80%;
}

/* Footer Styling */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    width: 100%;
}

/* Media Queries for Responsiveness */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    main {
        padding: 10px;
    }

    section {
        width: 100%;
    }
}

@media (max-width: 480px) {
    header h1 {
        font-size: 1.5em;
    }

    nav ul li {
        margin: 5px 0;
    }

    nav ul li a {
        padding: 8px;
    }
}
