<template>
  <div class="hello">
        <h3>3- Je sélectionne ma couleur</h3>
<div>
  <input type="checkbox" id="scales" name="scales"
         checked>
  <label for="scales">Blanc</label>
</div>

<div>
  <input type="checkbox" id="horns" name="horns">
  <label for="horns">Noir</label>
</div>
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
