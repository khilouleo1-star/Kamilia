<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Valentine Proposal ❤️</title>
<style>
  body {
    font-family: Arial, sans-serif;
    text-align: center;
    background: #ffe6f0;
    margin-top: 120px;
  }
  h1 {
    color: #cc0066;
    font-size: 32px;
  }
  button {
    padding: 15px 30px;
    font-size: 18px;
    margin: 20px;
    border-radius: 10px;
    border: none;
    cursor: pointer;
  }
  #yesBtn {
    background: #ff4d88;
    color: white;
  }
  #noBtn {
    background: #999;
    color: white;
    position: absolute;
  }
</style>
</head>

<body>

<h1>Will you be my Valentine? 💌</h1>

<button id="yesBtn" onclick="sayYes()">YES ❤️</button>
<button id="noBtn">No 😢</button>

<script>
function sayYes() {
  document.body.innerHTML = "<h1>Best choice ever 😍❤️</h1><p>I knew it!</p>";
}

const noBtn = document.getElementById("noBtn");

noBtn.addEventListener("mouseover", moveButton);
noBtn.addEventListener("click", moveButton);

function moveButton() {
  const x = Math.random() * (window.innerWidth - 120);
  const y = Math.random() * (window.innerHeight - 60);
  noBtn.style.left = x + "px";
  noBtn.style.top = y + "px";
}
</script>

</body>
</html>
