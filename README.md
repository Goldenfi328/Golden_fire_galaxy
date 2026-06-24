<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Golden Fire Jewelries and Watches</title>
<style>
body{font-family:Arial,sans-serif;margin:0;background:#fff;color:#222}
header{background:#000;color:#ffd700;padding:20px;text-align:center}
header h1{margin:0;font-size:24px}
.products{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:20px;padding:20px}
.card{border:1px solid #ddd;border-radius:12px;overflow:hidden;text-align:center}
.card img{width:100%;height:250px;object-fit:cover}
.card h3{margin:10px 0 5px}
.card p{margin:5px 0;color:#555}
.btn{display:inline-block;background:#25D366;color:#fff;padding:10px 20px;margin:10px 0 15px;border-radius:8px;text-decoration:none;font-weight:bold}
footer{text-align:center;padding:20px;background:#f5f5f5;margin-top:20px}
</style>
</head>
<body>
<header>
<h1>Golden Fire 🔥 Jewelries and Watches</h1>
<p>Genuine Watches & Gold Jewelry | WhatsApp Orders | Fast Delivery Nationwide</p>
</header>

<div class="products" id="products"></div>

<footer>
<p>© 2026 Golden Fire. Order via WhatsApp</p>
</footer>

<script>
const products = [
  "Reward VIP Watch|₦25,000|https://i.imgur.com/placeholder1.jpg|Sport Chronograph, Water resistant",
  "Poedagar Gold Watch|₦32,000|https://i.imgur.com/placeholder2.jpg|Luxury Quartz, Stainless steel"
];

const container = document.getElementById('products');
products.forEach(p => {
  const [name, price, img, desc] = p.split('|');
  container.innerHTML += `
  <div class="card">
    <img src="${img}" alt="${name}">
    <h3>${name}</h3>
    <p>${price}</p>
    <p style="font-size:14px">${desc}</p>
    <a class="btn" href="https://wa.me/2348021254993?text=Hi%20Golden%20Fire,%20I%20want%20to%20order%20${encodeURIComponent(name)}" target="_blank">Order on WhatsApp</a>
  </div>`;
});
</script>
</body>
</html>
