<template>

  <div>
    <h1>This is Home page</h1>
    <p>{{name}}</p>
    <Coder title/><br><br>
    <label for="">Name</label>
    <input type="text">
    <br><button>Submit</button>
    
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
