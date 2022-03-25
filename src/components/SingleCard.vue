<template>
   <div class="card-disco bg-secondary m-3 p-4">
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

<style>

</style>