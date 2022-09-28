<template>
  <v-container>
    <input class="bg-black" v-model="veri" /><input />
    <v-btn @click="ekle()">ekle</v-btn>
    <v-list :for="(name, index) in metinler" :key="index">{{
      name.text
    }}</v-list>
  </v-container>
</template>

<script>
export default {
  name: "to do",

  data: () => ({
    sayac: 0,
    veri: "",
    deneme: "",
    metinler: [],
  }),
  methods: {
    ekle() {
      this.metinler.push({
        text: this.veri,
        index: this.metinler.length + 1,
      });
    },
  },
};
</script>
