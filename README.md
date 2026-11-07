# KAGA-BOT
AI Binary Trading Chart Learning and Signal Analysis App
<!DOCTYPE html><html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KAGA BOT</title>
<style>
*{box-sizing:border-box}
body{
background:#101827;
color:white;
font-family:Arial,sans-serif;
text-align:center;
padding:15px;
margin:0;
}
h1{color:#00e5a0;font-size:32px}
.box{
background:#1e293b;
padding:20px;
border-radius:15px;
margin:15px 0;
}
button{
padding:14px 25px;
border:0;
border-radius:10px;
background:#00c98d;
color:white;
font-size:18px;
margin:10px;
cursor:pointer;
}
select{
padding:12px;
border-radius:8px;
width:90%;
margin:10px;
}
#signal{
font-size:27px;
font-weight:bold;
color:#00e5a0;
margin:20px;
}
p{line-height:1.7}
</style>
</head><body><h1>⚡ KAGA BOT</h1>
<p>AI Binary Trading Chart Learning</p><div class="box">
<h2>📊 Market Analysis</h2>
<p>শিক্ষামূলক চার্ট বিশ্লেষণ</p><select id="trend">
<option value="">Market Trend নির্বাচন করুন</option>
<option value="up">Bullish (Uptrend)</option>
<option value="down">Bearish (Downtrend)</option>
<option value="side">Sideways</option>
</select><select id="candle">
<option value="">Candlestick নির্বাচন করুন</option>
<option value="bull">Bullish Candle</option>
<option value="bear">Bearish Candle</option>
<option value="doji">Doji</option>
<option value="hammer">Hammer</option>
</select><button onclick="analyze()">🔍 ANALYZE</button>

<div id="signal">WAIT</div>
<p id="message">বিশ্লেষণের জন্য তথ্য নির্বাচন করুন।</p>
</div><div class="box">
<h2>📚 Learning Center</h2>
<p>🕯️ Candlestick</p>
<p>🟢 Bullish / 🔴 Bearish</p>
<p>📈 Support / Resistance</p>
<p>🔨 Hammer / Doji</p>
<p>📊 Timeframe</p>
<p>📉 Trend Analysis</p>
</div><div class="box">
<h3>⚠️ Important Notice</h3>
<p>এটি একটি শিক্ষামূলক অনুশীলন অ্যাপ। ফলাফল নিশ্চিত ট্রেডিং সিগন্যাল বা লাভের নিশ্চয়তা নয়।</p>
</div><script>
function analyze(){
let trend=document.getElementById("trend").value;
let candle=document.getElementById("candle").value;
let signal=document.getElementById("signal");
let message=document.getElementById("message");

if(!trend || !candle){
signal.innerText="WAIT";
message.innerText="প্রথমে Market Trend এবং Candlestick নির্বাচন করুন।";
return;
}

if(trend==="side" || candle==="doji"){
signal.innerText="WAIT";
message.innerText="বাজারে স্পষ্ট দিকনির্দেশনা নেই। আরও চার্ট শেখার অনুশীলন করুন।";
}
else if(trend==="up" && candle==="bull"){
signal.innerText="BULLISH";
message.innerText="উর্ধ্বমুখী প্রবণতা ও Bullish Candle মিলেছে। এটি নিশ্চিত পূর্বাভাস নয়।";
}
else if(trend==="down" && candle==="bear"){
signal.innerText="BEARISH";
message.innerText="নিম্নমুখী প্রবণতা ও Bearish Candle মিলেছে। এটি নিশ্চিত পূর্বাভাস নয়।";
}
else{
signal.innerText="WAIT";
message.innerText="চার্টের তথ্য পরস্পরের সঙ্গে মিলছে না।";
}
}
</script></body>
</html>
