<template>
  <div class="container">
    <Props :props-string="propsString" :props-number="propsNumber" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Props from '~/components/props.vue'

@Component({
  components: {
    Props
  }
})
export default class PagesData extends Vue {
  propsString: string = 'サンプルデータ(String)'
  propsNumber: number = 123
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
