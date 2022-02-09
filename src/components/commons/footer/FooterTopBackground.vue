<template>
<div class="imageContainerF"> 
  <div class="firstLayer">
    <img src="../../../assets/img/footer/about-call-to-action-57862405.jpg" alt="">
  </div>
  <div class="secondLayer">
    <img class="secondLaterImg" src="../../../assets/img/footer/about-call-to-action-57862405.jpg" alt="">
  </div>
</div>
 
</template>

<script>
export default {
  name: 'FooterTopBackground',
  props: {
    
  }
}
</script>


<style scoped lang="scss">
.imageContainerF{
  background-color: gray;
  height: 361px;
  .firstLayer{
    position: relative;
    overflow: hidden;
    height: 306px;
    img{
      position: absolute;
      bottom: -141px;
      width: 100%;

    }
  }
  .secondLayer{
    position: relative;
    overflow: hidden;
    height: 42px;
    .secondLaterImg{
      position: absolute;
      bottom: -227px;
      width: 100%;
    }

  }

}

</style>
