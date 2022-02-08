<template>
    <section>
      
      <h3>specialist in modern construction</h3>
      <div class="textContainer">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur voluptate amet suscipit architecto libero, placeat dolor iusto voluptates voluptatum labore esse voluptatem ea quisquam repellendus aliquid consequatur, error vero alias?</p>
      </div>
    </section>
</template>

<script>

export default {
  name: 'SpeciaList',
  
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
    font-weight: 100px;
    color: $doveGray;
  }
}





</style>
