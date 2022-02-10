<template>
    <div class="imgContainer">
      <div class="bendTop"></div>
      <div class="containerNumbers">
        <div v-for="(element, index) in cards" :key="index" class="containerItems">
          <div><i class="icon" :class=(element.icon)></i></div>
          <div class="number">{{element.number}}</div>
          <h6>{{element.title}}</h6>
        </div>
      </div>
      <div class="bendBottom"></div>
    </div>  
</template>

<script>

export default {
  name: 'FirstCurvedImgItems',
    data(){
      return{
          cards:[
              {
                icon:"fas fa-suitcase",
                number:"3534",
                title:"planning Applications",
              },
               {
                icon:"far fa-building",
                number:"896",
                title:"completed projects",
              },
               {
                icon:"fa-solid fa-users",
                number:"172",
                title:"trained professionals",

              },
               {
                icon:"fa-solid fa-globe",
                number:"19",
                title:"international offices",
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


.imgContainer{
  width: 100%;
  height: 600px;
  position: relative;
  background-image: url('../../../assets/img/home-244125289.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  .bendTop{
    background-color: $white;
    position: absolute;
    top:0;
    width: 100%;
    height: 120px;
    border: 1px solid white;
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
  .containerNumbers{
    width: 1000px;
    display: flex;
    justify-content: center;
    align-items: center;
    .containerItems{
      width: calc(100% / 4 - 20px);
      margin: 0 10px;
      display: flex;
      flex-direction: column;
      align-items: center;
      .icon,
      .number{
        color: $sun;
        font-size: 40px;
      }
      h6{
        color: $white;
        text-transform: uppercase;
        font-size: 13px;
      }

    }
  }
}





</style>
