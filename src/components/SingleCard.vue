<template>
   <div class="card-disco m-3 p-4">
    <img class="img-fluid" :src="cardData.poster" :alt="cardData.title">
    <h3 class="text-center py-2">{{ cardData.title }}</h3>
    <h4 class="text-center">{{ cardData.author }}</h4>
    <h4 class="text-center">{{ cardData.year }}</h4>
  </div>
</template>

<script>

export default {
    name: 'SingleCard',
    props: {
    cardData: Object,
    },
}

</script>

<style scoped lang='scss'>
@import '../assets/styles/variables.scss';
.card-disco{
    background-color: $header_background;
    h3{
        color: white;
        text-transform: uppercase;
        font-size: 1.5rem;
    }
    
}
</style>