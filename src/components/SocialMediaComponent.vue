<template>
    <div class="contenedor">
        <div class="circulo"></div>
        <div class="circulo1"></div>
        <div class="circulo2"></div>
    </div>


    <svg xmlns="http://www.w3.org/2000/svg">
        <clipPath id="clip">
            <path d="M 100 0 A 100 100 0 0 1 186.6 150 L 100 100 L 100 0 Z" fill="#000000" />
        </clipPath>
    </svg>
</template>

<style scoped>
* {
    margin: 0px;
    padding: 0px;
}


.contenedor {
    position: relative;
    width: 500px;
    height: 500px;
}

.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none !important;
    left: -99px;
    background: rgb(210, 160, 216);
    transform: scaleX(-1);
    z-index: 2;
    transition: 0.5s;
}

.circulo::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    top:-20px;
    clip-path: url('#clip');
    background-color: rgb(96, 9, 105);
    transform: scaleX(0.75) scaleY(0.75);
    border: none !important;
    z-index: 2 !important;

}


.circulo:hover {
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
    top: -32px;
    left: -118px;
    transform: rotateZ(120deg);
    background: rgb(210, 160, 216);
    z-index: 1;
    transition: 0.5s;
}

.circulo1::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background-color: rgb(96, 9, 105);
    transform: scaleX(0.75) scaleY(0.75);
    z-index: 2;
    left: -1px;
    top: -17px;

}

.circulo1:hover {
    background: yellow;
    top: -26px;
}

.circulo2 {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none !important;
    background: rgb(210, 160, 216);
    transform: scaleX(1);
    z-index: 0;
    transition: 0.5s;
    top: 0px;
    left: 0px;
}


.circulo2::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background: rgb(96, 9, 105);
    transform: scaleX(0.75) scaleY(0.75);
    z-index: 2;
    top:-20px;
}

.circulo2:hover {
    background: yellow;
    top: -5px;
    left: 8px;
}
</style>

