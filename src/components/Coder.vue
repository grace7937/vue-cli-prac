<template>
  <div>
    {{ name }}
  </div>
  <button @click="updateName">Change Name</button>
</template>



<script>
export default {
  data() {
    return {
      name: "apple",
    };
  },

  methods: {
    updateName() {
      this.name = "apple updated";
    },
  },
};
</script>







<style scoped>
</style>