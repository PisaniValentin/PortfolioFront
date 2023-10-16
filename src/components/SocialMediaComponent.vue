<template>
    <div class="circle row">
       
            <div class="elemento0 col-6"></div>
            <div class="elemento1 col-6"></div>
      
            <div class="elemento2 col-12"></div>
        
    </div>

</template>

<style scoped>
* {
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
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

.elemento0{
    position: relative;
    height: 50%;
    width: 50%;
    background: yellow;
    top: 0%;
    border-top-left-radius: 100%;
    z-index: 4;
}

.elemento0::after{
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
.elemento0:hover{
    background: white;
}
.elemento0:hover::after{
    background: white;
}

.elemento1{
    position: relative;
    height: 50%;
    width: 50%;
}

.elemento1::before{
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(240, 5, 5);
    top:0%;
    left: 0px;
    z-index: 7;
    clip-path: polygon(60% 0, 100% 0, 100% 100%, 0% 100%);
    border-top-right-radius: 100%;
}

.elemento1::after{
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
.elemento1:hover::before{
    background: white;
}
.elemento1:hover::after{
    background: white;
}


.elemento2{
    position: relative;
    height: 50%;
    width: 50%;
}

.elemento2::before{
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(44, 240, 5);
    top:0%;
    left: 50%;
    z-index: 8;
    clip-path: polygon(0 0, 0 0, 60% 100%, 0 100%);
    border-bottom-right-radius: 100%;
}
.elemento2::after{
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    background: rgb(44, 240, 5);
    top:0%;
    left: -50%;
    border-bottom-left-radius: 100%;
    z-index: 8;
}

.elemento2:hover::before{
    background: white;
}
.elemento2:hover::after{
    background: white;
}






</style>

