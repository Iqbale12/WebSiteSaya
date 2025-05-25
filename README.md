<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Baju Style - Trendy Clothing Store</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f9f9f9;
      color: #333;
    }
    header {
      background: #222;
      color: #fff;
      padding: 2rem 1rem;
      text-align: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.15);
    }
    header h1 {
      margin: 0;
      font-weight: 600;
      font-size: 2.5rem;
      letter-spacing: 2px;
    }
    header p {
      margin: 0.5rem 0 0;
      font-weight: 300;
      font-size: 1.1rem;
      color: #f0a500;
      letter-spacing: 1.5px;
    }
    main {
      max-width: 1200px;
      margin: 2rem auto;
      padding: 0 1rem;
    }
    section#products {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap: 2rem;
    }
    .product-card {
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      overflow: hidden;
      display: flex;
      flex-direction: column;
    }
    .product-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 28px rgba(0,0,0,0.2);
    }
    .product-image {
      width: 100%;
      height: 250px;
      object-fit: cover;
      border-bottom: 1px solid #eee;
    }
    .product-info {
      padding: 1rem 1.2rem;
      flex: 1;
      display: flex;
      flex-direction: column;
    }
    .product-name {
      font-weight: 600;
      font-size: 1.2rem;
      margin: 0 0 0.5rem;
      color: #222;
    }
    .product-desc {
      font-weight: 300;
      font-size: 0.95rem;
      flex-grow: 1;
      color: #555;
      margin-bottom: 1rem;
    }
    .product-price {
      font-weight: 700;
      font-size: 1.1rem;
      color: #f0a500;
      margin-bottom: 1rem;
    }
    .btn-buy {
      background: #f0a500;
      border: none;
      border-radius: 5px;
      padding: 0.7rem 1.4rem;
      font-weight: 700;
      font-size: 1rem;
      color: #222;
      cursor: pointer;
      transition: background-color 0.25s ease;
      align-self: flex-start;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      text-decoration: none;
      user-select: none;
    }
    .btn-buy:hover {
      background: #d18e00;
      color: #fff;
    }
    footer {
      background: #222;
      color: #aaa;
      text-align: center;
      padding: 1.5rem 1rem;
      font-size: 0.9rem;
      margin-top: 4rem;
    }
    footer a {
      color: #f0a500;
      text-decoration: none;
    }
    footer a:hover {
      text-decoration: underline;
    }
    @media (max-width: 600px) {
      header h1 {
        font-size: 1.8rem;
      }
      .product-image {
        height: 200px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Baju Style</h1>
    <p>Trendy Clothing for Every Occasion</p>
  </header>
  <main>
    <section id="products">
      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c?auto=format&fit=crop&w=400&q=80" alt="Casual White T-Shirt" />
        <div class="product-info">
          <h2 class="product-name">Casual White T-Shirt</h2>
          <p class="product-desc">Soft cotton white t-shirt, perfect for casual outings and relaxed days.</p>
          <div class="product-price">$19.99</div>
          <button class="btn-buy" onclick="buyProduct('Casual White T-Shirt')">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1521334884684-d80222895322?auto=format&fit=crop&w=400&q=80" alt="Denim Jacket" />
        <div class="product-info">
          <h2 class="product-name">Denim Jacket</h2>
          <p class="product-desc">Classic denim jacket with modern fit, ideal for layering any outfit.</p>
          <div class="product-price">$69.99</div>
          <button class="btn-buy" onclick="buyProduct('Denim Jacket')">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1490367532201-b9bc1dc483f6?auto=format&fit=crop&w=400&q=80" alt="Floral Summer Dress" />
        <div class="product-info">
          <h2 class="product-name">Floral Summer Dress</h2>
          <p class="product-desc">Light and airy floral dress, perfect for summer parties and outings.</p>
          <div class="product-price">$49.99</div>
          <button class="btn-buy" onclick="buyProduct('Floral Summer Dress')">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1503602642458-232111445657?auto=format&fit=crop&w=400&q=80" alt="Men's Formal Shirt" />
        <div class="product-info">
          <h2 class="product-name">Men's Formal Shirt</h2>
          <p class="product-desc">Elegant formal shirt made with fine cotton for business or events.</p>
          <div class="product-price">$39.99</div>
          <button class="btn-buy" onclick="buyProduct('Men\'s Formal Shirt')">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f?auto=format&fit=crop&w=400&q=80" alt="Cozy Hoodie" />
        <div class="product-info">
          <h2 class="product-name">Cozy Hoodie</h2>
          <p class="product-desc">Comfortable hoodie made from warm fleece fabric, great for colder days.</p>
          <div class="product-price">$34.99</div>
          <button class="btn-buy" onclick="buyProduct('Cozy Hoodie')">Add to Cart</button>
        </div>
      </article>
    </section>
  </main>
  <footer>
    &copy; 2024 Bale Style. Follow us on 
    <a href="https://instagram.com" target="_blank" rel="noopener">Instagram</a> | 
    <a href="https://facebook.com" target="_blank" rel="noopener">Facebook</a> | 
    <a href="https://twitter.com" target="_blank" rel="noopener">Twitter</a>
  </footer>
  <script>
    function buyProduct(productName) {
      alert(productName + ' has been added to your cart!');
    }
  </script>
</body>
</html>

