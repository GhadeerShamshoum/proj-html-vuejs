<template>
<div>
  <TrustedPartner/>
  <FooterTop/>
  <FooterBottom/>
  <FooterLastDiv/>
  
</div>
 
</template>

<script>
import TrustedPartner from './section/footer/TrustedPartner.vue'
import FooterTop from './section/footer/FooterTop.vue'
import FooterBottom from './section/footer/FooterBottom.vue'
import FooterLastDiv from './section/footer/FooterLastDiv.vue'



export default {
  name: 'Footer',
  props: {
    
  },
  components:{
    TrustedPartner,
    FooterTop,
    FooterBottom,
    FooterLastDiv
  }
}
</script>


<style scoped lang="scss">

</style>
