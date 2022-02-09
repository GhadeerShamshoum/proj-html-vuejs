<template>  
      <div class="imgContainer">
        <div class="bendTop"></div>
        <div class="container">
          <h3>Our home owners say</h3>
          <img src="../../assets/img/home-testimonial-113165296.jpg" alt="">
          <p>"No man but feels more of a man in the world if he have but a bit of ground that he can call his own. However small it is on the surface, it is four thousand miles deep: and that is a very handsome property"</p>
          <p class="nameAuthor">HARRY SMITH-NEW HOME OWNER</p>
         
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
.container{
  flex-direction: column;
  align-items: center;
  h3{
    color: $white;
    font-weight: 300;
    text-transform: capitalize;
    position: relative;
    padding: 20px 0;
    &::after{
      content: "";
      border-bottom: 2px solid $brightSun;
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 130px;
    }
  }
  img{
    border-radius: 50%;
    margin-top: 20px;
  }
  p{
    width: 635px;
    text-align: center;
    color: $white;
    font-weight: 300;
    margin: 30px;
  }
  .nameAuthor{
    font-weight: 500;
  }
}

  

.imgContainer{
  width: 100%;
  height: 798px;
  position: relative;
  background-image: url('../../assets/img/home-parallax-144609983.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
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
