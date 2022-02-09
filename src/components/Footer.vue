<template>
<div>
  <FooterTop/>
  <FooterMiddle/>
  <FooterBottom/>
  
</div>
 
</template>

<script>
import FooterTop from './section/footer/FooterTop.vue'
import FooterMiddle from './section/footer/FooterMiddle.vue'
import FooterBottom from './section/footer/FooterBottom.vue'



export default {
  name: 'Footer',
  props: {
    
  },
  components:{
    FooterTop,
    FooterMiddle,
    FooterBottom
  }
}
</script>


<style scoped lang="scss">

</style>
