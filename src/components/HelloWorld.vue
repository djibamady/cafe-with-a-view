<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
     <p>{{contenu}}</p>
     <ul>
        <li>Pommes: {{ costOfApples }}€</li>
        <li>Bananes: {{ costOfBananas }}€</li>
        <li>Noix de coco: {{ costOfCoconuts }}€</li>
      </ul>
      <p>Total: {{ totalAmount }}€</p>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Hello',
  props: {
    msg: String,
    contenu: String,
    costOfApples: Number,
    costOfBananas: Number,
    costOfCoconuts: Number

  },
    computed: {
    totalAmount() {
      return this.costOfApples + this.costOfBananas + this.costOfCoconuts
    }
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
