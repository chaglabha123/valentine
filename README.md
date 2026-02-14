<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Be My Valentine?</title>

<style>
body {
    background: linear-gradient(135deg, #ffb6c1, #ff69b4);
    font-family: Arial, sans-serif;
    text-align: center;
    height: 100vh;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.container {
    background: white;
    padding: 40px;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

h1 {
    color: #ff1493;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    margin: 15px;
    transition: 0.3s;
}

#yes {
    background-color: #ff1493;
    color: white;
}

#yes:hover {
    background-color: #ff69b4;
}

#no {
    background-color: #ffc0cb;
    color: white;
    position: absolute;
}
</style>
</head>

<body>

<div class="container">
    <h1>Will You Be My Valentine? 💕</h1>
    <button id="yes" onclick="yesClicked()">Yes 💖</button>
    <button id="no">No 😢</button>
</div>

<script>
const noBtn = document.getElementById("no");

noBtn.addEventListener("mouseover", function() {
    const x = Math.random() * window.innerWidth;
    const y = Math.random() * window.innerHeight;
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});

function yesClicked() {
    document.body.innerHTML = `
        <h1 style="color:white; font-size:50px;">
        YAAAAAY 💖💖💖 <br> 
        You just made me the happiest person alive 😍
        </h1>
    `;
}
</script>

</body>
</html>
