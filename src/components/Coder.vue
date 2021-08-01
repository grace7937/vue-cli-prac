<template>
  <div>
    {{ name }}
  </div>
    <p>{{ title }}</p>
  <button @click="updateName">Change Name</button>
  <slot name="header"></slot>
</template>



<script>
export default {
  props: {
    title: {
      type: String,
      require: false,
      default: 'basic',
    },
    age : {
      type: String,
      default: 'dasic name'
    }
  },
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