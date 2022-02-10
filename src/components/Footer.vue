<template>
<div>
  <FooterTop/>
  <FooterMiddle/>
  <FooterBottom/>
  <FooterLastDiv/>
  
</div>
 
</template>

<script>
import FooterTop from './section/footer/FooterTop.vue'
import FooterMiddle from './section/footer/FooterMiddle.vue'
import FooterBottom from './section/footer/FooterBottom.vue'
import FooterLastDiv from './section/footer/FooterLastDiv.vue'



export default {
  name: 'Footer',
  props: {
    
  },
  components:{
    FooterTop,
    FooterMiddle,
    FooterBottom,
    FooterLastDiv
  }
}
</script>


<style scoped lang="scss">

</style>
