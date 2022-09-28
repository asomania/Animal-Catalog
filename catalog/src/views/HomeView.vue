<template>
  <MyToDo />
</template>

<script>
import { defineComponent } from "vue";

// Components
import myToDo from "../components/myToDo.vue";
import MyToDo from "../components/myToDo.vue";

export default defineComponent({
  name: "HomeView",

  components: {
    myToDo,
    MyToDo,
  },
});
</script>
