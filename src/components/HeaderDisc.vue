<template>
  <header>
      <div class="container-fluid">
          <img src="../assets/spotify_logo.png" alt="">
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
    .container-fluid{

        background-color: $header-background;
        img{
            height: 50px;
            
        }
    }

</style>