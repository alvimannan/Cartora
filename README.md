<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cartora - Online Product Store</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f4f4f4; }
    header { background: #222; color: #fff; padding: 20px 0; text-align: center; }
    nav ul { list-style: none; padding: 0; display: flex; justify-content: center; gap: 20px; }
    nav ul li { display: inline; }
    nav ul li a { color: white; text-decoration: none; font-weight: bold; }
    .hero { background: #333; color: white; padding: 60px 20px; text-align: center; }
    .products { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; padding: 20px; }
    .product { background: white; padding: 15px; border-radius: 10px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); text-align: center; }
    .product img { max-width: 100%; border-radius: 10px; }
    .product h3 { margin: 10px 0; }
    .about, .contact, .order { padding: 20px; background: white; margin: 20px; border-radius: 10px; }
    form { display: grid; gap: 10px; }
    input, select, textarea { padding: 10px; border: 1px solid #ccc; border-radius: 5px; }
    button { padding: 10px; background: #222; color: white; border: none; border-radius: 5px; cursor: pointer; }
    footer { text-align: center; background: #222; color: white; padding: 10px 0; margin-top: 20px; }
  </style>
</head>
<body>
  <header>
    <h1>Cartora</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#order">Order</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero" id="home">
    <h2>Welcome to Cartora</h2>
    <p>Your one-stop online product store</p>
  </section>

  <section class="products" id="products">
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 1">
      <h3>Product 1</h3>
      <p>$10.00</p>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 2">
      <h3>Product 2</h3>
      <p>$15.00</p>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="Product 3">
      <h3>Product 3</h3>
      <p>$20.00</p>
    </div>
  </section>

  <section class="order" id="order">
    <h2>Place Your Order</h2>
    <form action="https://formspree.io/f/mnqezvka" method="POST">
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="tel" name="phone" placeholder="Phone Number" required>
      <input type="text" name="address" placeholder="Delivery Address" required>
      <input type="text" name="product" placeholder="Product Name" required>
      <input type="number" name="quantity" placeholder="Quantity" required>
      <select name="payment_method" required>
        <option value="">Select Payment Method</option>
        <option value="Bkash">Bkash</option>
        <option value="Nagad">Nagad</option>
        <option value="Debit Card">Debit Card</option>
        <option value="Credit Card">Credit Card</option>
      </select>
      <textarea name="trxid" placeholder="Transaction ID or Payment Note" required></textarea>
      <button type="submit">Submit Order</button>
    </form>
    <p><strong>Bkash/Nagad Number:</strong> 01XXXXXXXXX</p>
  </section>

  <section class="about" id="about">
    <h2>About Us</h2>
    <p>Cartora is an online platform where you can find quality products at affordable prices. We connect buyers and sellers to make e-commerce smooth and easy.</p>
  </section>

  <section class="contact" id="contact">
    <h2>Contact Us</h2>
    <p>Email: support@cartora.com</p>
    <p>Phone: +880 1234 567890</p>
  </section>

  <footer>
    <p>&copy; 2025 Cartora. All rights reserved.</p>
  </footer>
</body>
</html>
