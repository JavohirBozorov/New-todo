<template>
  <div>
    <h2 class="text-center py-5">My To Do App</h2>
    <div class="py-5">
      <form @submit.prevent="submitText">
        <input v-model="item" type="text" />
      </form>
    </div>
    
  </div>
</template>

<script>
export default {
  name: "ToDoInput",
  props: {
    type: Array,
  },
  data: () => ({
    item: "",
  }),
  methods: {
    submitText() {
      this.$emit("submit", this.item);
      this.item = "";
    },
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  input {
    width: 100px;
    height: 30px;
    padding: 0 10px;
    margin: 0;
    font-size: larger;
    border:  none;
    background-color: #fafafa;
  }
  input:focus, input:active {
    border: none;
  }
</style>
