<template>
    <section>    
      <h3>Exploree recent work</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="containerPics">
        <div class="listContainer">
          <img src="../../assets/img/project1-featured-294276386.jpg" alt="">   
        </div>
        <div class="listContainer">
          <img src="../../assets/img/project2-featured-15013609.jpg" alt="">   
        </div>
        <div class="listContainer">
          <img src="../../assets/img/project3-featured-189023420.jpg" alt="">   
        </div> 
      </div>
      <div>View all projects</div>   
      <div class="ourCoreValues">
        <h3>our core values</h3>
        <div class="textContainer">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
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
  padding: 40px 0;
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
    height: 500px;
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
.imgContainer{
  width: 100%;
  height: 600px;
  position: relative;
  background-image: url('../../assets/img/home-244125289.jpg');
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
