<template>
  <div class="hello">
    <h1 class="text-3xl text-gray-700 font-bold mt-8">
      TailwindCSS v2 + Vue v3
    </h1>
    <p class="text-gray-500 mt-4">
      {{ msg }}
    </p>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component"

@Options({
  props: {
    msg: String
  }
})
export default class HelloWorld extends Vue {
  msg!: string
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
p {
  font-style: italic;
}
</style>
