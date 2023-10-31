<template>
    <!--
       <ul>
        <li>
            <a href="">
                <span>
                    <ion-icon name="logo-github"></ion-icon>
                </span>
            </a>
        </li>
    </ul>  
    -->
    <div class="contenedor">
        <button class="buttonSocialMedia">
            <div class="mainPanel">
                <ion-icon name="logo-github"></ion-icon>
            </div>
            <div class="leftPanel"></div>
            <div class="rightPanel"></div>
        </button>
    </div>
</template>

<style scoped>
ul {
    position: absolute;
    display: flex;
    margin: 0;
    padding: 0;
    left: 20vw;
    top: 75%;
}

li {
    position: relative;
    list-style: none;
}

span {
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
}

a {
    color: rgb(134, 40, 40);
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgb(238, 14, 14);
    width: 3vw;
    height: 3vw;
    transform: rotate(339deg) skewX(36deg);
}

a:before {
    content: '';
    position: absolute;
    background: rgb(161, 33, 33);
    height: 20%;
    width: 100%;
    top: 3vw;
    left: -0.3vw;
    transform: skewX(-45deg) skewY(0deg);
}

.contenedor {
    position: absolute;
}

.buttonSocialMedia {
    background: none;
    border: none;
}

.mainPanel {
    position: absolute;
    left: -29vw;
    top: 13vw;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 3vw;
    background: rgb(238, 14, 14);
    width: 3vw;
    height: 3vw;
    transform: rotate(339deg) skewX(36deg);
    box-shadow: transparent;
    transition: background 0.5s,box-shadow 0.5s;
}

.mainPanel:hover {
    background: rgb(255, 67, 67);
    box-shadow: 5px -5px 11px #ef1717;
}

.leftPanel {
    position: absolute;
    background: rgb(161, 33, 33);
    height: 8px;
    width: 3.1vw;
    left: -27.55vw;
    top: 15.55vw;
    transform: rotate(339deg) skewX(-20deg);
}

.rightPanel {
    position: absolute;
    background: rgb(161, 33, 33);
    height: 8px;
    width: 3.5vw;
    left: -30.7vw;
    top: 15.09vw;
    transform: rotate(-327deg) skewX(32deg);
}

a:after {
    content: '';
    position: absolute;
    background: rgb(161, 33, 33);
    height: 100%;
    width: 20%;
    top: 0.3vw;
    left: -0.6vw;
    transform: skewY(-45deg) skewX(0deg);
}
</style>