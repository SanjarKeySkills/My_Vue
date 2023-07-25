<template>
  <div id="app">
      <AppTodo />
      <TodoList v-bind:todos="todos" />
  </div>
</template>

<script>
import TodoList from './components/TodoList.vue'
import AddTodo from "@/components/AddTodo.vue";
export default (await import('vue')).defineComponent({
  name: 'App',
  components: {
    TodoList,
      AddTodo
  },
    data() {
      return {
          message: "Message",
          someNumber: 23,
          todos: [
              {
                  id: 1,
                  todo: "Task 1",
                  completed: false,
                  effect: true,
                                },
              {
                  id: 2,
                  todo: "Task 2",
                  completed: false,
                  effect: false,
              },
              {
                  id: 3,
                  todo: "Task 3",
                  completed: false,
                  effect: true,
              },
              {
                  id: 4,
                  todo: "Task 4",
                  completed: true,
                  effect: false,
              },
              {
                  id: 5,
                  todo: "Task 5",
                  completed: true,
                  effect: true,
              },

          ]
      }
    },
    methods: {
        increment() {
         this.someNumber = this.someNumber + 1
      }
    },
    created() {
      console.log("created")
    },
    mounted() {
      console.log("mounted")
    }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
