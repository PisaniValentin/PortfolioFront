<script setup>
import NavigationBar from './NavigationBar.vue';
</script>

<template>
    <div class="information row d-flex justify-content-center">
        <h2>Contact Me</h2>
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
    width: 200px;
    z-index: 1;
    background: #181818;
    color: rgb(221, 221, 221);
    height: 250px;
    border-top-left-radius: 15px;
    border-bottom-left-radius: 15px;
}
a{
    font-size: 28px;
    color: rgb(13, 138, 221);
    height: 28px;
    display: flex;
    justify-content: center;
    align-items: center;
}
a:hover{
    background: transparent;
}

.informationTop{
    display: flex;
    flex-direction: column;
    align-items: center;

}
.informationBottom{
    display: flex;
    justify-content: center;
    gap: 35px;
}



</style>