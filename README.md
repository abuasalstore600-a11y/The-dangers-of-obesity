<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>التوعية بالسمنة</title>

<style>

body{
font-family:Arial;
direction:rtl;
margin:0;
background:#f2f2f2;
}

header{
background:#34495e;
color:white;
text-align:center;
padding:25px;
}

nav{
background:#2c3e50;
padding:10px;
text-align:center;
}

nav a{
color:white;
margin:10px;
text-decoration:none;
font-size:18px;
}

.container{
width:80%;
margin:auto;
background:white;
padding:20px;
margin-top:20px;
border-radius:10px;
}

h2{
color:#2c3e50;
}

button{
background:#27ae60;
color:white;
border:none;
padding:10px 20px;
font-size:16px;
border-radius:5px;
cursor:pointer;
}

input{
padding:8px;
margin:5px;
}

footer{
text-align:center;
padding:20px;
margin-top:20px;
background:#34495e;
color:white;
}

</style>
</head>

<body>

<header>
<h1>موقع التوعية بالسمنة</h1>
<p>تعرف على أسباب السمنة وكيفية الوقاية منها</p>
</header>

<nav>
<a href="#">الرئيسية</a>
<a href="#">الأسباب</a>
<a href="#">الأضرار</a>
<a href="#">الحلول</a>
</nav>

<div class="container">

<h2>ما هي السمنة؟</h2>
<p>
السمنة هي زيادة كبيرة في الدهون في الجسم وقد تؤدي إلى مشاكل صحية مثل أمراض القلب والسكري.
</p>

<h2>أسباب السمنة</h2>
<ul>
<li>تناول الطعام بكثرة</li>
<li>قلة النشاط البدني</li>
<li>الوجبات السريعة</li>
<li>العوامل الوراثية</li>
</ul>

<h2>أضرار السمنة</h2>
<ul>
<li>السكري</li>
<li>أمراض القلب</li>
<li>ارتفاع ضغط الدم</li>
<li>مشاكل المفاصل</li>
</ul>

<h2>احسب مؤشر كتلة الجسم BMI</h2>

<input id="w" placeholder="الوزن بالكيلو">
<input id="h" placeholder="الطول بالمتر">

<br><br>

<button onclick="bmi()">احسب</button>

<p id="result"></p>

</div>

<footer>
<p>موقع تعليمي عن السمنة</p>
</footer>

<script>

function bmi(){

let w=document.getElementById("w").value
let h=document.getElementById("h").value

let r=w/(h*h)

document.getElementById("result").innerHTML="BMI = "+r.toFixed(2)

}

</script>

</body>
</html>
