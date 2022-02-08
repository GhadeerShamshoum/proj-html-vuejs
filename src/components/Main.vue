<template>
<main>
  <HomeSlider/>
  <TextUnderSlider/>
  <SpeciaList/>
  <EploreRecentWork/>
  
</main>
 
</template>

<script>
import HomeSlider from './section/HomeSlider.vue'
import TextUnderSlider from './section/TextUnderSlider.vue'
import SpeciaList from './section/SpeciaList.vue'
import EploreRecentWork from './section/EploreRecentWork.vue'
export default {
  name: 'Main',
  props: {
    
    },
  components:{
    HomeSlider,
    TextUnderSlider,
    SpeciaList,
    EploreRecentWork
  }
}
</script>


<style scoped lang="scss">

</style>
