<template>
  <div>
    <nav-bar class="home-nav"><div slot="center">购物街</div></nav-bar>
  </div>
</template>
<script>
import NavBar from 'components/common/navbar/NavBar'
import {getHomeMutidata} from 'network/home.js'
export default{
  name:"Home",
  components:{
    NavBar
  },
  created(){
    getHomeMutidata().then(res=>{
      console.log(res)
    })
  }
}
</script>
<style scoped>
  .home-nav {
    background-color: var(--color-tint);
    color: #fff;
  }
</style>