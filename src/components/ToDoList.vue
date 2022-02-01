<template>
  <div>
    <ToDoInput />
    <ToDoItem />
  </div>
</template>

<script>
import ToDoInput from "@/components/ToDoInput.vue";
import ToDoItem from "@/components/ToDoItem.vue";

export default {
  name: 'TodoList',
  components: {
    ToDoInput,
    ToDoItem,
  },
  props: {
    modelValue: {
      type: Array
    },
  },
  data: () => ({

  }),
  methods: {
    
  }
}
</script>