<template>
  <main class="bg-primary">
    <div class="container py-5">
      <div class="row justify-content-center row-cols-2 row-cols-sm-3 row-cols-md-4 row-cols-lg-6">
        <div v-if="cardRay == null" class="text-center">Loading Data</div>
        <SingleCard v-for="card in cardRay" :key="card.id" :card-data="card"/>
      </div>
    </div>
  </main>
</template>

<script>
import axios from 'axios';
import SingleCard from './SingleCard.vue';
export default {
  name: 'MainDisc',
  components:{
    SingleCard
  },
  data() {
    return {
      cardRay: null,
    };
  },
  created() {
    axios
    .get('https://flynn.boolean.careers/exercises/api/array/music')
      .then((response) => {
        this.cardRay = response.data.response;
        console.log(response.data.response)
      });
  },
}
</script>

<style scoped lang='scss'>

</style>