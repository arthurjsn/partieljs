<template>
  <div class="hello">
    <h2>Personnalisez votre produit :</h2>
        <h3>1- J’indique mes dimensions</h3>
        <label for="name">Longueur du rail</label>
        <input type="number" id="name" min="0" max="200">
  </div>
</template>

<script>
export default {
  name: 'Personnalisation',
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
