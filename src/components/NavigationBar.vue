<template>
    <div class="navigationBar">
        <ul>
            <li class="list active" @click="toggleA('home')" id="home">
                <a href="#" class="active">
                    <span class="icon">
                        <ion-icon name="home-outline"></ion-icon>
                    </span>
                    <span class="text">Home</span>
                </a>
            </li>
            <li class="list" @click="toggleA('about')" id="about">
                <a href="#">
                    <span class="icon">
                        <ion-icon name="person-circle-outline"></ion-icon>
                    </span>
                    <span class="text">About</span>
                </a>
            </li>
            <li class="list" @click="toggleA('projects')" id="projects">
                <a href="#">
                    <span class="icon">
                        <ion-icon name="document-text-outline"></ion-icon>
                    </span>
                    <span class="text">Projects</span>
                </a>
            </li>
            <div class="indicator"></div>
        </ul>
    </div>
</template>


<script>

export default {
    data() {

    },
    methods: {
        toggleA: function (name) {
            const list = document.querySelectorAll('.list');
            list.forEach(element => {
                if(element.id == name){
                    element.classList.add('active');
                }else{
                    element.classList.remove('active');
                }
            });
        }
    },
}

</script>


<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.navigationBar {
    background: #fff;
    border: 2px solid rgb(100, 100, 100);
    border-radius: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 40px;
    width: 150px;
    margin-top: 20px;
}

.navigationBar ul {
    position: relative;
    display: flex;
    align-items: center;
}

.navigationBar ul li {
    position: relative;
    list-style: none;
    width: 35px;
    height: 35px;
    z-index: 1;
}

.navigationBar ul li a {
    position: relative;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    text-align: center;
    font-weight: bold;
    width: 100%;
}
.navigationBar ul li a:hover {
    background: transparent;
}

.navigationBar ul li a .icon {
    position: relative;
    display: block;
    align-items: center;
    text-align: center;
    line-height: 35px;
    color: black;
    font-size: 18px;
    transition: 0.5s;
}

.navigationBar ul li.active a .icon {
    transform: translateY(-21px);
}


.navigationBar ul li a .text {
    position: absolute;
    color: black;
    font-weight: bold;
    transition: 0.5s;
    font-size: 12px;
    opacity: 0;
}

.navigationBar ul li.active a .text {
    transform: translateY(5px);
    opacity: 1;
}

.indicator {
    position: absolute;
    width: 35px;
    height: 35px;
    top: -22px;
    left: 0px;
    background: rgb(13, 138, 221);
    border-radius: 50%;
    border: 6px solid #181818;
    transition: 0.5s;
}

.indicator::before {
    content: '';
    position: absolute;
    top: 13px;
    left: -18px;
    width: 20px;
    height: 20px;
    background: transparent;
    border-top-right-radius: 25px;
    box-shadow: 1px -9px 0 0 #181818;
}

.indicator::after {
    content: '';
    position: absolute;
    top: 13px;
    right: -18px;
    width: 20px;
    height: 20px;
    background: transparent;
    border-top-left-radius: 20px;
    box-shadow: -1px -9px 0 0 #181818;
}

.navigationBar ul li:nth-child(1).active~.indicator {
    transform: translateX(calc(35px*0));
}

.navigationBar ul li:nth-child(2).active~.indicator {
    transform: translateX(calc(35px*1));
}

.navigationBar ul li:nth-child(3).active~.indicator {
    transform: translateX(calc(35px*2));
}
</style>
