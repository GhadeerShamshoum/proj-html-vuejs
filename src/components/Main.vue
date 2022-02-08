<template>
<main>
  <HomeSlider/>
  <TextUnderSlider/>
  <SpeciaList/>
  
</main>
 
</template>

<script>
import HomeSlider from './section/HomeSlider.vue'
import TextUnderSlider from './section/TextUnderSlider.vue'
import SpeciaList from './section/SpeciaList.vue'
export default {
  name: 'Main',
  props: {
    
    },
  components:{
    HomeSlider,
    TextUnderSlider,
    SpeciaList
  }
}
</script>


<style scoped lang="scss">

</style>
