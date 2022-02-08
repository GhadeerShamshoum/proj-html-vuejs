<template>
<main>
  <HomeSlider/>
  <TextUnderSlider/>
  
</main>
 
</template>

<script>
import HomeSlider from './section/HomeSlider.vue'
import TextUnderSlider from './section/TextUnderSlider.vue'
export default {
  name: 'Main',
  props: {
    
    },
  components:{
    HomeSlider,
    TextUnderSlider
  }
}
</script>


<style scoped lang="scss">

</style>
