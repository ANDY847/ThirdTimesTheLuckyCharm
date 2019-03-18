<template>
  <!----flex center trys to make item in center of container------>
  <q-page class="flex flex-center">
    <!----self-start puts it at the top------>
    <q-card class="self-start row flex-center">
      <img
        class="col-auto"
        alt="Louis so cute"
        style="max-height: 200px; margin-top:50px;"
        src="~assets/IMG_4455.jpg"
      >
      <div class="col-auto self-start">Hey This Is Luie and hes a dog
        <q-input v-model="text" label="Maybe Sign In"/>isnt he so cute???
      </div>

      <!----- this first is a refrencing col as kind of a function class then you define the screen size and it will take in anthing the parents have after you declare col size x/12 like boot strap-->
      <div
        class="col-md-12 self-center"
      >this is another col that takes up whole row you should know this from boot</div>
    </q-card>
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
