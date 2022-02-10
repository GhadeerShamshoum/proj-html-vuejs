<template>
    <section>    
      <h3>Trusted Partners</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="partnersContainer">
        <div class="imgcontainer" v-for="(element, index) in sponsers" :key="index" >
          <img :src="require('../../../assets/img/sponsers/'+element.image+'.png') " alt="">
        </div>
      </div>
      
    </section>
</template>

<script>


export default {
  name: 'TrustedPartner',
  data(){
    return{
      sponsers:[
        {
          image:"home-logo11-219096700-320x202",
        },
        {
          image:"home-logo10-219096700-320x202",
        },
        {
          image:"home-logo2-219096700-320x202",
        },
        {
          image:"home-logo1-219096700-320x202",
        },
        {
          image:"home-logo9-219096700-320x202",
        },
      ]

    }
  },
 
  props: {
    
  },
  components:{
 
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
.partnersContainer{
  width: 1000px;
  height: 200px;
  display: flex;
  justify-content: space-between;
  .imgcontainer{
    width: calc(100% / 5 );
    img{
      width: 100%;
    }

  }
}

</style>
