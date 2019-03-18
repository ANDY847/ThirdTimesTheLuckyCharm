<template>
  <!----flex center trys to make item in center of container------>
  <q-page>
    <q-parallax :height="300" :speed=".75">
      <template v-slot:media>
        <img src="~assets/IMG_4452.jpg">
      </template>
      <h1 class="text-white absolute-bottom text-subtitle1 text-center">
        {{nameOfParty}}
        <q-btn color="deep-orange" glossy label="+ Add Me"/>
      </h1>
    </q-parallax>
    <div class="row">
      <!----------------this is importing the whole thing of picture and details componenets ---->
      <pictureAndDetails class="col-xs-12 col-md-6 col-lg-4"/>
      <mediaOptions class="col-xs-12 col-md-6 col-lg-8"/>
    </div>
    <!----self-start puts it at the top------>
    <!--------------------------tabs with cards----------------------------------->
    <!---------------------------insert picture and stuff here ---->
    <!-----------------toolbar row col 12 is for mobile md is for medium screen and i choose to make the div menu take up half of screen-------------------------------->
  </q-page>
</template>

<style></style>

<script>
// this imports my components
import pictureAndDetails from "../components/pictureAndDetails.vue";
import mediaOptions from "../components/mediaOptions.vue";

export default {
  name: "PageIndex",
  //this iniszilizes the components
  components: {
    pictureAndDetails,
    mediaOptions
  },
  data() {
    return {
      nameOfParty: "Party 1"
    };
  },
  methods: {
    onItemClick() {
      console.log("Clicked on an Item");
    }
  }
};
</script>
