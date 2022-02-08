<template>
    <section>
      <div class="containerUnderSlider">
        <div class="textUnderSlider">
          do you have a construction project we can help with?
        </div>
      </div>
    </section>
</template>

<script>
export default {
  name: 'TextUnderSlider',
  
  props: {
    
  }
}
</script>


<style scoped lang="scss">
@import "../../assets/style/variabiles.scss";



.containerUnderSlider{
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: $brightSun;
  .textUnderSlider{
    text-transform: capitalize;
    letter-spacing: 0.1em;
  }
}



</style>
