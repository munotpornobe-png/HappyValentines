<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>For My Chamomile 🌼</title>
    <style>
      body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #ffdde1, #ee9ca7);
    font-family: 'Poppins', sans-serif;
    overflow: hidden;
}

.container {
    text-align: center;
}

h1 {
    color: white;
    font-size: 2.2rem;
    margin-bottom: 20px;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    background-color: #ff4e88;
    color: white;
    cursor: pointer;
    transition: 0.3s ease;
}

button:hover {
    background-color: #ff1e63;
    transform: scale(1.1);
}

/* Chamomile Flower */
.flower {
    position: relative;
    width: 200px;
    height: 220px;
    margin: 30px auto 0;
    transform: scale(0);
    transition: transform 0.6s ease;
}

.petal {
    width: 60px;
    height: 100px;
    background: white;
    border-radius: 50%;
    position: absolute;
    top: 20px;
    left: 70px;
    transform-origin: center 80px;
}

.petal:nth-child(1) { transform: rotate(0deg); }
.petal:nth-child(2) { transform: rotate(45deg); }
.petal:nth-child(3) { transform: rotate(90deg); }
.petal:nth-child(4) { transform: rotate(135deg); }
.petal:nth-child(5) { transform: rotate(180deg); }
.petal:nth-child(6) { transform: rotate(225deg); }
.petal:nth-child(7) { transform: rotate(270deg); }
.petal:nth-child(8) { transform: rotate(315deg); }

.center {
    width: 80px;
    height: 80px;
    background: #ffcc33;
    border-radius: 50%;
    position: absolute;
    top: 55px;
    left: 60px;
    z-index: 2;
}

.stem {
    width: 6px;
    height: 100px;
    background: green;
    position: absolute;
    bottom: 0;
    left: 97px;
}

.message {
    color: white;
    font-size: 18px;
    margin-top: 20px;
    opacity: 0;
    transition: opacity 1s ease;
    max-width: 400px;
    margin-left: auto;
    margin-right: auto;
}

.show {
    transform: scale(1);
}

.show-message {
    opacity: 1;
}
    </style>
</head>
<body>

<div class="container">
    <h1>Happy Valentine's Day, My Love 💖</h1>
    <button onclick="showFlower()">Click Me 🌼</button>

    <div class="flower" id="flower">
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="petal"></div>
        <div class="center"></div>
        <div class="stem"></div>
    </div>

    <div class="message" id="message">
        Even though you are far away from me, my heart is always right beside you.<br><br>
        I am so proud of the amazing accountant and hardworking woman you are becoming.<br><br>
        Every late night, every challenge you face only makes me admire you more.<br><br>
        You bloom beautifully in your career, just like this chamomile flower.<br><br>
        No distance can ever lessen how deeply I love you. 🌼❤️
    </div>
</div>

<script>
function showFlower() {
    document.getElementById("flower").classList.add("show");
    document.getElementById("message").classList.add("show-message");
}
</script>

</body>
</html>
