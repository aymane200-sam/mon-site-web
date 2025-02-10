
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Samrani Élégance - Boutique en Ligne</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fdf6f0;
            color: #333;
        }

        header {
            background: linear-gradient(90deg, #2e4053, #4a69bd, #2e4053);
            color: #fff;
            padding: 30px 20px;
            text-align: center;
            border-bottom: 5px solid #e74c3c;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            animation: headerFadeIn 2s ease-out, gradientShift 10s infinite alternate;
        }

        @keyframes headerFadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }

        header h1 {
            font-size: 2.5em;
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            animation: textGlow 2s infinite alternate;
        }

        @keyframes textGlow {
            from { text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); }
            to { text-shadow: 0 0 20px rgba(255, 255, 255, 0.8), 0 0 40px rgba(255, 255, 255, 0.8); }
        }

        header p {
            margin: 10px 0 0;
            font-size: 1.1em;
            font-style: italic;
            animation: textSlideIn 1.5s ease-out 0.5s;
        }

        header .highlight {
            font-weight: bold;
            color: #e74c3c;
            text-decoration: underline;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
            padding: 10px 0;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 20px;
            font-weight: bold;
            font-size: 1em;
            transition: color 0.3s, transform 0.3s;
        }

        nav a:hover {
            color: #e74c3c;
            transform: scale(1.1);
        }

        .hero {
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(45deg, rgba(44, 62, 80, 0.9), rgba(52, 73, 94, 0.9)), url('https://via.placeholder.com/1200x400');
            background-size: cover;
            background-position: center;
            color: #fff;
            animation: heroFadeIn 2s ease-out;
        }

        @keyframes heroFadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .hero h1 {
            font-size: 2em;
            animation: textSlideIn 1.5s ease-out;
        }

        .hero p {
            font-size: 1.1em;
            animation: textSlideIn 1.5s ease-out 0.5s;
        }

        @keyframes textSlideIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            padding: 40px 20px;
        }

        .product {
            background-color: #fff;
            border: 1px solid #ddd;
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .product:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.25);
        }

        .product img {
            max-width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
        }

        .product h2 {
            font-size: 1.4em;
            margin: 15px 0;
            color: #2c3e50;
        }

        .product p {
            font-size: 1em;
            margin: 10px 0;
            color: #666;
        }

        .product button {
            background-color: #e74c3c;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }

        .product button:hover {
            background-color: #c0392b;
            transform: scale(1.1);
        }

        footer {
            background-color: #2c3e50;
            color: #fff;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.2);
        }

        footer p {
            margin: 0;
            font-size: 1em;
        }
    </style>
</head>
<body>
    <header>
        <h1>Parfum Élégance</h1>
        <p>Des parfums qui parlent de vous. <span class="highlight">Testeurs originaux et professionnels.</span></p>
    </header>

    <nav>
        <a href="#">Accueil</a>
        <a href="#produits">Produits</a>
        <a href="#contact">Contact</a>
        <a href="#about">À propos</a>
    </nav>

    <section class="hero">
        <h1>Votre parfum, votre élégance</h1>
        <p>Explorez notre collection exclusive de parfums.</p>
    </section>

    <section id="produits" class="products">
        <div class="product">
            <img src="https://i1.perfumesclub.com/grande/185660.jpg" alt="Parfum 1">
            <h2>Valentino</h2>
            <p>Prix : 39€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://images.bergdorfgoodman.com/ca/1/product_assets/C/0/7/Q/U/BGC07QU_az.jpg" alt="Parfum 2">
            <h2>Black Orchid</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://cdn.shopify.com/s/files/1/0259/7733/products/tom-ford-ombre-leather_grande.png?v=1557106907" alt="Parfum 3">
            <h2>Ombré Leather</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://www.fragrancefind.co.za/wp-content/uploads/2022/04/Givenchy-Gentleman-EDP-Reserve-Privee-100ml.jpg" alt="Parfum 4">
            <h2>Gentleman Givenchy</h2>
            <p>Prix : 40€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://fraguru.com/himg/o.gPYjLu8LSls.jpg" alt="Parfum 5">
            <h2>Oud Minérale</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://holtrenfrew.scene7.com/is/image/HoltRenfrew1/u_888066114325_03" alt="Parfum 6">
            <h2>Bitter Peach</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://pinoyfragrance.com/cdn/shop/products/Tom-Ford-Costa-Azzurra.jpg?v=1618836978" alt="Parfum 7">
            <h2>Costa Azzura</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="https://cdn.jarrolds.co.uk/brands/tom-ford/update/888066089302_2.jpg" alt="Parfum 8">
            <h2>White Suede</h2>
            <p>Prix : 49€</p>
            <button>Ajouter au panier</button>
        </div>
    </section>

    <section id="contact" style="text-align:center; padding: 20px;">
        <h2>Contactez-nous</h2>
        <p>Pour toute question, appelez-nous au : <a href="tel:0632362353" style="color: #e74c3c; text-decoration: none;">06 32 36 23 53</a></p>
    </section>

    <footer>
        <p>&copy; 2025 Parfum Élégance. Tous droits réservés.</p>
    </footer>
</body>
</html>
