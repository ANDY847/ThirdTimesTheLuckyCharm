<template>
  <!----flex center trys to make item in center of container------>
  <q-page>
    <!----this gutter makes it the text in the left of picture have spsace------>
    <q-card class="row q-gutter-x-md">
      <img
        alt="Louis so cute"
        style="max-height: 300px; max-width: 300px; "
        src="~assets/IMG_4453.jpg"
      >
      <div class="col q-gutter-sm">
        <div>DATE: {{date}}</div>
        <div>TIME: {{time}}</div>
        <div>Name: {{name}}</div>
        <q-btn color="black" label="Visit Website" @click="websiteLink"/>
        <div>Location: {{location}}</div>
        <q-btn color="black" label="Go To Map" @click="mapLink"/>
      </div>
    </q-card>
  </q-page>
</template>

<style></style>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      date: "Mar 14 2019",
      time: "4:20",
      location: "florida something",
      name: "disClub"
    };
  },
  methods: {
    websiteLink() {
      //these methods are just for the buttons you can change what they do here easy linking for you :D
      console.log("looped");
      for (let index = 0; index < 4; index++) {
        console.log("looped");
        console.log(index);
      }
    },
    mapLink() {
      if (1200 < this.$q.screen.width) {
        console.log("screen size is larger than medium");
      } else {
        console.log("screen size is smaller than medium");
      }

      //note the $q.screen.width is a call that has alot of option for your screen size and state of screen im efrencing this screen when i type this.
    }
  }
};
</script>
