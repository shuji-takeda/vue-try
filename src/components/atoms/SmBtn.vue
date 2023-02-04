<template>
  <div>
    <v-btn @click="onClick">{{ buttonName }}</v-btn>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";
import { Prop } from "vue-property-decorator";

@Component
export default class SmBtn extends Vue {
  @Prop()
  private buttonName!: string;

  private onClick() {
    this.$emit("click");
  }
}
</script>
