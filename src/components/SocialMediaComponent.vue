<template>
    <div class="contenedor">
        <button class="circulo"></button>
        <button class="circulo1"></button>
        <button class="circulo2"></button>
    </div>


    <svg xmlns="http://www.w3.org/2000/svg" viewBox="100 0 100 150">
        <clipPath id="clip">
            <path d="M 100 0 A 100 100 0 0 1 186.6 150 L 100 100 L 100 0 Z" fill="#000000" />
        </clipPath>
    </svg>
</template>

<style scoped>
* {
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

.contenedor{
    position:relative;
}

.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none;
    left: -99px;
    background: rgb(255, 0, 0);
    transform: scaleX(-1);
}
.circulo:hover{
    background: yellow;
    left: -105px;
    top: -4px;
}

.circulo1 {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none;
    background: rgb(98, 0, 255);
    left: -118px;
    top: -32px;
    transform: rotate(120deg)
}

.circulo1:hover{
    background: yellow;
    top: -26px;
}

.circulo2 {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none;
    background: rgb(0, 255, 55);
    transform: scale(1);
}
.circulo2:hover{
    background: yellow;
    top: -5px;
    left: 5px;
}


.circle {
    width: 200px;
    height: 200px;
    position: absolute;
    top: 530px;
    left: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.mask {
    width: 50%;
    height: 25%;
    background: black;
    position: absolute;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    top: 50%;
    left: 0%;
    z-index: 3;
    mask-image: url(../assets/mask.png);
    mask-position: start start;

}

.elemento0 {
    position: relative;
    height: 50%;
    width: 50%;
    background: yellow;
    top: 0%;
    border-top-left-radius: 100%;
    z-index: 4;
}

.elemento0::after {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0%;
    left: 100%;
    background: yellow;
    border-top-right-radius: 100%;
    z-index: 6;
    clip-path: polygon(0 0, 60% 0, 0 100%, 0 100%);
}

.elemento0:hover {
    background: white;
}

.elemento0:hover::after {
    background: white;
}

.elemento1 {
    position: relative;
    height: 50%;
    width: 50%;
}

.elemento1::before {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(240, 5, 5);
    top: 0%;
    left: 0px;
    z-index: 7;
    clip-path: polygon(60% 0, 100% 0, 100% 100%, 0% 100%);
    border-top-right-radius: 100%;
}

.elemento1::after {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    top: 100%;
    left: 0%;
    background: rgb(240, 5, 5);
    border-bottom-right-radius: 100%;
    clip-path: polygon(0 0, 100% 0, 100% 100%, 60% 100%);
    z-index: 6;
}

.elemento1:hover::before {
    background: white;
}

.elemento1:hover::after {
    background: white;
}


.elemento2 {
    position: relative;
    height: 50%;
    width: 50%;
}

.elemento2::before {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(44, 240, 5);
    top: 0%;
    left: 50%;
    z-index: 8;
    clip-path: polygon(0 0, 0 0, 60% 100%, 0 100%);
    border-bottom-right-radius: 100%;
}

.elemento2::after {
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(44, 240, 5);
    top: 0%;
    left: -50%;
    border-bottom-left-radius: 100%;
    z-index: 8;
}

.elemento2:hover::before {
    background: white;
}

.elemento2:hover::after {
    background: white;
}
</style>

