<template>
    <div class="contenedor">
        <button class="circulo"><span></span></button>
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


.contenedor {
    position: relative;
}

.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none;
    left: -97px;
    background: rgb(210, 160, 216);
    transform: scaleX(-1);
}
.circulo::after {
    position: absolute;
    content:'';
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    background: rgb(96, 9, 105);
    transform: scale(0.5);
    z-index: 15;
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
    transform: rotate(120deg);
    background: rgb(210, 160, 216);
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
    border: none;
    background: rgb(210, 160, 216);
    transform: scale(1);
}

.circulo2:hover {
    background: yellow;
    top: -5px;
    left: 8px;
}
</style>

