<template>
  <div id="app">
    <TodoList />

    <!-- <div>
      <button @click="showImage = !showImage">Toggle img</button>
    </div>
    <transition 
      enter-active="animate__animated animate__fadeInDown"
      leave-active="animate__animated animate__fadeOutUp"
    >
      <img v-if="showImage" src="@/assets/logo.png">
    </transition> -->

  </div>
</template>

<script>
import TodoList from "./components/ToDoList.vue";

export default {
  name: "App",
  components: {
    TodoList,
  },
  data: () => ({
    // showImage: true,
  }),
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-top: 60px;
  width: 100%;
  /* background-color: #cae141; */
}
/* img {
  display: inline-block;
  margin: 0 0.5rem;

  animation: bounce;
  animation-duration: 2s; 
} */
</style>
