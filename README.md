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
        <h1>Photina Candles</h1>
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
        <p>At Photina Candles, we craft high-quality, handcrafted candles that brighten every occasion. Customize your candle to make it truly yours!</p>
    </section>

    <section id="products">
        <h2>Our Custom Candles</h2>
        <div class="product">
            <h3>Choose Your Candle</h3>
            <label for="candle-type">Candle Type:</label>
            <select id="candle-type" onchange="updatePreview()">
                <option value="Soy">Soy Candle</option>
                <option value="Beeswax">Beeswax Candle</option>
                <option value="Scented">Scented Candle</option>
            </select>
            <br>
            <label for="candle-scent">Scent:</label>
            <select id="candle-scent" onchange="updatePreview()">
                <option value="Vanilla">Vanilla</option>
                <option value="Lavender">Lavender</option>
                <option value="Rose">Rose</option>
            </select>
            <br>
            <div id="preview" class="preview"></div>
            <button onclick="alert('Order Now!')">Order Now</button>
        </div>
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

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
    color: #333;
}

header {
    background-color: #fff;
    padding: 20px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

h1, h2 {
    color: #2c3e50;
}

section {
    padding: 40px;
    text-align: center;
}

.product {
    display: inline-block;
    margin: 20px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #fff;
    width: 250px;
}

.preview {
    margin-top: 15px;
    padding: 10px;
    border: 1px solid #2c3e50;
    background-color: #eaeaea;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #2c3e50;
    color: #fff;
}
function updatePreview() {
    const candleType = document.getElementById("candle-type").value;
    const candleScent = document.getElementById("candle-scent").value;
    const previewDiv = document.getElementById("preview");
    
    previewDiv.innerHTML = `<strong>Preview:</strong> ${candleType} Candle with ${candleScent} scent.`;
}
