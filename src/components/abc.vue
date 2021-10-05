
<template>
  <div class="hello">
   <input type="button" value="gfhui">

   <div id="app">
    <ul>
        <li v-for="item, index in items" :key="item.message">
            {{ item.message }}
            <button @click="removeTask(index)">Remove</button>

        </li>
    </ul>

    <form action="" v-on:submit.prevent="addTask">
        <input type="text" v-model="newTask">
        <input type="submit" value="Ajouter une tâche">
    </form>

</div>


  </div>
</template>





<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
