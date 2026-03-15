# mothers-day-card
my mothers day card for my mum
<!DOCTYPE html>
<html>
<head>
<title>Happy Mother's Day Mum ❤️</title>

<style>
body{
background: linear-gradient(pink, white);
font-family: Arial;
text-align:center;
padding-top:100px;
overflow:hidden;
}

h1{
font-size:50px;
color:#ff2e63;
}

p{
font-size:25px;
color:#333;
}

.heart{
position:absolute;
color:red;
font-size:30px;
animation: fall 5s linear infinite;
}

@keyframes fall{
0%{transform:translateY(-100px);}
100%{transform:translateY(100vh);}
}
</style>
</head>

<body>

<h1>💐 Happy Mother's Day Mum 💐</h1>

<p>
Thank you for loving me, helping me, and always being there for me.<br>
You are the best mum in the world! ❤️
</p>

<p>
Love from <br>
<b>Michael</b>
</p>

<script>
function createHeart(){
const heart = document.createElement("div");
heart.classList.add("heart");
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.animationDuration=(3+Math.random()*5)+"s";
document.body.appendChild(heart);

setTimeout(()=>{heart.remove();},5000);
}

setInterval(createHeart,300);
</script>

</body>
</html>
