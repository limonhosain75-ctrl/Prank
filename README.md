# Prank
A hidden surprise animation web prank
<!DOCTYPE html>
<html>
<head>
<title>😂 Surprise</title>
<style>
body {
  background: black;
  overflow: hidden;
}
.text {
  position: absolute;
  color: yellow;
  font-size: 30px;
  font-weight: bold;
  animation: float 4s linear infinite;
}
@keyframes float {
  from {transform: translateY(100vh);}
  to {transform: translateY(-10vh);}
}
</style>
</head>
<body>

<script>
setInterval(() => {
  let t = document.createElement("div");
  t.className = "text";
  t.innerText = "তুই একটা পাগল বলদ 😂👎";
  t.style.left = Math.random()*100 + "vw";
  document.body.appendChild(t);
}, 300);
</script>

</body>
</html>
