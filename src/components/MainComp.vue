<template>
    <main>
        <div id="jumbotron">

        </div>
        <section id="products">
            <div class="container">
                <span class="label-blue">CURRENT SERIES</span>
                <!--AREA FUMETTO-->
                <div class="area-fumetto">
                <FumettoComp v-for="(element, index) in fumetti "
                 :key="index"
                 :datiFumetto="element"/>
                </div>
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

import FumettoComp from '../components/FumettoComp.vue'

    export default {
        name: 'MainComp',
        components:{
            FumettoComp
        },
        data() {
            return {
                fumetti: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
]
            }
        }
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


    .label-blue{
        background-color:rgb(49, 126, 235) ;
        padding: 10px;
        color: white;
        position: relative;
        top: -55px;
    }
}

#jumbotron{
    background-image: url('../assets/jumbotron.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 300px;
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

.container{
    margin: 0 auto;
    width: 80%;
}

.area-fumetto{
    display: flex;
    flex-wrap: wrap;
    gap: 10px;

    h5{
        margin: 10px 0;
        width: 80%;
    }
}

</style>