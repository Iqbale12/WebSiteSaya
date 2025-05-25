<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Baju Style - Toko Pakaian Trendy</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Poppins', sans-serif;
      background: #f9f9f9;
      color: #333;
      line-height: 1.6;
    }
    header {
      background: linear-gradient(90deg,#f0a500 0,#222 80%);
      color: #fff;
      padding: 2.5rem 1rem 2rem 1rem;
      text-align: center;
      position: relative;
      box-shadow: 0 2px 16px rgba(0,0,0,0.12);
    }
    .logo {
      width: 60px; height: 60px; object-fit: contain; border-radius: 12px;
      position: absolute; left: 1.5rem; top: 2rem;
      background: #fff;
      border: 2px solid #f0a500;
    }
    nav {
      margin: 0 auto 1rem;
      display: flex;
      justify-content: center;
      gap: 2rem;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 500;
      font-size: 1.1rem;
      transition: color .2s;
      padding-bottom: 2px;
      border-bottom: 2px solid transparent;
    }
    nav a:hover {
      color: #f0a500;
      border-bottom: 2px solid #f0a500;
    }
    header h1 {
      margin: 0;
      font-weight: 700;
      font-size: 2.7rem;
      letter-spacing: 2px;
      text-shadow: 1px 2px 12px rgba(0,0,0,0.08);
    }
    header p {
      margin: 0.6rem 0 0;
      font-weight: 400;
      font-size: 1.25rem;
      color: #ffe49f;
      letter-spacing: 1.5px;
      text-shadow: 1px 2px 8px rgba(0,0,0,0.05);
    }
    main {
      max-width: 1200px;
      margin: 2.5rem auto;
      padding: 0 1rem;
    }
    section#products {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap: 2rem;
    }
    .product-card {
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.10);
      transition: transform 0.3s, box-shadow 0.3s;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      border: 1.5px solid #f0a50011;
      position: relative;
    }
    .product-card:hover {
      transform: translateY(-8px) scale(1.018);
      box-shadow: 0 12px 28px rgba(0,0,0,0.15);
      border-color: #f0a50033;
    }
    .product-image {
      width: 100%;
      height: 260px;
      object-fit: cover;
      border-bottom: 1px solid #eee;
      border-radius: 16px 16px 0 0;
      transition: transform .25s;
      background: #f9f9f9;
    }
    .product-card:hover .product-image {
      transform: scale(1.04);
      filter: brightness(0.95) contrast(1.06);
    }
    .badge {
      position: absolute;
      top: 14px;
      left: 14px;
      background: #f0a500;
      color: #222;
      padding: 5px 12px;
      border-radius: 8px;
      font-size: 0.95rem;
      font-weight: 600;
      box-shadow: 0 2px 6px #0001;
      letter-spacing: 1px;
    }
    .product-info {
      padding: 1rem 1.2rem;
      flex: 1;
      display: flex;
      flex-direction: column;
    }
    .product-name {
      font-weight: 600;
      font-size: 1.18rem;
      margin: 0 0 0.5rem;
      color: #222;
    }
    .product-desc {
      font-weight: 300;
      font-size: 1rem;
      flex-grow: 1;
      color: #555;
      margin-bottom: 1rem;
    }
    .product-price {
      font-weight: 700;
      font-size: 1.13rem;
      color: #f0a500;
      margin-bottom: 1rem;
    }
    .btn-buy {
      background: linear-gradient(90deg,#f0a500 70%,#ffe49f 100%);
      border: none;
      border-radius: 5px;
      padding: 0.75rem 1.6rem;
      font-weight: 700;
      font-size: 1rem;
      color: #222;
      cursor: pointer;
      transition: background 0.25s, color 0.25s;
      align-self: flex-start;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      box-shadow: 0 2px 12px #f0a50018;
      margin-bottom: 4px;
    }
    .btn-buy:hover, .btn-buy:focus {
      background: linear-gradient(90deg,#d18e00 60%,#f0a500 100%);
      color: #fff;
      outline: none;
    }
    footer {
      background: #222;
      color: #aaa;
      text-align: center;
      padding: 2rem 1rem 1.3rem;
      font-size: 1rem;
      margin-top: 4rem;
      border-top: 4px solid #f0a500;
    }
    .footer-social {
      margin-top: .7rem;
    }
    .footer-social a {
      color: #f0a500;
      margin: 0 7px;
      text-decoration: none;
      font-size: 1.1rem;
      transition: color .2s;
    }
    .footer-social a:hover { color: #fff; text-decoration: underline; }
    @media (max-width: 700px) {
      header h1 { font-size: 2rem; }
      header p { font-size: 1.05rem; }
      .product-image { height: 180px; }
      .logo { position: static; display: block; margin: 0 auto 1rem;}
      nav { flex-direction: column; gap: 1rem; }
    }
  </style>
</head>
<body>
  <header>
    <img src="https://i.ibb.co/4Z1L4Qn/logo-baju.png" alt="Logo Baju Style" class="logo" />
    <nav>
      <a href="#">Home</a>
      <a href="#products">Produk</a>
      <a href="#">Tentang Kami</a>
      <a href="#">Kontak</a>
    </nav>
    <h1>Baju Style</h1>
    <p>Trendy Clothing for Every Occasion</p>
  </header>
  <main>
    <section id="products">
      <article class="product-card">
        <span class="badge">Best Seller</span>
        <img class="product-image" src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c?auto=format&fit=crop&w=400&q=80" alt="Kaos Putih Santai, bahan katun lembut, cocok untuk acara santai." />
        <div class="product-info">
          <h2 class="product-name">Casual White T-Shirt</h2>
          <p class="product-desc">Kaos katun putih super lembut, cocok untuk acara santai dan harian.</p>
          <div class="product-price">Rp 299.000</div>
          <button class="btn-buy" onclick="buyProduct('Casual White T-Shirt')">Add to Cart</button>
        </div>
      </article>
      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1521334884684-d80222895322?auto=format&fit=crop&w=400&q=80" alt="Jaket Denim Modern, cocok untuk layering." />
        <div class="product-info">
          <h2 class="product-name">Denim Jacket</h2>
          <p class="product-desc">Jaket denim klasik dengan potongan modern, pas untuk segala gaya.</p>
          <div class="product-price">Rp 999.000</div>
          <button class="btn-buy" onclick="buyProduct('Denim Jacket')">Add to Cart</button>
        </div>
      </article>
      <article class="product-card">
        <span class="badge">New</span>
        <img class="product-image" src="https://images.unsplash.com/photo-1490367532201-b9bc1dc483f6?auto=format&fit=crop&w=400&q=80" alt="Dress Floral musim panas." />
        <div class="product-info">
          <h2 class="product-name">Floral Summer Dress</h2>
          <p class="product-desc">Dress floral ringan dan airy, cocok untuk pesta dan hangout musim panas.</p>
          <div class="product-price">Rp 749.000</div>
          <button class="btn-buy" onclick="buyProduct('Floral Summer Dress')">Add to Cart</button>
        </div>
      </article>
      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1503602642458-232111445657?auto=format&fit=crop&w=400&q=80" alt="Kemeja Formal Pria, bahan katun premium." />
        <div class="product-info">
          <h2 class="product-name">Men's Formal Shirt</h2>
          <p class="product-desc">Kemeja formal pria, bahan katun halus, cocok untuk kerja atau event resmi.</p>
          <div class="product-price">Rp 599.000</div>
          <button class="btn-buy" onclick="buyProduct('Men\'s Formal Shirt')">Add to Cart</button>
        </div>
      </article>
      <article class="product-card">
        <img class="product-image" src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f?auto=format&fit=crop&w=400&q=80" alt="Hoodie hangat dan nyaman." />
        <div class="product-info">
          <h2 class="product-name">Cozy Hoodie</h2>
          <p class="product-desc">Hoodie lembut dari fleece tebal, nyaman untuk hari dingin atau santai.</p>
          <div class="product-price">Rp 449.000</div>
          <button class="btn-buy" onclick="buyProduct('Cozy Hoodie')">Add to Cart</button>
        </div>
      </article>
    </section>
  </main>
  <footer>
    &copy; <span id="year"></span> Baju Style.<br>
    Kontak: <a href="mailto:info@bajustyle.com">info@bajustyle.com</a><br>
    <span class="footer-social">
      Follow us:
      <a href="https://instagram.com" target="_blank" rel="noopener">Instagram</a>
      |
      <a href="https://facebook.com" target="_blank" rel="noopener">Facebook</a>
      |
      <a href="https://twitter.com" target="_blank" rel="noopener">Twitter</a>
    </span>
  </footer>
  <script>
    // Update year automatically
    document.getElementById('year').textContent = new Date().getFullYear();
    function buyProduct(productName) {
      alert(productName + ' telah ditambahkan ke keranjang Anda!');
    }
  </script>
</body>
</html>
