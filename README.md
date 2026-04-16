# buyybridge
My global shopping service website
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Buy Bridge Store</title>

<style>
body {
  font-family: Arial;
  margin: 0;
  background: #f4f4f4;
}

header {
  background: #2c3e50;
  color: white;
  padding: 15px;
  text-align: center;
}

.products {
  display: flex;
  justify-content: center;
  gap: 20px;
  padding: 20px;
}

.product {
  background: white;
  padding: 15px;
  border-radius: 10px;
  width: 200px;
  text-align: center;
}

button {
  background: #3498db;
  color: white;
  border: none;
  padding: 10px;
  cursor: pointer;
}

.cart {
  position: fixed;
  top: 10px;
  right: 10px;
  background: white;
  padding: 10px;
  border-radius: 10px;
}
</style>
</head>

<body>

<header>
  <h1>Buy Bridge 🛒</h1>
</header>

<div class="cart">
  🛍 Cart: <span id="cart-count">0</span>
</div>

<div class="products">

  <div class="product">
    <h3>Shoes</h3>
    <p>$50</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>

  <div class="product">
    <h3>Watch</h3>
    <p>$80</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>

  <div class="product">
    <h3>Headphones</h3>
    <p>$40</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>

</div>

<script>
let count = 0;

function addToCart() {
  count++;
  document.getElementById("cart-count").innerText = count;
}
</script>

</body>
</html>
