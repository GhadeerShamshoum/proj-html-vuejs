<template>  
      <div class="imgContainer">
        <div class="bendTop"></div>
        <div class="containerNumbers">
          <div>
            <div><i class="fas fa-suitcase"></i></div>
            <div>3534</div>
            <h6>planning Applications</h6>
          </div>
           <div>
            <div><i class="far fa-building"></i></div>
            <div>896</div>
            <h6>planning Applications</h6>
          </div>
        </div>
        <div class="bendBottom"></div>
      </div>
</template>

<script>

export default {
  name: 'OurCoreImg',
 

  
  props: {
    
  },
  

}
</script>


<style scoped lang="scss">
@import "../../assets/style/variabiles.scss";

  

.imgContainer{
  width: 100%;
  height: 600px;
  position: relative;
  background-image: url('../../assets/img/home-parallax-144609983.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  .bendTop{
    background-color: #eeeded;
    position: absolute;
    top:0;
    width: 100%;
    height: 120px;
    border: 1px solid #eeeded;
    border-bottom-right-radius: 100%;
    border-bottom-left-radius: 100%;
  }
  .bendBottom{
    background-color: $white;
    position: absolute;
    bottom:0;
    width: 100%;
    height: 120px;
    border: 1px solid white;
    border-top-right-radius: 100%;
    border-top-left-radius: 100%;

  }
}






</style>
