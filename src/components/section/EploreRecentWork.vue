<template>
    <section>    
      <h3>Exploree recent work</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="containerPics">
        <div class="listContainer">
          <img src="../../assets/img/project2-featured-15013609.jpg" alt="">   
        </div>
        <div class="listContainer">
          <img src="../../assets/img/project1-featured-294276386.jpg" alt="">   
        </div>
        <div class="listContainer">
          <img src="../../assets/img/project3-featured-189023420.jpg" alt="">   
        </div> 
      </div>
      <div class="viewAllPro">View all projects</div>   
      <div class="ourCoreValues">
        <h3>our core values</h3>
        <div class="textContainer">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
        </div>
        
        <!-- Our Core Bottom -->
        <div class="ourCoreBottom">
           <div class="cardBottom">
            <div class="coloredIcon"><i class="fas fa-home"></i></div>
            <title>Great Services</title>
            <p>Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia</p>
          </div>
           <div class="cardBottom">
            <div class="coloredIcon"><i class="far fa-cog"></i></div>
            <title>Great Services</title>
            <p>Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia</p>
          </div>
          <div class="cardBottom">
            <div class="coloredIcon"><i class="fas fa-users"></i></div>
            <title>Great Services</title>
            <p>Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia</p>
          </div>
          <div class="cardBottom">
            <div class="coloredIcon"><i class="far fa-lightbulb"></i></div>
            <title>Great Services</title>
            <p>Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia</p>
          </div>
        </div>

      </div>
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
    </section>
</template>

<script>

export default {
  name: 'EploreRecentWork',
 

  
  props: {
    
  },
  

}
</script>


<style scoped lang="scss">
@import "../../assets/style/variabiles.scss";
section{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
h3{
  font-weight: 300;
  text-transform: capitalize;
  position: relative;
  padding: 40px 0;
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

.textContainer{
  width: 850px;
  p{
    margin: 50px 0;
    font-weight: 100px;
    color: $doveGray;
  }
}

.viewAllPro{
  position: relative;
  text-transform: uppercase;
  color:$doveGray;
  letter-spacing: 0.1rem;
  font-size: 15px;
  margin:60px 0;
}

.viewAllPro::before{
  content: '';
  position: absolute;
  left: 188px;
  top:50%;
  width: 393px;
  border: 1px solid $lightGray;
}
.viewAllPro::after{
  content: '';
  position: absolute;
  right: 188px;
  top:50%;
  width: 393px;
  border: 1px solid $lightGray;
}

.ourCoreValues{
  background-color: #eeeded;
  height: 500px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;


}

.containerPics{
  width: 1000px;
  display: flex;
  .listContainer{
    width: calc(100% / 3 - 10px);
    height: 310px;
    margin: 5px;
    display: flex;
    flex-direction: column;
    align-items: center;
    
    img{
      width: 100%;
      object-fit: cover;
    }
  }
}

.ourCoreBottom{
  width: 1000px;
  display: flex;

  .cardBottom{
    width: calc(100% / 4 - 10px);
    display: flex;
    flex-direction: column;
    align-items: center;

  }
}
.coloredIcon{
  background-color: #4EA4A5;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}
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
