<template>
  <div>
    <nav-bar/>
    <Nuxt />
     <div class="h-56 bg-blue-900 mt-40">
    <div class="flex justify-center">
      <div class="shadow-2xl w-10/12 h-40 rounded-md bg-gray-700 -mt-20 grid grid-cols-1 md:grid-cols-3 items-center">
        <div class="">
          <p class="text-4xl font-exo font-bold text-white ml-8">Start a Project</p>
        </div>
         <div class="">
          <p class="text-lg font-exo text-white ml-8">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Explicabo</p>
        </div>
         <div class="flex justify-center">
            <button
                    class="flex justify-center rounded-full text-white font-exo border-2 mt-4 border-white px-5 py-3 hover:bg-blue-600 hover:border-blue-600 hover:text-white font-body font-bold"
                  >
                    Visit Website
                  </button>
        </div>
      </div>
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
