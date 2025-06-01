<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Delivery Store</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f8f9fa;
      color: #333;
    }
    header {
      background: #007bff;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .container {
      padding: 2rem;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1.5rem;
    }
    .item {
      background: white;
      padding: 1rem;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      text-align: center;
    }
    .item img {
      max-width: 100%;
      border-radius: 8px;
    }
    .item h3 {
      margin: 0.5rem 0;
    }
    .item label {
      display: block;
      margin-top: 0.5rem;
    }
    .checkout {
      padding: 2rem;
      background: #fff;
      max-width: 600px;
      margin: 2rem auto;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .checkout input, .checkout textarea {
      width: 100%;
      padding: 0.75rem;
      margin: 0.5rem 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .checkout button {
      background: #007bff;
      color: white;
      padding: 1rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 1rem;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #f1f1f1;
    }
  </style>
</head>
<body>

  <header>
    <h1>QuickShop Delivery</h1>
    <p>Select items you'd like us to deliver</p>
  </header>

  <form method="POST" action="#">
    <div class="container">
      <div class="item">
        <img src="https://via.placeholder.com/200x150?text=Apples" alt="Apples">
        <h3>Apples</h3>
        <label>
          <input type="checkbox" name="items" value="Apples"> Select
        </label>
      </div>
      <div class="item">
        <img src="https://via.placeholder.com/200x150?text=Bread" alt="Bread">
        <h3>Bread</h3>
        <label>
          <input type="checkbox" name="items" value="Bread"> Select
        </label>
      </div>
      <div class="item">
        <img src="https://via.placeholder.com/200x150?text=Milk" alt="Milk">
        <h3>Milk</h3>
        <label>
          <input type="checkbox" name="items" value="Milk"> Select
        </label>
      </div>
      <div class="item">
        <img src="https://via.placeholder.com/200x150?text=Eggs" alt="Eggs">
        <h3>Eggs</h3>
        <label>
          <input type="checkbox" name="items" value="Eggs"> Select
        </label>
      </div>
    </div>

    <div class="checkout">
      <h2>Delivery Information</h2>
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="text" name="address" placeholder="Delivery Address" required />
      <input type="tel" name="phone" placeholder="Phone Number" required />
      <textarea name="notes" rows="4" placeholder="Additional Instructions (optional)"></textarea>
      <button type="submit">Place Order</button>
    </div>
  </form>

  <footer>
    &copy; 2025 QuickShop Delivery. All rights reserved.
  </footer>

</body>
</html>
