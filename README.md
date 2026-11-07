# KAGA-BOT
AI Binary Trading Chart Learning and Signal Analysis App
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KAGA BOT</title>
<style>
body {
  background:#101827;
  color:white;
  font-family:Arial;
  text-align:center;
  padding:20px;
}
.box {
  background:#1e293b;
  padding:20px;
  border-radius:15px;
  margin:15px 0;
}
h1 {color:#00e5a0;}
button {
  padding:14px 25px;
  border:0;
  border-radius:10px;
  background:#00c98d;
  color:white;
  font-size:18px;
  margin:10px;
}
#signal {
  font-size:28px;
  font-weight:bold;
}
</style>
</head>
<body>

<h1>⚡ KAGA BOT</h1>
<p>AI Binary Chart Learning</p>

<div class="box">
<h2>Market Analysis</h2>
<p>শিক্ষামূলক অনুশীলনের জন্য ফলাফল</p>
<div id="signal">WAIT</div>
<button onclick="analyze()">ANALYZE</button>
</div>

<div class="box">
<h3>Learning Center</h3>
<p>Candlestick</p>
<p>Bullish / Bearish</p>
<p>Support / Resistance</p>
<p>Hammer / Doji</p>
</div>

<script>
function analyze() {
 document.getElementById("signal").innerText =
 "WAIT — চার্টের তথ্য যোগ করুন";
}
</script>

</body>
</html>
