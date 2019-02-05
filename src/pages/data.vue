<template>
  <div class="container">
    <div class="item">data(string): {{ sampleDataString }}</div>
    <div class="item">data(number): {{ sampleDataNumber }}</div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class PagesData extends Vue {
  sampleDataString: string = 'サンプルデータ(String)'
  sampleDataNumber: number = 123
}
</script>

<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  padding: 50px;
}
.item {
  padding: 10px;
}
</style>
