// Descrizione:
// Create un nuovo progetto utilizzando Vue CLI: aiutatevi con le slide per ripercorrere i vari passaggi dell'installazione come visti a lezione.
// Create e utilizzate un componente Title, il quale contiene un titolo che recita "La mia prima app con Vue CLI!"
// Bonus:
// Creare un secondo componente Hero, che visualizza un jumbotron.
<template>
  <div id="app">
    <appTitle msg="Welcome to Your Vue.js App" />
    <appHero :heroPath="hero.path" :heroTitle="hero.title"/>
  </div>
</template>

<script>
import appTitle from './components/appTitle.vue'
import appHero from './components/appHero.vue'

export default {
  name: 'App',
  components: {
    appTitle,
    appHero
  },
  data: function() {
    return {
      hero: {
        path: "vue.png",
        title: "Vue Hero"
      }
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 2rem;
  
  height: 100vh;
}
</style>
