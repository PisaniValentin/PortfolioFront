<template>
    <ul>
        <li>
            <a href="">
                <span>
                    <ion-icon name="logo-github"></ion-icon>
                </span>
            </a>
        </li>

    </ul>
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
    list-style: none;
}

span {
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    left: 25%;
    top: 25%;
}

a {
    color: rgb(134, 40, 40);
    display: block;
    background: rgb(238, 14, 14);
    width: 3vw;
    height: 3vw;
    transform: rotate(335deg) skewX(29deg);
}

a:before {
    content: '';
    position: absolute;
    background: rgb(161, 33, 33);
    height: 20%;
    width: 100%;
    top: 23px;
    left: -2px;
    transform: skewX(-45deg);
}

a:after {
    content: '';
    position: absolute;
    background: rgb(161, 33, 33);
    height: 100%;
    width: 20%;
    top: 3px;
    left: -5px;
    transform: skewY(-45deg);
}
</style>