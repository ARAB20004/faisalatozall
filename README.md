<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Faisal A to Z All - Online Store</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background-color: #218838; }
        header { background-color: #333; color: white; text-align: center; padding: 20px; }
        .container { max-width: 1200px; margin: 0 auto; padding: 20px; }
        .products { display: flex; flex-wrap: wrap; gap: 20px; }
        .product { background: orange; border: 1px solid #ddd; padding: 15px; width: 300px; text-align: center; }
        .product img { width: 100%; height: 200px; object-fit: cover; }
        button { background: #28a745; color: white; border: none; padding: 10px; cursor: pointer; }
        button:hover { background: #28a745; }
        #cart { margin-top: 20px; background: white; padding: 15px; border: 1px solid #ddd; }
        footer { background: #333; color: gray; text-align: low; padding: 10px; margin-top: 20px; }
    </style>
</head>
<body>
    <header>
        <h1>Faisal A to Z All</h1>
        <p>Your One-Stop Shop for Everything!</p>
    </header>
    
    <div class="container">
        <h2>Our Products</h2>
        <div class="products">
            <div class="product">
                <img src="https://via.placeholder.com/300x200?text=Product+A" alt="Product A">
                <h3>Product A</h3>
                <p>Price: $10</p>
                <button onclick="addToCart('Product A', 15)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://via.placeholder.com/300x200?text=Product+B" alt="Product B">
                <h3>Product B</h3>
                <p>Price: $15</p>
                <button onclick="addToCart('Product B', 10)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://via.placeholder.com/300x200?text=Product+C" alt="Product C">
                <h3>Product C</h3>
                <p>Price: $20</p>
                <button onclick="addToCart('Product C', 20)">Add to Cart</button>
            </div>
            <!-- Add more products here -->
        </div>
        
        <div id="cart">
            <h3>Shopping Cart</h3>
            <ul id="cart-items"></ul>
            <p>Total: $<span id="total">0</span></p>
            <button onclick="checkout()">Checkout</button>
        </div>
    </div>
    
    <footer>
        <p>Contact: faisalansari05713@gmail.com | Phone: +91-90220-96145</p>
    </footer>
    
    <script>
        let cart = [];
        let total = 0;
        
        function addToCart(name, price) {
            cart.push({ name, price });
            total += price;
            updateCart();
        }
        
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            cartItems.innerHTML = '';
            cart.forEach(item => {
                const li = document.createElement('li');
                li.textContent = `₹{case} - $${item.price}`;
                cartItems.appendChild(li);
            });
            document.getElementById('total').textContent = total;
        }
        
        function checkout() {
            alert('Checkout feature not implemented. Integrate with a payment gateway like PayPal or Stripe!');
        }
    </script>
</body>
</html>
<address></address>Add:  
38/2/1/G1 Ghunghat Nagar Near Noori Masjid Bhiwandi Thane Maharashtra-421302
<footer>
    <p>&copy; 2025 Faisal A to Z All. All rights reserved. No part of this website may be reproduced, distributed, or transmitted in any form or by any means, including photocopying, recording, or all types of product sell on my name basic methods, without the prior written permission of the owner, except in the case of brief quotations embodied in critical reviews and certain other noncommercial uses permitted by copyright law.</p>
    <p>Contact: faisalansari05713@gmail.com | Designed by [FAISAL ANSARI]</p>
</footer>


