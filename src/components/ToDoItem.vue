<template>

  <div>
    <!-- <input 
      v-for=""
      type="text" 
      v-model="text" 
    /> -->

    <ul id="example-1">
      <li v-for="item in items" :key="item.id" >
        <h2>{{ item.text }}</h2>
      </li>
    </ul>
  </div>

</template>

<script>
export default {
  name: "TodoItem",
  components: {
    
  },
  props: {
    type: Array
  },
  data: () => ({
    items: [
      {text:"First Comment", id:'1', isCompleted:false},
      {text: "Second Comment", id: '2', isCompleted:false},
      {text: "Third Comment", id: '3', isCompleted:false},
    ],
  }),
  // el: "#example-1",
  // data: () => {
  //   items: [
  //     { message: 'Foo', id:1 },
  //     { message: 'Bar', id:2 },
  //   ]
  // },
  computed: {
    
  },
  methods: {
    
  },
}
</script>

<style scoped>
  ul li {
    list-style-type: none;
  }
</style>