<template>
<menu>
    <ul>
        <li class="listMenu" :class='{visabile: element.current==true}' v-for="(element, index) in links" :key="index">
          <a :class='{active: element.current==true}' href="#">{{element.text}}</a>
        </li>
    </ul>
    <button><a href="#">Get Quote</a></button>
</menu>
 
</template>

<script>
export default {
  name: 'Menu',
   data(){
      return{
          links:[
              {
                text:"Home",
                url:"#",
                current:true
              },
              {
                text:"About",
                url:"#",
                current:false
              },
              {
                text:"Services",
                url:"#",
                current:false
              },
              {
                text:"Work",
                url:"#",
                current:false
              },
              {
                text:"Articles",
                url:"#",
                current:false
              }     
          ]
      }
  },
  
  props: {
    
  }
}
</script>


<style scoped lang="scss">
@import "../../assets/style/variabiles.scss";

menu{
  display: flex;
  align-items: center;
  height: 100%;


  ul{
    display: flex;
    align-items: center;
    list-style: none;
    margin: 0;
    height: 100%;
    .listMenu{
      margin: 10px; 
      position: relative;
      display: flex;
      align-items: center;
      height: 100%;
      cursor: pointer;
      &:hover a{
        color:$brightSun;
      }
      &:hover::after{
        visibility: visible;
      }
      &::after  {
      content:'';
      position: absolute;
      bottom: -10px;
      left: 50%;
      height: 20px;
      width: 20px;
      background-color: $white;
      transform: rotate(45deg);
      visibility: hidden;
      z-index: 99;
      }
     
        a{
          color:$doveGray; 
          
        }
    }
  }
}
button{
  background-color: $brightSun;
  border: none;
  width: 132px;
  height: 33px;
  margin-left: 10px;
  &:hover{
    background-color: black;
    transition: all .5s linear;
  }
  &:hover a{
    color: white;
  }
  a{
    text-decoration: none;
    color:$doveGray; 
    text-transform:uppercase;
  }
}
.active{
    color:$brightSun !important;
}
.listMenu.visabile::after{
  visibility: visible;
  z-index: 99;

}


</style>
