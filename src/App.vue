<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <ul>
      <li v-for="(todo,index) in todos" v-bind:class="{'checked':todo.done}">
          <label>{{index+1}}.{{todo.value}}</label>
          <time>{{todo.created | date}}</time>
      </li>
    </ul>
  </div>
</template>

<script>
import moment from 'moment'
import 'moment/locale/zh-cn'
moment.locale('zh-cn')

export default {
  name: 'app',
  data () {
    return {
      title: 'Vue-Todos',
      todos:[
        {value:'Java',done:false,created:Date.now()},
        {value:'Python',done:true,created:Date.now()+3000000},
        {value:'Node.js',done:false,created:Date.now()-3000000}
      ]
    }
  },
  filters:{
    date(val){
    return moment(val).calendar()
  }
}
}
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
li {
  list-style-type:none;
}
</style>
