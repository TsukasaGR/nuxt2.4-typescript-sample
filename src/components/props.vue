<template>
  <div>
    <div class="item">props(string): {{ propsString }}</div>
    <div class="item">props(number): {{ propsNumber }}</div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class ComponentsProps extends Vue {
  @Prop(String)
  propsString!: string
  @Prop(Number)
  propsNumber!: number
}
</script>

<style scoped>
.item {
  padding: 10px;
}
</style>
