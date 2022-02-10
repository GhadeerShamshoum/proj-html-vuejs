<template>
<div class="containerItemsFT"> 
  <div class="itemsLeft">
    <h3>Building inspiring spaces</h3>
    <div class="textContainerL">
      <p class="textLeft">Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit </p>
    </div>
  </div>
  <div class="itemsRight">
    <button class="buttonFooterTop"><a href="#">Get a free quote</a></button>
    <div class="textUnderBtn">Only takes a few seconds!</div>

  </div>
  <div>
  </div>
  
</div>
 
</template>

<script>
export default {
  name: 'FooterTopItems',
  props: {
    
  }
}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";
.containerItemsFT{
  display: flex;
  align-items: center;
  width: 1000px;
  margin: auto;
  height: 100%;
  .itemsLeft{
    width: 50%;
  }

}
h3{
  color: $white;
  font-weight: 300;
  text-transform: capitalize;
  position: relative;
  padding: 20px 0;
  &::after{
    content: "";
    border-bottom: 2px solid $brightSun;
    position: absolute;
    bottom: 0;
    left: 0;
    width: 130px;
  }
}

.textContainerL{
  width: 100%;
  .textLeft{
    color: $white;
  font-weight: 300;
  text-transform: capitalize;
  position: relative;
  padding: 20px 0;
  }
}

.itemsRight{
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  .buttonFooterTop{
    position: relative;
    border: none;
    padding: 11px 40px;
    background-color: $brightSun;
    &:hover{
    background-color: black;
    transition: all .5s linear;
  }
  &:hover a{
    color: white;
  } 
    a{
      letter-spacing: 0.1rem;
      color:$doveGray ;
    }
  }
  .textUnderBtn{
    position: relative;
    color: $white;
    padding: 20px 0;
  }
}

</style>
