<template>
    <div class="aboutMeContainer">
        <img src="https://cdn.icon-icons.com/icons2/2468/PNG/512/user_kids_avatar_user_profile_icon_149314.png" alt="">
        <h2>Hi, Im Valentin Pisani</h2>
        <h4>Full Stack Developer</h4>
        <p>Actually studying Engineer in Systems of Information at UNS (Universidad Nacional Del Sur) in Argentina</p>
        <div>
            <p>CONTACT ME</p>
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
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Teko:wght@500&display=swap');

* {
    margin: 0px;
    padding: 0px;
    font-family: 'Teko', sans-serif;
}

.aboutMeContainer {
    width: 100%;
    background-image: linear-gradient(to right top, #3803b9, #431fc1, #4d30ca, #5740d1, #614ed9);
    border-top-left-radius: 15px;
    padding: 20px;
    color:white;
    margin-bottom: 30px;
    box-shadow: rgba(0, 0, 0, 0.45) -19px 20px 20px 0px;

}

h2{
    font-size: 30px;
}

h4{
    font-size: 15px;
    color: rgb(207, 207, 207);
}
p{
    font-size: 15px;
    color: rgb(207, 207, 207);
}

a{
    font-size: 15px0px;
}
img {
    align-self: center;
    width: 220px;
    background: white;
    border-radius: 50%;
    border: 8px solid rgb(150, 150, 156);
}
</style>