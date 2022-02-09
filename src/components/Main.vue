<template>
<main>
  <HomeSlider/>
  <TextUnderSlider/>
  <SpeciaList/>
  <EploreRecentWork/>
  <LatestNews/>
  
</main>
 
</template>

<script>
import HomeSlider from './section/HomeSlider.vue'
import TextUnderSlider from './section/TextUnderSlider.vue'
import SpeciaList from './section/SpeciaList.vue'
import EploreRecentWork from './section/EploreRecentWork.vue'
import LatestNews from './section/LatestNews.vue'
export default {
  name: 'Main',
  props: {
    
    },
  components:{
    HomeSlider,
    TextUnderSlider,
    SpeciaList,
    EploreRecentWork,
    LatestNews
  }
}
</script>


<style scoped lang="scss">

</style>
