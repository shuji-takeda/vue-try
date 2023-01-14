<template>
  <div>
    <p>This is Home View Page</p>
    <SmBtn buttonName="button" @click="click" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SmBtn from "../components/atoms/SmBtn.vue";
import Component from "vue-class-component";

@Component
export default class Home extends Vue {
  onClick(): void {
    window.alert("onClcik");
  }

  click(): void {
    window.alert("click");
  }
}
</script>
