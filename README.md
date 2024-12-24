# webdproject

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StyleShop - Your Fashion Destination</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        /* Navigation */
        nav {
            background-color: #333;
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            color: white;
            font-size: 1.5rem;
            font-weight: bold;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #ffd700;
        }

        /* Hero Section */
        .hero {
            background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('/api/placeholder/1200/600');
            height: 60vh;
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
        }

        .hero-content h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        .cta-button {
            padding: 1rem 2rem;
            background-color: #ffd700;
            color: #333;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background-color 0.3s;
        }

        .cta-button:hover {
            background-color: #ffed4a;
        }

        /* Products Section */
        .products {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 1rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .product-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-image {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .product-info {
            padding: 1rem;
        }

        .product-title {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .product-price {
            color: #e44d26;
            font-weight: bold;
            margin-bottom: 1rem;
        }

        .add-to-cart {
            display: block;
            width: 100%;
            padding: 0.8rem;
            background-color: #333;
            color: white;
            text-align: center;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .add-to-cart:hover {
            background-color: #555;
        }

        /* Features Section */
        .features {
            background-color: #f5f5f5;
            padding: 4rem 1rem;
        }

        .features-grid {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            text-align: center;
        }

        .feature-card {
            padding: 2rem;
        }

        .feature-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            padding: 3rem 1rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section ul li {
            margin-bottom: 0.5rem;
        }

        .footer-section ul li a {
            color: white;
            text-decoration: none;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero-content h1 {
                font-size: 2rem;
            }

            .hero-content p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <nav>
        <div class="nav-container">
            <a href="#" class="logo">StyleShop</a>
            <div class="nav-links">
                <a href="#">Home</a>
                <a href="#">Products</a>
                <a href="#">Categories</a>
                <a href="#">Cart</a>
                <a href="#">Contact</a>
            </div>
        </div>
    </nav>

    <section class="hero">
        <div class="hero-content">
            <h1>Welcome to StyleShop</h1>
            <p>Discover the latest trends in fashion</p>
            <a href="#" class="cta-button">Shop Now</a>
        </div>
    </section>

    <section class="products">
        <h2 class="section-title">Featured Products</h2>
        <div class="product-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <img src="/api/placeholder/300/200" alt="Product 1" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Casual T-Shirt</h3>
                    <p class="product-price">$29.99</p>
                    <a href="#" class="add-to-cart">Add to Cart</a>
                </div>
            </div>

            <!-- Product 2 -->
            <div class="product-card">
                <img src="/api/placeholder/300/200" alt="Product 2" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Denim Jeans</h3>
                    <p class="product-price">$59.99</p>
                    <a href="#" class="add-to-cart">Add to Cart</a>
                </div>
            </div>

            <!-- Product 3 -->
            <div class="product-card">
                <img src="/api/placeholder/300/200" alt="Product 3" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Summer Dress</h3>
                    <p class="product-price">$49.99</p>
                    <a href="#" class="add-to-cart">Add to Cart</a>
                </div>
            </div>

            <!-- Product 4 -->
            <div class="product-card">
                <img src="/api/placeholder/300/200" alt="Product 4" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Sports Shoes</h3>
                    <p class="product-price">$79.99</p>
                    <a href="#" class="add-to-cart">Add to Cart</a>
                </div>
            </div>
        </div>
    </section>

    <section class="features">
        <div class="features-grid">
            <div class="feature-card">
                <div class="feature-icon">🚚</div>
                <h3>Free Shipping</h3>
                <p>On orders over $50</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">↩️</div>
                <h3>Easy Returns</h3>
                <p>30-day return policy</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">🔒</div>
                <h3>Secure Payment</h3>
                <p>Safe & encrypted</p>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>About Us</h3>
                <ul>
                    <li><a href="#">Our Story</a></li>
                    <li><a href="#">Careers</a></li>
                    <li><a href="#">Press</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>Customer Service</h3>
                <ul>
                    <li><a href="#">Contact Us</a></li>
                    <li><a href="#">Shipping Info</a></li>
                    <li><a href="#">Returns</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>Connect With Us</h3>
                <ul>
                    <li><a href="#">Facebook</a></li>
                    <li><a href="#">Instagram</a></li>
                    <li><a href="#">Twitter</a></li>
                </ul>
            </div>
        </div>
    </footer>
</body>
</html>
