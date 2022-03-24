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

@import '../assets/styles/variables.scss';
@import '../assets/styles/general.scss';
    .container{
        width: 1600px;
        margin: 0 auto;
        height: 100px;
        background-color: $header-background;
        img{
            height: 100%;
            padding: .5em 2em;
        }
    }

</style>