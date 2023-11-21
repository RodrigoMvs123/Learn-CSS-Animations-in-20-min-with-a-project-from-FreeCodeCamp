# Learn-CSS-Animations-in-20-min-with-a-project-from-FreeCodeCamp

https://www.youtube.com/watch?v=qDij4BD_v78 

https://raw.githubusercontent.com/RodrigoMvs123/Learn-CSS-Animations-in-20-min-with-a-project-from-FreeCodeCamp/main/README.md

https://github.com/RodrigoMvs123/Learn-CSS-Animations-in-20-min-with-a-project-from-FreeCodeCamp/blame/main/README.md

Visual Studio Code
Explorer 
Open Editors
index.html

index.html

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Ferris Wheel</title>
        <link rel="stylesheet" hrel="">
    </head>
    <body>
        
    </body>
</html>

Visual Studio Code
Explorer 
Open Editors
index.html
styles.css

Visual Studio Code
Explorer 
Open Editors
index.html
styles.css

index.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Ferris Wheel</title>
        <link rel="stylesheet" hrel="styles.css">
    </head>
    <body>
        <div class="wheel">
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
            <div class="cabin"></div>
            <div class="cabin"></div>
            <div class="cabin"></div>
            <div class="cabin"></div>
            <div class="cabin"></div>
            <div class="cabin"></div>
        </div>
    </body>
</html>


Visual Studio Code
Explorer 
Open Editors
index.html
styles.css

styles.css
.wheel {
    border: 2px solid black;
    border-radius: 50%;
    margin-left: 50px;
    position: absolute;
    height: 55vw;
    width: 55vw;
    max-height: 500px;
    max-width: 500px;
    animation-name: wheel;
    animation-duration: 10s;
    animation-iteration-count: infinite;
    animation-timing-function: liner;
}

.line {
    background-color: black;
    width: 50px;
    height: 2px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform-origin: 0% 0%/;
}

.line:nth-of-type(2) {
    transform: rotate(60deg);
}

.line:nth-of-type(3) {
    transform: rotate(120deg);
}

.line:nth-of-type(4) {
    transform: rotate(180deg);
}

.line:nth-of-type(5) {
    transform: rotate(240deg);
}

.line:nth-of-type(6) {
    transform: rotate(300deg);
}

.cabin {
    background-color: red;
    width:20%;
    height: 20%;
    position: absolute;
    border: 2px solid;
    transform-origin: 50% 0%;
    animation: cabins 10s ease-in-out infinite;
    
}

cabin:nth-of-type(1) {
    right: -8.5%;
    top: 50%;
}


cabin:nth-of-type(2) {
    right: 17%;
    top: 93.5%;
}


cabin:nth-of-type(3) {
    right: 67%;
    top: 93.5%;
}


cabin:nth-of-type(4) {
    left: -8.5%;
    top: 50%;
}


cabin:nth-of-type(5) {
    left: 17%;
    top: 93.5%;
}


cabin:nth-of-type(6) {
    right: 17%;
    top: 7%;
}

@keyframes wheel {
    0% {
        transform: rotate(0deg)
    },
    100% {
        transform: rotate(360deg)
    }
}

@keyframe cabins {
    0% {
        transform: rotate(0deg);
    }
    25% {
        background-color: yellow;
    }
    50% {
        background-color: purple;
    }
    75% {
        background-color: yellow;
    }
    100% {
        transform: rotate(-360deg)
    }
}






