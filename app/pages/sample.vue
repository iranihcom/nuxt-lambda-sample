<template>
<div>
  <h1>This is Test</h1>
  <pre>{{testUser}}</pre>
  <v-btn>ボタン2</v-btn>
</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  components: {
  },
})
export default class SamplePage extends Vue {
  myname = {
      firstName: "Masanari",
      lastName: "Mochizuki"
    }
  get testUser(){
    return this.myname
  }
}
</script>