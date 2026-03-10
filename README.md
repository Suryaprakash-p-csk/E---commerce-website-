<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tech Store</title>

<style>

body{
font-family: Arial;
margin:0;
background:#f4f4f4;
}

header{
background:#111;
color:white;
padding:20px;
text-align:center;
position:relative;
}

.cart-icon{
position:absolute;
right:20px;
top:20px;
font-size:18px;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:20px;
padding:30px;
}

.card{
background:white;
border-radius:12px;
box-shadow:0 4px 10px rgba(0,0,0,0.2);
padding:15px;
text-align:center;
transition:0.3s;
}

.card:hover{
transform:translateY(-5px);
}

.card img{
width:100%;
height:160px;
object-fit:cover;
border-radius:8px;
}

.price{
color:green;
font-weight:bold;
margin:10px 0;
}

button{
background:#ff6b00;
border:none;
color:white;
padding:10px 15px;
border-radius:6px;
cursor:pointer;
font-weight:bold;
}

button:hover{
background:#e65c00;
}

footer{
background:#111;
color:white;
text-align:center;
padding:15px;
}

</style>
</head>

<body>

<header>

<h1>Tech Store</h1>
<p>Simple E-Commerce Website</p>

<div class="cart-icon">
🛒 Cart (<span id="cartCount">0</span>)
</div>

</header>

<section class="products">

<div class="card">
<img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=500">
<h3>Laptop</h3>
<p>Powerful laptop for work and study</p>
<p class="price">₹50,000</p>
<button onclick="addToCart('Laptop')">Add to Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=500">
<h3>Smartphone</h3>
<p>Latest Android smartphone</p>
<p class="price">₹20,000</p>
<button onclick="addToCart('Smartphone')">Add to Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=500">
<h3>Headphones</h3>
<p>High quality sound</p>
<p class="price">₹3,000</p>
<button onclick="addToCart('Headphones')">Add to Cart</button>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1546868871-7041f2a55e12?w=500">
<h3>Smart Watch</h3>
<p>Track your fitness daily</p>
<p class="price">₹5,000</p>
<button onclick="addToCart('Smart Watch')">Add to Cart</button>
</div>

</section>

<footer>
© 2026 Tech Store
</footer>

<script>

let cartCount = 0;

function addToCart(product){

cartCount++;

document.getElementById("cartCount").textContent = cartCount;

alert(product + " added to cart!");

}

</script>

</body>
</html>
