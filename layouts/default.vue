<template>
  <div>
    <nav-bar/>
    <Nuxt />
    <div>
      <div class="bg-blue-900 h-1/4">
       <h1>Hello</h1> 
      </div>
    </div>
  </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
  name:"WholeLayout",
   components:{
    NavBar,
  }
}
</script>
<style>

</style>
