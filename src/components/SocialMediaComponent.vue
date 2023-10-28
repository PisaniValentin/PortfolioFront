<template>
    <div class="contenedor">
        <div class="circuloContainer">
            <div class="circulo">
                <ion-icon name="logo-linkedin"></ion-icon>
            </div>
        </div>

        <div class="circulo1Container">
            <div class="circulo1">
                <ion-icon name="logo-github"></ion-icon>
            </div>
        </div>
        <div class="circulo2Container">
            <div class="circulo2">
                <ion-icon name="mail-outline"></ion-icon>
            </div>
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

@media (max-width: 425px) {
    * {
        height: 0px;
        width: 0px;
        display: none;
    }
}

.contenedor {
    position: absolute;
    z-index: 3;
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

.circuloContainer:hover {
    filter: drop-shadow(-29px -12px 27px rgb(118, 18, 231))
}

.circulo {
    position: absolute;
    width: 300px;
    height: 300px;
    clip-path: url('#clip');
    border: none !important;
    left: -102px;
    background: #1e161f;
    transform: scaleX(-0.6) scaleY(0.6) translateZ(0);
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
    left: -106px;
    top: -2px;
    color: white
}

.circulo1Container:hover {
    filter: drop-shadow(4px 26px 27px rgb(118, 18, 231))
}

.circulo1 {
    position: absolute;
    width: 300px;
    height: 300px;
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
    border: none;
    top: -17px;
    left: -112px;
    transform: rotate(120deg) scaleX(0.6) scaleY(0.6) translateZ(0);
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
    top: -14px;
    color: white
}

.circulo2Container:hover {
    filter: drop-shadow(30px -12px 27px rgb(118, 18, 231));
}

.circulo2 {
    position: absolute;
    width: 300px;
    height: 300px;
    -webkit-clip-path: url('#clip');
    clip-path: url('#clip');
    border: none !important;
    background: #1e161f;
    transform: scaleX(0.6) scaleY(0.6) translateZ(0);
    z-index: 1 !important;
    transition: 0.5s;
    top: 0px;
    left: -40px;
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
    top: -2px;
    left: -36px;
    color: white
}

.circulo1 ion-icon {
    transform: rotate(240deg);
}
</style>

