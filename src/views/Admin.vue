<template>
  <div class="admin">
    <img alt="Vue logo" src="../assets/logo.png" />
    <TextField :text.sync="name" />
    <p>{{ name }}</p>
  </div>
</template>

<style scoped>
.admin {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import TextField from "@/components/TextField.vue"; // @ is an alias to /src

@Component({
  components: {
    TextField
  }
})
export default class Admin extends Vue {
  name = "";
}
</script>
