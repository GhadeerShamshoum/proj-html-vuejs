<template>
<menu>
    <ul>
        <li v-for="(element, index) in links" :key="index">
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


  ul{
    display: flex;
    align-items: center;
    list-style: none;
    margin: 0;
    li{
      margin: 10px; 
        text-transform:uppercase;
        a{
          color:$doveGray; 
          &:hover{
            color:$brightSun;

          }
        }
    }
  }
}
button{
  background-color: $brightSun;
  border: none;
  width: 132px;
  height: 33px;
  a{
    text-decoration: none;
    color:$doveGray; 
    text-transform:uppercase;
  }
}
.active{
    color:$brightSun !important;
}

</style>
