<template>
    <div class="CardsContainer row">
        <div class="card col-sm-12 col-md-3">
            <img class="card-img-top" src="https://api.boosthive.eu/media/image/4c/88/81965a5dffce6e4d223649ef0f78.jpeg"
                alt="Card image cap">
            <div class="card-body">
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
                    content.</p>
            </div>
        </div>
        <div class="card col-sm-12 col-md-3">
            <img class="card-img-top" src="https://api.boosthive.eu/media/image/4c/88/81965a5dffce6e4d223649ef0f78.jpeg"
                alt="Card image cap">
            <div class="card-body">
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
                    content.</p>
            </div>
        </div>
        <div class="card col-sm-12 col-md-3">
            <img class="card-img-top" src="https://api.boosthive.eu/media/image/4c/88/81965a5dffce6e4d223649ef0f78.jpeg"
                alt="Card image cap">
            <div class="card-body">
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
                    content.</p>
            </div>
        </div>
        <div class="card col-sm-12 col-md-3">
            <img class="card-img-top" src="https://api.boosthive.eu/media/image/4c/88/81965a5dffce6e4d223649ef0f78.jpeg"
                alt="Card image cap">
            <div class="card-body">
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
                    content.</p>
            </div>
        </div>
       
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Saira:wght@100;300&display=swap');
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
@media (min-width: 320px) {
    .CardsContainer{
        padding: 20px;
        border-radius: 15px;
    }
}
.CardsContainer {
    display: flex;
    justify-content: center;
    background-image: linear-gradient(to left top, #3803b9, #431fc1, #4d30ca, #5740d1, #614ed9);
    border-bottom-right-radius: 15px;
    border-top-right-radius: 15px;
    min-height: 100%;
    gap: 15px;
    box-shadow: rgba(0, 0, 0, 0.45) 16px 20px 20px 0px;
    
}
.card{
    height: 35%;
    font-family: 'Teko', sans-serif;
}
.card-img-top{
    padding: 5px;
}
.card-body{
    padding: 15px;
    padding-top: 10px;
}

</style>