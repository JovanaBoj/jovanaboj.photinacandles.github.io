<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Photina Candles</title>
</head>
<body>
    <header>
        <h1>Welcome to Photina Candles</h1>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Us</h2>
        <p>At Photina Candles, we create high-quality handcrafted candles that bring warmth, light, and joy to every occasion.</p>
    </section>

    <section id="products">
        <h2>Our Candles</h2>
        <div class="product">
            <img src="candle1.jpg" alt="Candle 1">
            <h3>Vanilla Bliss</h3>
            <p>A soothing vanilla-scented candle perfect for creating a cozy atmosphere.</p>
            <button onclick="alert('Order Now!')">Order Now</button>
        </div>
        <div class="product">
            <img src="candle2.jpg" alt="Candle 2">
            <h3>Lavender Dreams</h3>
            <p>Relax with our calming lavender-scented candle.</p>
            <button onclick="alert('Order Now!')">Order Now</button>
        </div>
        <!-- Add more products as needed -->
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <input type="submit" value="Send">
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Photina Candles. All rights reserved.</p>
    </footer>
</body>
</html>
