<template>
  <div>
    <!-- <img src="../assets/vue.png" alt="Vue Hero" class="c-hero"/> -->
    <img :src="require(`@/assets/img/${heroPath}`)" :alt="heroTitle" class="c-hero"/>
  </div>
</template>

<script>
export default {
  name: 'appHero',
  props: {
    heroPath: String,
    heroTitle: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.c-hero {
  width: 100%;
}
</style>
