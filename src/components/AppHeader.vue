<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            navbarLinks : [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP',
            ]

        }
    }
}
</script>

<template>
  <header class="container">
        <div class="header-logo">
            <img src="../assets/img/dc-logo.png" alt="logo-image">
        </div>
        <div class="navbar">        
            <ul>
                <li v-for="link in navbarLinks" >
                    <a :href="link">
                        {{ link }}
                    </a>
                </li>
            </ul>          
        </div>
    </header>
</template>

<style lang="scss" scoped>

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

  header{
        
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100px;

        .header-logo img{
            color: $primaryColor;
            height: 80px;  
        }

        .navbar ul{
            display: flex;
            
            
            li a{
                padding: .8rem;
                font-size: .8rem;
                font-weight: 600;
                transition: color .5s ease;

                &:hover{
                    color: $primaryColor;
                    
                }
            }
        }     
    }
</style>
