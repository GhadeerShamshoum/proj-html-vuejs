<template>
    <div>    
        <!-- Our Core Bottom -->
        <div  class="ourCoreBottom">
           <div v-for="(element, index) in cards" :key="index" class="cardBottom">
            <div :class=(element.color) class="coloredIcon"><i class="icon" :class=(element.icon)></i></div>
            <h4>{{element.title}}</h4>
            <p>{{element.text}}</p>
          </div>
        </div>
    </div>
</template>

<script>

export default {
  name: 'OurCoreBottom',
   data(){
      return{
          cards:[
              {
                icon:"fas fa-home ",
                color:"turquoise",
                title:"Great Services",
                text:"Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia"
              },
               {
                icon:"fa-solid fa-gear",
                color:"blue",
                title:"Highest Standards",
                text:"Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia"
              },
               {
                icon:"fa-solid fa-users",
                color:"orange",
                title:"Professional Team",
                text:"Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia"
              },
               {
                icon:"far fa-lightbulb",
                color:"green",
                title:"Creative Solutions",
                text:"Neque porro quisquam est. qui dolorem ipsum quia dolor sit amet. consectetur, adipisci velit, sed quia"
              },
               
          ]
      }
  },
 

  
  props: {
    
  },
  

}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";

.ourCoreBottom{
  width: 1000px;
  display: flex;
  flex-direction: row;

  .cardBottom{
    width: calc(100% / 4 - 10px);
    display: flex;
    flex-direction: column;
    align-items: center;
    &:hover .coloredIcon{
    background-color: $sun;
    }
    &:hover h4{
    color: $sun;
    }
    h4{
      color: $doveGray;
      padding: 20px 0;
      position: relative;
      &::after{
        content: '';
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translate(-50%);
        width: 20px;
        border:1px solid $LimedSpruce;
      }
    }

    p{
      text-align: center;
      color: $doveGray;
    }

  }
}
.coloredIcon{
  border-radius: 50%;
  width: 80px;
  height: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  
}
.icon{
  color: $white;
  font-size: 35px;
}

.show{
  display: block;
}
.turquoise{
  background-color: #4EA4A5;
}
.blue{
  background-color: #4E6DA5;
}
.orange{
  background-color: #F6722A;
}

.green{
  background-color: #A7CF47;
}


</style>
