<template>
  <q-page class="flex flex-center">
    <img alt="Louis so cute" src="~assets/IMG_4452.jpg" width="1000px">
    <q-parallax :height="800" :speed="0.5">
      <template v-slot:media>
        <img alt="Louis so cute" src="~assets/IMG_4455.jpg">
      </template>

      <h1 class="text-white">Loui</h1>
    </q-parallax>
    <img alt="Louis so cute" src="~assets/IMG_4453.jpg" width="1000px">
  </q-page>
</template>

<style></style>

<script>
export default {
  name: "PageIndex",
  methods: {
    onItemClick() {
      console.log("Clicked on an Item");
    }
  }
};
</script>
