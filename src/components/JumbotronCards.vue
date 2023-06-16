<script>
export default {
    name: 'JumbotronCards',
    props : [
        'singleCard',
    ]
}
</script>

<template>
    <div class="card">
        <div class="card-image">
            <img :src= "singleCard.thumb" alt="series-image"> 
        </div>
        
        <div class="title">
            {{ singleCard.series }}
        </div>
    </div>

</template>

<style lang="scss" scoped>

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    .card{
        width: calc((100% / 6) - 30px);
        color: $colorText;
        
        
    }
    .card-image{
        height: 200px;

    }
    .card-image img{
        width: 100%;
        height: 100%;
    }

    

  
</style>