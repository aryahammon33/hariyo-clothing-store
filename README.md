<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HARIYO | Clothing Store</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f8f8f8;
            color: #111;
        }

        header {
            background: #111;
            color: white;
            padding: 20px 6%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 25px;
            font-weight: bold;
            letter-spacing: 2px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
        }

        .hero {
            min-height: 600px;
            background:
                linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.45)),
                url("https://images.unsplash.com/photo-1445205170230-053b83016050?auto=format&fit=crop&w=1600&q=80");
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            padding: 8%;
            color: white;
        }

        .hero h1 {
            font-size: 60px;
            max-width: 600px;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 20px;
            margin-bottom: 30px;
        }

        .shop-button {
            background: white;
            color: black;
            padding: 15px 30px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
        }

        .products {
            padding: 70px 6%;
        }

        .products h2 {
            text-align: center;
            font-size: 40px;
            margin-bottom: 40px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 25px;
        }

        .product {
            background: white;
            padding-bottom: 20px;
        }

        .product img {
            width: 100%;
            height: 350px;
            object-fit: cover;
        }

        .product h3 {
            margin: 15px;
        }

        .price {
            margin: 0 15px;
            font-weight: bold;
            font-size: 18px;
        }

        .buy-button {
            display: block;
            margin: 15px;
            padding: 12px;
            width: calc(100% - 30px);
            background: #111;
            color: white;
            border: none;
            cursor: pointer;
        }

        footer {
            background: #111;
            color: white;
            text-align: center;
            padding: 30px;
            margin-top: 50px;
        }

        @media (max-width: 900px) {
            .product-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .hero h1 {
                font-size: 45px;
            }
        }

        @media (max-width: 600px) {
            nav {
                display: none;
            }

            .product-grid {
                grid-template-columns: 1fr 1fr;
                gap: 10px;
            }

            .product img {
                height: 250px;
            }
        }
    </style>
</head>

<body>

<header>
    <div class="logo">HARIYO</div>

    <nav>
        <a href="#">Home</a>
        <a href="#shop">Shop</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <div>
        <h1>Wear Your Confidence.</h1>

        <p>
            Discover stylish clothing made for your everyday look.
        </p>

        <a href="#shop" class="shop-button">
            SHOP NOW
        </a>
    </div>
</section>

<section class="products" id="shop">

    <h2>Latest Collection</h2>

    <div class="product-grid">

        <div class="product">

            <img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?auto=format&fit=crop&w=800&q=80">

            <h3>Classic White T-Shirt</h3>

            <p class="price">₦18,000</p>

            <button class="buy-button">
                Add to Cart
            </button>

        </div>

        <div class="product">

            <img src="https://images.unsplash.com/photo-1556821840-3a63f95609a7?auto=format&fit=crop&w=800&q=80">

            <h3>Oversized Hoodie</h3>

            <p class="price">₦35,000</p>

            <button class="buy-button">
                Add to Cart
            </button>

        </div>

        <div class="product">

            <img src="https://images.unsplash.com/photo-1595777457583-95e059d581b8?auto=format&fit=crop&w=800&q=80">

            <h3>Women's Dress</h3>

            <p class="price">₦42,000</p>

            <button class="buy-button">
                Add to Cart
            </button>

        </div>

        <div class="product">

            <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=800&q=80">

            <h3>Cargo Trousers</h3>

            <p class="price">₦30,000</p>

            <button class="buy-button">
                Add to Cart
            </button>

        </div>

    </div>

</section>

<footer id="contact">
    <p>© 2026 HARIYO. All Rights Reserved.</p>
</footer>

</body>
</html>
