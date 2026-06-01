# ggtt54.github.io
I Love You Ramoussa ❤️
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Falling Hearts</title>
<style>
body {
    margin: 0;
    overflow: hidden;
    background: black;
}

.heart {
    position: absolute;
    color: red;
    font-size: 24px;
    animation: fall linear infinite;
}

@keyframes fall {
    from {
        transform: translateY(-50px);
    }
    to {
        transform: translateY(110vh);
    }
}
</style>
</head>
<body>

<script>
function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";

    heart.style.left = Math.random() * window.innerWidth + "px";
    heart.style.fontSize = (20 + Math.random() * 30) + "px";
    heart.style.animationDuration = (3 + Math.random() * 5) + "s";

    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 8000);
}

setInterval(createHeart, 200);
</script>

</body>
</html>
