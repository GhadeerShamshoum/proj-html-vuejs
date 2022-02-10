<template>
<div >
  <div class="footerLastDiv">
    <div class="container">
      <div class="partLeft">
      Copyright 2012-2015 avada theme by theme by <strong>theme fusion</strong>  | all rights reserved | powered by <strong>wordpress</strong> 
      </div>
      <div class="partRight">
        <div class="brands"><i class="fa-brands fa-facebook-f"></i></div>
        <div class="brands"><i class="fa-brands fa-twitter"></i></div>
        <div class="brands"><i class="fa-brands fa-youtube"></i></div>
        <div class="brands"><i class="fa-brands fa-instagram"></i></div>
      </div>
    </div>

  </div>

  
  
</div>
 
</template>

<script>
export default {
  name: 'FooterLastDiv',
  props: {
    
  }
}
</script>


<style scoped lang="scss">
@import "../../../assets/style/variabiles.scss";
.footerLastDiv{
  height: 100px;
  background-color: black;
  display: flex;
  align-items: center;
  .container{
    margin: auto;
    justify-content: space-between;
    align-items: center;
    .partLeft{
      text-transform: uppercase;
      color: $doveGray;
      width: 50%;
      font-size: 10px;
      strong{
        color: $silver;
      }
    }
    .partRight{
      color: $doveGray;
      display: flex;
      .brands{
        padding: 0 5px;
      }
    }
  }
}
 

</style>
