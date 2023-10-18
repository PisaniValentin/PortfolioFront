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
}

.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none !important;
    left: -14%;
    background: rgb(210, 160, 216);
    transform: scaleX(-1);
    z-index: 2;
}

.circulo::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background-color: rgb(96, 9, 105);
    transform: scaleX(0.95) scaleY(0.95) rotateZ(0);
    border: none !important;
    top: -5px;
    left: -5px;
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
    top: -34px;
    left: -117px;
    transform: rotateZ(120deg);
    background: rgb(210, 160, 216);
    z-index: 1;

}

.circulo1::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background: rgb(96, 9, 105);
    top: -3px;
    left: -3px;
    transform: scaleX(0.95) scaleY(0.95) translateZ(0);
    z-index: 2;

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
}


.circulo2::before {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background: rgb(96, 9, 105);
    transform: scaleX(0.95) scaleY(0.95) translateZ(0);
    top: -3px;
    left: -3px;
    z-index: 2;
}

.circulo2:hover {
    background: yellow;
    top: -5px;
    left: 8px;
}
</style>

