<template>

  <div>
    <h1>This is Home page</h1>
    <p>{{name}}</p>
    <Coder/>
  </div>
  
</template>



<script>

import Coder from '@/components/Coder.vue';

export default {

  components: {
    Coder
  },

  data() {
    return {
      name: "coder",

    }
  },
}
</script>


<style scoped>

</style>
