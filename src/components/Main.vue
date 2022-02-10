<template>
<main>
  <HomeSlider/>
  <TextUnderSlider/>
  <SpeciaList/>
  <EploreRecentWork/>
  <LatestNews/>
  <TrustedPartner/>
  
  
</main>
 
</template>

<script>
import HomeSlider from './section/main/HomeSlider.vue'
import TextUnderSlider from './section/main/TextUnderSlider.vue'
import SpeciaList from './section/main/SpeciaList.vue'
import EploreRecentWork from './section/main/EploreRecentWork.vue'
import LatestNews from './section/main/LatestNews.vue'
import TrustedPartner from './section/TrustedPartner.vue'
export default {
  name: 'Main',
  props: {
    
    },
  components:{
    HomeSlider,
    TextUnderSlider,
    SpeciaList,
    EploreRecentWork,
    LatestNews,
    TrustedPartner
  }
}
</script>


<style scoped lang="scss">

</style>
