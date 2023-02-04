<template>
  <div class="pa-10">
    <todo-card />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import TodoCard from "../components/molecules/TodoCard.vue";
import Component from "vue-class-component";

@Component({
  components: {
    TodoCard,
  },
})
export default class Home extends Vue {
  onClick(): void {
    window.alert("onClcik");
  }

  click(): void {
    window.alert("click");
  }
}
</script>
