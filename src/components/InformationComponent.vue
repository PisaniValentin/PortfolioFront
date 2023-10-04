<script setup>
import NavigationBar from './NavigationBar.vue';
</script>

<template>
    <div class="information row d-flex justify-content-center">
        <div class="informationTop">
            <p>Valentin</p>
            <p>Contact Me:</p>
        </div>
        <div class="informationBottom">
            <a href="">
                <ion-icon name="mail-outline"></ion-icon>
            </a>
            <a href="">
                <ion-icon name="logo-linkedin"></ion-icon>
            </a>
            <a href="">
                <ion-icon name="logo-github"></ion-icon>
            </a>
        </div>
        <NavigationBar />
    </div>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.information {
    display: flex;
    position: fixed;
    top: 20%;
    width: 200px;
    z-index: 1;
    background: #181818;
    border-radius: 15px;
    color: rgb(221, 221, 221);
    height: 250px;
    border: 1px solid rgb(204, 207, 209);
}
a{
    font-size: 28px;
    color: rgb(13, 138, 221);
    height: 28px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.informationTop{

}
.informationBottom{
    display: flex;
    justify-content: center;
    gap: 35px;
}



</style>