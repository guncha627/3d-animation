# 3d-animation
example for making cube
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
  <style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    height: 100vh ;
    display: grid;
    justify-items: center;
}
.button_down {
    padding: 10px;
    background-color: yellowgreen;
    height: 40px;
    width: 60px;
}

.cube {
    width: 600px;
    flex: row wrap;    
}
.sides1,
.sides2,
.sides3,
.sides4 {
    position: relative;
    transition: transform 3s;
    transform-style: preserve-3d;
    width: 200px;
    height: 200px;
    display: inline-block;
    top: 100px;
    margin: 30px;
}
.side1,
.side2,
.side3,
.side4,
.side5,
.side6 {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    width: 200px;
    height: 200px;
    background-color: burlywood;
    text-align: center;
    font-size: 3em;
    padding: 1.5em;
    margin: auto;   
}
.side1 {
    transform: translateZ(100px) ;
    transition: 3s;
    background-color: red;
}
.side2 {
    transform: rotateY(90deg) translateZ(100px);
    transition: 3s;
    background-color: blue;
}
.side3 {
    transform: rotateY(180deg) translateZ(100px);
    transition: 3s;
    background-color: pink;
}
.side4 {
    transform: rotateY(-90deg) translateZ(100px) ;
    transition: 3s;
    background-color: green;
}
.side5 {
    transform-style: preserve-3d;
    transform: rotateX(90deg) translateZ(100px);
    perspective: 100px;
    transition: 3s;
    background-color: yellow;
}
.side6 {
    transform-style: preserve-3d;
    transform: rotateX(-90deg) translateZ(100px);
    transition: 3s;
    background-color: purple;
}
.sides1:hover {
    transform: rotateY(-360deg);
}
.sides2:hover {
    transform: rotateY(360deg);
}
.sides3:hover {
    transform: rotateX(-360deg);
}
.sides4:hover {
    transform: rotateX(360deg);
}

</style>
</head>
<body>
    <div class="cube">
        <div class="sides1">
            <div class="side1">1</div>
            <div class="side2">2</div>
            <div class="side3">3</div>
            <div class="side4">4</div>
            <div class="side5">5</div>
            <div class="side6">6</div>
        </div>
        <div class="sides2">
            <div class="side1">1</div>
            <div class="side2">2</div>
            <div class="side3">3</div>
            <div class="side4">4</div>
            <div class="side5">5</div>
            <div class="side6">6</div>
        </div>
        <div class="sides3">
            <div class="side1">1</div>
            <div class="side2">2</div>
            <div class="side3">3</div>
            <div class="side4">4</div>
            <div class="side5">5</div>
            <div class="side6">6</div>
        </div>
        <div class="sides4">
            <div class="side1">1</div>
            <div class="side2">2</div>
            <div class="side3">3</div>
            <div class="side4">4</div>
            <div class="side5">5</div>
            <div class="side6">6</div>
        </div>
    </div>
</body>
</html>
