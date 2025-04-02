# Shopping-website-
<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        .product {
            display: inline-block;
            border: 1px solid #ddd;
            padding: 10px;
            margin: 10px;
            width: 200px;
        }
        button {
            padding: 10px;
            background-color: #28a745;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Shopping Website</h1>
    <div class="product">
        <h2>Product 1</h2>
        <p>Price: $10</p>
        <button onclick="addToCart('Product 1', 10)">Add to Cart</button>
    </div>
    <div class="product">
        <h2>Product 2</h2>
        <p>Price: $15</p>
        <button onclick="addToCart('Product 2', 15)">Add to Cart</button>
    </div>
    <h2>Shopping Cart</h2>
    <ul id="cart"></ul><script>
    function addToCart(product, price) {
        let cart = document.getElementById("cart");
        let item = document.createElement("li");
        item.innerText = `${product} - $${price}`;
        cart.appendChild(item);
    }
</script>

</body>
</html>
