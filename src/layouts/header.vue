<template>
  <header>
    <nuxt-link to="/" tag="div" class="item">top</nuxt-link>
    <nuxt-link to="data" tag="div" class="item">data</nuxt-link>
    <nuxt-link to="props" tag="div" class="item">props</nuxt-link>
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 60px;
  border-bottom: 1px solid gray;
}
.item {
  cursor: pointer;
}
</style>
