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
      <OurCoreBottom/> 
      </div>
      <OurCoreImg/>
    </section>
</template>

<script>
import OurCoreBottom from '../commons/OurCoreBottom.vue'
import OurCoreImg from './OurCoreImg.vue'

export default {
  name: 'EploreRecentWork',
 

  
  props: {
    
  },
  components:{
    OurCoreBottom,
    OurCoreImg
  }
  

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

</style>
