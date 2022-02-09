<template>
    <section>    
      <h3>specialist in modern construction</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
      <div class="container">
        <div class="listContainer">
          <div class="iconContainer"><i class="far fa-building"></i></div>
          <h2>Buildings</h2>
          <p>Quis autem vel eum iure reprodent qui in ea voluptate velit esse quam nihit molestiae consequatu</p>
        </div>
        <div class="listContainer">
          <div class="iconContainer"><i class="fas fa-sync-alt"></i></div>
          <h2>Renovate</h2>
          <p>Quis autem vel eum iure reprodent qui in ea voluptate velit esse quam nihit molestiae consequatu</p>
        </div>
        <div class="listContainer">
          <div class="iconContainer"><i class="fas fa-home"></i></div>
          <h2>Construct</h2>
          <p>Quis autem vel eum iure reprodent qui in ea voluptate velit esse quam nihit molestiae consequatu</p>
        </div>
        <div class="listContainer">
          <div class="iconContainer"><i class="fas fa-truck"></i></div>
          <h2>Exclusive</h2>
          <p>Quis autem vel eum iure reprodent qui in ea voluptate velit esse quam nihit molestiae consequatu</p>
        </div>
      </div>
      <FirstCurvedImgItems/>
     
    </section>
</template>

<script>
import FirstCurvedImgItems from '../commons/FirstCurvedImgItems.vue'

export default {
  name: 'SpeciaList',

  
  props: {
    
  },
  components:{
    FirstCurvedImgItems
  }
  

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
    font-weight: 100px;
    color: $doveGray;
  }
}

.listContainer{
  width: calc(100% / 4 - 10px);
  margin: 5px;
  background-color: #eeeded;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 23px;
  border-radius: 5px;
  color: $doveGray;
  .iconContainer{
    color: $doveGray;
    width: 30px;
    height: 30px;
    padding: 30px;
    border: 1px solid black;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  h2{
    font-weight: 300;
    color: black;
  }
  p{
    text-align: center;
  }
}




</style>
