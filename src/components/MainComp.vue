<template>
    <main>
        <section id="products">
            <div>
                <h2>Contents goes here...</h2>
            </div>
        </section>
        <section id="bg-images">
            <div class="images-flex">
               <div>
                <img src="../assets/buy-comics-digital-comics.png" alt="buy-comics1">
                <span>DIGITAL COMICS</span>
            </div>
            <div>
                <img src="../assets/buy-comics-merchandise.png" alt="merch">
                <span>DC MERCHANDISE</span>
            </div>
            <div>
                <img src="../assets/buy-comics-subscriptions.png" alt="sub">
                <span>SUBSCRIPTION</span>
            </div>
            <div>
                <img src="../assets/buy-comics-shop-locator.png" alt="locator">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div>
                <img class="img-svg" src="../assets/buy-dc-power-visa.svg" alt="visa">
                <span>DC POWER VISA</span>
            </div> 
            </div>
            
        </section>

    </main>
</template>

<script>
    export default {
        name: 'MainComp'
    }
</script>

<style lang="scss" scoped>

#products>div,
#bg-images>div{
    width: 80%;
    margin: 0 auto;
}

#products{
    background-color: #1C1C1C;
    color: white;
    padding: 50px;
}

#bg-images{
    background-color: rgb(49, 126, 235);
    display: flex;
    align-content: center;
    justify-content: space-around;
    padding: 50px 0;

    div{
        display:flex;
        gap: 10px;
        align-items: center;
        color: white;
        font-weight: bold;
    }


    img{
        height: 50px;
    }

    .img-svg{
        width: 45px;
    }
}
.images-flex{
    display: flex;
    justify-content: space-around;
}

</style>