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
    <footer>
        <div class="container">
            <section class="footer-left">
                <button>SIGN-UP NOW!</button>
            </section>
            <section class="footer-right">
                <h2>FOLLOW US</h2>
                <div class="icons">
                    <img src="../assets/img/footer-facebook.png" alt="facebook-logo">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest-logo">
                    <img src="../assets/img/footer-periscope.png" alt="periscope-logo">
                    <img src="../assets/img/footer-twitter.png" alt="twitter-logo">
                    <img src="../assets/img/footer-youtube.png" alt="youtube-logo">
                </div>


            </section>
            </div>         
    </footer>
  
</template>

<style lang="scss" scoped>

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

footer{
    background-color: $footerColor;
    
    & .container{
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
}
}
.footer-left button{
    border: 2.5px solid $primaryColor;
    padding: 7px 12px;
    background-color: $footerColor;
    color: $colorText;
    transition: all 1s cubic-bezier(.215, .61, .355, 1);

    &:hover{background-color: $primaryColor;}
}

.footer-right{
    display: flex;
    align-items: center;

    h2{
        color: $primaryColor;
        margin-right: 1rem;
    }

    .icons img{
        margin-left: 0.8rem;
    }
}

  
</style>