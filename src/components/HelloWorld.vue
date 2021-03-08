<template>
  <div>
    <h3>Halo DIL POC</h3>
    <div>
       <label> Public Variable </label>
       <span> Value {{publicVariableValue}} </span>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  private publicVariableValue: string;

  public constructor() {
    super();
    this.publicVariableValue = "New Pubic Variable";
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
