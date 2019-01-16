<template>
  <div style="position: relative">
    <slot name="poppups"></slot>
    <!-- 滑动条 -->
    <div class="verify-bar-area"></div>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop } from "vue-property-decorator";

@Component({})
export default class App extends Vue {
  @Prop({ default: "" }) public myAtty!: string;
}
</script>
<style lang="stylus">
.verify-bar-area {
  position: relative;
  background: #FFFFFF;
  text-align: center;
  -webkit-box-sizing: content-box;
  -moz-box-sizing: content-box;
  box-sizing: content-box;
  border: 1px solid #ddd;
  -webkit-border-radius: 4px;
}
</style>

