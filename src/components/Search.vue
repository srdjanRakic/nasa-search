<template>
  <div class="search">
    <h2>Type In Your Search Term:</h2>
    <form v-on:submit.prevent="getResult(query)">
      <input type="text" placeholder="Type in your search" v-model="query">
    </form>
    
  </div>
</template>

<script>
export default {
  name: 'search',
  data () {
    return {
      msg: 'Search:',
      query: "Srle"
    }
  }, 
  methods: {
    getResult(query) {
      alert(query);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
