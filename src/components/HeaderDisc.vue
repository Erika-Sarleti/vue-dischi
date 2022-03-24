<template>
  <header>
      <div class="container">
          <img src="../assets/logo.png" alt="">
      </div>
  </header>
</template>

<script>
export default {
    name:'HeaderDisc'

}
</script>

<style scoped lang='scss'>

@import url(../assets/styles/variables.scss);
    .container{
        width: 1400px;
        margin: 0 auto;
        height: 100px;
        background-color: $header-background;
    }

</style>