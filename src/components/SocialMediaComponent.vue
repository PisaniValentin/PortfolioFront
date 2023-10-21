<template>
    <div class="contenedor">
        <div class="circulo">
            <ion-icon name="logo-linkedin"></ion-icon>
        </div>
        <div class="circulo1">
            <ion-icon name="logo-github"></ion-icon>
        </div>
        <div class="circulo2">
            <ion-icon name="mail-outline"></ion-icon>
        </div>
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

ion-icon {
    width: 38px;
    height: 38px;
    z-index: 4;
    position: absolute;
    left: 125px;
    top: 54px;
    transform: scaleX(-1);
    border-radius: 100%;
    border: none;
}


.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none !important;
    left: -100px;
    background: #1e161f;
    transform: scaleX(-1) translateZ(0);
    z-index: 3 !important;
    transition: 0.5s;

}

.circulo::after {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    left: -6px;
    top: -4px;
    transform: scaleX(0.92) scaleY(0.92) translateZ(0);
    z-index: 3 !important;
    background: linear-gradient(238deg, rgba(15, 0, 17, 1) 0%, rgba(215, 215, 215, 1) 100%);
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
}

.circulo:hover {
    background: rgb(118, 18, 231);
    left: -108px;
    top: -5px;
}

.circulo1 {
    position: absolute;
    width: 300px;
    height: 300px;
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
    border: none;
    top: -31px;
    left: -118px;
    transform: rotate(120deg) translateZ(0);
    ;
    background: #1e161f;
    z-index: 2;
    transition: 0.5s;
}

.circulo1::after {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    left: -6px;
    top: -2.3px;
    transform: scaleX(0.92) scaleY(0.92)translateZ(0);
    z-index: 2 !important;
    background: linear-gradient(238deg, rgba(15, 0, 17, 1) 0%, rgba(215, 215, 215, 1) 100%);
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');

}

.circulo1:hover {
    background: rgb(118, 18, 231);
    top: -23px;
}

.circulo2 {
    position: absolute;
    width: 300px;
    height: 300px;
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
    border: none !important;
    background: #1e161f;
    transform: scaleX(1) translateZ(0);
    z-index: 1 !important;
    transition: 0.5s;
    top: 0px;
    left: 0px;
}

.circulo2::after {
    content: '';
    position: absolute;
    width: 300px;
    height: 300px;
    left: -6px;
    top: -4px;
    transform: scaleX(0.92) scaleY(0.92) translateZ(0);
    z-index: 0 !important;
    background: linear-gradient(238deg, rgba(15, 0, 17, 1) 0%, rgba(215, 215, 215, 1) 100%);
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
}

.circulo2:hover {
    background: rgb(118, 18, 231);
    top: -5px;
    left: 8px;
}

.circulo1 ion-icon {
    transform: rotate(240deg);
}
</style>

