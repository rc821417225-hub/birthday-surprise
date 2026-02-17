<!DOCTYPE html>
<html>
<head>
<title>Birthday Surprise 🎂</title>

<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  font-family:Arial;
  background:linear-gradient(45deg,#ff4e50,#fc913a,#f9d423);
  background-size:400% 400%;
  animation:bgMove 8s infinite alternate;
  color:white;
  text-align:center;
}

@keyframes bgMove{
  0%{background-position:left;}
  100%{background-position:right;}
}

.container{
  background:rgba(0,0,0,0.4);
  padding:30px;
  border-radius:20px;
}

button{
  padding:15px 25px;
  font-size:18px;
  border:none;
  border-radius:10px;
  background:#fff;
  color:#ff4e50;
  cursor:pointer;
  font-weight:bold;
}

h1{
  font-size:40px;
  animation:pop 1.5s infinite alternate;
}

@keyframes pop{
  from{transform:scale(1);}
  to{transform:scale(1.1);}
}
</style>
</head>

<body>

<div class="container">
  <h1 id="msg">🎁 Click Below For Surprise 🎁</h1>
  <button onclick="showWish()">Open Surprise</button>
</div>

<audio id="music">
  <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
</audio>

<script>
function showWish(){
  document.getElementById("msg").innerHTML =
  "🎉 HAPPY BIRTHDAY Megha 🎂<br><br>May your happiness rise like mountains, your problems flow away like river and your sucess expand like universe! 🌟";
  
  document.body.style.background =
  "linear-gradient(45deg,#ff0080,#7928ca,#2af598)";
  
  document.getElementById("music").play();
}
</script>

</body>
</html>
