<template>
    <section>
      <h1>Building Inspiring spaces</h1>
      <h2>We Build Inspiring Residential &amp; Commercial Spaces</h2>
      <div class="buttons">
        <button class="buttonLeft"><a href="#">Explore recent Work</a></button>
        <button class="buttonRight"><a href="#">Get a quote today</a></button>
      </div>
      <div class="containerBtn"> 
        <div class="demoContainer">
          <i class="fa-solid fa-folder-open"></i>
          <div class="textUnderIcon">Demos</div>
        </div>
          <div class="demoContainer">
          <div class="price">
            <div class="dolar">$</div>
            <span class="thePrice"><strong>39</strong></span>
          </div>
          <div class="textUnderIcon">On Sale</div>
        </div>

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
    position: relative;
    h1{
      text-transform:uppercase;
      color: $white;
      font-size: 70px;
      font-weight: 700;
    }
    h2{
      color: $brightSun;
    }
    .containerBtn{
      position: absolute;
      top:5px;
      right: 5px;
      

      .demoContainer{
        height: 40px;
        width: 40px;
        border-radius: 5px;
        background-color: $white;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: $blue;
        margin-bottom: 5px;
        .textUnderIcon{
          font-size: 10px;
        }
        .price{
          color: rgb(25, 192, 25);
          display: flex;
          height: 19px;
          .dolar{
            font-size: 10px;
            margin-top: 0;
          }
          .thePrice{
            font-size: 18px;
          }
        }
      }
    }
}

.buttons{
  margin-top: 40px;
  display: flex;
  button{
    border: none;
    padding: 10px 80px;
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
