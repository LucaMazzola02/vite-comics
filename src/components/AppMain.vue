<script>
export default {
    name: 'AppHeader',
    data(){
        return{

        }
    }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="container">
                <h2>-- Content goes here --</h2>
            </div>    
        </div>
        <div class="main-bottom">
            <div class="container flex">
                <div class="sections">
                   <section>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h2>SHOP</h2>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </section>
                <section>
                    <h2>DC</h2>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </section>
                <section>
                    <h2>SITES</h2>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>MAD Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                    
                </section> 
                </div>
                <div class="main-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="main logo image">
                </div>
                
                
            </div>
        </div>
    </main>
  
</template>

<style lang="scss" scoped>

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    .main-top{
        display: flex;
        align-items: center;
        height: 120px;
        background-color: $secondaryColor;
        color: $colorText;
        text-align: left;

        h2{
            font-size: 1.5rem;
        }
    }

    .main-bottom{
        display: flex;
        height: 400px;
        background-image: url(../assets/img/footer-bg.jpg);

        section{
            padding-top: 2rem;
            margin-right: 2.7rem;
        }

        section h2{
            color: $colorText;
            margin: 1rem 0 .6rem ;
        }

        section ul li{
            color: #9c9c9c;
            font-size: .8rem;
            margin-bottom: 0.4rem;
            transition: all .3s cubic-bezier(.215, .61, .355, 1);
        }
        section ul li:hover{
            color: $colorText;
        }

    }
    .sections{display: flex;}

    .main-logo{
        display: flex;
        justify-content: center;
        align-items: center;
        padding-left: 12%;
    }
    .main-logo img{
        width: 400px;

    }
</style>