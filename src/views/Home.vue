<template>
  <div>
    <h1>This is Home page</h1>
    <p>{{ name }}</p>
    <Coder title /><br /><br />
    <label for="">Name</label>
    <input type="text" />
    <br /><button>Submit</button>

    <InputField :name="name" @update-name="name = $event.target.value" />
    <!-- <InputField v-model="name">   위 코드를 이렇게 변경가능! -->

    <div>{{ name }}</div>
  </div>
</template>


<script>
import Coder from "@components/Coder.vue";
import InputField from "../components/InputField.vue";

export default {
  components: {
    Coder,
    InputField,
  },

  data() {
    return {
      name: "coder",
    };
  },
  // methods: {
  //   updateName(name) {
  //     this.name = name;
  //   }
  // }
};
</script>

<style scoped>
</style>
