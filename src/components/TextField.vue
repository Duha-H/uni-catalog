<template>
  <input type="text" v-model="text" />
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class TextField extends Vue {
  @Prop() private text = "";
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input {
  padding: 5px;
  background: #333333;
  color: white;
  border: 1px solid transparent;
  border-radius: 5px;
}

input:focus {
  border: 1px solid var(--accent);
}
</style>
