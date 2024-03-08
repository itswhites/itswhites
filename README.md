<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nomx Store</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #232f3e;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
        }
        nav a:hover {
            text-decoration: underline;
        }
        section {
            padding: 20px;
        }
        .product {
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #fff;
            padding: 20px;
            margin-bottom: 20px;
        }
        .product img {
            max-width: 100%;
            height: auto;
        }
        footer {
            background-color: #232f3e;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Nomx Store</h1>
    </header>
    <nav>
        <a href="#">Home</a>
        <a href="#">Shop</a>
        <a href="#">Contact</a>
    </nav>
    <section>
        <div class="product">
            <img src="product1.jpg" alt="Product 1">
            <h2>Product 1</h2>
            <p>Description of Product 1.</p>
            <p>$19.99</p>
            <button>Add to Cart</button>
        </div>
        <div class="product">
            <img src="product2.jpg" alt="Product 2">
            <h2>Product 2</h2>
            <p>Description of Product 2.</p>
            <p>$29.99</p>
            <button>Add to Cart</button>
        </div>
        <!-- Add more products as needed -->
    </section>
    <footer>
        <p>&copy; 2024 Nomx Store. All rights reserved.</p>
    </footer>
</body>
</html>
