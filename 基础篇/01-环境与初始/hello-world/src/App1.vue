<template>
  <div id="app">
    <ol>
      <todo-item
        v-for="item in groceryList"
        v-bind:todo="item"
        v-bind:key="item.id"
      ></todo-item>
    </ol>
  </div>
</template>

<script>
import TodoItem from './components/TodoItem.vue'

export default {
  name: 'app',
  data () {
    return {
      groceryList: [
        {
          id: 0,
          text: '蔬菜'
        },
        {
          id: 1,
          text: '奶酪'
        },
        {
          id: 2,
          text: '随便其他什么人吃的东西'
        }
      ]
    }
  },
  components: {
    TodoItem
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>