<template>
<div> 
  <FooterTopBackground/>
</div>
 
</template>

<script>
import FooterTopBackground from '../../commons/footer/FooterTopBackground.vue'

export default {
  name: 'FooterTop',
  props: {
    
  },
  components:{
    FooterTopBackground,
  }
}
</script>


<style scoped lang="scss">
.imageContainer{
  background-color: gray;
  height: 350px;
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
