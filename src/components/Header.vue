<template>
 <header>
    <div class="container">
        <Logo/>
        <Menu/>
    </div>
 </header>
</template>

<script>
import Logo from './commons/Logo.vue'
import Menu from './commons/Menu.vue'
export default {
  name: 'Header',
  props: {
    
  },
  components: {
   Logo,
   Menu
  }
}
</script>


<style scoped lang="scss">
@import "../assets/style/variabiles.scss";
header{
    background-color: $white;
    height: 100px;
    display: flex;
    justify-content: center;
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    
}

</style>
