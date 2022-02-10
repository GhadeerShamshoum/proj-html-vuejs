<template>
    <section>
      <div class="containerUnderSlider">
        <div class="textUnderSlider">
          do you have a construction project we can help with?
        </div>
         <button class="buttonCenter"><a href="#">Get a free quote</a></button>
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
@import "../../../assets/style/variabiles.scss";



.containerUnderSlider{
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: $brightSun;
  position: relative;
  .textUnderSlider{
    text-transform: capitalize;
    letter-spacing: 0.1em;
  }
  button{
    position: absolute;
    bottom:-15px;
    border: 1px solid white;
    background-color: $LimedSpruce;
    padding: 5px 30px;
    &:hover{
    background-color: $white;
    transition: all .5s linear;
    border:2px solid black;
    }
    &:hover a{
      color: $doveGray;
    }
    a{
      color: $white;
      font-size: 12px;
      letter-spacing: 0.1rem;
    }
  }
}



</style>
