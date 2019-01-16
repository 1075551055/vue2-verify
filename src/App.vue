<template>
  <components
    :is="type"
    v-bind="$attrs"
  ></components>
</template>

<script lang="ts">
import { Component, Vue, Prop } from "vue-property-decorator";
import Slide from "./components/Slide.vue";

@Component({
  components: {
    Slide
  }
})
export default class App extends Vue {
  @Prop({ default: "slide" }) public type!: string;
}
</script>
