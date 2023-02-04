<template>
  <span>{{ text }}</span>
</template>

<script lang="ts">
import { Component, Vue, Prop } from "vue-property-decorator";

@Component
export default class SmText extends Vue {
  @Prop()
  private text!: string;
}
</script>
