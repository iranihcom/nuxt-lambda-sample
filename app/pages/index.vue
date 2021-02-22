<template>
<div>
  <h1>This is Test</h1>
  <pre>{{testUser}}</pre>
  <v-btn>ボタン</v-btn>
</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  components: {
  },
})
export default class IndexPage extends Vue {
  myname = {
      firstName: "Masanari",
      lastName: "Mochizuki"
    }
  get testUser(){
    return this.myname
  }
}
</script>