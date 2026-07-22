# Edirisingha-Food-Cabin
Restaurant website for Edirisingha Food Cabin
<!DOCTYPE html>
<html>
<head>
<title>Food Cabin - Ordering</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    font-family: Arial;
    background:#fff8f0;
    margin:0;
}
header{
    background:#ff6b00;
    color:white;
    text-align:center;
    padding:20px;
}
.container{
    padding:20px;
}
.card{
    background:white;
    padding:15px;
    margin:10px 0;
    border-radius:10px;
    box-shadow:0 0 5px #ccc;
}
button{
    background:#25D366;
    color:white;
    border:none;
    padding:15px;
    width:100%;
    border-radius:8px;
    font-size:18px;
}
input{
    width:100%;
    padding:10px;
    margin:5px 0;
}
</style>

</head>

<body>

<header>
<h1>🍔 Food Cabin</h1>
<p>Fresh Food - Easy Ordering</p>
</header>

<div class="container">

<div class="card">
<h3>🍳 Bittra</h3>
<p>Price: Rs.25</p>
<input id="egg" type="number" value="0">
</div>

<div class="card">
<h3>🍱 Special Food</h3>
<p>Price: Rs.100</p>
<input id="food" type="number" value="0">
</div>

<div class="card">
<h3>Customer Details</h3>
<input id="name" placeholder="Your Name">
<input id="phone" placeholder="Phone Number">
</div>

<button onclick="order()">Order via WhatsApp</button>

<p>
📍 Pickup: Udagaladeniya - Medagaladeniya - Rambukkana<br>
⏰ Time: 4 PM - 9 PM
</p>

</div>


<script>

function order(){

let name=document.getElementById("name").value;
let phone=document.getElementById("phone").value;

let eggs=document.getElementById("egg").value;
let food=document.getElementById("food").value;

let msg=
"Food Cabin Order%0A%0A"+
"Name: "+name+"%0A"+
"Phone: "+phone+"%0A"+
"Bittra: "+eggs+"%0A"+
"Food: "+food;

window.open("https://wa.me/94717574178?text="+msg);

}

</script>

</body>
</html>
