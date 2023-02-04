<template>
  <v-checkbox />
</template>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";
import { Prop } from "vue-property-decorator";

@Component
export default class SmCheckBox extends Vue {
  @Prop()
  private buttonName!: string;

  private onClcikEmit() {
    this.$emit("doExecute");
  }
}
</script>
