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
                <section>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                    </ul>
                    <h2>SHOP</h2>
                    <ul>
                        <li>shop</li>
                        <li>shop</li>
                    </ul>
                </section>
                <section>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                    </ul>
                </section>
                <section>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                        <li>characters</li>
                    </ul>
                    
                </section>
                
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
        }

    }








</style>