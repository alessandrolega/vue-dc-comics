<template>
    <footer>
        <div class="container">
          <div class="footer-list">
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>
                </ul>

                <h3>SHOP</h3>

                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                   
                </ul>
            </div>
            <div>
                <h3>DC</h3>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy Policy (New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Show Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div>
                <h3>SITES</h3>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>

        
        </div>
    <div class="bg-logo">
        <!-- <img src="../assets/dc-logo-bg.png" alt=""> -->
    </div>  
        </div>

        <section id="footer-cta">
            <div class="container">
                <div class="btn">
                    SIGN UP NOW!
                </div>
                <div class="footer-socials">
                    <h3>FOLLOW US</h3>
                    <img src="../assets/footer-facebook.png" alt="socials">
                    <img src="../assets/footer-twitter.png" alt="socials">
                    <img src="../assets/footer-youtube.png" alt="socials">
                    <img src="../assets/footer-pinterest.png" alt="socials">
                    <img src="../assets/footer-periscope.png" alt="socials">

                </div>

            </div>

        </section>
        
    </footer>
</template>

<script>
    export default {
        name: 'FooterComp'
    }
</script>

<style lang="scss" scoped>

footer{
    background-image: url('../assets/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white;

    #footer-cta{
        background-color: #303030;
        padding: 30px 0;

        .btn{
            padding: 15px;
            border: 2px solid rgb(49, 126, 235);
            font-weight: bold;
            font-size: 1.1rem;
        }

    }

    .container{
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;

    }
    
    a{
        color: white;
    }

    .footer-list{
        padding: 30px 0;
        display: flex;
        line-height: 30px;
    }
    .footer-list a{
        color: grey;
    }
}

.bg-logo{
    background-image: url('../assets/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    width: 40%;
}

.footer-list div{
    padding: 20px;
}

.footer-socials{
    display: flex;
    gap: 10px;
    align-items: center;
}
.footer-socials > h3{
    color: rgb(49, 126, 235) ;
    font-size: 1.3rem;
    font-weight: bold;
}

</style>