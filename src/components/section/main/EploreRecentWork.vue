<template>
    <section>    
      <h3>Explore recent work</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="containerPics">
        <div v-for="(element, index) in images" :key="index" class="listContainer">
          <img :src="require('../../../assets/img/'+element.image+'.jpg') " alt="">  
          <div class="cardHover">
            <div class="hoverItemsCard">
              <div class="searchLink">
                <div class="linki"><i class="linkIcon fa-solid fa-link"></i></div>
                <div class="searchi"><i class="searchIcon fa-solid fa-magnifying-glass"></i></div>
              </div>
              <div class="florida">Florida Health Facility</div>
              <div class="commercial">Commercial</div>
            </div>
          </div> 
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
import OurCoreBottom from '../../commons/OurCoreBottom.vue'
import OurCoreImg from '../../commons/OurCoreImg.vue'

export default {
  name: 'EploreRecentWork',
  data(){
    return{
      images:[
        {
          image: "project2-featured-15013609"
        },
        {
          image: "project1-featured-294276386"
        },
        {
          image: "project3-featured-189023420"
        },
      ]
    }
  },
  
  props: {
    
  },
  components:{
    OurCoreBottom,
    OurCoreImg
  }
  

}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";
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
    position: relative;
    overflow: hidden;
    &:hover{
      transition: all 2s linear;
    }
    &:hover .cardHover{
      display: block;
    }
    .cardHover{
      position: absolute;
      top:0;
      right: 0;
      width: 100%;
      height: 100%;
       background-color: $brightSun;
       display: none;
       .hoverItemsCard{
         height: 100%;
         display: flex;
         flex-direction: column;
         justify-content: center;
         align-items: center;
         .searchLink{
           display: flex;
           .searchi,
           .linki{
             height: 50px;
             width: 50px;
             background-color: white;
             border-radius: 50%;
             margin: 10px;
             display: flex;
             justify-content: center;
             align-items: center;
             .searchIcon,
             .linkIcon{
               color: $sun;
             }
            
           }
         }
          .florida{
            font-size: 15px;
            color:white;
          }
          .commercial{
            font-size: 12px;
            color:white
          }
       }
    }
    
    img{
      width: 100%;
      object-fit: cover;
    }
  }
}

</style>
