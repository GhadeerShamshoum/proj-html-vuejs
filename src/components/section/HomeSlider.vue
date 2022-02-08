<template>
    <section>
      <h1>Building Inspiring spaces</h1>
      <h2>We Build Inspiring Residential &amp; Commercial Spaces</h2>
      <div class="buttons">
        <button class="buttonLeft"><a href="#">Explore recent Work</a></button>
        <button class="buttonRight"><a href="#">Get a quote today</a></button>
      </div>
      

    </section>
</template>

<script>

export default {
  name: 'HomeSlider',
  
  props: {
    
  },
  

}
</script>


<style scoped lang="scss">
@import "../../assets/style/variabiles.scss";
section{
    height: 1000px;
    background-image: url('../../assets/img/home-slider-62528242.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h1{
      text-transform:uppercase;
      color: $white;
      font-size: 70px;
      font-weight: 700;
    }
    h2{
      color: $brightSun;
    }
}

.buttons{
  display: flex;
  button{
    border: none;
    padding: 10px 20px;
    margin: 5px;
  }
  .buttonLeft{
    background-color:$LimedSpruce;
    a{
      color: $white;
    }
  }
  .buttonRight{
    background-color: $brightSun;
    a{
      color:$doveGray ;
    }
  }
}
.containerUnderSlider{
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: $brightSun;
  .textUnderSlider{
    text-transform: capitalize;
  }
}



</style>
